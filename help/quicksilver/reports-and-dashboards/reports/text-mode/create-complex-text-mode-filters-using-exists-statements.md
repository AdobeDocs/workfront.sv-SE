---
product-area: reporting
navigation-topic: text-mode-reporting
title: Skapa komplexa textlägesfilter med EXISTS-satser
description: Skapa komplexa textlägesfilter med EXISTS-satser
author: Nolan
feature: Reports and Dashboards
exl-id: 106f7c9d-46cc-46c5-ae34-93fd13a36c14
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '2803'
ht-degree: 0%

---

# Skapa komplexa textlägesfilter med EXISTS-satser

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: do not EVER&nbsp;delete this article as long as Text Mode still exists in the system.&nbsp;Google ordered this article to be written and we wrote it with the help of consultants, so the use case is very complex and very hard to understand without this. It is also very much used by many customers)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;Alina: **~ Replace screen shot of icons when list/ reporting UI changes)</p>
-->

>[!IMPORTANT]
>
>Den här artikeln kräver en grundlig förståelse för Adobe Workfront API och rapportgränssnittet för textläge. Mer information om Workfront API finns i [Grunderna i API](../../../wf-api/general/api-basics.md).\
>Mer information om hur du använder textläge finns i [Översikt över textläge](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Översikt över objektrelationer i Workfront

Alla objekt är länkade till andra objekt i Workfront-databasen.

Genom att förstå hierarkin och objektens inbördes beroende kan du ta reda på vilka objekt som kan refereras i rapporter.

Mer information om vilka objekt som finns i Workfront och om deras hierarki och inbördes beroende finns i [Förstå objekt i Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

När du skapar filter kan du referera till andra objekt som är anslutna till filtrets objekt inom upp till två relationsnivåer med hjälp av standardrapporteringsgränssnittet.

Du kan t.ex. referera till Portfolio-ID:t i ett utgåvfilter för att endast visa problem i projekt som är kopplade till en viss portfölj med hjälp av standardgränssnittet. I det här fallet är portföljen två nivåer bort från emissioner.

Du kan emellertid inte referera till Portfolio-ägaren i ett emissionsfilter med hjälp av standardgränssnittet för att endast visa problem från projekt som är kopplade till portföljer där ägaren är en viss användare. Du måste använda textläge för att komma åt fältet Portfolio Ägarnamn, som ligger tre nivåer bort från problemen.

![issue_to_portfolio_owner_right_line_icons.PNG](assets/issue-to-portfolio-owner-sraight-line-icons-350x83.png)

En fullständig lista över objekt i Workfront finns i [API Explorer](../../../wf-api/general/api-explorer.md).

Mer information om hur du navigerar i API-utforskaren och söker efter objekt finns i [Använda API Explorer](../../../wf-api/general/using-api-explorer.md).

När du skapar filter måste du skapa komplexa satser i textlägesgränssnittet för att kunna referera till de här objekttyperna.

Mer information om hur du skapar komplexa filter finns i [Översikt över komplexa textlägesfilter som använder EXISTS-satser](#overview-of-complex-text-mode-filters-that-use-exists-statements) -avsnitt.

## Översikt över komplexa textlägesfilter som använder EXISTS-satser {#overview-of-complex-text-mode-filters-that-use-exists-statements}

Tänk på följande när du skapar filter som sträcker sig över flera nivåer i objekthierarkin eller filter för saknade objekt:

* Du måste skapa komplexa filter när du vill referera till objekt som inte är direkt kopplade till filterobjektet.
* Du måste använda en EXISTS-programsats för att göra följande:

   * Skapa filter som sträcker sig över flera nivåer.
   * Skapa filter som söker efter objekt som saknas.\
      När du skapar en användarrapport kan du till exempel filtrera efter användare som inte har loggat tid under en viss tidsperiod.

Tänk på följande regler när du använder EXISTS-programsatser i ett filter:

* Det finns tre objekt som du kan referera till i ett EXISTS-filter:

   * Filtrets objekt (ursprungsobjekt).
   * Det objekt vars fält du vill referera till (målobjekt).
   * Det objekt som ansluter till det ursprungliga objektet och målobjekten, om de inte är direkt kopplade till varandra (länka objekt).

* Filter som använder EXISTS innehåller två separata satser länkade med ett likhetstecken:

   * Programsatsen före likhetstecknet refererar till det objekt som du refererar till (länkningen eller målobjektet).
   * Programsatsen efter likhetstecknet refererar till det objekt du refererar till (det ursprungliga objektet).

* Du måste använda objektkoden för det länkade objektet för att koppla programsatserna.\
   Du hittar objektkoden för alla objekt i API Explorer.\
   Information om API Explorer finns i [API Explorer](https://one.workfront.com/s/api-explorer).

* När ett länkat objekt saknas på grund av att det ursprungliga objektet och målobjektet är direktanslutna kan du använda objektkoden för målobjektet i stället för det länkade objektet.
* Du kan referera till flera fält (målfält) på samma objekt (målobjekt). Då måste du koppla ihop de rader som refererar till fälten med AND.\
   Ett exempel på filtrering av mer än ett fält som tillhör målobjektet finns i [Exempel 4: Filtrera efter flera fält: uppgifter efter Portfolio-ägarnamn och Portfolio-justeringsstyrkort-ID](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id) i den här artikeln.

* Den enda modifierare som stöds för en EXISTS-sats är NOTEXISTS.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att redigera filter i en rapport</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter till en rapport för att redigera filter i en rapport</p> <p>Hantera behörigheter för ett filter för att redigera det</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Skapa komplexa textlägesfilter som spänner över flera nivåer i objekthierarkin

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***[This information is somewhat duplicated from the section below: Create Text-Mode Filters for Missing Objects])</p>
-->

Du kan skapa ett filter som refererar till objekt på flera nivåer i objekthierarkin där filterobjektet finns. Du kan till exempel skapa ett problemfilter för problem i projekt som inte är kopplade till en viss Portfolio-ägare.

Du måste alltid använda en EXISTS-sats och textlägesgränssnittet för att skapa det här filtret.

Exempel på filter finns i [Exempel 1: Filter för utleveranser efter Portfolio ägarnamn](#example-1-filter-for-issues-by-portfolio-owner-name) i den här artikeln.

Så här skapar du ett filter som sträcker sig över flera nivåer i objekthierarkin:

1. Identifiera objektet i filtret. Det här objektet kallas ursprungsobjekt.\
   Exempel: Utgåva.
1. Identifiera fältet som du vill filtrera efter. Vi hänvisar till det här objektet som målfält som tillhör ett målobjekt.\
   Till exempel fältet ownerID (målfält) som tillhör Portfolio (målobjekt).
1. (Villkorligt) Om det ursprungliga objektet (Issue) och målfältet (ownerID) inte är direkt kopplade till varandra, måste du hitta ett tredje objekt, ett länkat objekt (Project), som kopplar dem. Länkningsobjektet måste ha minst ett fält som refereras från flikarna Fält eller Referenser för det ursprungliga objektet (länkningsfältet visas på det ursprungliga objektet) och det måste också ha ett länkningsfält till målobjektet som visas på flikarna Fält eller Referenser för det länkade objektet. Länkningsfältet till målobjektet som visas på det länkade objektet (eller det länkade fältet som visas på det länkade objektet) måste matcha målfältet.\
   Exempel: (Projekt)-ID (Länkningsfält som visas på det ursprungliga objektet) refereras till från Problem (ursprungsobjekt). (Portfolio) ownerID (Länkar fält till målobjektet) visas på fliken Fält i projektet (Länkar objekt). Portfolio ownerID är också ett fält i målobjektet (Portfolio). Länkningsfältet på det länkade objektet matchar målfältet.\
   ![portfolio_id_in_the_project_api_object.PNG](assets/portfolio-id-in-the-project-api-object-350x88.png)

1. Identifiera API-utforskaren med **Objektkod** för det länkade objektet (projektet).\
   Objektkoden för Project är till exempel PROJ.\
   ![project_objCode_in_the_API.PNG](assets/project-objcode-in-the-api-350x84.png)

1. Skapa ett filter för det ursprungliga objektet.\
   Skapa till exempel ett Issue-filter.\
   Mer information om hur du skapar filter finns i [Översikt över filter i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klicka **Växla till textläge**.
1. Klistra in följande formelexempel i textlägesgränssnittet för det nya filtret och ersätt den föreslagna texten med rätt objekt och fält:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>
   EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

   Ett exempel på hur du använder fälten som vi har identifierat ovan finns i [Exempel 1: Filter för utleveranser efter Portfolio ägarnamn](#example-1-filter-for-issues-by-portfolio-owner-name) i den här artikeln.

1. Klicka **Spara filter**.

## Skapa komplexa textlägesfilter för saknade objekt

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: **^[This information is somewhat duplicated from the section above: Create Text-Mode Filters that Span Multiple Levels in the Object Hierarchy])</p>
-->

Du kan skapa ett filter som refererar till objekt som saknas. Du kan till exempel skapa ett användarfilter som visar vilka användare som inte har loggat timmar i Workfront.

Du måste alltid använda en *EXISTS* -programsats och textlägesgränssnittet för att skapa det här filtret.

Exempel på filter för saknade objekt finns i följande avsnitt i den här artikeln:

* [Exempel 2: Filter för saknade objekt: anpassade fält som inte visas i anpassade formulär](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [Exempel 3: Filter för saknade objekt: användare som inte loggade in på en viss tid](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)

Så här skapar du ett filter som refererar till saknade objekt:

1. Identifiera objektet i filtret. Det här objektet kallas ursprungsobjekt.\
   Exempel: Parameter eller Anpassat fält.
1. Identifiera fältet som du vill filtrera efter. Vi hänvisar till det här objektet som målfält som tillhör ett målobjekt.\
   Till exempel fältet categoryID (målfält) som tillhör kategorin (målobjekt).
1. Eftersom det ursprungliga objektet (Parameter) och målfältet (categoryID) inte är direkt kopplade till varandra, måste du hitta ett tredje objekt, ett länkat objekt (en kategoriparameter) som kopplar dem. Länkningsobjektet måste ha minst ett fält som refereras från flikarna Fält eller Referenser för det ursprungliga objektet (länkningsfältet visas på det ursprungliga objektet) och det måste också ha ett länkningsfält till målobjektet som visas på flikarna Fält eller Referenser för det länkade objektet. Länkningsfältet till målobjektet som visas på det länkade objektet (eller det länkade fältet som visas på det länkade objektet) måste matcha målfältet.\
   Till exempel refereras ID:t för kategoriparametern (länkningsfältet som visas i det ursprungliga objektet) från Parameter (det ursprungliga objektet). parameterID (som länkar fält till målobjektet) visas på fliken Fält i kategoriparametern (som länkar objekt). Länkningsfältet till målobjektet som visas på det länkade objektet matchar målfältet.
1. Identifiera API-utforskaren med **Objektkod** för det länkade objektet (kategoriparameter).\
   Objektkoden för kategoriparametern är till exempel CTGYPA.\
   ![category_parameter_objcode_in_api.PNG](assets/category-parameter-objcode-in-api-350x79.png)

1. Skapa ett filter för det ursprungliga objektet.\
   Skapa till exempel ett parameterfilter.\
   Mer information om hur du skapar filter finns i [Översikt över filter i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klicka **Växla till textläge**.
1. (Villkorligt) Om du filtrerar efter objekt som saknas, klistrar du in följande formelexempel i det nya filtrets textlägesgränssnitt och ersätter den föreslagna texten med rätt objekt och fält:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   Ett exempel på rapportering om anpassade fält som inte är kopplade till anpassade Forms finns i [Exempel 2: Filter för saknade objekt: anpassade fält som inte visas i anpassade formulär](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms) i den här artikeln.

1. Klicka **Spara filter**.

## Exempel på textlägesfilter som sträcker sig över flera nivåer i objekthierarkin

* [Exempel 1: Filter för utleveranser efter Portfolio ägarnamn](#example-1-filter-for-issues-by-portfolio-owner-name)
* [Exempel 2: Filter för saknade objekt: anpassade fält som inte visas i anpassade formulär](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [Exempel 3: Filter för saknade objekt: användare som inte loggade in på en viss tid](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)
* [Exempel 4: Filtrera efter flera fält: uppgifter efter Portfolio-ägarnamn och Portfolio-justeringsstyrkort-ID](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id)

### Exempel 1: Filter för utleveranser efter Portfolio ägarnamn {#example-1-filter-for-issues-by-portfolio-owner-name}

Med hjälp av textlägesgränssnittet kan du skapa ett filter för en lista med problem som bara visar problem i projekt som är kopplade till en portfölj vars ägare är en viss användare.

Så här filtrerar du utleveranser efter Portfolio ägarnamn:

1. Skapa ett problemfilter.\
   Mer information om hur du skapar filter finns i [Översikt över filter i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klicka **Växla till textläge**.
1. Se följande allmänna kod:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

1. Klistra in följande kod i **Ange filterregler för rapporten** det område som ska ersätta den generiska koden ovan:

   <pre>EXISTS:A:$$OBJCODE=PROJ<br>EXISTS:A:ID=FIELD:projectID<br>EXISTS:A:portfolio:ownerID=4d94d7da001699b19edf50de15682221</pre>

   >[!NOTE]
   >
   >* Originalobjektet är rapportens objekt: Problem
   >* Målobjektet är Portfolio.
   >* Det länkade objektet är Projekt.
   >* Målfältet och det länkade fältet till målobjektet som refereras från det länkade objektet är ownerID.
   >* Objektkoden för det länkade objektet här är PROJ.
   >* Länkningsfältet som visas på det ursprungliga objektet är projectID och länkningsfältet är ID.


1. Ersätt värdet för målfältet (ownerID) i den senaste satsen med ett användar-ID från din miljö.
1. Klicka **Spara filter**.

### Exempel 2: Filter för saknade objekt: anpassade fält som inte visas i anpassade formulär {#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms}

Med hjälp av textlägesgränssnittet kan du skapa ett filter för att visa anpassade fält (parametrar) som inte är kopplade till anpassade Forms (kategorier). Det här filtret länkar parametrar till kategorier som är anslutna via ett annat objekt, Kategoriparameter. Eftersom de två fälten inte är direkt kopplade till varandra och eftersom du filtrerar efter saknad information måste du använda en EXISTS-sats.

>[!IMPORTANT]
>
>En parameter är ett fält som det finns i fältbiblioteket som refereras i ett anpassat formulär. En kategoriparameter är den version av ett fält som visas i ett visst formulär. Om samma fält t.ex. visas på 5 formulär finns det 1 parameter och 5 kategoriparametrar i Workfront-databasen.

Så här filtrerar du efter anpassade fält som inte är kopplade till ett anpassat formulär:

1. Skapa en parameter eller ett anpassat fältfilter.\
   Mer information om hur du skapar filter finns i [Översikt över filter i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klicka **Växla till textläge**.
1. Se följande allmänna kod:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. Klistra in följande kod i **Ange filterregler för rapporten** det område som ska ersätta den generiska koden ovan:

   <pre>EXISTS:A:$$OBJCODE=CTGYPA<br>EXISTS:A:parameterID=FIELD:ID<br>EXISTS:A:$$EXISTSMOD=NOTEXISTS</pre>

   >[!NOTE]
   >
   >* Originalobjektet är rapportens objekt: Parameter.
   >* Målobjektet är kategori.
   >* Det länkade objektet är en kategoriparameter.
   >* Objektkoden för det länkade objektet är CTGYPA.
   >* Länkningsfältet till målobjektet är parameterID eftersom parameterID finns både i tabellen för länkade objekt och i tabellen för målobjekt.
   >* Länkningsfältet som visas på det ursprungliga objektet är ID (för kategoriparametern).


1. Klicka **Spara filter**.

### Exempel 3: Filter för saknade objekt: användare som inte loggade in på en viss tid {#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time}

Med hjälp av textlägesgränssnittet kan du skapa ett filter för att visa användare som inte har loggat tid under en viss tidsperiod. Det här filtret länkar användare till timmar, som är direkt kopplade till varandra. Du måste emellertid använda en EXISTS-sats och textlägesgränssnittet för att kunna filtrera efter information.information som saknas.

Så här filtrerar du efter användare som inte loggade in tid under den senaste veckan:

1. Skapa ett användarfilter.\
   Mer information om hur du skapar filter finns i [Översikt över filter i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klicka **Växla till textläge**.
1. Se följande allmänna kod:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. Klistra in följande kod i **Ange filterregler för rapporten** det område som ska ersätta den generiska koden ovan:

   ```
   EXISTS:A:$$OBJCODE=HOUR<br>EXISTS:A:ownerID=FIELD:ID<br>EXISTS:A:entryDate=$$TODAYb-1w<br>EXISTS:A:entryDate_Range=$$TODAYe-1w<br>EXISTS:A:entryDate_Mod=between<br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   >[!NOTE]
   >
   >* Originalobjektet är rapportens objekt: Användare.
   >* Målobjektet är Timme.
   >* Du behöver inte länka objekt i det här exemplet eftersom användare och timmar är direkt anslutna i Workfront-databasen.
   >* Eftersom det inte finns något länkat objekt måste du använda objektkoden för målobjektet: TIMME.
   >* Länkningsfältet till målobjektet är ownerID (som visas på det ursprungliga objektet). det länkade objektet saknas).
   >* Det länkfält som visas på det ursprungliga objektet är ID (för timmen) (som visas på målobjektet). det länkade objektet saknas.)
   >* EXISTS:A:Programsatsen entryDate refererar till fält som definierar målobjektet (Hour) och använder samma syntax som i en vanlig filterprogramsats. Detta garanterar att du bara visar de användare som inte har loggat in på en viss tidsperiod, i det här fallet föregående vecka.
   >* NOTEXISTS-modifieraren anger att vi letar efter objekt (timmar) som inte finns för rapportens objekt (användare).


1. Klicka **Spara filter**.

### Exempel 4: Filtrera efter flera fält: uppgifter efter Portfolio-ägarnamn och Portfolio-justeringsstyrkort-ID {#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id}

Med hjälp av textlägesgränssnittet kan du skapa ett filter som refererar till mer än ett fält i målobjektet. I det här fallet måste filterprogramsatserna som refererar till målfälten vara kopplade av AND.

Du kan till exempel filtrera en lista med uppgifter så att endast uppgifter som uppfyller följande villkor visas:

* De är kopplade till ett projekt som är kopplat till en portfölj vars ägare är en specifik användare.
* De är kopplade till ett projekt som är kopplat till en portfölj vars projekt inte är kopplade till ett visst justeringskort.

Så här filtrerar du uppgifter efter Portfolio ägarens namn och Portfolio justeringsstyrkortets ID:

1. Skapa ett uppgiftsfilter.\
   Mer information om hur du skapar filter finns i [Översikt över filter i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klicka **Växla till textläge**.
1. Klistra in följande kod i **Ange filterregler för rapporten** område:
   <pre>EXISTS:A:$$OBJCODE=PROJ<br>EXISTS:A:ID=FIELD:projectID<br>EXISTS:A:portfolio:ownerID=4d80ce520000528787d57807732a33f<br>OCH:A:EXISTS:A:$$EXISTSMOD=NOTEXISTS<br>OCH:A:EXISTS:A:$$OBJCODE=PROJ<br>OCH:A:EXISTS:A:ID=FIELD:projectID<br>OCH:A:EXISTS:A:portfolio:alignmentScoreCardID=4da387b0001cbc732bb259355c33dad</pre>

   >[!NOTE]
   >
   >* Originalobjektet är filtrets objekt: Uppgift.
   >* Målobjektet är Portfolio.
   >* Det första målfältet är ownerID.
   >* Det andra målfältet är Styrkort-ID för justering.
   >* Det länkade objektet är Projekt.
   >* Objektkoden för det länkade objektet är PROJ.
   >* Länkningsfältet till målobjektet är ID:t (för Portfolio).
   >* Länkningsfältet som visas på det ursprungliga objektet är projectID.
   >* Ersätt ownerID med ett användar-ID från din miljö.


1. Klicka **Spara filter**.

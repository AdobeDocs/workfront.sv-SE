---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Lägga till en fråga i en rapport
description: Filter och uppmaningar liknar varandra i den bemärkelsen att de båda begränsar den mängd information som du visar i en rapport.
author: Nolan
feature: Reports and Dashboards
exl-id: b4058fb3-7360-474f-8be1-1c6b584749b0
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '1251'
ht-degree: 0%

---

# Lägga till en fråga i en rapport

## Skillnaden mellan uppmaningar och filter

Filter och uppmaningar liknar varandra i den bemärkelsen att de båda begränsar den mängd information som du visar i en rapport.

Du skapar ett filter när du vill att den information som visas i rapporten ska filtreras med samma villkor varje gång du kör rapporten. Filter skapas en gång och de är hårdkodade i rapporten. Mer information om hur du skapar filter finns i artikeln [Översikt över filter](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Frågar är öppna filter som kan anpassas och tillämpas på olika sätt varje gång du kör en rapport.

När du lägger till uppmaningar i rapporten kan du anpassa filtreringsinformationen genom att redigera frågevillkoren varje gång du kör rapporten. Rapporten körs med olika filter varje gång, beroende på vilka modifieringar du väljer, i stället för att hårdkoda modifieringarna en gång i rapportfiltret.

Frågar fungerar som ett anpassningsbart filter på rapporter som kan uppdateras precis innan du kör rapporten. Du kan skapa generiska rapporter och sedan begränsa resultaten baserat på den information du vill se för den dagen eller på den information som är relevant för en uppsättning kriterier som är individuella för dig. Om du till exempel har en timrapport och vill ändra informationen i rapporten baserat på följande kriterier:

* Datumen när timmarna loggades
* Användarna som angav timmarna
* Det angivna timbeloppet

Du skapar tre prompter där villkoren är de kriterier som krävs och rapporten ser annorlunda ut varje gång du kör den, beroende på vilken information du väljer för dina uppmaningar.

Ett filter kan instruera Adobe Workfront att endast visa de timmar som anges mellan juni och augusti i år. Med en uppmaning kan du emellertid använda olika tidsramar varje gång du kör rapporten (till exempel mellan januari och februari eller oktober och december).

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
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Du måste skapa en rapport innan du kan lägga till en fråga.

Instruktioner om hur du skapar en rapport finns i [Skapa en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)

## Skapa en fråga

1. Gå till rapporten där du vill lägga till en fråga.
1. Expandera **Rapportåtgärder** och klicka sedan på **Redigera**.

1. Klicka **Rapportinställningar**.
1. I **Rapportera uppmaningar** område, klicka **Lägg till en fråga**.\
   ![](assets/qs-add-a-prompt-350x216.png)

1. (Villkorligt) Markera det fält som du vill att uppmaningen ska baseras på. Börja skriva namnet på fältet och klicka för att markera det när det visas i listan.\
   Vilka alternativ som är tillgängliga för användare som kör rapporten varierar beroende på vilket fält du väljer.\
   Om du t.ex. väljer ett datumfält som Faktiskt slutförandedatum i en aktivitetsrapport, är &quot;Faktiskt slutförandedatum&quot; namnet på uppmaningen. När du redigerar den här uppmaningen när du kör den här rapporten kan du välja bland en uppsättning modifierare för att skapa din filtersats. Den här processen är identisk med att skapa ett filter. Mer information om modifierare finns i [Filter- och villkorsmodifierare](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Villkorligt) Klicka **Anpassad fråga** för att skapa en egen uppmaning.

   En anpassad fråga är en fördefinierad fråga där du hårdkodar filtervillkoren innan du kör rapporten. I det här fallet finns en anpassad fråga närmare ett filter än en fråga.

   Kommandot är dock lika flexibelt som en vanlig prompt eftersom du kan välja mellan flera fördefinierade satser, till skillnad från att bara ha ett hårdkodat filter i rapporten.

   Ange följande information för den anpassade prompten: Villkoret för en anpassad prompt kan bara redigeras i textläge. Detta gör att flera villkor kan användas i ett enda fält.

   * **Fält:** Detta är namnet på uppmaningen, som du ser den innan du kör rapporten.
   * **Etikett:** Det här är namnet på ett av alternativen i uppmaningen som du ser det innan du kör rapporten.
   * **Villkor:** Ange ett villkor som definierar uppmaningen.

   Använd samma syntax som du använder när du anger ett textlägesfilter och koppla programsatser till &quot;&amp;&quot;. Mer information om hur du redigerar ett filter i textläge finns i [Redigera ett filter i textläge](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

   Till exempel **Villkor** fält för den anpassade uppmaningen för följande scenarier kan se ut så här:

   * alla uppgifter i framtida projekt där projektstatusen är Idea, Begärd, Planerad och Aktuell:

     ```
     project:plannedStartDate=$$TODAY&project:plannedStartDate_Mod=gte&project:status=IDA,REQ,PLN,CUR&project:status_Mod=in
     ```

   * alla uppgifter i slutförda (tidigare) projekt där projektstatusen är Slutförd eller Död:

     ```
     project:actualCompletionDate=$$TODAY&project:actualCompletionDate_Mod=lte&project:status=CPL,DED&project:status_Mod=in
     ```

   Mer information om modifiering i textläge finns i [Filter- och villkorsmodifierare](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Du kan inte ändra villkoren för en anpassad fråga när du kör rapporten, som du skulle göra med en standardfråga. Du kan ha så många fördefinierade villkor för en anpassad fråga som du behöver.

1. (Valfritt) Upprepa steg 4 eller steg 5 för att skapa så många uppmaningar som behövs.
1. Klicka **Klar** och sedan klicka **Spara+stäng** för att spara rapporten.

## Använda en uppmaning i en rapport

När du har lagt till en fråga i en rapport är standardfliken för rapporten alltid fliken Fråga.

Så här kör du en rapport med en fråga:

1. Gå till rapporten med uppmaningen.

   ![](assets/qs-prompt-drop-downs-350x229.png)

1. Välj ett villkor för en eller alla uppmaningar som visas på **Fråga** -fliken.\
   (Valfritt) Du kan lämna uppmaningarna tomma och inte filtrera rapporten efter uppmaningsvillkoren.

1. Klicka **Kör rapport**.\
   (Villkorligt) Om du fyllde i uppmaningarna filtreras rapporten efter de villkor som du har valt för dina uppmaningar.\
   (Villkorligt) Om du lämnade uppmaningarna tomma filtreras inte rapporten efter uppmaningsvillkoren. Rapporten visas som om den inte filtrerats.

   >[!NOTE]
   >
   >En rapport som innehåller ett filter förutom en prompt filtrerar resultaten enligt både villkoren som definierats i filtret och prompten kombinerat.

## Begränsningar för delning av obligatoriska rapporter

>[!CAUTION]
>
>När du delar en rekommenderad rapport utanför Workfront måste den användare som visar rapporten vara inloggad på Workfront för att köra rapporten med hjälp av uppmaningen. Om användaren som visar rapporten inte är inloggad visas alla rapportresultat utan att uppmaningen tillämpas.

Följande är begränsningar när det gäller att dela rapporter från Workfront:

* När du delar en rapport offentligt kan användarna inte köra rapporten genom att köra uppmaningen, såvida de inte har Workfront-inloggningsuppgifter och först loggar in för att visa rapporten i Workfront.

  Mer information om att dela rapporter finns i artikeln [Dela en rapport i Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
* När du schemalägger en begärd rapport för leverans innehåller rapporten i e-postbilagan de data som efterfrågas. När användaren klickar på länken i e-postmeddelandet för att få åtkomst till rapporten måste han/hon logga in först för att kunna visa rapporten och köra uppmaningen själv.

  Mer information om att schemalägga en levererad rapport finns i [Schemalägg automatisk rapportleverans](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

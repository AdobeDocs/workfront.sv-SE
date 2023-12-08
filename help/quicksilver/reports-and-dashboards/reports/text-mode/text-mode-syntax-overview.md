---
product-area: reporting
navigation-topic: text-mode-reporting
title: Översikt över syntaxen i textläge
description: Du kan använda textlägesgränssnittet för att skapa mer komplexa vyer, filter, grupperingar och anpassade uppmaningar i listor och rapporter. Genom att använda textläge kan du komma åt fält och deras attribut som inte är tillgängliga i standardlägesgränssnittet.
author: Nolan
feature: Reports and Dashboards
role: User
exl-id: f24430e1-c5f7-4925-93df-0e956a03c863
source-git-commit: 6279106f56fa0d128e0dd03cd13b63a71d4c2952
workflow-type: tm+mt
source-wordcount: '1865'
ht-degree: 0%

---

# Översikt över syntaxen i textläge

Du kan använda textlägesgränssnittet för att skapa mer komplexa vyer, filter, grupperingar och anpassade uppmaningar i listor och rapporter. Genom att använda textläge kan du komma åt fält och deras attribut som inte är tillgängliga i standardlägesgränssnittet.

Information om och överväganden om textläge innan du börjar finns i [Översikt över textläge](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

En fullständig lista över alla våra rapportbara fält och deras attribut finns i [API Explorer](../../../wf-api/general/api-explorer.md).

Mer information om hur du skapar rapporter i textläge, inklusive klasser, videoklipp och självstudiekurser, finns i avsnittet Lär dig på Adobe Experience League webbplats.

## Att tänka på när det gäller syntax i textläge

* Du måste förstå Adobe Workfront-syntax innan du kan börja skapa rapportelement i textläge. Workfront-syntaxen för textläge är unik för det här programmet och har unika egenskaper som du måste känna till.
* Innan du börjar använda textläge i dina rapporter rekommenderar vi att du går igenom våra lektioner för avancerad rapportering för att få en bättre förståelse för vårt textläge. <!--outdated link: For training materials on reporting see [Workfront Reports and Dashboards Learning Paths](https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ).-->
* Du kan anpassa vyer, filter och grupperingar med hjälp av standardlägesgränssnittet. Du kan dock endast skapa anpassade uppmaningar i textläge.

## Allmänna riktlinjer för att skapa rapportelement i textläge

Nedan följer några vanliga riktlinjer när du skapar ett rapporterings- eller listelement i textläge:

* Använd alltid kamelskiftläge när du refererar till objekt eller attribut i Workfront-databasen.
* Tänk på hierarkin med objekt i Workfront. Det finns följande skillnader mellan vyer, filter och grupperingar:

   * Du kan visa ett objekt som är tre objekt bort från rapporten eller listobjektet i en vy.
   * Du kan inte referera till objekt som är mer än två objekt från huvudobjektet i en gruppering, ett filter eller en anpassad prompt.

  **Exempel:** Du kan visa Portfolio-ägarens namn eller GUID i en uppgiftsvy:


  `valuefield=project:portfolio:ownerID`

  Du kan inte gruppera, filtrera eller fråga efter Portfolio-ägaren i en uppgiftsvy:

  `project:portfolio:ownerID=5808f4bc00790b270a9629dd128e63fa`


  I de här exemplen är Portfolio ägar-ID tre objekt från listans objekt.

  Mer information om hierarkin för objekt i Workfront finns i:

   * [Förstå objekt i Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
   * [API Explorer](../../../wf-api/general/api-explorer.md)

* Använd jokertecken när det är möjligt för att göra rapporter och listor mer dynamiska och undvika att duplicera dem för olika användare och liknande tidslinjer.

## Översikt över kameraärenden

När du refererar till Workfront-fält eller deras attribut i textläge, kräver Workfront att du skriver deras namn med kamelstil. I det här fallet stavas ennamnsfälten med gemener. Sammansatta fält är stavade enligt följande mönster:

`camelCaseSyntax`

>[!IMPORTANT]
>
>Alla rapportelement följer det här övergångsmönstret.

Egenskaperna hos kamelfodral är:

* Det första ordet börjar alltid med en gemen bokstav.
* Följande ord börjar alltid med en versal.
* Det finns inga mellanslag mellan orden.

**Exempel:** För att referera till det faktiska slutförandedatumet för ett projekt är namnet på fältet som du skulle använda när du skapade rapportelement för textläge

`actualCompletionDate`

## Syntax för textläge för olika rapportelement

Följande likheter finns mellan syntaxen för uppsättningarna med rapportelement nedan när de skapas i textläge:

* Raderna med kod och syntax är desamma för vyer och grupperingar.

  Mer information om kodraderna för vyer och grupperingar när du skapar dem i textläge finns i:

   * [Redigera en vy i textläge](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
   * [Redigera textläge i en gruppering](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

* Kod- och syntaxraderna är desamma för filter och anpassade uppmaningar.

  Mer information finns i:

   * [Redigera ett filter i textläge](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
   * [Lägga till en fråga i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

### Syntax för vyer och grupperingar

Kodraderna när du skapar vyer och grupperingar är lika.

Mer information om hur du skapar vyer och grupperingar finns i följande artiklar:

* [Översikt över vyer i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Översikt över grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

Den viktigaste kodraden för en vy eller gruppering är den rad som identifierar det objekt som refereras i vyns kolumn eller i grupperingen. Den här kodraden kan börja med `valuefield` eller `valueexpression` baserat på om det här fältet är en direkt referens till ett databasfält i Workfront eller en beräkning mellan flera fält.

I följande tabell visas de vanligaste kodraderna i en vy eller gruppering:

| Kodrad | Beskrivning |
|-----------------|------------------------------------------------------------------------------------------------------------------------------|
| `valuefield` | Identifierar det objekt som vyns kolumn eller gruppering refererar till. Detta är en direkt referens till det refererade objektet. |
| `valueexpression` | Identifierar det objekt som vyns kolumn eller gruppering refererar till. Detta är en beräkning mellan flera fält. |
| `valueformat` | Identifierar det format i vilket Workfront returnerar det värde som anges i värdefältet eller värdesuttrycksraderna. |
| `width` | Identifierar bredden på en kolumn i pixlar. |
| `stretch` | Identifierar vilka kolumner som upptar extra utrymme som inte behövs för vyn. |

>[!TIP]
>
>* Även om kodraderna i exemplen nedan är lika mellan vyer och grupperingar, måste du alltid komma ihåg att varje kodrad för en gruppering börjar med grupperingsnumret.
>
>  Om du vill gruppera efter projektnamn i en projektlista eller rapport använder du följande rad för gruppering på första nivån:
>
>  `group.0.valuefield=name`
>  
>* Om du redigerar flera kolumner i en vy i samma kolumn (som när det gäller delade kolumner) måste du komma ihåg att varje kodrad för varje kolumn börjar med kolumnnumret.
>
>  Använd följande format för att identifiera den första kolumnen i en vy:
>
>  `column.0.valuefield=name`
>  
>  Mer information om att dela kolumner finns i [Visa: sammanfoga information från flera kolumner i en delad kolumn](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).
>

#### `Valuefield` syntaxöversikt för vyer och grupperingar

`Valuefield=` är en nyckelrad med kod i vyer och grupperingar som identifierar det objekt som du refererar till direkt.

Syntaxen för direkt referensfält är identisk för grupperingar och vyer.

Följande regler gäller när du refererar till Workfront-objekt med en `valuefield` rad:

* Använd kamelcase för att referera till fält direkt.

  **Exempel:** Använd följande rad om du vill referera till det faktiska slutförandedatumet för aktiviteten i en uppgiftsvy:

  `valuefield=actualCompletionDate`

* Använd kamelcase och kolon för att separera fält som relaterar till varandra för samma objekt.

  **Exempel:** Använd följande rad om du vill referera till projektets planerade slutförandedatum i en aktivitetsvy:

  `valuefield=project:plannedCompletionDate`

  Information om hur objekt refererar till varandra i Workfront-databasen finns i [API Explorer](../../../wf-api/general/api-explorer.md).

* När du refererar till ett anpassat fält ska du använda fältets namn exakt som det visas i gränssnittet.

  **Exempel:** Om du vill referera till ett anpassat projektfält med namnet Ytterligare information i en uppgiftsvy använder du följande rad:

  `valuefield=project:Additional Details`

#### `Valueexpression` syntaxöversikt för vyer och grupperingar

Du kan ersätta `valuefield=` kodrad med `valueexpression=` när du skapar vyer och grupperingar i textläge när du vill referera till en beräkning mellan två eller flera fält.

>[!TIP]
>
>Även om du kan skapa beräkningsfält som du kan visa i rapporter, är beräknade vyer och grupperingar mer dynamiska. Beräknade vyer och grupperingar uppdateras med ny information varje gång du kör rapporten eller visar en lista.
>
>Mer information om hur du skapar beräknade kolumner i en vy finns i [Beräknade anpassade fält kontra beräknade kolumner](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

Att skapa en beräknad gruppering påminner om att skapa en beräknad kolumn i en vy.

Följande regler gäller när du refererar till Workfront-objekt med en `valueexpression` rad:

* Använd kamelcase för att referera till fält direkt och omsluta varje fält med klammerparenteser.

  **Exempel:** Visa fältet Uppgiftsnamn i en uppgiftskolumn med `valueexpression`använder du följande rad:

  `valueexpression={name}`


* Använd kamelcase och punkter för att separera fält som hör ihop.

  **Exempel:** Använd följande rader om du vill visa namnet på ett projekt som är sammanfogat med namnet på uppgiften i en aktivitetsrapport:

   * I en vy:

     `valueexpression=CONCAT({project}.{name},' - ',{name})`

   * I en gruppering:

     `group.0.valueexpression=CONCAT({project}.{name},' - ',{name})`

  Information om hur objekt refererar till varandra i Workfront-databasen finns i [API Explorer](../../../wf-api/general/api-explorer.md).

* Använd följande regler när du refererar till ett anpassat fält:

   * Använd namnet på fältet exakt som det visas i gränssnittet.
   * Föregående fältets namn med &quot;DE:&quot;.
   * Omsluter fältet med klammerparenteser.
   * Avgränsa fälten som hör till objektet med punkter.

  **Exempel:** Använd följande rad för att visa det anpassade fältet Ytterligare information i en uppgiftsvy på en värdesuttrycksrad:

  `valueexpression={project}.{DE:Additional Details}`

* Du kan använda ett jokertecken i en `valueexpression` men inte i `valuefield` linje.

  Mer information om jokertecken finns i [Översikt över filtervariabler för jokertecken](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).


#### `Valueformat` översikt för vyer och grupperingar

Den näst viktigaste kodraden i en vy eller gruppering är `valueformat=` linje. Detta anger för Workfront i vilket format du vill returnera det värde du anger i dialogrutan `valuefield` eller `valueexpression` rader. Du kan använda olika format för `valueformat` rader rekommenderar vi att du alltid använder följande värde när du använder `valueexpression`:

`valueformat=HTML`

För ytterligare `valueformat` värden, se även följande artiklar:

* [Formatera datum i textlägesrapporter](../../reports/text-mode/format-dates-in-text-mode-reports.md)
* [Formatera tal, valuta och procentvärden i textlägesrapporter](../../reports/text-mode/format-numbers-in-text-mode-reports.md)

#### `width` översikt för vyer

`width=` är kodraden där du kan ange bredden på varje kolumn i pixlar. Workfront har en föreslagen bredd för varje fält, men beroende på fälttyp och format kan du behöva göra justeringar.

Du måste använda ytterligare `usewidths=true` kodrad för att framtvinga bredden som anges för kolumnen.

**Exempel:** Om du vill visa en kolumn med en bredd på 80 pixlar använder du följande rader:

`width=80`

`usewidths=true`

#### `stretch` översikt för vyer

The `stretch` används för att identifiera vilka kolumner som upptar extra utrymme som inte behövs för vyn. Användargränssnittets bredd för en vanlig användare är cirka 850 pixlar. Det innebär att om du har en vy med fyra kolumner (150 pixlar vardera) så upptar vyn 600 av 850 pixlar. Det finns 250 extra pixlar i gränssnittet som läggs till i kolumner som har en sträckningsprocent.

En kolumns sträckning används när du använder den extra kodraden: `usewidths=true` för minst en av kolumnerna i vyn.

**Exempel:** Om du vill ange att en kolumn kan använda 70 % av det tomma utrymmet i en vy använder du följande rader:

`stretch=70`

`usewidths=true`

### Syntax för filter och anpassade uppmaningar

Syntaxen för att skapa filter liknar den för att skapa egna uppmaningar.

>[!TIP]
>
>Du kan skapa en anpassad fråga genom att först skapa ett filter för satsen som du vill inkludera i prompten. Koppla ihop alla kodrader i ett filter med &quot;&amp;&quot; utan blanksteg mellan raderna och det blir din egen uppmaning.

Mer information om hur du skapar filter och anpassade uppmaningar finns i:

* [Översikt över filter i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Lägga till en fråga i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

Mer information om hur du skapar filter i textläge finns i [Redigera ett filter i textläge](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

Du kan använda följande element för att skapa filter och anpassade uppmaningar i textläge:

* En kodrad som refererar till filtersatsens objekt. Använd kameraläge för filterobjektet.
* En kodrad som refererar till filterobjektet och modifieraren för filterobjektets värde. Använd kameraläge för filterobjektet på den här raden.

  >[!TIP]
  >
  >När du refererar till intervall kräver detta två modifieringslinjer.

* En satsanslutning som ansluter flera filtersatser:

   * OCH

     Det här är standardkopplingen mellan filtersatser.

   * ELLER

     >[!TIP]
     >
     >Satskopplingar är skiftlägeskänsliga och alltid versaler. &quot;AND&quot; kan utelämnas i textläge.

* Jokertecken för att göra filter mer dynamiska och anpassa dem för aktuell tid eller för användaren som är inloggad. Mer information om jokertecken finns i [Översikt över filtervariabler för jokertecken](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

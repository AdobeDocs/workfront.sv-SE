---
title: Visa resurskapaciteten i Förbättrad analys
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Du kan bedöma om ett team är över, under eller i kapacitet när du tittar på Ökad resursvisualisering för analyser i Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 5bb45ef6-9e49-4063-8e53-c9f3bc994870
source-git-commit: d9a8af627c8d3da4a7625cd5180bfca69da43b3d
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 0%

---

# Visa resurskapaciteten i Förbättrad analys

<!--Audited: 01/2024-->

Du kan bedöma om ett team är över, under eller i kapacitet när du tittar på Ökad resursvisualisering för analyser i Adobe Workfront.

De team som illustreras i resursvisualiseringen avser det hemteam med användare som har tilldelats arbetet under den angivna tidsperioden.

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront</a>*</td> 
   <td> <p>Aktuell: Business eller högre</p>
   eller
   <p>Nytt: Alla</p>
    </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens*</td> 
   <td> <p>Aktuell: Granska eller senare</p>
   eller
   <p>Nytt: Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivåkonfiguration</td> 
   <td> <p>Visa åtkomst till projekt</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörighet för ett projekt</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har. Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Förutsättningar

Information om krav för att använda Förbättrad analys finns i avsnittet Krav i [Förbättrad analys - översikt](../enhanced-analytics/enhanced-analytics-overview.md).

## Förstå resurskapaciteten visualisering

Resurskapaciteten visas om ett team är över, under eller på kapaciteten. Denna beräkning bygger på följande:

* **Tillgänglig kapacitet**: Det totala antalet timmar som ett hemteam har tillgängligt för att arbeta under den filtrerade tidsperioden

  >[!NOTE]
  >
  >Om du tittar på en framtida tidsperiod beräknas den tillgängliga kapaciteten baserat på teamets kapacitet för de senaste 7 dagarna. Därför beaktas inte schemalagd PTO.

* **Planerad kapacitet**: Det totala antalet planerade arbetstimmar som förväntas av hemteamet under den filtrerade tidsperioden

Den här jämförelsen av ett hemteams planerade timmar och faktiska schemalagda timmar kan hjälpa dig att avgöra om du inte tilldelar tillräckligt med arbete till hemteamet eller om de kan drabbas av problem på grund av en hög arbetsbelastning.

![](assets/resource-capacity-350x110.png)

I Resurskapaciteten visas följande information:

* **Planerad kapacitet**: Den blå cirkeln motsvarar det antal timmar som hemteamet har tilldelats.

  ![](assets/resource-capacity-blue-circle.png)

* **Faktisk kapacitet**: Den lodräta linjen står i linje med hemteamets namn och visar antalet tillgängliga timmar för hemteamet.

  ![](assets/resource-capacity-vertical-line.png)

* **Överkapacitet**: När den vågräta linjen och den blå cirkeln visas till höger om den lodräta linjen tilldelades arbetsteamet mer arbete än vad de kan slutföra under det tillgängliga antalet timmar. Detta innebär att teamet kan vara överkapacitetskassan under den filtrerade tidsperioden. Det antal timmar som teamet behöver slutföra visas till höger om den blå cirkeln.

  ![](assets/resource-capacity-over-capacity.png)

* **Under kapacitet**: När den vågräta linjen och den blå cirkeln visas till vänster om den lodräta linjen har hemteamet fler tillgängliga timmar än det antal planerade arbetstimmar de tilldelats. Detta innebär att teamet kan vara under kapacitet för den filtrerade tidsperioden. Det ytterligare antalet tillgängliga timmar för hemteamet att slutföra arbetet visas till vänster om den blå cirkeln.

  ![](assets/resource-capacity-under-capacity.png)

När du hovrar över en teamrad visas det exakta antalet timmar för planerad kapacitet och tillgänglig kapacitet, liksom antalet timmar som hemteamet är över eller under kapacitet.

Om du ser den här informationen blir det lättare att avgöra:

* Om teamet är överallokerat eller underallokerat.
* Det största projektet är att hemteamet är fokuserat på.
* Vilka team som finns tillgängliga för arbete.

Om du vill veta hur du får de bästa data för den här visualiseringen kan du läsa [Förbättrad analys - översikt](../enhanced-analytics/enhanced-analytics-overview.md).

## Visa resurskapaciteten som visualisering

{{step1-to-analytics}}

1. I den vänstra panelen väljer du **Folk**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (Valfritt) Om du vill använda ett annat datumintervall väljer du nya start- och slutdatum från datumintervallfiltret i diagrammets övre högra hörn.

   ![](assets/filters-select-date-range-350x344.png)

   Mer information om hur du använder datumintervallfiltret finns i [Använda filter i Förbättrad analys](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Villkorligt) Om du inte har ställt in teamfiltret lägger du till teamfiltret och väljer varje team som du vill se data för.

   Mer information om hur du lägger till filter i Förbättrad analys finns i [Använda filter i Förbättrad analys](../enhanced-analytics/use-enhanced-analytics-filters.md).

   När du har lagt till filter visas data för upp till 50 projekt och filtren förblir aktiva även när du lämnar sidan eller loggar ut från Workfront.

1. (Valfritt) Om du vill zooma in ett datumintervall markerar du en punkt i visualiseringen för början av datumintervallet och drar till slutet av datumintervallet.

   Alla andra visualiseringar uppdateras till samma datumintervall och ett tidsramsfilter skapas.

   ![](assets/timeframe-filter-350x220.png)

1. Hovra över teamlinjen för hemmabruk för att se följande:

   * Hur många timmar som fortfarande är tillgängliga för schemaläggning
   * Antal timmar som hemteamet har planerat att slutföra
   * Det totala antalet arbetade timmar. Det totala antalet arbetade timmar kan ha följande etiketter:

      * Över
      * Under
      * På kapaciteten.

   ![](assets/resource-capacity-capacity-pop-up-350x213.png)

1. (Valfritt) Om du vill exportera visualiseringsdata klickar du på **Ikonen Exportera** ![](assets/export.png) i det övre högra hörnet av visualiseringen väljer du exportformat:

   * **Diagram (PNG)**
   * **Datatabell (XSLX)**

1. Klicka på ett hemteamnamn om du vill se mer information i teamkapacitetvisualiseringen.

   Mer information om teamkapacitetvisualisering finns i [Visa teamkapacitetvisualisering i Förbättrad analys](../enhanced-analytics/team-capacity-overview.md).



---
title: Visa Burndown-visualisering i Förbättrad analys
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: I Burndown-visualiseringen visas ett specifikt projekts nedgång över tid och hjälper dig att förstå förhållandet mellan projektvillkor, hastighet och återstående timmar - eller dagar.
author: Nolan
feature: Reports and Dashboards
exl-id: e67c92d5-b309-406b-b6f0-4d414d0e7dcc
source-git-commit: 59e021aa3ae66e4fc8d9ce9eb57616f948e6cd90
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 0%

---

# Visa Burndown-visualisering i Förbättrad analys

>[!IMPORTANT]
>
>Förbättrad analys kommer att tas bort från Workfront den 26 maj. Workfront Data Connect är en ny alternativ lösning som kan användas för att replikera de utökade analyser du använder just nu. <br>Mer information finns i guiden [Borttagning av utökad analys](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md).


<!-- Audited: 12/2023 -->

I Burndown-visualiseringen visas ett specifikt projekts nedgång över tid och hjälper dig att förstå förhållandet mellan projektvillkor, hastighet och återstående timmar - eller dagar.

![Exempel på utökad analysnedladdning](assets/burndown120623.png)

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>
      <p>Nytt: Alla</p>
      <p>eller</p>
      <p>Aktuell: Business eller högre</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
      <p>Nytt: Ljus eller högre</p>
      <p>eller</p>
      <p>Aktuell: Granska eller senare</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa åtkomst till projekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa</p> </td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Förutsättningar

Förutsättningar för att använda Förbättrad analys finns i avsnittet Förutsättningar i [Översikt över förbättrade analyser](../enhanced-analytics/enhanced-analytics-overview.md).

## Förstå Burndown-visualiseringen

Den täckande blå raden visar den planerade hastigheten från startdatumet till det planerade slutförandedatumet. Den här raden justeras när arbete läggs till, tas bort eller uppdateras, och den ändras till en streckad vertikal linje när projektet når det planerade slutförandedatumet.

![Planerad hastighet](assets/burndown-planned-line.png)

Den faktiska raden visar hur många timmar - eller dagar - som har ägnats åt projektet över tid. Färgen på den här raden anger projektets villkor varje dag:

* **Grön**: Projektet är på mål.

  ![På målet](assets/burndown-green.png)

* **Orange**: Projektet är i fara.

  ![I riskzonen](assets/burndown-orange.png)

* **Röd**: Projektet är i trubbel.

  ![I problem](assets/burndown-red.png)

Mer information om de här projektvillkoren finns i [Översikt över projektvillkor och villkorstyp](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

När den faktiska raden flyttas uppåt lodrätt har arbete lagts till i projektet. När raden flyttas nedåt lodrätt har arbetet tagits bort eller slutförts för projektet.

Under x-axeln i visualiseringen kan du se mer information om hur uppgifter och timmar - eller dagar - ändrades en viss dag (mängden som lades till, mängden som fylldes i och skillnaden mellan de två).

Genom att se all den här informationen i Burndown-visualiseringen kan du avgöra:

* Det enskilda projektets hälsa över tiden
* Hur problem som kommer in (eller oplanerade arbeten) påverkade det planerade arbetet
* Vilka händelser som förlängde ditt projekt efter det ursprungliga slutförandedatumet

Om du vill lära dig hur du får bästa möjliga data för den här visualiseringen kan du läsa [Översikt över förbättrade analyser](../enhanced-analytics/enhanced-analytics-overview.md).

## Visa Burndown-visualisering

{{step1-to-analytics}}

1. (Valfritt) Om du vill använda ett annat datumintervall väljer du nya start- och slutdatum från datumintervallfiltret.

   ![Välj datum](assets/filters-select-date-range-350x344.png)

   Mer information om hur du använder datumintervallfiltret finns i [Använda filter i Förbättrad analys](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Villkorligt) Om du behöver begränsa projektdatauppsättningen markerar och tillämpar du de filter som du vill använda.

   Mer information om hur du lägger till filter i Förbättrad analys finns i [Använda filter i Förbättrad analys](../enhanced-analytics/use-enhanced-analytics-filters.md).

   När du har lagt till filter visas data för upp till 50 projekt och filtren förblir aktiva även när du lämnar sidan eller loggar ut från Workfront.

1. (Valfritt) Om du vill zooma in ett datumintervall markerar du en punkt i visualiseringen för början av datumintervallet och drar den till slutet av datumintervallet.

   Alla andra visualiseringar uppdateras till samma datumintervall och ett tidsramsfilter skapas automatiskt.

   ![Tidsbildrutefilter](assets/timeframe-filter-350x220.png)

1. Klicka på ett projekt i Flight-planen eller på Project treemap-visualisering för att visa mer information.

   Burndown och Tasks visas i flygvisualiseringar.

   >[!NOTE]
   >
   >Mer information om dessa andra visualiseringar finns i:
   >
   >   * [Visa visualisering av flygplan i Förbättrad analys](../enhanced-analytics/flight-plan-overview.md)
   >   * [Visa visualisering av projekttreemap i Förbättrad analys](../enhanced-analytics/project-treemap-overview.md)
   >   * [Visa uppgifter i flygvisualisering i Förbättrad analys](../enhanced-analytics/tasks-in-flight-overview.md)
   >

1. (Valfritt) Ändra vyn från planerade timmar till **varaktighet**.

   Planerade timmar väljs som standard.

   >[!NOTE]
   >
   >Om du väljer **varaktighet** ändras all timinformation till dagar.\
   >![Varaktighet för nedladdning](assets/duration-burndown-350x112.png)\
   >Mer information om varaktighet i området Förbättrad analys finns i avsnittet&quot;Varaktighet&quot; i [Översikt över förbättrade analyser](../enhanced-analytics/enhanced-analytics-overview.md#duration-view).

1. Klicka på en punkt i linjediagrammet.

   Det exakta datumet visas under diagrammet och ytterligare information om uppgifter och timmar - eller dagar - för den valda dagen.

   ![Nedladdningsinformation](assets/burndown-task-and-hour-changes-350x121.png)

   >[!NOTE]
   >
   >Om den faktiska hastigheten är en platt linje som löper längs x-axeln (inline med 0 timmar eller 0 dagar) i visualiseringen innebär det att inga planerade timmar - eller dagar - har lagts till i projektet.\
   >Om den faktiska hastigheten är en platt linje ovanför x-axeln (i linje med ett antal timmar eller antal dagar) som aldrig går ned, innebär det att inga uppgifter har slutförts inom den filtrerade tidsperioden.

1. (Valfritt) Om du vill exportera visualiseringsdata klickar du på ikonen **Exportera** ![Exportera ](assets/export.png) i det övre högra hörnet av visualiseringen och väljer exportformat:

   * Diagram (PNG)
   * Datatabell (XSLX)

1. (Valfritt) Om du vill se information om förloppet för uppgifter i det valda projektet tittar du på Aktiviteter i flygvisualisering som visas under nedladdningsvisualiseringen. Mer information finns i [Visa uppgifter i flygvisualisering i Förbättrad analys](/help/quicksilver/enhanced-analytics/tasks-in-flight-overview.md).

---
title: Visa Burndown-visualisering i Förbättrad analys
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: I Burndown-visualiseringen visas ett specifikt projekts nedgång över tid och hjälper dig att förstå förhållandet mellan projektvillkor, hastighet och återstående timmar - eller dagar.
author: Nolan
feature: Reports and Dashboards
exl-id: e67c92d5-b309-406b-b6f0-4d414d0e7dcc
source-git-commit: d337008d4fca8c41b98b10f9059ec1cc379811e1
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 0%

---

# Visa Burndown-visualisering i Förbättrad analys

I Burndown-visualiseringen visas ett specifikt projekts nedgång över tid och hjälper dig att förstå förhållandet mellan projektvillkor, hastighet och återstående timmar - eller dagar.

![](assets/burndown-350x112.png)

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront</a>*</td> 
   <td> <p>Företag eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Översikt över Adobe Workfront-licenser</a>*</td> 
   <td> <p>Granska eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa åtkomst till projekt</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå.<br>Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Information om krav för att använda Förbättrad analys finns i avsnittet Krav i [Förbättrad analys - översikt](../enhanced-analytics/enhanced-analytics-overview.md).

## Förstå Burndown-visualiseringen

Den täckande blå raden visar den planerade hastigheten från startdatumet till det planerade slutförandedatumet. Den här raden justeras när arbete läggs till, tas bort eller uppdateras och ändras till en streckad vertikal linje när projektet når det planerade slutförandedatumet.

![](assets/burndown-planned-line.png)

Den faktiska raden visar hur många timmar - eller dagar - som har ägnats åt projektet över tid. Färgen på den här raden anger projektets villkor varje dag:

* **Grön**: Projektet är på mål.

   ![](assets/burndown-green.png)

* **Orange**: Projektet är i fara.

   ![](assets/burndown-orange.png)

* **Röd**: Projektet är i trubbel.

   ![](assets/burndown-red.png)

Mer information om projektvillkoren finns i [Översikt över projektvillkor och villkorstyp](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

När den faktiska raden flyttas uppåt lodrätt har arbete lagts till i projektet. När raden flyttas nedåt lodrätt har arbetet tagits bort eller slutförts för projektet.

Under x-axeln i visualiseringen kan du se mer information om hur uppgifter och timmar - eller dagar - ändrades en viss dag (mängden som lades till, mängden som fylldes i och skillnaden mellan de två).

Genom att se all den här informationen i Burndown-visualiseringen kan du avgöra:

* Det enskilda projektets hälsa över tiden
* Hur problem (eller oplanerade arbeten) påverkade det planerade arbetet.
* Vilka händelser som förlängde ditt projekt efter det ursprungliga slutförandedatumet.

Om du vill veta hur du får de bästa data för den här visualiseringen kan du läsa [Förbättrad analys - översikt](../enhanced-analytics/enhanced-analytics-overview.md).

## Visa Burndown-visualisering

1. Klicka på ikonen Huvudmeny ![](assets/main-menu-icon-16x12.png)väljer **Analyser**.
1. (Valfritt) Om du vill använda ett annat datumintervall väljer du nya start- och slutdatum från datumintervallfiltret.

   ![](assets/filters-select-date-range-350x344.png)

   Mer information om hur du använder datumintervallfiltret finns i [Använd filter i Förbättrad analys](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Villkorligt) Om du behöver begränsa projektdatauppsättningen markerar och tillämpar du de filter som du vill använda.

   Mer information om hur du lägger till filter i Förbättrad analys finns i [Använd filter i Förbättrad analys](../enhanced-analytics/use-enhanced-analytics-filters.md).

   När du har lagt till filter visas data för upp till 50 projekt och filtren förblir aktiva även när du lämnar sidan eller loggar ut från Workfront.

1. (Valfritt) Om du vill zooma in ett datumintervall markerar du en punkt i visualiseringen för början av datumintervallet och drar till slutet av datumintervallet.

   Alla andra visualiseringar uppdateras till samma datumintervall och ett tidsramsfilter skapas.

   ![](assets/timeframe-filter-350x220.png)

1. Klicka på ett projekt i Flight-planen eller på Project treemap-visualisering för att visa mer information.

   Burndown och Tasks visas i flygvisualiseringar.

   >[!NOTE]
   >
   >Mer information om dessa andra visualiseringar finns i:
   >
   >   
   >   
   >   * [Visa flygplansvisualisering i Förbättrad analys](../enhanced-analytics/flight-plan-overview.md)
   >   * [Visa projekttreemap-visualisering i Förbättrad analys](../enhanced-analytics/project-treemap-overview.md)
   >   * [Visa uppgifter i flygvisualisering i Förbättrad analys](../enhanced-analytics/tasks-in-flight-overview.md)


1. (Valfritt) Ändra vyn från planerade timmar till **varaktighet**.

   Planerade timmar väljs som standard.

   >[!NOTE]
   >
   >Markera **varaktighet** ändrar all timinformation till dagar.\
   >![](assets/duration-burndown-350x112.png)\
   >Mer information om varaktighet i området Förbättrad analys finns i avsnittet&quot;Varaktighet&quot; i [Förbättrad analys - översikt](../enhanced-analytics/enhanced-analytics-overview.md).

1. Klicka på en punkt i linjediagrammet.

   Det exakta datumet visas och ytterligare information om uppgifter och timmar - eller dagar - för den valda dagen visas nedan.

   ![](assets/burndown-task-and-hour-changes-350x121.png)

   >[!NOTE]
   >
   >Om den faktiska hastigheten är en platt linje som löper längs x-axeln (inline med 0 timmar eller 0 dagar) i visualiseringen innebär det att inga planerade timmar - eller dagar - har lagts till i projektet.\
   >Om den faktiska hastigheten är en platt linje ovanför x-axeln (i linje med ett antal timmar eller antal dagar) som aldrig går ned, innebär det att inga uppgifter har slutförts inom den filtrerade tidsperioden.

1. (Valfritt) Om du vill exportera visualiseringsdata klickar du på **Exportera** icon ![](assets/export.png)i det övre högra hörnet av visualiseringen väljer du exportformat:

   * **Diagram (PNG)**
   * **Datatabell (XSLX)**

1. (Valfritt) Om du vill se information om förloppet för uppgifter i det valda projektet tittar du på Aktiviteter i flygvisualisering som visas under nedladdningsvisualiseringen.

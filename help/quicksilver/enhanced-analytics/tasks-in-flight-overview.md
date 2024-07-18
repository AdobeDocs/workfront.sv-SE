---
title: Visa uppgifter i flygvisualisering i Förbättrad analys
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Aktiviteter vid flygvisualisering visar hur många uppgifter (inom de filtervillkor som tillämpas) som pågår för ett projekt, hur många procent av arbetet som har slutförts för varje uppgift och hur enligt tidsplanen uppgifterna utförs.
author: Nolan
feature: Reports and Dashboards
exl-id: cc738450-362a-49e8-836f-611fa82057b5
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 0%

---

# Visa uppgifter i flygvisualisering i Förbättrad analys

Aktiviteter vid flygvisualisering visar hur många uppgifter (inom de filtervillkor som tillämpas) som pågår för ett projekt, hur många procent av arbetet som har slutförts för varje uppgift och hur enligt tidsplanen uppgifterna utförs.

![](assets/tasks-in-flight-possible-replacement-350x104.png)

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront-plan</a>*</td> 
   <td> <p>Företag eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Översikt över Adobe Workfront-licenser</a>*</td> 
   <td> <p>Granska eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa åtkomst till projekt</p> <p>Visa åtkomst till uppgifter (Om du vill uppdatera uppgifter måste du ha redigeringsåtkomst till uppgifter.)</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå.<br>Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörighet för både projekt- och uppgiftsobjekt</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Förutsättningar för att använda Förbättrad analys finns i avsnittet Förutsättningar i [Översikt över förbättrade analyser](../enhanced-analytics/enhanced-analytics-overview.md).

## Förstå uppgifter vid flygvisualisering

Aktiviteter i visualisering av färdplan visar följande aktivitetsinformation:

* **Planerad aktivitetslängd**: Längden på ett aktivitetsfält anger planerad varaktighet, baserat på aktivitetens startdatum och slutförandedatum.

  ![](assets/tasks-in-flight-duration-350x80.png)

* **Arbetsinsatsen har slutförts**: Den mörkblå färgen i ett aktivitetsfält anger mängden arbete som har slutförts för en aktivitet. Den här procentandelen för slutförande visas till höger om aktivitetsfältet.

  ![](assets/tasks-in-flight-dark-blue-350x35.png)

* **Återstående arbetsinsats**: Den ljusblå färgen i ett aktivitetsfält anger mängden arbete som behöver slutföras för en aktivitet.

  ![](assets/tasks-in-flight-light-blue-350x35.png)

Den här informationen kan hjälpa dig att avgöra:

* Var arbetet har inriktats.
* Vilka uppgifter skulle kunna utgöra en risk för ett projekt.
* Hur nära en uppgift är att slutföra.
* Vem du ska prata med om en viss uppgift.

Om du vill lära dig hur du får bästa möjliga data för den här visualiseringen kan du läsa [Översikt över förbättrade analyser](../enhanced-analytics/enhanced-analytics-overview.md).

## Visa uppgifter i flygvisualisering

1. Klicka på ikonen Huvudmeny ![](assets/main-menu-icon-16x12.png) och välj sedan **Analys**.
1. (Valfritt) Om du vill använda ett annat datumintervall väljer du nya start- och slutdatum från datumintervallfiltret.

   ![](assets/filters-select-date-range-350x344.png)

   Mer information om hur du använder datumintervallfiltret finns i [Använda filter i Förbättrad analys](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Villkorligt) Om du behöver begränsa projektdatauppsättningen markerar och tillämpar du de filter som du vill använda.

   Mer information om hur du lägger till filter i Förbättrad analys finns i [Använda filter i Förbättrad analys](../enhanced-analytics/use-enhanced-analytics-filters.md).

   När du har lagt till filter visas data för upp till 50 projekt och filtren förblir aktiva även när du lämnar sidan eller loggar ut från Workfront.

1. Klicka på ett projekt i Flight-planen eller på Project treemap-visualisering för att visa mer information.

   Burndown och Tasks visas i flygvisualiseringar.

   >[!NOTE]
   >
   >Mer information om dessa andra visualiseringar finns i:
   >
   >   
   >   
   >   * [Visa visualisering av flygplan i Förbättrad analys](../enhanced-analytics/flight-plan-overview.md)
   >   * [Visa visualisering av projekttreemap i Förbättrad analys](../enhanced-analytics/project-treemap-overview.md)
   >   * [Visa Burndown-visualisering i Förbättrad analys](../enhanced-analytics/burndown-overview.md)
   >   
   >

1. (Valfritt) Om du vill zooma in ett datumintervall markerar du en punkt i visualiseringen för början av datumintervallet och drar till slutet av datumintervallet.

   Alla andra visualiseringar uppdateras till samma datumintervall och ett tidsramsfilter skapas.

   ![](assets/timeframe-filter-350x220.png)

1. (Valfritt) Om du vill ändra hur uppgifterna sorteras klickar du på menyn **Sortera efter** och väljer sedan ett nytt sorteringsalternativ:

   * **Slutförandedatum**
   * **Alfabetiskt A-Ö**
   * **Uppdelad arbetsstruktur** (Det här alternativet matchar den ordning som aktiviteterna visas i projektet.)

   Alla andra visualiseringar på sidan uppdateras för att matcha din sorteringsmarkering.

1. Granska förloppet för uppgifter i det valda projektet och hovra sedan över en viss uppgift för att se antalet planerade timmar, planerat förfallodatum och slutförandeprocenten.

   ![](assets/tasks-in-flight-task-details-350x242.png)

1. Klicka på en uppgift för att öppna uppgiften Detaljer till höger på skärmen, där du kan se mer information om uppgiften, visa eller ange uppdateringar eller göra ändringar i uppgiften.

   ![](assets/task-details-qs-350x675.png)

1. (Valfritt) Om du vill exportera visualiseringsdata klickar du på ikonen **Exportera** ![](assets/export.png) i det övre högra hörnet av visualiseringen och väljer sedan exportformat:

   * **Diagram (PNG)**
   * **Datatabell (XSLX)**


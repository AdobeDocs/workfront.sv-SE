---
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: Visa projekttreemap-visualisering i Förbättrad analys
description: Visualisering av projekttreemap är en vy över timmar - eller dagar - som har arbetats i ett visst tidsfönster jämfört med andra arbetsinsatser i storlek. Detta hjälper er att förstå hur mycket tid folk har ägnat åt ett projekt.
author: Nolan
feature: Reports and Dashboards
exl-id: 6216465e-c3bb-4f2f-b71c-766ad0c2ed40
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 0%

---

# Visa projekttreemap-visualisering i Förbättrad analys

Visualisering av projekttreemap är en vy över timmar - eller dagar - som har arbetats i ett visst tidsfönster jämfört med andra arbetsinsatser i storlek. Detta hjälper er att förstå hur mycket tid folk har ägnat åt ett projekt.

![](assets/project-treemap-350x126.png)

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

## Förstå projekttreemaps visualisering

Rutorna i projekttreemap-visualisering representerar projekt och rutornas storlek visar en jämförelse av hur mycket tid som har ägnats åt olika projekt. Ju större låda, desto mer tid läggs på projektet.

Visualiseringen av projekttreemap består av:

* **Mindre, ljusblå rutor**: Projekt som har färre timmar - eller dagar - visas som mindre rutor med ljusblå färg.

   ![](assets/project-treemap-smaller-box.png)

* **Större, mörkblå rutor**: Projekt som har fler timmar - eller dagar - visas som större rutor med en mörkblå färg.

   ![](assets/project-treemap-larger-box-350x205.png)

* **Medelstora, blå rutor**: Projekt som hamnar mellan de två kategorierna visas som medelstora rutor med en blå nyans mellan de mörkblå och ljusblå färgerna. Det finns tre möjliga nyanser av blått för de medelstora rutorna.

Förklaringen till höger visar en uppdelning av slutförda timmar för varje blå nyans. Den här teckenförklaringen är dynamisk och uppdateras utifrån data.

![](assets/project-treemap-hours-completed.png)

>[!NOTE]
>
>Om du tittar på Project treemap-visualisering efter varaktighet i stället för efter planerade timmar, visar den här förklaringen en uppdelning av antalet dagar som har bearbetats för varje ton med blått.\
>![](assets/project-treemap-days-worked.png)>

Om du ser den här informationen blir det lättare att avgöra:

* Prioriteten för saker som bearbetas under det valda datumintervallet.
* Vilka team spenderar tid på.
* Om team fokuserar på rätt saker.
* När du klickar på ett visst projekt, hur mycket omfattningen av ett projekt har ändrats under den tidsperioden.

Om du vill veta hur du får de bästa data för den här visualiseringen kan du läsa [Förbättrad analys - översikt](../enhanced-analytics/enhanced-analytics-overview.md).

## Visa visualisering av projekttreemap

1. Klicka på ikonen Huvudmeny ![](assets/main-menu-icon-16x12.png)väljer **Analyser**.
1. (Valfritt) Om du vill använda ett annat datumintervall väljer du nya start- och slutdatum från datumintervallfiltret.

   ![](assets/filters-select-date-range-350x344.png)

   Mer information om hur du använder datumintervallfiltret finns i [Använd filter i Förbättrad analys](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Villkorligt) Om du behöver begränsa projektdatauppsättningen markerar och tillämpar du de filter som du vill använda.

   Mer information om hur du lägger till filter i Förbättrad analys finns i [Använd filter i Förbättrad analys](../enhanced-analytics/use-enhanced-analytics-filters.md).

   När du har lagt till filter visas data för upp till 50 projekt och filtren förblir aktiva även när du lämnar sidan eller loggar ut från Workfront.

1. (Valfritt) Om du vill ändra hur projekten sorteras klickar du på **Sortera efter** i det övre högra hörnet av projekttreemaps-visualisering och välj sedan ett nytt sorteringsalternativ:

   * **A - Z**
   * **Z - A**
   * **Planerat slutförandedatum**
   * **Planerat startdatum**

   Alla andra visualiseringar på sidan uppdateras för att matcha din sorteringsmarkering.

1. (Villkorligt) Om det finns fler än 50 projekt i datauppsättningen använder du pilarna i det nedre vänstra hörnet av visualiseringen för att navigera mellan 50 projekt i en grupp.

   Alla andra visualiseringar på sidan uppdateras så att de matchar sidans val.

   ![](assets/pagination-350x118.png)

1. (Valfritt) Ändra vyn från **planerade timmar** till **varaktighet**.

   Planerade timmar väljs som standard.

1. Håll muspekaren över ett projekt för att se projektvillkoren, liksom antalet totala planerade timmar, antalet slutförda timmar och det genomsnittliga antalet timmar som har ägnats åt projektet per dag.

   ![](assets/project-treemap-project-details-350x404.png)

   >[!NOTE]
   >
   >Om du valde **varaktighet** visas följande information om varaktighet:
   >
   >* **Planerad tidsram**: Antalet dagar som planeras för att slutföra projektet.
   >* **Dagar som har arbetats**: Den planerade varaktigheten för varje aktivitet som slutfördes inom det datumintervall som valts överst, dividerat med antalet timmar per dag.

   >   
   >![](assets/duration-treemap-350x159.png)
   >
   >Mer information om varaktighet finns i avsnittet Längd i [Förbättrad analys - översikt](../enhanced-analytics/enhanced-analytics-overview.md).

1. (Valfritt) Om du vill exportera visualiseringsdata klickar du på **Ikonen Exportera** ![](assets/export.png) i det övre högra hörnet av visualiseringen väljer du exportformat:

   * **Diagram (PNG)**
   * **Datatabell (XSLX)**

1. Klicka på ett projekt för att öppna Burndown and Tasks i flygvisualiseringar för att få en djupare inblick i hur uppgifter och timmar - eller dagar - har bidragit till ett projekts storlek.

Mer information om Burndown-visualisering finns i [Visa Burndown-visualisering i Förbättrad analys](../enhanced-analytics/burndown-overview.md). Mer information om uppgifter vid flygvisualisering finns i [Visa uppgifter i flygvisualisering i Förbättrad analys](../enhanced-analytics/tasks-in-flight-overview.md).


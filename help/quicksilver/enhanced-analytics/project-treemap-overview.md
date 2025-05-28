---
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: Visa projekttreemap-visualisering i Förbättrad analys
description: Visualisering av projekttreemap är en vy över timmar - eller dagar - som har arbetats i ett visst tidsfönster jämfört med andra arbetsinsatser i storlek. Detta hjälper er att förstå hur mycket tid folk har ägnat åt ett projekt.
author: Nolan
feature: Reports and Dashboards
exl-id: 6216465e-c3bb-4f2f-b71c-766ad0c2ed40
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '893'
ht-degree: 0%

---

# Visa projekttreemap-visualisering i Förbättrad analys

>[!IMPORTANT]
>
>Förbättrad analys togs bort från Workfront den 27 maj. Workfront Data Connect är en ny alternativ lösning som kan användas för att replikera de utökade analyser du använder just nu. <br>Mer information finns i guiden [Borttagning av utökad analys](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md).


<!-- Audited: 12/2023 -->

Visualisering av projekttreemap är en vy över timmar - eller dagar - som har arbetats i ett visst tidsfönster jämfört med andra arbetsinsatser i storlek. Detta hjälper er att förstå hur mycket tid folk har ägnat åt ett projekt.

![Projekttreemap](assets/project-treemap-350x126.png){width="700"}

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">Adobe Workfront</a></td> 
   <td> <p>Företag eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Översikt över Adobe Workfront-licenser</a></td> 
   <td>   <p>Nytt:</p> 
   <ul><li>Ljus eller högre</li></ul>
   <p>Aktuell:</p>
   <ul><li>Granska eller högre</li></ul>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa åtkomst till projekt</p> <!--<p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level.<br>For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p>--> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa</p> <!--<p>For information on requesting additional access, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p>--> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Förutsättningar för att använda Förbättrad analys finns i avsnittet Förutsättningar i [Översikt över förbättrade analyser](../enhanced-analytics/enhanced-analytics-overview.md).

## Förstå projekttreemaps visualisering

Rutorna i projekttreemap-visualisering representerar projekt och rutornas storlek visar en jämförelse av hur mycket tid som har ägnats åt olika projekt. Ju större låda, desto mer tid läggs på projektet.

Visualiseringen av projekttreemap består av:

* **Mindre, ljusblå rutor**: Projekt som har färre timmar - eller dagar - visas som mindre rutor med ljusblå färg.

  ![Mindre ruta](assets/project-treemap-smaller-box.png)

* **Större, mörkblå rutor**: Projekt som har fler timmar - eller dagar - visas som större rutor med en mörkblå färg.

  ![Större ruta](assets/project-treemap-larger-box-350x205.png)

* **Blå rutor i Medium-storlek**: Projekt som hamnar mellan de två kategorierna visas som medelstora rutor med en blå nyans mellan de mörkblå och ljusblå färgerna. Det finns tre möjliga nyanser av blått för de medelstora rutorna.

Förklaringen till höger visar en uppdelning av slutförda timmar för varje blå nyans. Den här teckenförklaringen är dynamisk och uppdateras utifrån data.

![Trädkartimmar har slutförts](assets/project-treemap-hours-completed.png)

>[!NOTE]
>
>Om du tittar på Project treemap-visualisering efter varaktighet i stället för efter planerade timmar, visar den här förklaringen en uppdelning av antalet dagar som har bearbetats för varje ton med blått.\
>![Trädkartsdagar arbetade](assets/project-treemap-days-worked.png)>

Om du ser den här informationen blir det lättare att avgöra:

* Prioriteten för saker som bearbetas under det valda datumintervallet.
* Vilka team spenderar tid på.
* Om team fokuserar på rätt saker.
* När du klickar på ett visst projekt, hur mycket omfattningen av ett projekt har ändrats under den tidsperioden.

Om du vill lära dig hur du får bästa möjliga data för den här visualiseringen kan du läsa [Översikt över förbättrade analyser](../enhanced-analytics/enhanced-analytics-overview.md).

## Visa visualisering av projekttreemap

1. Klicka på ikonen Huvudmeny ![Huvudmeny](assets/main-menu-icon-16x12.png) och välj sedan **Analys**.
1. (Valfritt) Om du vill använda ett annat datumintervall väljer du nya start- och slutdatum från datumintervallfiltret.

   ![Välj datumintervall](assets/filters-select-date-range-350x344.png)

   Mer information om hur du använder datumintervallfiltret finns i [Använda filter i Förbättrad analys](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Villkorligt) Om du behöver begränsa projektdatauppsättningen markerar och tillämpar du de filter som du vill använda.

   Mer information om hur du lägger till filter i Förbättrad analys finns i [Använda filter i Förbättrad analys](../enhanced-analytics/use-enhanced-analytics-filters.md).

   När du har lagt till filter visas data för upp till 50 projekt och filtren förblir aktiva även när du lämnar sidan eller loggar ut från Workfront.

1. (Valfritt) Om du vill ändra hur projekten sorteras klickar du på menyn **Sortera efter** i det övre högra hörnet av visualiseringen av projekttreemap och väljer sedan ett nytt sorteringsalternativ:

   * **A - Z**
   * **Z - A**
   * **Planerat slutförandedatum**
   * **Planerat startdatum**

   Alla andra visualiseringar på sidan uppdateras för att matcha din sorteringsmarkering.

1. (Villkorligt) Om det finns fler än 50 projekt i datauppsättningen använder du pilarna i det nedre vänstra hörnet av visualiseringen för att navigera mellan 50 projekt i en grupp.

   Alla andra visualiseringar på sidan uppdateras så att de matchar sidans val.

   ![Sidnumrering](assets/pagination-350x118.png)

1. (Valfritt) Ändra vyn från **planerade timmar** till **varaktighet**.

   Planerade timmar väljs som standard.

1. Håll muspekaren över ett projekt för att se projektvillkoren, liksom antalet totala planerade timmar, antalet slutförda timmar och det genomsnittliga antalet timmar som har ägnats åt projektet per dag.

   ![Information om Treemap-projekt](assets/project-treemap-project-details-350x404.png)

   >[!NOTE]
   >
   >Om du valde vyn **duration** ser du följande varaktighetsinformation:
   >
   >* **Planerad tidsram**: Antal dagar som planeras för att slutföra projektet.
   >* **Antal arbetsdagar**: Den planerade varaktigheten för varje aktivitet som har slutförts inom det datumintervall som har valts överst, dividerat med antalet timmar per dag.
   >   
   >![Trädkartans varaktighet](assets/duration-treemap-350x159.png)
   >
   >Mer information om varaktighet finns i avsnittet Varaktighet i [Översikt över förbättrade analyser](../enhanced-analytics/enhanced-analytics-overview.md).

1. (Valfritt) Om du vill exportera visualiseringsdata klickar du på ikonen **Exportera** ![Exportera ](assets/export.png) i det övre högra hörnet av visualiseringen och väljer exportformat:

   * **Diagram (PNG)**
   * **Datatabell (XSLX)**

1. Klicka på ett projekt för att öppna Burndown and Tasks i flygvisualiseringar för att få en djupare inblick i hur uppgifter och timmar - eller dagar - har bidragit till ett projekts storlek.

Mer information om Burndown-visualisering finns i [Visa Burndown-visualisering i Förbättrad analys](../enhanced-analytics/burndown-overview.md). Mer information om uppgifter vid flygvisualisering finns i [Visa uppgifter vid flygvisualisering i Förbättrad analys](../enhanced-analytics/tasks-in-flight-overview.md).


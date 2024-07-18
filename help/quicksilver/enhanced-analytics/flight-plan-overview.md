---
title: Visa flygplansvisualisering i Förbättrad analys
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: I flygplansvisualiseringen visas hur många projekt (inom de filtervillkor som tillämpats) som har varit under drift, vilka villkorsändringar som har gjorts under projektens livslängd och hur nära dessa projekt har uppfyllt de planerade tidsfristerna.
author: Nolan
feature: Reports and Dashboards
exl-id: c64ed752-151a-40f7-ab18-684e2cd032bc
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '863'
ht-degree: 0%

---

# Visa flygplansvisualisering i Förbättrad analys

I flygplansvisualiseringen visas hur många projekt (inom de filtervillkor som tillämpats) som har varit under drift, vilka villkorsändringar som har gjorts under projektens livslängd och hur nära dessa projekt har uppfyllt de planerade tidsfristerna.

![](assets/flight-plan-350x132.png)

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
   <td> <p>Visa åtkomst till projekt</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå.<br>Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa åtkomst till projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Förutsättningar för att använda Förbättrad analys finns i avsnittet Förutsättningar i [Översikt över förbättrade analyser](../enhanced-analytics/enhanced-analytics-overview.md).

## Förstå visualiseringen av flygplanen

Under projektets faktiska längd kan du bara se följande projektvillkor:

* På mål
* Risk
* I problem

Mer information om projektvillkor finns i [Översikt över projektvillkor och villkorstyp](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

I Flight-planvisualiseringen visas följande projektinformation:

* **Planerad varaktighet**: Den vågräta blå linjen representerar den planerade längden på projektet, med trianglarna i vardera ände av raden som anger startdatum och slutdatum.

  ![](assets/planned-duration-line-350x37.png)

* **Faktisk varaktighet**: Den tjocka, färgade linjen under den planerade längden representerar projektets faktiska längd. Linjens färg ändras beroende på projektets skick vid den aktuella tidpunkten under projektets livstid.

  ![](assets/actual-duration-line.png)

* **Faktiskt villkor**: Den tjocka, färgade linjen visar också villkoret för ett projekt vid olika tidpunkter. Linjens färg ändras beroende på projektets skick:

   * **Grön**: På mål
   * **Orange**: Riskerar
   * **Röd**: I problem

  ![](assets/actual-condition-color.png)

Genom att hovra över en projektrad i visualiseringen av flygplanen kan du visa information om projektets planerade tidsram, det aktuella projektvillkoret och, om tillämpligt, det anpassade villkoret. Om du vill få en mer detaljerad bild av vad som kan ha påverkat varaktighet eller villkor kan du titta på de andra visualiseringarna i området Förbättrad analys.

Om du ser den här informationen blir det lättare att avgöra:

* Vilka händelser som förlänger ett projekt efter det ursprungliga planerade slutförandedatumet.
* När ett projekt börjar stöta på problem.
* Hur många projekt som är öppna under samma tidsperiod.
* Hur många projekt som är aktiva.
* Vilka projekt som behöver extra uppmärksamhet eller support.

Mer information om hur du får bäst data för den här visualiseringen finns i [Översikt över förbättrade analyser](../enhanced-analytics/enhanced-analytics-overview.md).

## Visa visualisering av flygplan

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon-16x12.png) och välj sedan **Analys**.
1. (Valfritt) Om du vill använda ett annat datumintervall väljer du nya start- och slutdatum från datumintervallfiltret.

   ![](assets/filters-select-date-range-350x344.png)

   Mer information om hur du använder datumintervallfiltret finns i [Använda filter i Förbättrad analys](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Villkorligt) Om du behöver begränsa projektdatauppsättningen markerar och tillämpar du de filter som du vill använda.

   Mer information om hur du lägger till filter i Förbättrad analys finns i [Använda filter i Förbättrad analys](../enhanced-analytics/use-enhanced-analytics-filters.md).

   När du har lagt till filter visas data för upp till 50 projekt och filtren förblir aktiva även när du lämnar sidan eller loggar ut från Workfront.

1. (Valfritt) Om du vill zooma in ett datumintervall markerar du en punkt i visualiseringen för början av datumintervallet och drar till slutet av datumintervallet.

   Alla andra visualiseringar uppdateras till samma datumintervall och ett tidsramsfilter skapas.

   ![](assets/timeframe-filter-350x220.png)

1. (Valfritt) Om du vill ändra hur projekten sorteras klickar du på menyn **Sortera efter** i det övre högra hörnet i visualiseringen av flygplanen och väljer sedan ett nytt sorteringsalternativ:

   * **A - Z**
   * **Z - A**
   * **Planerat slutförandedatum**
   * **Planerat startdatum**

   Alla andra visualiseringar på sidan uppdateras för att matcha din sorteringsmarkering.

1. (Villkorligt) Om det finns fler än 50 projekt i datauppsättningen använder du pilarna i det nedre vänstra hörnet av visualiseringen för att navigera mellan 50 projekt i en grupp.

   Alla andra visualiseringar på sidan uppdateras så att de matchar sidans val.

   ![](assets/pagination-350x118.png)

1. Håll pekaren över diagrammet i projektfältet om du vill visa den blå datumraden samt följande information:

   * Planerad tidslinje
   * Aktuellt villkor
   * Anpassat villkor (om tillämpligt)

   ![](assets/project-bar-graph-350x143.png)

1. (Valfritt) Om du vill exportera visualiseringsdata klickar du på ikonen **Exportera** ![](assets/export.png) i det övre högra hörnet av visualiseringen och väljer sedan exportformat:

   * **Diagram (PNG)**
   * **Datatabell (XSLX)**

1. Om du vill visa mer projektinformation klickar du på ett projekt i visualiseringen för att öppna &quot;Burndown&quot; och &quot;Tasks&quot; i flygvisualiseringar.

   Dessa visualiseringar kan hjälpa er att få djupare insikter om vad som gjorde att projektet inte fungerade. De gör det också enkelt att checka in ett pågående projekt.\
   Mer information om Burndown-visualisering finns i [Visa Burndown-visualisering i Förbättrad analys](../enhanced-analytics/burndown-overview.md). Mer information om uppgifter vid flygvisualisering finns i [Visa uppgifter vid flygvisualisering i Förbättrad analys](../enhanced-analytics/tasks-in-flight-overview.md).


---
title: Visa teamkapacitetvisualisering i Förbättrad analys
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Teamkapacitetvisualiseringen visar den totala kapacitet som ett hemteam har, oavsett om de är överallokerade eller underallokerade, och hur dynamisk kapaciteten är över tiden.
author: Nolan
feature: Reports and Dashboards
exl-id: cfeb1a87-01be-4088-9e33-53a97e3871ad
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# Visa teamkapacitetvisualisering i Förbättrad analys

Teamkapacitetvisualiseringen visar den totala kapacitet som ett hemteam har, oavsett om de är överallokerade eller underallokerade, och hur dynamisk kapaciteten är över tiden.

![](assets/team-capacity-350x110.png)

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

## Förstå teamets kapacitetvisualisering

Teamkapacitetvisualiseringen visar den arbetsvolym som tilldelats hemteamet en viss dag.

* **Burnout**: När den mörkare blå fyllningsfärgen är ovanför den prickade linjen har hemteamet fler arbetstimmar än de kan fylla i det antal timmar teamet är tillgängligt att arbeta. Detta visar att teamet är överallokerat och kan komma att närma sig utbränning.

   ![](assets/team-capacity-over-capacity.png)

* **Obestridd**: När den mörkare blå fyllningsfärgen är under den prickade linjen har hemarbeteamet fler arbetstimmar än den mängd arbete de tilldelats. Detta visar att teamet är underallokerat och kan vara obestritt.

   ![](assets/team-capacity-under-capacity.png)

* **Saldo**: När den ljusare eller mer genomskinliga blå fyllningsfärgen är precis ovanför, precis nedanför eller på den prickade linjen har hemarbetsteamet tilldelats ett antal arbetstimmar som de ska kunna slutföra inom sina tillgängliga arbetstimmar. Detta visar att teamets arbetsbelastning är mer balanserad.

   ![](assets/team-capacity-at-capacity.png)

När du hovrar över en punkt i visualiseringen visas följande information för en viss dag:

* **Schemalagda timmar**: Detta är antalet planerade arbetstimmar som teamet behöver för att slutföra.
* **Tillgängliga timmar**: Detta är antalet arbetstimmar som teamet är tillgängligt för att arbeta.
* **Kapacitet**: Förutom en kapacitetsprocent visas även beteckningarna På kapacitet, Under kapacitet eller Över kapacitet.

Om du ser den här informationen blir det lättare att avgöra:

* När hemteamet var övertilldelat eller undertilldelat.
* Om hemteamet är övertilldelat eller undertilldelat dagligen.
* Hur konsekvent ett hemteams arbetsbörda är från dag till dag.
* Om du skapar kapacitetsproblem med nytt arbete.

Om du vill veta hur du får de bästa data för den här visualiseringen kan du läsa [Förbättrad analys - översikt](../enhanced-analytics/enhanced-analytics-overview.md).

## Visa teamkapacitetvisualisering

1. Klicka på ikonen Huvudmeny ![](assets/main-menu-icon-16x12.png)väljer **Analyser**.
1. Välj **Folk**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (Valfritt) Om du vill använda ett annat datumintervall väljer du nya start- och slutdatum från datumintervallfiltret.

   ![](assets/filters-select-date-range-350x344.png)

   Mer information om hur du använder datumintervallfiltret finns i [Använd filter i Förbättrad analys](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Villkorligt) Om du inte har ställt in teamfiltret lägger du till teamfiltret och väljer varje team som du vill se data för.

   Mer information om hur du lägger till filter i Förbättrad analys finns i [Använd filter i Förbättrad analys](../enhanced-analytics/use-enhanced-analytics-filters.md).

   När du har lagt till filter visas data för upp till 50 projekt och filtren förblir aktiva även när du lämnar sidan eller loggar ut från Workfront.

1. Klicka på ett team för att se mer information om resurskapaciteten.

   Visualisering av teamkapacitet visas.

   Mer information om resursvisualisering finns i [Visa resurskapaciteten i Förbättrad analys](../enhanced-analytics/resource-capacity-overview.md).

1. (Valfritt) Om du vill zooma in ett datumintervall markerar du en punkt i visualiseringen för början av datumintervallet och drar till slutet av datumintervallet.

   Alla andra visualiseringar uppdateras till samma datumintervall och ett tidsramsfilter skapas.

   ![](assets/timeframe-filter-350x220.png)

1. Håll muspekaren över en punkt på den graderade linjen för att se de schemalagda timmarna och de planerade timmarna för det angivna datumet, samt kapacitetsprocenten och om hemteamet var över, under eller vid tidpunkten.

   ![](assets/team-capacity-capacity-pop-up-350x351.png)

1. (Valfritt) Om du vill exportera visualiseringsdata klickar du på **Ikonen Exportera** ![](assets/export.png) i det övre högra hörnet av visualiseringen väljer du exportformat:

   * **Diagram (PNG)**
   * **Datatabell (XSLX)**


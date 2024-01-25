---
title: Visa teamkapacitetvisualisering i Förbättrad analys
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Teamkapacitetvisualiseringen visar den totala kapacitet som ett hemteam har, oavsett om de är överallokerade eller underallokerade, och hur dynamisk kapaciteten är över tiden.
author: Nolan
feature: Reports and Dashboards
exl-id: cfeb1a87-01be-4088-9e33-53a97e3871ad
source-git-commit: 45dac4c5e8ff584546783d561c04d137697a03a4
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 0%

---

# Visa teamkapacitetvisualisering i Förbättrad analys

<!-- Audited: 01/2024 -->

Teamkapacitetvisualiseringen visar den totala kapacitet som ett hemteam har, oavsett om de är överallokerade eller underallokerade, och hur dynamisk kapaciteten är över tiden.

![Teamkapacitet](assets/team-capacity.png)

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
   <td role="rowheader">Översikt över Adobe Workfront-licenser</td>
   <td>
      <p>Nytt: Ljus eller högre</p>
      <p>eller</p>
      <p>Aktuell: Granska eller senare</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>Visa åtkomst till projekt</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>Visa </td> 
  </tr> 
 </tbody> 
</table>

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Förutsättningar

Information om krav för att använda Förbättrad analys finns i avsnittet Krav i [Förbättrad analys - översikt](../enhanced-analytics/enhanced-analytics-overview.md).

## Förstå teamets kapacitetvisualisering

Teamkapacitetvisualiseringen visar den arbetsvolym som tilldelats hemteamet en viss dag.

* **Burnout**: När den mörkare blå fyllningsfärgen är ovanför den prickade linjen har hemteamet fler arbetstimmar än de kan fylla i det antal timmar teamet är tillgängligt för arbete. Detta visar att teamet är överallokerat och kan komma att närma sig utbränning.

  ![Överkapacitet](assets/team-capacity-over-capacity.png)

* **Obestridd**: När den mörkare blå fyllningsfärgen är under den prickade linjen har arbetsteamet fler timmar att arbeta än den mängd arbete de tilldelats. Detta visar att teamet är underallokerat och kan vara obestritt.

  ![Under kapacitet](assets/team-capacity-under-capacity.png)

* **Saldo**: När den ljusare eller mer genomskinliga blå fyllningsfärgen är precis ovanför, precis nedanför eller på den prickade linjen har hemarbetsteamet tilldelats ett antal arbetstimmar som de ska kunna slutföra inom sina tillgängliga arbetstimmar. Detta visar att teamets arbetsbelastning är mer balanserad.

  ![Vid kapacitet](assets/team-capacity-at-capacity.png)

När du hovrar över en punkt i visualiseringen visas följande information för en viss dag:

* **Schemalagda timmar**: Det här är antalet planerade arbetstimmar som teamet behöver för att slutföra.
* **Tillgängliga timmar**: Det här är antalet arbetstimmar som teamet kan arbeta under.
* **Kapacitet**: Förutom en kapacitetsprocent visas även beteckningarna På kapacitet, Under kapacitet eller Över kapacitet.

Om du ser den här informationen blir det lättare att avgöra:

* När hemteamet var övertilldelat eller undertilldelat.
* Om hemteamet är övertilldelat eller undertilldelat dagligen.
* Hur konsekvent ett hemteams arbetsbörda är från dag till dag.
* Om du skapar kapacitetsproblem med nytt arbete.

Om du vill veta hur du får de bästa data för den här visualiseringen kan du läsa [Förbättrad analys - översikt](../enhanced-analytics/enhanced-analytics-overview.md).

## Visa teamkapacitetvisualisering

{{step1-to-analytics}}

1. I den vänstra panelen väljer du **Folk**.

   ![Välj personer](assets/people-area-cropped-qs-350x276.png)

1. (Valfritt) Om du vill använda ett annat datumintervall väljer du nya start- och slutdatum från datumintervallfiltret.

   ![Datumintervallfilter](assets/filters-select-date-range-350x344.png)

   Mer information om hur du använder datumintervallfiltret finns i [Använda filter i Förbättrad analys](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Villkorligt) Om du inte har ställt in teamfiltret lägger du till teamfiltret och väljer varje team som du vill se data för.

   Mer information om hur du lägger till filter i Förbättrad analys finns i [Använda filter i Förbättrad analys](../enhanced-analytics/use-enhanced-analytics-filters.md).

   När du har lagt till filter visas data för upp till 50 projekt och filtren förblir aktiva även när du lämnar sidan eller loggar ut från Workfront.

1. Klicka på ett team för att se mer information om resurskapaciteten.

   Visualisering av teamkapacitet visas.

   Mer information om resursvisualisering finns i [Visa resurskapaciteten i Förbättrad analys](../enhanced-analytics/resource-capacity-overview.md).

1. (Valfritt) Om du vill zooma in ett datumintervall markerar du en punkt i visualiseringen för början av datumintervallet och drar till slutet av datumintervallet.

   Alla andra visualiseringar uppdateras till samma datumintervall och ett tidsramsfilter skapas.

   ![Tidsramsfilter](assets/timeframe-filter-350x220.png)

1. Håll muspekaren över en punkt på den graderade linjen för att se de schemalagda timmarna och de planerade timmarna för det angivna datumet, samt kapacitetsprocenten och om hemteamet var över, under eller vid tidpunkten.

   ![Popup för teamkapacitet](assets/team-capacity-capacity-pop-up-350x351.png)

1. (Valfritt) Om du vill exportera visualiseringsdata klickar du på **Exportera** icon ![Ikonen Exportera](assets/export.png) i det övre högra hörnet av visualiseringen väljer du exportformat:

   * Diagram (PNG)
   * Datatabell (XSLX)


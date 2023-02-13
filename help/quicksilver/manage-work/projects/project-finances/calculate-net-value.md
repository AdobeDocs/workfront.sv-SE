---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Beräkna nettovärde
description: Nettovärdet för ett projekt är det sammanlagda förväntade värdet av projektet efter att man har beräknat dess nytta och tagit bort kostnaderna.
author: Alina
feature: Work Management
exl-id: 44e3f211-c816-4ee1-aafc-c40fc8732f1a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---

# Beräkna nettovärde

Nettovärdet för ett projekt är det sammanlagda förväntade värdet av projektet efter att man har beräknat dess nytta och tagit bort kostnaderna. 

## Översikt över projektets nettovärde

Adobe Workfront beräknar nettovärdet för ett projekt med följande formel: 

```
Project Net Value = Planned Benefit - Budgeted Cost - Potential Risk Cost
```

Följande fält kan påverka ett projekts nettovärde:

* **Planerad förmån**: Detta är en manuell inmatning som anges av projektägaren när **Projektinformation** området i affärsärendet.\
   Mer information om en planerad förmån för ett projekt finns i [Projektinformation](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) avsnitt i artikeln [Översikt över affärsområdet](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* **Budgeterad kostnad**: Det här är den totala kostnaden som är associerad med projektet enligt den uppskattning du gjorde när du startade projektet första gången.

   The **Budgeterad kostnad** använder **Budgeterad arbetskostnad** det värde som beräknas i området Resursbudgetering i affärsärendet och det tar hänsyn till antalet budgeterade timmar för dina jobbroller i resursplaneraren och kostnaden per timme för varje jobbroll.\
   Budgeterad kostnad påverkar **Nettovärde** av projektet. Mer information om hur den budgeterade kostnaden beräknas finns i [Beräkna budgeterad kostnad](../../../manage-work/projects/project-finances/budgeted-cost.md).

* **Potentiell riskkostnad**: Detta är kostnaden som är associerad med eventuella risker i projektet, enligt definition i Affärsfall eller på fliken Risker i projektet.\
   Mer information om hur du beräknar den potentiella riskkostnaden för ett projekt finns i artikeln [Beräkna potentiella riskkostnader](../../../manage-work/projects/project-finances/potential-risk-cost.md).

    

## Hitta projektets nettovärde

Nettovärdet för ett projekt finns i följande områden i Workfront:

* Under Affärsärendesammanfattning \
   Mer information om området Affärsärendesammanfattning finns i avsnittet &quot;Förstå ärendesammanfattningen&quot; i artikeln [Skapa ett affärsärende för ett projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md) [Skapa ett affärsärende för ett projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

   ![](assets/net-value-on-business-case-summary-highlighted-350x444.png)

* I Portfolio-optimering om projektet är kopplat till en portfölj

   >[!TIP]
   >
   >Summan av alla projektets nettovärden är portföljens nettovärde.

   Mer information om Portfolio Optimizer finns i [Portfolio Optimizer - översikt](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* I fältet Nettovärde för projekt i följande listor och rapporter:

   * Projekt
   * Uppgift
   * Problem
   * Projekt (ekonomiska data)
   Mer information om hur du skapar en rapport finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

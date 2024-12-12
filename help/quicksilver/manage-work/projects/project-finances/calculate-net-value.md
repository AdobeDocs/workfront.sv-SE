---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Beräkna nettovärde
description: Nettovärdet för ett projekt är det sammanlagda förväntade värdet av projektet efter att man har beräknat dess nytta och tagit bort kostnaderna.
author: Lisa
feature: Work Management
exl-id: 44e3f211-c816-4ee1-aafc-c40fc8732f1a
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
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

* **Planerad förmån**: Detta är en manuell inmatning som anges av projektägaren när området **Projektinformation** i affärsärendet slutförs.\
  Mer information om den planerade fördelen med ett projekt finns i avsnittet [Projektinformation](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) i artikeln [Översikt över områden i affärsärendet](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* **Budgeterad kostnad**: Det här är den totala kostnaden som är associerad med projektet som den beräknas när du startar projektet första gången.

  Den **budgeterade kostnaden** använder värdet **Budgeterad arbetskostnad** som beräknas i området Resursbudgetering i affärsärendet och tar hänsyn till antalet timmar som budgeterats för dina jobbroller i resursplaneraren och kostnaden per timme för varje jobbroll.\
  Budgeterad kostnad påverkar projektets **nettovärde**. Mer information om hur den budgeterade kostnaden beräknas finns i [Beräkna budgeterad kostnad](../../../manage-work/projects/project-finances/budgeted-cost.md).

* **Potentiell riskkostnad**: Det här är kostnaden som är associerad med risker i projektet, så som de definieras i Affärsfall eller på fliken Risker i projektet.\
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

  Mer information om optimering av Portfolio finns i [Översikt över optimering av Portfolio](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* I fältet Nettovärde för projekt i följande listor och rapporter:

   * Projekt
   * Uppgift
   * Problem
   * Projekt (ekonomiska data)

  Mer information om hur du skapar en rapport finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Beräkna räntabilitet
description: Avkastning på investering (ROI, Return On Investment) är ett Adobe Workfront-mått som gör att portföljansvariga snabbt kan se hur projektet fungerar jämfört med projektets ursprungliga planerade förmån och budgeterade kostnad.
author: Alina
feature: Work Management
exl-id: 1a3d16cb-8cb1-472e-8102-0ea8e0bc0edd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Beräkna räntabilitet

Avkastning på investering (ROI, Return On Investment) är ett Adobe Workfront-mått som gör att portföljansvariga snabbt kan se hur projektet fungerar jämfört med projektets ursprungliga planerade förmån och budgeterade kostnad.

## Översikt över projektets avkastning på investering

Workfront beräknar avkastningen med hjälp av följande formel:

```
Project ROI = [(Project Planned Benefit - Project Budgeted Cost) / Project Budgeted Cost] x 100
```

Följande fält påverkar avkastningen på ett projekt:

* **Projektplanerad förmån**: Detta är en manuell inmatning som anges av projektägaren när området Projektinformation i affärsärendet slutförs. Det här är en uppskattning av vad du som projektägare tror kan ha nytta av projektet om du slutför projektet. Detta är ett specifikt valutabelopp och måste vara ett positivt värde.\
  Mer information om den planerade fördelen med ett projekt finns i avsnittet Projektinformation i artikeln [Skapa ett affärsärende för ett projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

* **Projektbudgeterad kostnad**: Det här är den totala kostnaden som är associerad med projektet som den beräknas när du startar projektet första gången.

  Den **budgeterade kostnaden** använder värdet **Budgeterad arbetskostnad** som beräknas i området Resursbudgetering i affärsärendet och tar hänsyn till antalet timmar som budgeterats för dina jobbroller i resursplaneraren och kostnaden per timme för varje jobbroll.\
  Mer information finns i [Beräkna budgeterad kostnad](../../../manage-work/projects/project-finances/budgeted-cost.md).

## Hitta projektets avkastning på investering

Du kan visa ROI-värdet för ett projekt i följande områden i Workfront:

* I Portfolio-optimering om projektet är kopplat till en portfölj

  >[!NOTE]
  >
  >Summan av projektets alla avkastningsvärden är portföljens avkastning.

  Mer information om optimering av Portfolio finns i artikeln [Översikt över optimering av Portfolio](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* I fältet Projektavkastning i följande listor och rapporter: 

   * Projekt
   * Uppgift
   * Problem
   * Projekt (ekonomiska data)

  Mer information om hur du skapar rapporter i Workfront finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Beräkna potentiella riskkostnader
description: I den potentiella riskkostnaden för ett projekt beaktas de potentiella kostnaderna för projektriskerna och sannolikheten för att de uppstår.
author: Alina
feature: Work Management
exl-id: f4dc1950-efd8-4936-83fd-1280ee465923
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Beräkna potentiella riskkostnader

I den potentiella riskkostnaden för ett projekt beaktas de potentiella kostnaderna för projektriskerna och sannolikheten för att de uppstår.

## Översikt över potentiella riskkostnader för ett projekt

Adobe Workfront beräknar den potentiella riskkostnaden för ett projekt med följande formel:

```
Potential Risk Cost =SUM(Potential Risk Costs * Risk Probability)
```

Tänk på följande när du ser över den potentiella riskkostnaden för ett projekt:

* Den planerade riskkostnaden för ett projekt är identisk med den potentiella riskkostnaden. 
* Den potentiella riskkostnaden ingår inte i den planerade kostnaden för ett projekt. Den används i stället för att fastställa dess nettovärde. .

## Hitta den potentiella riskkostnaden för ett projekt

Risker för ett projekt och deras potentiella kostnader finns i följande områden i Workfront:

* På fliken Risker i projektet.
* I Översikt över affärsärenden.\
   Mer information om ett projekts affärsfall finns i artikeln [Skapa ett affärsärende för ett projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).
* I en projektrapport när du lägger till fältet Planerad riskkostnad i rapportens kolumner.\
   Mer information om hur du skapar rapporter i Workfront finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* I Portfolio-optimering, när projektet är kopplat till ett Portfolio, i riskkolumnen.\
   Summan av alla potentiella riskkostnader för alla projekt i portföljen adderar till risken för Portfolio.\
   Mer information om Portfolio-optimering finns i artikeln [Portfolio Optimizer - översikt](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

Mer information om hur du skapar risker i ett projekt finns i artikeln [Skapa och redigera risker i projekt](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)

Mer information om ett projekts affärsfall finns i artikeln [Skapa ett affärsärende för ett projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

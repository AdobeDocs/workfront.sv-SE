---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: KPI-frågor
description: Förbättrade analysfrågor
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
source-git-commit: eccecaece64b78aa19444407b182ea80b2115a63
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---


# KPI-frågor

Du kan använda frågorna i den här artikeln för att skapa datavisualiseringar som liknar dem i Förbättrad analys.

>[!IMPORTANT]
>
>Frågor ger liknande resultat som de som visas i Förbättrad analys, men de kanske inte matchar exakt.


## Förutsättningar

Innan du börjar måste du

1. Skapa en anslutning till ditt Business Intelligence (BI)-verktyg:
   1. [Skapa ett läsarkonto eller en anslutning till Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)
   1. [Upprätta en anslutning till Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md)

När du har upprättat en anslutning kan du använda frågorna i den här artikeln för att extrahera och visualisera data.

## Slutförda projekt

I KPI:n för slutförda projekt visas hur många projekt inom den filtrerade tidsperioden som har slutförts samt hur procentandelen har ökat eller minskat sedan föregående tidsperiod. Under dessa siffror kan du se antalet projekt som har slutförts under den föregående tidsperioden samt antalet dagar under den föregående tidsperioden.

![KPI-projekt har slutförts](assets/kpi-projects-completed-350x182.png)

### Fråga

```
WITH completedProjectsInRange as ( 
SELECT COUNT(t0.PROJECTID) as PROJECT_COUNT FROM PROJECTS_CURRENT t0 
WHERE t0.ACTUALCOMPLETIONDATE >= '2025-01-01' 
AND t0.ACTUALCOMPLETIONDATE <= '2025-01-31' 
), completedProjectsPreviousRange as ( 
SELECT COUNT(t0.PROJECTID) as PROJECT_COUNT FROM PROJECTS_CURRENT t0 
WHERE t0.ACTUALCOMPLETIONDATE >= '2024-12-01' 
AND t0.ACTUALCOMPLETIONDATE <= '2024-12-31' 
), rawChange as ( 
SELECT (a.PROJECT_COUNT - b.PROJECT_COUNT) as CHANGE_FROM_PREVIOUS_PERIOD FROM completedProjectsInRange a, completedProjectsPreviousRange b 
), percentChange as ( 
SELECT  
CASE 
WHEN a.PROJECT_COUNT = b.PROJECT_COUNT THEN 0.00 
WHEN b.PROJECT_COUNT > 0 THEN ((a.PROJECT_COUNT - b.PROJECT_COUNT) / b.PROJECT_COUNT * 100) 
END AS PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
FROM completedProjectsInRange a, completedProjectsPreviousRange b 
) 
SELECT 
a.PROJECT_COUNT, 
b.PROJECT_COUNT as PREVIOUS_PROJECT_COUNT, 
c.CHANGE_FROM_PREVIOUS_PERIOD, 
d.PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
FROM completedProjectsInRange a, completedProjectsPreviousRange b, rawChange c, 
percentChange d
```

## Projekt slutförda i tid

I KPI för projekt som slutförts i tid visas hur stor andel projekt inom den filtrerade tidsperioden som har slutförts i tid samt hur procentandelen har ökat eller minskat sedan föregående tidsperiod. Under dessa siffror kan du se hur många projekt som har slutförts i tid under den föregående tidsperioden samt antalet dagar under den föregående tidsperioden.

![KPI-projekt slutförda i tid](assets/kpi-projects-completed-on-time-350x180.png)

## Medel. projektvaraktighet

Den genomsnittliga. KPI för projektvaraktighet visar den genomsnittliga slutförandetiden - i dagar, veckor eller år - för projekt med faktiska slutdatum inom den filtrerade tidsperioden samt hur procentandelen har ökat eller minskat sedan föregående tidsperiod. Under dessa siffror kan du se den genomsnittliga slutförandetiden för projekt med faktiska slutdatum under den föregående tidsperioden samt antalet dagar under den föregående tidsperioden.

![Genomsnittlig projektvaraktighet för KPI](assets/kpi-avg.-project-duration-350x168.png)

## Genomsnittliga uppgifter per projekt

I Genomsn, uppgifter per projekt-KPI visas det genomsnittliga antalet uppgifter som tilldelats projekt inom den filtrerade tidsperioden samt hur procentandelen ökade eller minskade sedan föregående tidsperiod. Under dessa nummer kan du se det genomsnittliga antalet uppgifter som tilldelats projekt under den föregående tidsperioden samt antalet dagar under den föregående tidsperioden.

![KPI-genomsnittsuppgifter per projekt](assets/kpi-average-tasks-per-project-350x179.png)
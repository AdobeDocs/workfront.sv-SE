---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Frågor om projekttreemap
description: Förbättrade analysfrågor
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 3943703a-0d0b-46d3-a708-52987d330523
source-git-commit: bd39c5794c55e27a876da185e67bf8c654a003b2
workflow-type: tm+mt
source-wordcount: '110'
ht-degree: 0%

---

# Frågor om projekttreemap

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

## Planerade timmar för projekt som pensionerats

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        workrequired, 
        percentcomplete, 
        calendardate, 
        (workrequired - (workrequired * percentcomplete)) as remainingMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.workrequired) as projectTotalWork, 
    sum(tdw.remainingMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```

### Planerade timmar för projekt som pensionerats: nedbränning

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        workrequired, 
        percentcomplete, 
        calendardate, 
        (workrequired - (workrequired * percentcomplete)) as remainingMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.workrequired) as projectTotalWork, 
    sum(tdw.remainingMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```

## Projektets planerade varaktighet har tagits bort 

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        planneddurationminutes, 
        percentcomplete, 
        calendardate, 
        (planneddurationminutes - (planneddurationminutes * percentcomplete)) as remainingDurationMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.planneddurationminutes) as projectTotalWork, 
    sum(tdw.remainingDurationMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```

### Projektets planerade varaktighet har tagits bort: nedladdning

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        planneddurationminutes, 
        percentcomplete, 
        calendardate, 
        (planneddurationminutes - (planneddurationminutes * percentcomplete)) as remainingDurationMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.planneddurationminutes) as projectTotalWork, 
    sum(tdw.remainingDurationMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```

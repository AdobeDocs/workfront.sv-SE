---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Exempel på frågor om dataanslutning
description: Exempelfrågor som du kan använda för att bekanta dig med syntaxen och strukturen för specifika typer av frågor.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: 16809b2d1801dd7aa4ab1f452e4687601fc1ac59
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Exempel på Workfront Data Connect-frågor

För att du bättre ska kunna utnyttja dina Workfront Data Connect-data innehåller den här sidan enkla exempelfrågor som du kan använda för att bekanta dig med syntaxen och strukturen för specifika typer av frågor.

## Anpassad datafråga

I det här exemplet visas hur du kan skapa en fråga som returnerar anpassade data i Workfront, till exempel anpassade formulär och anpassade fält.

### Scenario

Din organisation, PeopleSoft, använder ett anpassat formulär som heter Finance Integration. Formuläret är kopplat till varje projekt och innehåller följande fält:

* **PeopleSoft Business Unit** - Ett anpassat fält som innehåller en sträng.
* **PeopleSoft ProjectID** - Ett anpassat fält som innehåller en numerisk sträng.
* **Utökat projektnamn** - Ett beräknat anpassat datafält som sammanfogar värdena för PeopleSoft Business Unit, PeopleSoft ProjectID och Workfront-projektnamnet i en enda sträng.

Du måste inkludera den här informationen i svaret på en fråga mot Data Connect. Anpassade datavärden för en post i datasjön finns i kolumnen `parameterValues`. Den här kolumnen lagras som ett JSON-objekt.

### Fråga:

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:PeopleSoft Business Unit" :: int as PeopleSoftBusinessUnit,
    parametervalues:"DE:PeopleSoft Project ID" :: int as PeopleSoftProjectID,
    parametervalues:"DE:Expanded Project Name" :: text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### Svar

Frågan ovan returnerar följande data:

* `projectid` - det inbyggda Workfront-projekt-ID:t
* `parametervalues` - en kolumn som lagrar ett JSON-objekt
* `name` - Workfront egna projektnamn
* `PeopleSoft Business Unit` - ett anpassat datavärde som ingår i objektet `parametervalues`
* `PeopleSoft Project ID` - ett anpassat datavärde som ingår i objektet `parametervalues`
* `Expanded Project Name` - ett anpassat datavärde som ingår i objektet `parametervalues`

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->

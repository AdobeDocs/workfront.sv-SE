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
source-git-commit: 364b668f23f5437e5cca0c4cc4793b17d444fb56
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Exempel på Workfront Data Connect-frågor

För att du bättre ska kunna utnyttja dina Workfront Data Connect-data innehåller den här sidan enkla exempelfrågor som du kan använda för att bekanta dig med syntaxen och strukturen för specifika typer av frågor.

## Anpassad datafråga

I det här exemplet visas hur du kan skapa en fråga som returnerar anpassade data i Workfront, till exempel anpassade formulär och anpassade fält.

### Scenario

Din organisation använder ett anpassat formulär som heter Finance Integration. Formuläret är kopplat till varje projekt och innehåller följande fält:

* **Affärsenhet** - Ett anpassat fält som innehåller en sträng.
* **ProjectID** - Ett anpassat fält som innehåller en numerisk sträng.
* **Utökat projektnamn** - Ett beräknat anpassat datafält som sammanfogar värdena för affärsenhet, projekt-ID och Workfront-projektnamnet i en enda sträng.

Du måste inkludera den här informationen i svaret på en fråga mot Data Connect. Anpassade datavärden för en post i datasjön finns i kolumnen `parametervalues`. Den här kolumnen lagras som ett JSON-objekt.

### Fråga:

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:Business Unit"::int as BusinessUnit,
    parametervalues:"DE:Project ID"::int as ProjectID,
    parametervalues:"DE:Expanded Project Name"::text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### Svar:

Frågan ovan returnerar följande data:

* `projectid` - det inbyggda Workfront-projekt-ID:t
* `parametervalues` - en kolumn som lagrar ett JSON-objekt
* `name` - Workfront egna projektnamn
* `Business Unit` - ett anpassat datavärde som ingår i objektet `parametervalues`
* `Project ID` - ett anpassat datavärde som ingår i objektet `parametervalues`
* `Expanded Project Name` - ett anpassat datavärde som ingår i objektet `parametervalues`

### Förklaring:

När du frågar JSON-objektet `parametervalues` kan du komma åt varje anpassat datafält som en kolumn med hjälp av följande:

`<field_name>:"<parameter_name>"::<data_type> as <column_name>`

* `<field_name>` är namnet på JSON-objektet i tabellen som efterfrågas. För anpassade data är detta alltid `parametervalues`.
* `<parameter_name>` är strängen `parametername` som finns i formulärkonfigurationsverktyget, men den kanske inte alltid matchar det här värdet.

>[!NOTE]
>
>Om parameterns namn ändras i Workfront formulärkonfigurationsverktyg representeras det som en ny kolumn i JSON-objektet. Därför rekommenderar vi att du inte ändrar namnet på en kolumn när den har skapats i formulärkonfigurationsverktyget. Etiketten kan dock ändras utan att JSON-objektet påverkas.
>
>Om textsträngen för parameternamnet är felaktig returnerar kolumnen ett NULL-värde i stället för ett fel.

* `<data_type>` konverterar värdet som returneras från JSON-objektet till en datatyp som passar fältet. Om du väljer en inkompatibel datatyp för det värde som returneras resulterar det i ett felmatchningsfel för datatypen. Möjliga datatyper är:

   * `text`
   * `varchar`
   * `int`
   * `float`
   * `number(len,precision)` (t.ex. `Number(32,4)` returnerar 1234,0987)
   * `date`
   * `timestamp`

* `<column_name>` är den etikett du skapar för varje anpassad datakolumn.

>[!NOTE]
>
>Endast parametrar som har värden tilldelade till sig i formuläret inkluderas i JSON-objektet. Om ett anpassat datafält är tomt i formuläret visas det inte.

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->

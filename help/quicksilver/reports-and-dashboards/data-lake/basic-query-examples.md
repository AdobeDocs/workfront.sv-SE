---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Exempel på frågor om dataanslutning
description: Exempelfrågor som du kan använda för att bekanta dig med syntaxen och strukturen för specifika typer av frågor.
author: Nolan
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: c8a25bcc8c9b56a649ca7764918c86f9cdd5b3e2
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 0%

---

# Exempel på Workfront Data Connect-frågor

För att du bättre ska kunna utnyttja dina Workfront Data Connect-data innehåller den här sidan enkla exempelfrågor som du kan använda för att bekanta dig med syntaxen och strukturen för specifika typer av frågor.

## Anpassad datafråga

I det här exemplet visas hur du kan skapa en fråga som returnerar anpassade data i Workfront, till exempel anpassade formulär och anpassade fält.

### Scenario

Din organisation använder ett anpassat formulär som heter Finance Integration. Formuläret är kopplat till varje projekt och innehåller följande fält:

* **Affärsenhet**: Ett anpassat fält som innehåller en sträng.
* **ProjectID**: Ett anpassat fält som innehåller en numerisk sträng.
* **Utökat projektnamn**: Ett beräknat anpassat datafält som sammanfogar värdena för affärsenheten, ProjectID och Workfront-projektnamnet i en enda sträng.

Du måste inkludera den här informationen i svaret på en fråga mot Data Connect. Anpassade datavärden för en post i datasjön finns i kolumnen `parametervalues`. Den här kolumnen lagras som ett JSON-objekt.

### Fråga

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

### Svar

Frågan ovan returnerar följande data:

* `projectid`: Det inbyggda Workfront-projekt-ID:t.
* `parametervalues`: En kolumn som lagrar ett JSON-objekt.
* `name`: Workfront egna projektnamn.
* `Business Unit`: Ett anpassat datavärde som ingår i objektet `parametervalues`.
* `Project ID`: Ett anpassat datavärde som ingår i objektet `parametervalues`.
* `Expanded Project Name`: Ett anpassat datavärde som ingår i objektet `parametervalues`.

### Förklaring

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

## Tid i statusfråga

I det här exemplet visas hur du mäter tiden som ett projekt har tillbringats i tidigare tilldelade statusar. Den kan enkelt anpassas för att mäta aktivitet eller utgivningstid i en status eller anpassas för att mäta hur länge ett objekt har andra attribut (inklusive anpassade datavärden) tillämpade.

### Scenario

Företagets ledning tror att ni spenderar för mycket tid i varje steg i arbetscykeln. Innan du ger rekommendationer om hur processen ska förbättras, vill du skapa ett baslinjemått för hur ofta en projektstatus ändras över tid och hur många dagar ett projekt behåller en viss status.

Du kommer att använda datavyn PROJECTS_EVENT för att hämta en lista över varje statusändring mot projektobjektet. Du kommer att jämföra den nya statusen med den tidigare statusen, ta reda på det gällande tidsintervallet för den tidigare tilldelade statusen och sedan beräkna antalet dagar som har tillbringats i den statusen.

Med hjälp av den här obearbetade tidsåtgången för varje status per projekt kan du börja skapa visualiseringar eller lägga samman data ytterligare för att skapa tidsmedelvärden för status efter status, projekttyp eller tid på året. Baslinjen används sedan för att ange ett riktmärke som ni kan mäta er mot för att uppfylla era ledarskaps förväntningar.

Följande fråga använder datavyn Data Connect PROJECTS_EVENTS för att jämföra varje händelse för statusändring och visa tiden i status.

### Fråga

```
-- Calculate the begin/end effective timestamp and duration in days 

SELECT 

    projectid, 
    name as project_name, 
    prev_status as previous_status, 
    status, 
    status_change_date as status_begin_effective_timestamp, 
    case 
        when status_change_date is null then NULL
        else
            nvl(lead(status_change_date) ignore nulls over (partition by projectid order by status_change_date), current_timestamp) 
    end as status_end_effective_timestamp, 
    datediff('DAYS',status_change_date, nvl(lead(status_change_date) ignore nulls over (partition by projectid order by status_change_date), current_timestamp)) as status_duration_days 

FROM 
    ( -- Filter to just the records that have changed 
     SELECT projectid, 
        name, 
        prev_status, 
        status, 
        begin_effective_timestamp as status_change_date    
     FROM 
        (  -- Calculate records where previous status is different 
          SELECT DISTINCT  
           pe.projectid, 
           pe.name AS name, 
           pe.STATUS, 
           nvl(lag(pe.STATUS) over (partition by pe.projectid order by pe.BEGIN_EFFECTIVE_TIMESTAMP), status) prev_status, 
           begin_effective_timestamp 

          FROM projects_event pe 
         -- Set any WHERE conditions to limit the results as needed 
         --WHERE 
            -- pe.PROJECTID = '5ebe…c1e1' 
        ) 
        WHERE prev_status != status 
    ) 
    order by status_change_date; 
```

### Svar

Frågan ovan returnerar följande data:

* `PROJECTID`: Det projekt-ID för Workfront som är associerat med statusändringshändelsen.
* `PROJECT_NAME`: Workfront-projektnamnet.
* `PREVIOUS_STATUS`: Projektets status omedelbart före ändringen.
* `STATUS`: Projektets status efter ändringen.
* `STATUS_BEGIN_EFFECTIVE_TIMESTAMP`: Tidsstämpeln för ändringshändelsen när föregående status angavs.
* `STATUS_END_EFFECTIVE_TIMESTAMP`: Tidsstämpeln för ändringshändelsen när det uppdaterade statusvärdet angavs.
* `STATUS_DURATION_DAYS`: Skillnaden (i dagar) mellan den sista gällande tidsstämpeln och den första effektiva tidsstämpeln.

### Förklaring

Frågan använder Data Connect:s funktioner för händelsespårning.  Det avgör vilket datum en händelse med ett nytt statusvärde som skiljer sig från den tidigare händelsen utlöstes. 

Undersöker frågan inifrån och ut: 

1. Beräkna poster där föregående status är annorlunda: 
   * För varje change-händelse använder du funktionen lag() för att identifiera det tidigare statusvärdet. 

2. Filtrera till bara de poster som har ändrats: 

   * Välj poster från beräkning i steg 1 där föregående status != aktuell status. 

3. Beräkna tidsstämpeln för start/slut och varaktighet i dagar: 

   * `<status_begin_effective_timestamp>`: Beräknas i steg 2. 

   * `<status_end_effective_timestamp>`: Beräknas utifrån nästa (lead()). `<status_begin_effective_timestamp>`: Visa bara statusen om `<status_begin_effective_timestamp>` INTE är NULL. 
   * `<status_duration_days>`: Dataskillnad mellan `<status_begin_effective_timestamp>` och `<status_end_effective_timestamp>`. 

>[!NOTE]
>
>Vi rekommenderar att du använder den här frågan som en egen&quot;vy&quot; i PowerBI eller Tableau.  Om du vill hämta in andra fält från `<object>_event view` ansluter du resultatet från den här frågan till `<object>_event view`.  Kopplingsfälten blir följande: <br>
>>For projects_event: 
>>`From projects_event p`
>>`Join <above query> c on c.projectid = p.projectid  `
>>`and c. status_begin_effective_timestamp = p begin_effective_timestamp`



<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->

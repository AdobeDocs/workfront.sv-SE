---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: Data Lake Data-ordlista
description: Den här sidan innehåller information om datastrukturen och innehållet i Workfront datasjön.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: 81f8477dd26b828c4255c678b36d98789cd81ff8
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 0%

---

# Workfront Data Lake Data Didictionary

Den här sidan innehåller information om datastrukturen och innehållet i Workfront datasjön.

>[!NOTE]
>
>Data i Workfront Data Lake uppdateras var fjärde timme, så de senaste ändringarna kanske inte omedelbart återspeglas.

## Tabelltyper

Det finns ett antal tabelltyper som du kan använda för att visa dina Workfront-data på ett sätt som ger dig den mest insikt.

* **Aktuell tabell**

  I den aktuella tabellen visas data på ungefär samma sätt som i Workfront, alla objekt och det aktuella läget. Den kan navigeras med mycket lägre latens än inom Workfront.

* **Händelsetabell**

  Händelsetabellen spårar alla ändringsposter i Workfront: det vill säga varje gång ett objekt ändras skapas en post som visar när ändringen inträffade, vem som gjorde ändringen och vad som ändrades. Den här tabellen är därför användbar för jämförelser vid olika tidpunkter. Denna tabell innehåller endast poster från de senaste tre åren.

* **Daglig historiktabell**

  Tabellen Daglig historik innehåller en förkortad version av tabellen Event, eftersom den visar varje objekts tillstånd dagligen i stället för när varje enskild händelse inträffade. Den här tabellen är därför användbar för trendanalys.

<!-- Custom table -->

## Enhetsrelationsdiagram

Objekt i Workfront (och därför i din datalinje) definieras inte bara av deras individuella värden, utan av deras relationer med andra objekt. I entitetsrelationsdiagrammet nedan finns en mappning på hög nivå av objektrelationer i Workfront datasjön. Diagrammet kan visas och laddas ned via följande länk:

[Workfront Data Lake Entity Relations Diagram](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

>[!IMPORTANT]
>
>Entitetsrelationsdiagrammet är ett pågående arbete - därför är det bara till för referens och kan ändras.

## Datumtyper

Det finns ett antal datumobjekt som ger information om när specifika händelser inträffar.

* `DL_LOAD_TIMESTAMP`: Det här datumet används för intern referens och reflekteras när data lästes in i tabellen Aktuell, Händelse eller Daglig historik. Detta datum ska inte användas för dataanalys och ska tas bort under betaversionen av Workfront Data Lake.
* `CALENDAR_DATE`: Det här datumet finns bara i tabellen Daglig historik. Den här tabellen innehåller information om hur data ser ut vid 11:59 UTC för varje datum som anges i `CALENDAR_DATE`.
* `BEGIN_EFFECTIVE_TIMESTAMP`: Det här datumet finns både i tabellerna Händelse och Dagshistorik, och det registreras exakt när en post ändrade värdet _till_ på den aktuella raden.
* `END_EFFECTIVE_TIMESTAMP`: Det här datumet finns i tabellerna Händelse och Daglig historik, och det registreras exakt när en post ändrade värdet _från_ i den aktuella raden till ett värde i en annan rad. För att tillåta mellan frågor på `BEGIN_EFFECTIVE_TIMESTAMP` och `END_EFFECTIVE_TIMESTAMP` är det här värdet aldrig null, även om det inte finns något nytt värde. Om en post fortfarande är giltig (d.v.s. värdet inte har ändrats) har `END_EFFECTIVE_TIMESTAMP` värdet 2300-01-01.

## Terminologisk tabell

Följande tabell korrelerar objektnamn i Workfront (samt deras namn i gränssnittet och API) med deras motsvarande namn i datasjön.

<table>
<thead>
  <tr>
    <th>Workfront entitetsnamn</th>
    <th>Gränssnittsreferenser</th>
    <th>API-referens | Etikett</th>
    <th>Data Lake-tabeller</th>
    <th>Anteckningar</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Tilldelning</td>
    <td>Tilldelning</td>
    <td>ASSGN | Tilldelning</td>
    <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>CustomEnum</td>
    <td>Villkor, Prioritet, Allvarlighetsgrad, Status</td>
    <td>CSTEM | Anpassad uppräkning</td>
    <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT</td>
    <td>Posttypen identifieras med egenskapen enumClass. Följande typer förväntas:<br>CONDITION_OPTASK<br>CONDITION_PROJ<br>CONDITION_TASK<br>PRIORITY_OPTASK<br>PRIORITY_PROJ<br>PRIORITY_TASK<br>SEVERITY_OPTASK<br>STATUS_OPTASK<br>STATUS_PROJ<br>STATUS_TAUS SK</td>
  </tr>
  <tr>
    <td>Dokument</td>
    <td>Dokument</td>
    <td>DOCU | Dokument</td>
    <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT<br><br>DOCUMENTS_CUSTOM_VALUE_CURRENT<br>DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>DOCUMENTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>DocumentVersion</td>
    <td>Dokumentversion</td>
    <td>DOCV | Dokumentversion</td>
    <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Grupp</td>
    <td>Grupp</td>
    <td>GRUPP | Grupp</td>
    <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Timme</td>
    <td>Timme</td>
    <td>TIMME | Timme</td>
    <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Timtyp</td>
    <td>Timtyp</td>
    <td>TID | Timtyp</td>
    <td>HOURTYPES_CURRENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Milstolpe</td>
    <td>Milstolpe</td>
    <td>MILE | Milstolpe</td>
    <td>MILESTONES_CURRENT<br>MILESTONES_DAILY_HISTORY<br>MILESTONES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>MilstolpePath</td>
    <td>Sökväg för milstolpe</td>
    <td>MPATH | Sökväg för milstolpe</td>
    <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Anteckning</td>
    <td>Anteckning</td>
    <td>ANMÄRKNING | Anteckning</td>
    <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>OpTask</td>
    <td>Problem, begäran</td>
    <td>OPTASK | Problem</td>
    <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT<br><br>OPTASKS_CUSTOM_VALUE_CURRENT<br>OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>OPTASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Portfolio</td>
    <td>Portfolio</td>
    <td>PORT | Portfolio</td>
    <td>PORTFOLIO_CURRENT<br>PORTFOLIO_DAILY_HISTORY<br>PORTFOLIO_EVENT<br><br>PORTFOLIO_CUSTOM_VALUE_CURRENT<br>PORTFOLIO_CUSTOM_VALUE_DAILY_HISTORY<br>PORTFOLIO_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Program</td>
    <td>Program</td>
    <td>PRGM | Program</td>
    <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT<br><br>PROGRAMS_CUSTOM_VALUE_CURRENT<br>PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>PROGRAMS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Projekt</td>
    <td>Projekt</td>
    <td>PROJ | Projekt</td>
    <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT<br><br>PROJECTS_CUSTOM_VALUE_CURRENT<br>PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>PROJECTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Roll</td>
    <td>Jobbroll</td>
    <td>ROLE | Jobbroll</td>
    <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Schema</td>
    <td>Schema</td>
    <td>SCHED | Schema</td>
    <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Uppgift</td>
    <td>Uppgift</td>
    <td>UPPGIFT | Uppgift</td>
    <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT<br><br>TASKS_CUSTOM_VALUE_CURRENT<br>TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>TASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Team</td>
    <td>Team</td>
    <td>TEAMOB | Team</td>
    <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Tidrapport</td>
    <td>Tidrapport</td>
    <td>TSTIPSE | Tidrapport</td>
    <td>TIMESHEETS_CURRENT<br>TIMESHEETS_DAILY_HISTORY<br>TIMESHEETS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Användare</td>
    <td>Användare</td>
    <td>ANVÄNDARE | Användare</td>
    <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT<br><br>USERS_CUSTOM_VALUE_CURRENT<br>USERS_CUSTOM_VALUE_DAILY_HISTORY<br>USERS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
</tbody>
</table>

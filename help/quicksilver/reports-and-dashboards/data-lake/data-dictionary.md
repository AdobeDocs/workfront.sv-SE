---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: Data Lake Data-ordlista
description: Den här sidan innehåller information om datastrukturen och innehållet i Workfront datasjön.
author: Nolan
feature: Reports and Dashboards
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: c82f70c78bc23f69bed2351a67c2e0d0bac9e973
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---

# Workfront Data Lake Data Didictionary

Den här sidan innehåller information om datastrukturen och innehållet i Workfront datasjön.

>[!NOTE]
>
>Data i Workfront Data Lake uppdateras var fjärde timme, så de senaste ändringarna kanske inte omedelbart återspeglas.

## Tabelltyper

Det finns ett antal tabelltyper som du kan använda för att visa dina Workfront-data på ett sätt som ger dig den mest insikt.

### Aktuell tabell

I den aktuella tabellen visas data på ungefär samma sätt som i Workfront, alla objekt och det aktuella läget. Den kan navigeras med mycket lägre latens än inom Workfront.

### Händelsetabell

Händelsetabellen spårar alla ändringsposter i Workfront: det vill säga varje gång ett objekt ändras skapas en post som visar när ändringen inträffade, vem som gjorde ändringen och vad som ändrades. Den här tabellen är därför användbar för jämförelser vid olika tidpunkter. Denna tabell innehåller endast poster från de senaste tre åren.

### Daglig historiktabell

Tabellen Daglig historik innehåller en förkortad version av tabellen Event, eftersom den visar varje objekts tillstånd dagligen i stället för när varje enskild händelse inträffade. Den här tabellen är därför användbar för trendanalys.

<!-- Custom table -->

## Enhetsrelationstabell

I följande tabell korreleras objektnamnen i Workfront (samt deras namn i gränssnittet och API:t) med deras motsvarande namn i datarutan.

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
    <td>ASSIGNMENTS_CURRENT<br>     ASSIGNMENTS_DAILY_HISTORY<br>     ASSIGNMENTS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>CustomEnum</td>
    <td>Villkor, Prioritet, Allvarlighetsgrad, Status</td>
    <td>CSTEM | Anpassad uppräkning</td>
    <td>CUSTOMENUMS_CURRENT<br>     CUSTOMENUMS_DAILY_HISTORY<br>     CUSTOMENUMS_EVENT</td>
    <td>Posttypen identifieras med egenskapen enumClass. Följande typer förväntas:<br>     CONDITION_OPTASK<br>     CONDITION_PROJ<br>     CONDITION_TASK<br>     PRIORITY_OPTASK<br>     PRIORITY_PROJ<br>     PRIORITY_TASK<br>     SEVERITY_OPTASK<br>     STATUS_OPTASK<br>     STATUS_PROJ<br>     STATUS_TASK</td>
  </tr>
  <tr>
    <td>Dokument</td>
    <td>Dokument</td>
    <td>DOCU | Dokument</td>
    <td>DOCUMENTS_CURRENT<br>     DOCUMENTS_DAILY_HISTORY<br>     DOCUMENTS_EVENT<br>     <br>     DOCUMENTS_CUSTOM_VALUE_CURRENT<br>     DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>     DOCUMENTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>DocumentVersion</td>
    <td>Dokumentversion</td>
    <td>DOCV | Dokumentversion</td>
    <td>DOCUMENTVERSIONS_CURRENT<br>     DOCUMENTVERSIONS_DAILY_HISTORY<br>     DOCUMENTVERSIONS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Grupp</td>
    <td>Grupp</td>
    <td>GRUPP | Grupp</td>
    <td>GROUPS_CURRENT<br>     GROUPS_DAILY_HISTORY<br>     GROUPS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Timme</td>
    <td>Timme</td>
    <td>TIMME | Timme</td>
    <td>HOURS_CURRENT<br>     HOURS_DAILY_HISTORY<br>     HOURS_EVENT</td>
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
    <td>MILESTONES_CURRENT<br>     MILESTONES_DAILY_HISTORY<br>     MILESTONES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>MilstolpePath</td>
    <td>Sökväg för milstolpe</td>
    <td>MPATH | Sökväg för milstolpe</td>
    <td>MILESTONEPATHS_CURRENT<br>     MILESTONEPATHS_DAILY_HISTORY<br>     MILESTONEPATHS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Anteckning</td>
    <td>Anteckning</td>
    <td>ANMÄRKNING | Anteckning</td>
    <td>NOTES_CURRENT<br>     NOTES_DAILY_HISTORY<br>     NOTES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>OpTask</td>
    <td>Problem, begäran</td>
    <td>OPTASK | Problem</td>
    <td>OPTASKS_CURRENT<br>     OPTASKS_DAILY_HISTORY<br>     OPTASKS_EVENT<br>     <br>     OPTASKS_CUSTOM_VALUE_CURRENT<br>     OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>     OPTASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Portfolio</td>
    <td>Portfolio</td>
    <td>PORT | Portfolio</td>
    <td>PORTFOLIO_AKTUELL<br>     PORTFOLIO_DAILY_HISTORY<br>     PORTFOLIO_EVENT<br>     <br>     PORTFOLIO_CUSTOM_VALUE_CURRENT<br>     PORTFOLIO_CUSTOM_VALUE_DAILY_HISTORY<br>     PORTFOLIO_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Program</td>
    <td>Program</td>
    <td>PRGM | Program</td>
    <td>PROGRAMS_CURRENT<br>     PROGRAMS_DAILY_HISTORY<br>     PROGRAMS_EVENT<br>     <br>     PROGRAMS_CUSTOM_VALUE_CURRENT<br>     PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>     PROGRAMS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Projekt</td>
    <td>Projekt</td>
    <td>PROJ | Projekt</td>
    <td>PROJECTS_CURRENT<br>     PROJECTS_DAILY_HISTORY<br>     PROJECTS_EVENT<br>     <br>     PROJECTS_CUSTOM_VALUE_CURRENT<br>     PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>     PROJECTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Roll</td>
    <td>Jobbroll</td>
    <td>ROLE | Jobbroll</td>
    <td>ROLES_CURRENT<br>     ROLES_DAILY_HISTORY<br>     ROLES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Schema</td>
    <td>Schema</td>
    <td>SCHED | Schema</td>
    <td>SCHEDULES_CURRENT<br>     SCHEDULES_DAILY_HISTORY<br>     SCHEDULES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Uppgift</td>
    <td>Uppgift</td>
    <td>UPPGIFT | Uppgift</td>
    <td>TASKS_CURRENT<br>     TASKS_DAILY_HISTORY<br>     TASKS_EVENT<br>     <br>     TASKS_CUSTOM_VALUE_CURRENT<br>     TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>     TASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Team</td>
    <td>Team</td>
    <td>TEAMOB | Team</td>
    <td>TEAMS_CURRENT<br>     TEAMS_DAILY_HISTORY<br>     TEAMS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Tidrapport</td>
    <td>Tidrapport</td>
    <td>TSTIPSE | Tidrapport</td>
    <td>TIMESHEETS_CURRENT<br>     TIMESHEETS_DAILY_HISTORY<br>     TIMESHEETS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Användare</td>
    <td>Användare</td>
    <td>ANVÄNDARE | Användare</td>
    <td>USERS_CURRENT<br>     USERS_DAILY_HISTORY<br>     USERS_EVENT<br>     <br>     USERS_CUSTOM_VALUE_CURRENT<br>     USERS_CUSTOM_VALUE_DAILY_HISTORY<br>     USERS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
</tbody>
</table>
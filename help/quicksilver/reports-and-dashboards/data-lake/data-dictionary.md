---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Connect-dataordlista
description: Den här sidan innehåller information om datastrukturen och innehållet i Workfront Data Connect.
author: Courtney
feature: Reports and Dashboards
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: c669086f5954f9e2cf850887f4100e53c0c3e716
workflow-type: tm+mt
source-wordcount: '8904'
ht-degree: 1%

---

# Workfront Data Connect-dataordlista

Den här sidan innehåller information om datastrukturen och innehållet i Workfront Data Connect.

>[!NOTE]
>
>Data i Data Connect uppdateras var fjärde timme, så de senaste ändringarna kanske inte återspeglas direkt.

## Vytyper

Det finns ett antal visningstyper som du kan använda i Data Connect för att visa dina Workfront-data på ett sätt som ger dig den bästa insikten.

* **Aktuell vy**

  I den aktuella vyn visas data på ungefär samma sätt som i Workfront, alla objekt och det aktuella läget. Den kan navigeras med mycket lägre latens än inom Workfront.

* **Händelsevy**

  Händelseläget spårar alla ändringsposter i Workfront: varje gång ett objekt ändras skapas en post som visar när ändringen inträffade, vem som gjorde ändringen och vad som ändrades. Den här vyn är därför användbar för jämförelser vid olika tidpunkter. Den här vyn innehåller endast poster från de senaste tre åren.

* **Vyn Daglig historik**

  Vyn Daglig historik innehåller en förkortad version av händelsevyn, eftersom den visar varje objekts tillstånd varje dag i stället för när varje enskild händelse inträffar. Den här vyn är därför användbar för trendanalys.

<!-- Custom view -->

## Entitetsrelationsdiagram

Objekt i Workfront (och därför i Data Connect-datavinen) definieras inte bara av deras individuella värden, utan av deras relationer med andra objekt.

Enhetsrelationsdiagrammen nedan tillhandahåller en mappning på hög nivå av objektrelationer i Data Connect för viktiga Workfront-objekt.

>[!IMPORTANT]
>
>Diagrammen är centrerade kring enskilda objekt och representerar inte ett fullständigt entitetsrelationsdiagram för hela Workfront-programmet. <br>
>Dessa diagram är avsedda att innehålla exempel på hur relationerna kan användas för att koppla data till närliggande objekt.

### Exempel på entitetsrelationsdiagram

+++ Expandera för att visa exempeldiagrammen

>[!TIP]
>
>Om du vill visa ett diagram mer detaljerat högerklickar du på bilden och väljer **Öppna bild på den nya fliken**.


### Uppdrag

![Tilldelningarnas entitetsrelationsdiagram](assets/Assignment-centered-ERD.png)


### Godkännanden av dokument och dokument

![Enhetsrelationsdiagram för dokument och dokumentgodkännande](assets/Document-and-Document-Approvals-centered-ERD.png)

### Timmar och tidrapporter

![Timmar och tidrapporter, entitetsrelationsdiagram](assets/Hours-and-Timesheet-centered-ERD.png)


### Problem

![Utfärdar entitetsrelationsdiagram](assets/Issue-centered-ERD.png)

### Projekt

![Affärsenhetsrelationsdiagram för projekt](assets/Project-centered-ERD.png)


### Uppgifter

![Affärsenhetsrelationsdiagram för uppgifter](assets/Task-centered-ERD.png)


### Användare

![Relationsdiagram för användarentitet](assets/User-centered-ERD.png)

+++

## Datumtyper

Det finns ett antal datumobjekt som ger information om när specifika händelser inträffar.

* `DL_LOAD_TIMESTAMP`: Det här datumet uppdateras när en datauppdatering har slutförts och innehåller tidsstämpeln för när uppdateringsjobbet som skickade den senaste versionen av en post påbörjades.
* `CALENDAR_DATE`: Det här datumet finns bara i vyn Daglig historik. Vyn Daglig historik visar hur data ser ut vid :59 `CALENDAR_DATE` UTC för varje datum som anges i .
* `BEGIN_EFFECTIVE_TIMESTAMP`: Det här datumet finns både i vyn Händelse och Daglig historik och representerar den tid då en post blir det aktuella värdet i programmet.
* `END_EFFECTIVE_TIMESTAMP`: Det här datumet finns både i vyerna Händelse och Daglig historik, och det registreras exakt när en post har ändrat _från_ värdet i den aktuella raden till ett värde i en annan rad. För att tillåta mellan frågor på `BEGIN_EFFECTIVE_TIMESTAMP` och `END_EFFECTIVE_TIMESTAMP` är det här värdet aldrig null, även om det inte finns något nytt värde. Om en post fortfarande är giltig (d.v.s. värdet inte har ändrats) har `END_EFFECTIVE_TIMESTAMP` värdet 2300-01-01.

## Terminologisk tabell

Följande tabell korrelerar objektnamn i Workfront (samt deras namn i gränssnittet och API) med deras motsvarande namn i Data Connect, och innehåller referensfält för varje objekt till andra Workfront-objekt.

>[!NOTE]
>
>Nya fält kan läggas till i objektvyerna utan föregående meddelande för att stödja datautvecklingen i Workfront-programmet. Vi varnar för att använda SELECT-frågor där den underordnade datamottagaren inte är beredd att hantera ytterligare kolumner när de läggs till.<br>
>Om du behöver byta namn på eller ta bort en kolumn visas ett meddelande om dessa ändringar.

### Åtkomstnivå

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Åtkomstnivå</td>
            <td>Åtkomstnivå</td>
            <td>ACSLVL</td>
            <td>Åtkomstnivå</td>
            <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSLEVELID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>APPGLOBALID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LEGACYACCESSLEVELID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på OBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i OBJCODE-fältet</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Åtkomstregel

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Åtkomstregel</td>
            <td>Dela</td>
            <td>ACSRUL</td>
            <td>Dela</td>
            <td>ACCESSREGLER_CURRENT<br>ACCESSREGLER_DAILY_HISTORY<br>ACCESSREGLER_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSORID</td>
             <td>FK</td>
             <td>Variabel, baserad på ACCESSOROBJCODE</td>
             <td>Primärnyckeln/ID för objektet som identifieras i fältet ACCESSOROBJCODE</td>
        </tr>
        <tr>
             <td>ACCESSRULEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>ANCESTORID</td>
             <td>PK</td>
             <td>Variabel, baserad på ANCESTOROBJCODE</td>
             <td>Primärnyckeln/ID för objektet som identifieras i fältet ANCESTOROBJCODE</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SECURITYOBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på SECURITYOBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i fältet SECURITYOBJCODE</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Godkännandesökväg

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Godkännandesökväg</td>
            <td>Godkännandesökväg</td>
            <td>ARVPTH</td>
            <td>Godkännande</td>
            <td>APPROVALPATHS_CURRENT<br>APPROVALPATHS_DAILY_HISTORY<br>APPROVALPATHS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>TYPGODKÄNNANDEPATID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>GODKÄNNANDEPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>GODKÄNNANDEPROCESSID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GLOBALPATHID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Godkännandeprocess

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Godkännandeprocess</td>
            <td>Godkännandeprocess</td>
            <td>ARVPRC</td>
            <td>Godkännandeprocess</td>
            <td>APPROVALPROCESSES_CURRENT<br>APPROVALPROCESSES_DAILY_HISTORY<br>APPROVALPROCESSES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GODKÄNNANDEPROCESSID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Godkännandesteg

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Godkännandesteg</td>
            <td>Godkännandesteg</td>
            <td>ARVSTP</td>
            <td>Godkännandefas</td>
            <td>APPROVALSTEPS_CURRENT<br>APPROVALSTEPS_DAILY_HISTORY<br>APPROVALSTEPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>TYPGODKÄNNANDEPATID</td>
             <td>FK</td>
             <td>APPROVALPATHS_CURRENT</td>
             <td>TYPGODKÄNNANDEPATID</td>
        </tr>
        <tr>
             <td>APPROVALSTEPID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Godkännarstatus

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Godkännarstatus</td>
            <td>Godkännarstatus</td>
            <td>ARVSTS</td>
            <td>Godkännarstatus</td>
            <td>APPROVERSTATUSES_CURRENT<br>APPROVERSTATUSES_DAILY_HISTORY<br>APPROVERSTATUSES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GODKÄNNARSTATUSID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>APPROVABLEOBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på APPROVABLEOBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i fältet APPROVABLEOBJCODE</td>
        </tr>
        <tr>
             <td>APPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>GODKÄND</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>DELEGATEUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OVERRIDDENUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>STEPAPPROVERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSYID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>AKTIVITET</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
        <tr>
             <td>WILDCARDUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Tilldelning

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tilldelning</td>
            <td>Tilldelning</td>
            <td>ASSGN</td>
            <td>Tilldelning</td>
            <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>TILLDELNING</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CLASSIFIERID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
      <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>AKTIVITET</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
    </tbody>
</table>

### Väntar på godkännanden

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Väntar på godkännanden</td>
            <td>Väntar på godkännanden</td>
            <td>AWAPVL</td>
            <td>Väntar på godkännanden</td>
            <td>AWAITINGAPPROVALS_CURRENT<br>AWAITINGAPPROVALS_DAILY_HISTORY<br>AWAITINGAPPROVALS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ÅTKOMSTBEGÄRAN</td>
             <td>–</td>
             <td colspan="2">Åtkomstbegärandetabellen stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>TYPGODKÄNNANDE</td>
             <td>FK</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>GODKÄNNANDE</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>AWAITINGAPPROVALID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>DOCUMENTVERSIONID</td>
             <td>FK</td>
             <td>DOCUMENTVERSIONS_CURRENT</td>
             <td>DOCUMENTVERSIONID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>AKTIVITET</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>TIDSPEL</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIDSPEL</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Baslinje

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Baslinje</td>
            <td>Baslinje</td>
            <td>BLIN</td>
            <td>Baslinje</td>
            <td>BASELINES_CURRENT<br>BASELINES_DAILY_HISTORY<br>BASELINES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BASELINEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Originalaktivitet

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Originalaktivitet</td>
            <td>Originalaktivitet</td>
            <td>BSTSK</td>
            <td>Originalaktivitet</td>
            <td>BASELINETASKS_CURRENT<br>BASELINETASKS_DAILY_HISTORY<br>BASELINETASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BASELINEID</td>
             <td>FK</td>
             <td>BASELINES_CURRENT</td>
             <td>BASELINEID</td>
        </tr>
        <tr>
             <td>BASELINETASKID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>AKTIVITET</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
    </tbody>
</table>

### Faktureringstakt

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Faktureringstakt</td>
            <td>Klassificera eller åsidosätt hastighet</td>
            <td>KURS</td>
            <td>Faktureringstakt</td>
            <td>RATES_CURRENT<br>RATES_DAILY_HISTORY<br>RATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>TILLDELNING</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>TILLDELNING</td>
        </tr>
        <tr>
             <td>CLASSIFIERID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>NLBRCATEGORYID</td>
             <td>FK</td>
             <td>NLBRCATEGORIES_CURRENT</td>
             <td>NLBRCATEGORYID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCEID</td>
             <td>FK</td>
             <td>NONLABORRESOURCES_CURRENT</td>
             <td>NONLABORRESOURCEID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på OBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i OBJCODE-fältet</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>RATEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SOURCERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRNT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Faktureringspost

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Faktureringspost</td>
            <td>Faktureringspost</td>
            <td>BILL</td>
            <td>Faktureringspost</td>
            <td>BILLINGRECORDS_CURRENT<br>BILLINGRECORDS_DAILY_HISTORY<br>BILLINGRECORDS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>INVOICEID</td>
             <td>–</td>
             <td colspan="2">Fakturatabellen stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Bokning

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Bokning</td>
            <td>Bokning</td>
            <td>BOOKNG</td>
            <td>Bokning</td>
            <td>BOOKINGS_CURRENT<br>BOOKINGS_DAILY_HISTORY<br>BOOKINGS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BOOKINGID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>NLBRCATEGORYID</td>
             <td>FK</td>
             <td>NLBRCATEGORIES_CURRENT</td>
             <td>NLBRCATEGORYID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCEID</td>
             <td>FK</td>
             <td>NONLABORRESOURCES_CURRENT</td>
             <td>NONLABORRESOURCEID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på OBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i OBJCODE-fältet</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>AKTIVITET</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på TOPOBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i TOPOBJCODE-fältet</td>
        </tr>
    </tbody>
</table>

### Affärsprofil

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Affärsprofil</td>
            <td>Affärsprofil</td>
            <td>BSNPRF</td>
            <td>BusinessProfile</td>
            <td>BUSINESSPROFILE_CURRENT<br>BUSINESSPROFILE_DAILY_HISTORY<br>BUSINESSPROFILE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSLEVELID</td>
             <td>FK</td>
             <td>ACCESSLEVELS_CURRENT</td>
             <td>ACCESSLEVELID</td>
        </tr>
        <tr>
             <td>BUSINESSPROFILEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Affärsregel

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Affärsregel</td>
            <td>Affärsregel</td>
            <td>BSNRUL</td>
            <td>Affärsregel</td>
            <td>BUSINESSRULE_CURRENT<br>BUSINESSRULE_DAILY_HISTORY<br>BUSINESSRULE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BUSINESSRULEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Kategori

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Kategori</td>
            <td>Eget formulär</td>
            <td>CTGY</td>
            <td>Kategori</td>
            <td>CATEGORIES_CURRENT<br>CATEGORIES_DAILY_HISTORY<br>CATEGORIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Kategoriparameter

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Kategoriparameter</td>
            <td>Anpassade formulärfält</td>
            <td>CTGYPA</td>
            <td>Kategoriparameter</td>
            <td>CATEGORIESPARAMETERS_CURRENT<br>CATEGORIESPARAMETERS_DAILY_HISTORY<br>CATEGORIESPARAMETERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>KATEGORIESPARAMETERIER</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>PARAMETERGROUPID</td>
             <td>FK</td>
             <td>PARAMETERGROUPS_CURRENT</td>
             <td>PARAMETERGROUPID</td>
        </tr>
        <tr>
             <td>PARAMETERID</td>
             <td>FK</td>
             <td>PARAMETERS_CURRENT</td>
             <td>PARAMETERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Klassificerare

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Klassificerare</td>
            <td>Plats</td>
            <td>CLSF</td>
            <td>Plats</td>
            <td>CLASSIFIER_CURRENT<br>CLASSIFIER_DAILY_HISTORY<br>CLASSIFIER_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CLASSIFIERID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Företag

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Företag</td>
            <td>Företag</td>
            <td>CMPY</td>
            <td>Företag</td>
            <td>COMPANIES_CURRENT<br>COMPANIES_DAILY_HISTORY<br>COMPANIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Anpassat kvartal

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Anpassat kvartal</td>
            <td>Anpassat kvartal</td>
            <td>CSTQRT</td>
            <td>Anpassat kvartal</td>
            <td>CUSTOMQUARTERS_CURRENT<br>CUSTOMQUARTERS_DAILY_HISTORY<br>CUSTOMQUARTERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CUSTOMQUARTERID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Anpassad uppräkning

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>CustomEnum</td>
            <td>Villkor, Prioritet, Allvarlighetsgrad, Status</td>
            <td>CSTEM</td>
            <td>Anpassad uppräkning</td>
            <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ANPASSAD</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

>[!NOTE]
>
>Posttypen identifieras med egenskapen `enumClass`. Följande typer förväntas:<br>
><ul><li>CONDITION_OPTASK</li>
&gt;<li>CONDITION_PROJ</li>
&gt;<li>CONDITION_TASK</li>
&gt;<li>PRIORITY_OPTASK</li>
&gt;<li>PRIORITY_PROJ</li>
&gt;<li>PRIORITY_TASK</li>
&gt;<li>SEVERITY_OPTASK</li>
&gt;<li>STATUS_OPTASK</li>
&gt;<li>STATUS_PROJ</li>
&gt;<li>STATUS_TASK</li></ul>


### Dokument

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Dokument</td>
            <td>Dokument</td>
            <td>DOCU</td>
            <td>Dokument</td>
            <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CHECKEDOUTBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>DOCUMENTREQUESTID</td>
             <td>–</td>
             <td colspan="2">Dokumentbegärandetabellen stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>NOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på OBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i OBJCODE-fältet</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RELEASEVERSIONID</td>
             <td>–</td>
             <td colspan="2">Versionsversionstabellen stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>AKTIVITET</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på TOPOBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i TOPOBJCODE-fältet</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Godkännande av dokument

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Godkännande av dokument</td>
            <td>Godkännande av dokument</td>
            <td>DOCAPL</td>
            <td>Godkännande av dokument</td>
            <td>DOCAPPROVALS_CURRENT<br>DOCAPPROVALS_DAILY_HISTORY<br>DOCAPPROVALS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GODKÄNNANDE</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>DOCAPPROVALID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>NOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>BEGÄRAN</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Dokumentgodkännande (NYTT)

Begränsad kundtillgänglighet

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Godkännande av dokument</td>
            <td>Godkännande</td>
            <td>Ej tillämpligt</td>
            <td>Ej tillämpligt</td>
            <td>APPROVAL_CURRENT<br>APPROVAL_DAILY_HISTORY<br>Approval_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td class="key">GODKÄND</td>
             <td>PK</td>
             <td>–</td>
             <td>OBS! Detta är också ID:t för det DOCUMENTVERSION-objekt som godkännandet är kopplat till.</td>
        </tr>
        <tr>
             <td class="key">ASSETID</td>
             <td>FK</td>
             <td>Variabel, baserad på ASSETTYPE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i fältet ASSETTYPE</td>
        </tr>
        <tr>
             <td class="key">CREATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">EAUTHTENANTID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td class="key">PRODUCTID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td class="key">REALCREATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Dokumentgodkännandefas (NYTT)

Begränsad kundtillgänglighet

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Dokumentgodkännandefas</td>
            <td>Godkännandefas</td>
            <td>Ej tillämpligt</td>
            <td>Ej tillämpligt</td>
            <td>APPROVAL_STAGE_CURRENT<br>APPROVAL_STAGE_DAILY_HISTORY<br>Approval_STAGE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td class="key">GODKÄND</td>
             <td>FK</td>
             <td>APPROVAL_CURRENT</td>
             <td>GODKÄND</td>
        </tr>
        <tr>
             <td class="key">APPROVALSTAGEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td class="key">CREATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">OBJID</td>
             <td class="type">FK</td>
             <td class="relatedtable">Variabel, baserad på OBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i OBJCODE-fältet</td>
        </tr>
    </tbody>
</table>

### Deltagare i dokumentgodkännandefasen (NYTT)

Begränsad kundtillgänglighet

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Deltagare i dokumentgodkännandefasen</td>
            <td>Godkännandebeslut</td>
            <td>Ej tillämpligt</td>
            <td>Ej tillämpligt</td>
            <td>APPROVAL_STAGE_PARTICIPANT_CURRENT<br>APPROVAL_STAGE_PARTICIPANT_DAILY_HISTORY<br>APPROVAL_STAGE_PARTICIPANT_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td class="key">GODKÄND</td>
             <td>FK</td>
             <td>APPROVAL_CURRENT</td>
             <td>GODKÄND</td>
        </tr>
        <tr>
             <td class="key">APPROVALSTAGEPARTICIPANTID/td&gt;
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td class="key">ASSETID</td>
             <td>FK</td>
             <td>Variabel, baserad på ASSETTYPE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i fältet ASSETTYPE</td>
        </tr>
        <tr>
             <td class="key">BESLUIONUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">OBJID</td>
             <td class="type">FK</td>
             <td class="relatedtable">Variabel, baserad på OBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i OBJCODE-fältet</td>
        </tr>
        <tr>
             <td class="key">DELTAGARANTID</td>
             <td>FK</td>
             <td class="relatedtable">Variabel, baserad på PARTICIPANTTYPE</td>
             <td>Primärnyckeln/ID för objektet som identifieras i fältet PARTICIPANTTYPE</td>
        </tr>
        <tr>
             <td class="key">REALREQUESTORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">REALUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">BEGÄRAN</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">STAGEID</td>
             <td>FK</td>
             <td>APPROVAL_STAGE_CURRENT</td>
             <td>STAGEID</td>
        </tr>
    </tbody>
</table>

### Dokumentmapp

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Dokumentmapp</td>
            <td>Dokumentmapp</td>
            <td>DOCFLD</td>
            <td>DocsFolders</td>
            <td>DOCFOLDERS_CURRENT<br>DOCFOLDERS_DAILY_HISTORY<br>DOCFOLDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCFOLDERID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROBLEM</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>LINKEDFOLDERID</td>
             <td>FK</td>
             <td>LINKEDFOLDERS_CURRENT</td>
             <td>LINKEDFOLDERID</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>DOCFOLDERS_CURRENT</td>
             <td>DOCFOLDERID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>AKTIVITET</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Metadata för dokumentleverantör

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Metadata för dokumentleverantör</td>
            <td>Metadata för dokumentleverantör</td>
            <td>DOCMET</td>
            <td>DocumentProviderMetadata</td>
            <td>DOCPROVIDERMETA_CURRENT<br>DOCPROVIDERMETA_DAILY_HISTORY<br>DOCPROVIDERMETA_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCPROVIDERMETAID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Dokumentleverantör

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Dokumentleverantör</td>
            <td>Dokumentleverantör</td>
            <td>DOCPRO</td>
            <td>Dokumentleverantör</td>
            <td>DOCPROVIDERS_CURRENT<br>DOCPROVIDERS_DAILY_HISTORY<br>DOCPROVIDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCPROVIDERCONFIGID</td>
             <td>FK</td>
             <td>DOCPROVIDERCONFIG_CURRENT</td>
             <td>DOCPROVIDERCONFIGID</td>
        </tr>
        <tr>
             <td>DOCPROVIDERID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Dokumentproviderkonfiguration

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Dokumentproviderkonfiguration</td>
            <td>Dokumentproviderkonfiguration</td>
            <td>DOCCFG</td>
            <td>Dokumentproviderkonfiguration</td>
            <td>DOCPROVIDERCONFIG_CURRENT<br>DOCPROVIDERCONFIG_DAILY_HISTORY<br>DOCPROVIDERCONFIG_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCPROVIDERCONFIGID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Dokumentversion

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Dokumentversion</td>
            <td>Dokumentversion</td>
            <td>DOCV</td>
            <td>Dokumentversion</td>
            <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>DOCUMENTPROVIDERID</td>
             <td>FK</td>
             <td>DOCPROVIDERS_CURRENT</td>
             <td>DOCUMENTPROVIDERID</td>
        </tr>
        <tr>
             <td>DOCUMENTVERSIONID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXTERNALSTORAGEID</td>
             <td>–</td>
             <td colspan="2">Det externa ID:t i det externa lagringssystemet</td>
        </tr>
        <tr>
             <td>PROOFAPPROVALSTATUSID</td>
             <td>–</td>
             <td colspan="2">Registret för godkännandestatus stöds för närvarande inte</td>
        </tr>
        <tr>
             <td>PROOFEDBYUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROOFID</td>
             <td>–</td>
             <td colspan="2">Korrekturtabell stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>PROOFOWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROOFSTAGEID</td>
             <td>FK</td>
             <td>–</td>
             <td colspan="2">Korrekturstegstabellen stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Växelkurs

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Växelkurs</td>
            <td>Växelkurs</td>
            <td>EXRATERA</td>
            <td>Växelkurs</td>
            <td>EXCHANGERATES_CURRENT<br>EXCHANGERATES_DAILY_HISTORY<br>EXCHANGERATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Utgift

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Utgift</td>
            <td>Utgift</td>
            <td>EXPNS</td>
            <td>Utgift</td>
            <td>EXPENSES_CURRENT<br>EXPENSES_DAILY_HISTORY<br>EXPENSES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>BILLINGRECORDID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>UTGIFTSKOSTNAD</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>EXPENSETYPEID</td>
             <td>FK</td>
             <td>EXPENSETYPES_CURRENT</td>
             <td>EXPENSETYPEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på OBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i OBJCODE-fältet</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>AKTIVITET</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på TOPBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i TOPBJCODE-fältet</td>
        </tr>
    </tbody>
</table>

### Utgiftstyp

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Utgiftstyp</td>
            <td>Utgiftstyp</td>
            <td>EXPTYP</td>
            <td>Utgiftstyp</td>
            <td>EXPENSETYPES_CURRENT<br>EXPENSETYPES_DAILY_HISTORY<br>EXPENSETYPES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>EXPENSETYPEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på OBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i OBJCODE-fältet</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Grupp

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Grupp</td>
            <td>Grupp</td>
            <td>GRUPP</td>
            <td>Grupp</td>
            <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BUSINESSLEADERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>ROOTID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Timme

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Timme</td>
            <td>Timme</td>
            <td>TIMME</td>
            <td>Timme</td>
            <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GODKÄND</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>BILLINGRECORDID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CLASSIFIERID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>DUPID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>EXTERNALTIMESHEETID</td>
             <td>–</td>
             <td colspan="2">Inte en Workfront-relation, används för integration med externa system
Själv</td>
        </tr>
        <tr>
             <td>HOURID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>HOURTYPEID</td>
             <td>FK</td>
             <td>HOURTYPES_CURRENT</td>
             <td>HOURTYPEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>PROJECTOVERHEADID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>AKTIVITET</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
        <tr>
             <td>TIDSPEL</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIDSPEL</td>
        </tr>
    </tbody>
</table>

### Timtyp

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Timtyp</td>
            <td>Timtyp</td>
            <td>TID</td>
            <td>Timtyp</td>
            <td>HOURTYPES_CURRENT<br>HOURTYPES_DAILY_HISTORY<br>HOURTYPES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>HOURTYPEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på OBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i OBJCODE-fältet</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Upprepning

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Upprepning</td>
            <td>Upprepning</td>
            <td>ITRN</td>
            <td>Upprepning</td>
            <td>ITERATIONS_CURRENT<br>ITERATIONS_DAILY_HISTORY<br>ITERATIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
    </tbody>
</table>

### Journalpost

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Journalpost</td>
            <td>Journalpost</td>
            <td>JRNLE</td>
            <td>Journalpost</td>
            <td>JOURNALENTRIES_CURRENT<br>JOURNALENTRIES_DAILY_HISTORY<br>JOURNALENTRIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GODKÄNNARSTATUSID</td>
             <td>FK</td>
             <td>APPROVERSTATUSES_CURRENT</td>
             <td>GODKÄNNARSTATUSID</td>
        </tr>
        <tr>
             <td>TILLDELNING</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>TILLDELNING</td>
        </tr>
        <tr>
             <td>AUDITRECORDID</td>
             <td>–</td>
             <td colspan="2">Registret för granskningsposter stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>BASELINEID</td>
             <td>FK</td>
             <td>BASELINES_CURRENT</td>
             <td>BASELINEID</td>
        </tr>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>BILLINGRECORDID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>DOCUMENTSHAREID</td>
             <td>–</td>
             <td colspan="2">Dokumentdelningstabellen stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>EDITEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>UTGIFTSKOSTNAD</td>
             <td>FK</td>
             <td>EXPENSES_CURRENT</td>
             <td>UTGIFTSKOSTNAD</td>
        </tr>
        <tr>
             <td>HOURID</td>
             <td>FK</td>
             <td>HOURS_CURRENT</td>
             <td>HOURID</td>
        </tr>
        <tr>
             <td>INITIATIVEID</td>
             <td>–</td>
             <td colspan="2">Initiativtabellen stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>JOURNALENTRIESID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på OBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i OBJCODE-fältet</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SUBOBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på SUBBOBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i fältet SUBOBJCODE</td>
        </tr>
        <tr>
             <td>SUBSCRIBEID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>AKTIVITET</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TIDSPEL</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIDSPEL</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på TOPOBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i TOPOBJCODE-fältet</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Länkad mapp

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Länkad mapp</td>
            <td>Länkad mapp</td>
            <td>LNKFDR</td>
            <td>LinkedFolder</td>
            <td>LINKEDFOLDERS_CURRENT<br>LINKEDFOLDERS_DAILY_HISTORY<br>LINKEDFOLDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCUMENTPROVIDERID</td>
             <td>FK</td>
             <td>DOCPROVIDERS_CURRENT</td>
             <td>DOCUMENTPROVIDERID</td>
        </tr>
        <tr>
             <td>EXTERNALSTORAGEID</td>
             <td>–</td>
             <td colspan="2">Det externa ID:t i det externa lagringssystemet</td>
        </tr>
        <tr>
             <td>FOLDERID</td>
             <td>FK</td>
             <td>DOCFOLDERS_CURRENT</td>
             <td>FOLDERID</td>
        </tr>
        <tr>
             <td>LINKEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LINKEDFOLDERID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Milstolpe

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Milstolpe</td>
            <td>Milstolpe</td>
            <td>MILE</td>
            <td>Milstolpe</td>
            <td>MILESTONES_CURRENT<br>MILESTONES_DAILY_HISTORY<br>MILESTONES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>MILESTONEPATID</td>
             <td>FK</td>
             <td>MILESTONEPATHS_CURRENT</td>
             <td>MILESTONEPATID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Sökväg för milstolpe

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Sökväg för milstolpe</td>
            <td>Sökväg för milstolpe</td>
            <td>MPATH</td>
            <td>Sökväg för milstolpe</td>
            <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEPATID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Resurs vid annat än arbete

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Resurs vid annat än arbete</td>
            <td>Icke-arbetsrelaterad resurs</td>
            <td>NLBR</td>
            <td>Icke-arbetsrelaterad resurs</td>
            <td>NONLABORRESOURCES_CURRENT<br>NONLABORRESOURCES_DAILY_HISTORY<br>NONLABORRESOURCES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>HOMEGROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCECATEGORYID</td>
             <td>FK</td>
             <td>NLBRCATEGORIES_CURRENT</td>
             <td>NLBRCATEGORYID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Resurskategori för icke-arbetsplats

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Resurskategori för icke-arbetsplats</td>
            <td>Resurskategori för icke-arbetsplats</td>
            <td>NLBRY</td>
            <td>Resurskategori utanför arbetsplats</td>
            <td>NLBRCATEGORIES_CURRENT<br>NLBRCATEGORIES_DAILY_HISTORY<br>NLBRCATEGORIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>NLBRCATEGORYID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Ledig dag

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Ledig dag</td>
            <td>Schemaundantag</td>
            <td>NONWKD</td>
            <td>Ledig arbetsdag</td>
            <td>NONWORKDAYS_CURRENT<br>NONWORKDAYS_DAILY_HISTORY<br>NONWORKDAYS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>NONWORKDAYID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på OBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i OBJCODE-fältet</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Obs

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Obs</td>
            <td>Obs</td>
            <td>ANMÄRKNING</td>
            <td>Obs</td>
            <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ATTACHDOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>ATTACHOBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på ATTACHOBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i OBJCODE ATTACHOBJCODE</td>
        </tr>
        <tr>
             <td>ATTACHOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>ATTACHWORKID</td>
             <td>FK</td>
             <td>WORKITEMS_CURRENT</td>
             <td>WORKITEM-ID</td>
        </tr>
        <tr>
             <td>ATTACHWORKUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>AUDITRECORDID</td>
             <td>–</td>
             <td colspan="2">Registret Granskningspost stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>EXTERNALSERVICEID</td>
             <td>–</td>
             <td colspan="2">Inte en Workfront-relation, används för integration med externa system</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>NOTEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på NOTEOBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i NOTEOBJCODE-fältet</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PARENTENDORSEMENTID</td>
             <td>–</td>
             <td colspan="2">Bekräftelsetabellen stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>PARENTJOURNALENTRYID</td>
             <td>FK</td>
             <td>JOURNALENTRIES_CURRENT</td>
             <td>JOURNALENTRYID</td>
        </tr>
        <tr>
             <td>PARENTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>PROOFACTIONID</td>
             <td>–</td>
             <td colspan="2">Korrekturåtgärdstabellen stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>PROOFID</td>
             <td>–</td>
             <td colspan="2">Korrekturtabell stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>RICHTEXTNOTEID</td>
             <td>FK</td>
             <td>RESERVEDTEXTNOTES_CURRENT</td>
             <td>RICHTEXTNOTEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>AKTIVITET</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TREADID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>TIDSPEL</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIDSPEL</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på TOPOBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i TOPOBJCODE-fältet</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>


</table>

### Objektintegrering

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Objektintegrering</td>
            <td>Objektintegrering</td>
            <td>OBJEKT</td>
            <td>ObjectIntegration</td>
            <td>OBJECTINTEGRATION_CURRENT<br>OBJECTINTEGRATION_DAILY_HISTORY<br>OBJECTINTEGRATION_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LINKEDOBJECTID</td>
             <td>FK</td>
             <td>Variabel, baserad på LINKEDOBJECTCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i fältet LINKEDOBJECTCODE</td>
        </tr>
        <tr>
             <td>OBJECTINTEGRATIONID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på OBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i OBJCODE-fältet</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>

</table>

### Objektkategori

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Objektkategori</td>
            <td>Objektkategorier</td>
            <td>OBJCAT</td>
            <td>Objektkategori</td>
            <td>OBJECTSCATEGORIES_CURRENT<br>OBJECTSCATEGORIES_DAILY_HISTORY<br>OBJECTSCATEGORIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>OBJECTSCATEGORYID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på OBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i OBJCODE-fältet</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### OpTask / Issue

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>OpTask</td>
            <td>Problem, begäran</td>
            <td>OPTASK</td>
            <td>Problem</td>
            <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GODKÄNNANDEPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>GODKÄNNANDEPROCESSID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CURRENTAPPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>KANBANBOARDID</td>
             <td>–</td>
             <td colspan="2">Kanban-tavlan stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>LASTCONDITIONNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>QUEUEDEFID</td>
             <td>–</td>
             <td colspan="2">Ködefinitionstabellen stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>QUEUETOPICID</td>
             <td>–</td>
             <td colspan="2">Tabellen Köämne stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>RESOLVEOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>RESOLVEPROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RESOLVETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
        <tr>
             <td>RESOLVINGOBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på RESOLVINGOBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i fältet RESLVINGOBJCODE</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SOURCEOBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på SOURCEOBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i fältet SOURCEOBJCODE</td>
        </tr>
        <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
    </tbody>
</table>

### Parameter

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Parameter</td>
            <td>Anpassat fält</td>
            <td>PARAM</td>
            <td>Parameter</td>
            <td>PARAMETERS_CURRENT<br>PARAMETERS_DAILY_HISTORY<br>PARAMETERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PARAMETERFILTERID</td>
             <td>–</td>
             <td colspan="2">Parameterfiltertabellen stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>PARAMETERID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Parametergrupp

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Parametergrupp</td>
            <td>Formuläravsnitt</td>
            <td>PARAM</td>
            <td>Parametergrupp</td>
            <td>PARAMETERGROUPS_CURRENT<br>PARAMETERGROUPS_DAILY_HISTORY<br>PARAMETERGROUPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PARAMETERGROUPID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Parameteralternativ

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Parameteralternativ</td>
            <td>Parameteralternativ</td>
            <td>POPT</td>
            <td>Parameteralternativ</td>
            <td>PARAMETEROPTIONS_CURRENT<br>PARAMETEROPTIONS_DAILY_HISTORY<br>PARAMETEROPTIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PARAMETERID</td>
             <td>FK</td>
             <td>PARAMETERS_CURRENT</td>
             <td>PARAMETERID</td>
        </tr>
        <tr>
             <td>PARAMETEROPTIONID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Portalavsnitt/rapport

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Portalavsnitt</td>
            <td>Rapport</td>
            <td>PTLSEC</td>
            <td>Rapport</td>
            <td>PORTALSECTIONS_CURRENT<br>PORTALSECTIONS_DAILY_HISTORY<br>PORTALSECTIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>FILTERID</td>
             <td>FK</td>
             <td>UIFILTERS_CURRENT</td>
             <td>FILTERID</td>
        </tr>
        <tr>
             <td>GROUPBYID</td>
             <td>FK</td>
             <td>UIGROUPBYS_CURRENT</td>
             <td>GROUPBYID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTVIEWEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på OBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i OBJCODE-fältet</td>
        </tr>
        <tr>
             <td>PORTALSECTIONID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>FK</td>
             <td>PREFERENCES_CURRENT</td>
             <td>PREFERENCEID</td>
        </tr>
        <tr>
             <td>PUBLICRUNASUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>RAPPORTFOLDERID</td>
             <td>FK</td>
             <td>REPORTFOLDERS_CURRENT</td>
             <td>RAPPORTFOLDERID</td>
        </tr>
        <tr>
             <td>RUNASUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SCHEDULEDREPORTID</td>
             <td>–</td>
             <td colspan="2">Schemalagd rapporttabell stöds för närvarande inte</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>VISA</td>
             <td>FK</td>
             <td>UIVIEWS_CURRENT</td>
             <td>VISA</td>
        </tr>
    </tbody>
</table>

### Fliken Portal/Dashboard

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Portal Tab</td>
            <td>Kontrollpanel</td>
            <td>PTLTAB</td>
            <td>Kontrollpanel</td>
            <td>PORTALTABS_CURRENT<br>PORTALTABS_DAILY_HISTORY<br>PORTALTABS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTALPROFILEID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>PORTALTABID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Portal Tab Section

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Portal Tab Section</td>
            <td>Instrumentpanelsavsnitt</td>
            <td>PRTBSC</td>
            <td>Portal Tab Section</td>
            <td>PORTALTABSPORTALSECTIONS_CURRENT<br>PORTALTABSPORTALSECTIONS_DAILY_HISTORY<br>PORTALTABSPORTALSECTIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CALENDARPORTALSECTIONID</td>
             <td>–</td>
             <td colspan="2">Kalenderportalavsnittet stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>EXTERNALSECTIONID</td>
             <td>–</td>
             <td colspan="2">Tabellen Externa avsnitt stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>INTERNALSECTIONID</td>
             <td>FK</td>
             <td>PORTALSECTIONS_CURRENT</td>
             <td>PORTALSECTIONID</td>
        </tr>
        <tr>
             <td>PORTALSECTIONOBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på PORTALSECTIONOBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i fältet PORTALSECTIONOBJCODE</td>
        </tr>
        <tr>
             <td>PORTALTABID</td>
             <td>FK</td>
             <td>PORTALTABS_CURRENT</td>
             <td>PORTALTABID</td>
        </tr>
        <tr>
             <td>PORTALTABSECTIONID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Senaste visningsprogram för portalavsnitt

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>PortalSectionLastViewer</td>
            <td>Rapportera senaste visningsprogram</td>
            <td>PLSLSV</td>
            <td>PortalSectionLastViewer</td>
            <td>REPORTLASTVIEWERS_CURRENT<br>REPORTLASTVIEWERS_DAILY_HISTORY<br>REPORTLASTVIEWERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RAPPORTERA</td>
             <td>FK</td>
             <td>PORTALSECTIONS_CURRENT</td>
             <td>RAPPORTERA</td>
        </tr>
        <tr>
             <td>RAPPORTLASTVIEWERID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>VIEWERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Portfolio

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Portfolio</td>
            <td>Portfolio</td>
            <td>PORT</td>
            <td>Portfolio</td>
            <td>PORTFOLIOS_CURRENT<br>PORTFOLIOS_DAILY_HISTORY<br>PORTFOLIOS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ALIGNMENTSCORECARDID</td>
             <td>–</td>
             <td colspan="2">Styrkortstabellen stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Inställningar

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Inställningar</td>
            <td>Visa, Filtrera, Gruppera, Rapportdefinition</td>
            <td>PROSET</td>
            <td>Inställningar</td>
            <td>PREFERENCES_CURRENT<br>PREFERENCES_DAILY_HISTORY<br>PREFERENCES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Program

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Program</td>
            <td>Program</td>
            <td>PRGM</td>
            <td>Program</td>
            <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Projekt

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Projekt</td>
            <td>Projekt</td>
            <td>PROJ</td>
            <td>Projekt</td>
            <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>AEMNATIVEFOLDERTREESREFID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>ALIGNMENTSCORECARDID</td>
             <td>–</td>
             <td colspan="2">Styrkortstabellen stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>GODKÄNNANDEPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>GODKÄNNANDEPROCESSID</td>
        </tr>
        <tr>
             <td>ATTACHEDRATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKORIGINATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CURRENTAPPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>LEVERABLESCORECARDID</td>
             <td>–</td>
             <td colspan="2">Styrkortstabellen stöds inte för närvarande</td>
        </tr>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTCONDITIONNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEPATID</td>
             <td>FK</td>
             <td>MILESTONEPATHS_CURRENT</td>
             <td>MILESTONEPATID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>POPACCOUNTID</td>
             <td>–</td>
             <td colspan="2">Pop Account table not supported current</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>QUEUEDEFID</td>
             <td>–</td>
             <td colspan="2">Ködefinitionstabellen stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>AVVISNINGSUMEID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>RESURCEPOOLID</td>
             <td>FK</td>
             <td>RESOURCEPOOLS_CURRENT</td>
             <td>RESURCEPOOLID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SPONSORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Projektteamanvändare

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Projektteamanvändare</td>
            <td>Projektteamanvändare</td>
            <td>PRTU</td>
            <td>Projektanvändare</td>
            <td>PROJECTSUSERS_CURRENT<br>PROJECTSUSERS_DAILY_HISTORY<br>PROJECTSUSERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>PROJECTSUSERID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>TMPUSERID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Användarroll för projektteam

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Användarroll för projektteam</td>
            <td>Användarroll för projektteam</td>
            <td>PTEAM</td>
            <td>ProjektAnvändarroll</td>
            <td>PROJECTSUSERSROLES_CURRENT<br>PROJECTSUSERSROLES_DAILY_HISTORY<br>PROJECTSUSERSROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>PROJECTSUSERSROLEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Hastighetskort

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Hastighetskort</td>
            <td>Hastighetskort</td>
            <td>RTCRD</td>
            <td>Hastighetskort</td>
            <td>RATECARD_CURRENT<br>RATECARD_DAILY_HISTORY<br>RATECARD_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>RATECARDID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SECURITYROOTID</td>
             <td>FK</td>
             <td>Variabel, baserad på SECURITYOBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i fältet SECURITYOBJCODE</td>
        </tr>
        <tr>
             <td>SOURCEID</td>
             <td>FK</td>
             <td>Variabel, baserad på SOURCEOBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i fältet SOURCEOBJCODE</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>

</table>

### Rapportmapp

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Rapportmapp</td>
            <td>Rapportmapp</td>
            <td>RPTFDR</td>
            <td>Rapportmapp</td>
            <td>REPORTFOLDERS_CURRENT<br>REPORTFOLDERS_DAILY_HISTORY<br>REPORTFOLDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RAPPORTFOLDERID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Rapportvy - statistikantal

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Rapportvy - statistikantal</td>
            <td>Rapportvy - statistikantal</td>
            <td>PLSVST</td>
            <td>PortalSectionStatisticInfo</td>
            <td>REPORTVIEWSTATISTICCOUNTS_CURRENT<br>REPORTVIEWSTATISTICCOUNTS_DAILY_HISTORY<br>REPORTVIEWSTATISTICCOUNTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RAPPORTERA</td>
             <td>FK</td>
             <td>PORTALSECTIONS_CURRENT</td>
             <td>PORTALSECTIONID</td>
        </tr>
        <tr>
             <td>RAPPORTVIEWSTATISTICCOUNTID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Rapporteringsskyldiga budgeterade timmar

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Rapporteringsskyldiga budgeterade timmar</td>
            <td>Rapporteringsskyldiga budgeterade timmar</td>
            <td>RPBGHR</td>
            <td>Budgeterad timme</td>
            <td>REPORTABLEBUDGETEDHOURS_CURRENT<br>REPORTABLEBUDGETEDHOURS_DAILY_HISTORY<br>REPORTABLEBUDGETEDHOURS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RAPPORTABLEBUDGETEDHOURID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Reserverad tid / PTO

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Reserverad tid</td>
            <td>(Personligt) Tid av</td>
            <td>RESVT</td>
            <td>Tid av</td>
            <td>RESERVEDTIMES_CURRENT<br>RESERVEDTIMES_DAILY_HISTORY<br>RESERVEDTIMES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RESERVEDTIMEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>AKTIVITET</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Resurshanteraren

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Resurshanteraren</td>
            <td>Resurshanteraren</td>
            <td>RESMGR</td>
            <td>Resurshanteraren</td>
            <td>RESOURCEMANAGERS_CURRENT<br>RESOURCEMANAGERS_DAILY_HISTORY<br>RESOURCEMANAGERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RESOURCEMANAGERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Resurspool

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Resurspool</td>
            <td>Resurspool</td>
            <td>RSPL</td>
            <td>Resurspool</td>
            <td>RSRCPOOLS_CURRENT<br>RSRCPOOLS_DAILY_HISTORY<br>RSRCPOOLS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>RESURCEPOOLID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### RTF-anteckning

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>RTF-anteckning</td>
            <td>RTF-anteckning</td>
            <td>RHNOTE</td>
            <td>RTF-anteckning</td>
            <td>RESERVEDTEXTNOTES_CURRENT<br>RESERVEDTEXTNOTES_DAILY_HISTORY<br>RESERVEDTEXTNOTES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RICHTEXTNOTEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Parametervärde för RTF

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Parametervärde för RTF</td>
            <td>Parametervärde för RTF</td>
            <td>RCHVAL</td>
            <td>RichTextParameterValue</td>
            <td>RICHTEXTPARAMETERVALUES_CURRENT<br>RICHTEXTPARAMETERVALUES_DAILY_HISTORY<br>RICHTEXTPARAMETERVALUES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PARAMETERVALUEID</td>
             <td>–</td>
             <td colspan="2">Parametervärdestabellen stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>RICHTEXTPARAMETERVALUEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### risk

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>risk</td>
            <td>risk</td>
            <td>RISK</td>
            <td>risk</td>
            <td>RISKS_CURRENT<br>RISKS_DAILY_HISTORY<br>RISKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RISKID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>RISKTYPEID</td>
             <td>FK</td>
             <td>RISKTYPES_CURRENT</td>
             <td>RISKTYPEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Risktyp

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Risktyp</td>
            <td>Risktyp</td>
            <td>RSKTYP</td>
            <td>Risktyp</td>
            <td>RISKTYPES_CURRENT<br>RISKTYPES_DAILY_HISTORY<br>RISKTYPES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RISKTYPEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Roll

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Roll</td>
            <td>Jobbroll</td>
            <td>ROLE</td>
            <td>Jobbroll</td>
            <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>–</td>
             <td colspan="2">Layoutmallstabellen stöds inte</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Schema

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Schema</td>
            <td>Schema</td>
            <td>SCHED</td>
            <td>Schema</td>
            <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>HOMEGROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Personalplan

Begränsad kundtillgänglighet

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Personalplan</td>
            <td>Personalplan</td>
            <td>STAFFP</td>
            <td>Personalplan</td>
            <td>STAFFING_PLAN_CURRENT<br>STAFFING_PLAN_DAILY_HISTORY<br>STAFFING_PLAN_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ATTACHEDRATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT </td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>        
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>        
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>        
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>       
         <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID
</td>
        </tr>        
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID
</td>
        </tr>        
        <tr>
             <td>STAFFINGPLANID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
    </tbody>
</table>

### Resurs för personalplan

Begränsad kundtillgänglighet

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Resurs för personalplan</td>
            <td>Resurs för personalplan</td>
            <td>PERSONAL</td>
            <td>Resurs för personalplan</td>
            <td>STAFFING_PLAN_RESOURCE_CURRENT<br>STAFFING_PLAN_RESOURCE_DAILY_HISTORY<br>STAFFING_PLAN_RESOURCE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>        
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>        
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>        
        <tr>
             <td>STAFFINGPLANID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_CURRENT</td>
             <td>STAFFINGPLANID</td>
        </tr>       
         <tr>
             <td>STAFFINGPLANRESOURCEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>        
    </tbody>
</table>

### Steggodkännare

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Steggodkännare</td>
            <td>Steggodkännare</td>
            <td>SPAPVR</td>
            <td>Scengodkännare</td>
            <td>STEPAPPROVERS_CURRENT<br>STEPAPPROVERS_DAILY_HISTORY<br>STEPAPPROVERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>STEPAPPROVERID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Uppgift

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Uppgift</td>
            <td>Uppgift</td>
            <td>UPPGIFT</td>
            <td>Uppgift</td>
            <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GODKÄNNANDEPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>GODKÄNNANDEPROCESSID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>BILLINGRECORDID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKORIGINATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CURRENTAPPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>KANBANBOARDID</td>
             <td>–</td>
             <td colspan="2">Kanban-tavlan stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>LASTCONDITIONNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEID</td>
             <td>FK</td>
             <td>MILESTONES_CURRENT</td>
             <td>MILESTONEID</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>ÅTERKOMMANDE</td>
             <td>–</td>
             <td colspan="2">Regeltabellen för upprepning stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>AVVISNINGSUMEID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>RESERVEDTIMEID</td>
             <td>FK</td>
             <td>RESERVEDTIMES_CURRENT</td>
             <td>RESERVEDTIMEID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>SUBMITTEDBYID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>AKTIVITET</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
    </tbody>
</table>

### Aktivitetsföregångare

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Aktivitetsföregångare</td>
            <td>Föregående</td>
            <td>PRED</td>
            <td>Föregående</td>
            <td>PREDECESSORS_CURRENT<br>PREDECESSORS_DAILY_HISTORY<br>PREDECESSORS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>FÖRBESTÄLL</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
        <tr>
             <td>SUCCESSORID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Team

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Team</td>
            <td>Team</td>
            <td>TEAMOB</td>
            <td>Team</td>
            <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>–</td>
             <td colspan="2">Layoutmallstabellen stöds inte</td>
        </tr>
        <tr>
             <td>MYWORKVIEWID</td>
             <td>FK</td>
             <td>UIVIEWS_CURRENT</td>
             <td>UIVIEWID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>BEGÄRANDVIEWID</td>
             <td>FK</td>
             <td>UIVIEWS_CURRENT</td>
             <td>UIVIEWID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
    </tbody>
</table>

>[!NOTE]
>
>Det finns tre teamtyper som lagras i Team-objekttabellerna: PROJECT, TEMPLATE och ADHOC. <br>
>Var och en av de här teamtyperna representeras tillsammans i Data Connect-datavinjevyerna. Om du vill isolera den typ av team som du vill returnera måste du filtrera på kolumnen `teamtype`. Om du till exempel bara vill ha de traditionella team som ingår i din organisationsstruktur, som är konfigurerade i programområdet, kan du ha en fråga som ser ut ungefär så här: <code>select * from teams_current där teamtype = &#39;ADHOC&#39;;</code>

### Teammedlem

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Teammedlem</td>
            <td>Andra team, teammedlem</td>
            <td>TEAMMB</td>
            <td>Teammedlem</td>
            <td>TEAMMEMBERS_CURRENT<br>TEAMMEMBERS_DAILY_HISTORY<br>TEAMMEMBERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>TEAMMEMBERID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Teammedlemsroll

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Teammedlemsroll</td>
            <td>Teammedlemsroll</td>
            <td>TEAMMR</td>
            <td>Teammedlemsroll</td>
            <td>TEAMMEMBERROLES_CURRENT<br>TEAMMEMBERROLES_DAILY_HISTORY<br>TEAMMEMBERROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>TEAMMEMBERROLEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Mall

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Mall</td>
            <td>Mall, projektmall</td>
            <td>TMPL</td>
            <td>Mall</td>
            <td>TEMPLATES_CURRENT<br>TEMPLATES_DAILY_HISTORY<br>TEMPLATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GODKÄNNANDEPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>GODKÄNNANDEPROCESSID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>LEVERABLESCORECARDID</td>
             <td>–</td>
             <td colspan="2">Slutprodukt styrkortsregister stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEPATID</td>
             <td>FK</td>
             <td>MILESTONEPATHS_CURRENT</td>
             <td>MILESTONEPATID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>QUEUEDEFID</td>
             <td>–</td>
             <td colspan="2">Ködefinitionstabellen stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
    </tbody>
</table>

### Mallaktivitetstilldelning

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Mallaktivitetstilldelning</td>
            <td>Malltilldelning</td>
            <td>TASSGN</td>
            <td>Malltilldelning</td>
            <td>TEMPLATEASSIGNMENTS_CURRENT<br>TEMPLATEASSIGNMENTS_DAILY_HISTORY<br>TEMPLATEASSIGNMENTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på OBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i OBJCODE-fältet</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>TEAMTIMELINEABLEID</td>
             <td>–</td>
             <td colspan="2">Tidslinjerbar tabell för team stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>TEMPLATEASSIGNMENTID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
    </tbody>
</table>

### Malluppgift

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Malluppgift</td>
            <td>Malluppgift</td>
            <td>TTSK</td>
            <td>Malluppgift</td>
            <td>TEMPLATETASKS_CURRENT<br>TEMPLATETASKS_DAILY_HISTORY<br>TEMPLATETASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GODKÄNNANDEPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>GODKÄNNANDEPROCESSID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEID</td>
             <td>FK</td>
             <td>MILESTONES_CURRENT</td>
             <td>MILESTONEID</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>ÅTERKOMMANDE</td>
             <td>–</td>
             <td colspan="2">Regeltabellen för upprepning stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>TEAMTIMELINEABLEID</td>
             <td>–</td>
             <td colspan="2">Tidslinjerbar tabell för team stöds inte för närvarande</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
    </tbody>
</table>

### Föregångare för mallaktivitet

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Föregångare för mallaktivitet</td>
            <td>Mallföregångare</td>
            <td>TPRED</td>
            <td>Föregående</td>
            <td>TEMPLATEPREDECESSORS_CURRENT<br>TEMPLATEPREDECESSORS_DAILY_HISTORY<br>TEMPLATEPREDECESSORS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>FÖRBESTÄLL</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>SUCCESSORID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEPREDECESSORID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Tidsfasad KPI kombinerad

Begränsad kundtillgänglighet

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tidsfasad KPI kombinerad</td>
            <td>Tidsfasad KPI</td>
            <td>TMPH</td>
            <td>TimePhasedKPI</td>
            <td>TIMEPHASED_COMBINED_CURRENT<br>TIMEPHASED_COMBINED_DAILY_HISTORY<br>TIMEPHASED_COMBINED_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>TILLDELNING</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>TILLDELNING</td>
        </tr>
                <tr>
             <td>EVENT_ID    </td>
             <td>PK</td>
             <td>Detta är en naturlig nyckel för den tidsfasade KPI-posten</td>
             <td>–</td>
        </tr>
                        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
                        <tr>
             <td>LOCATIONID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
                        <tr>
             <td>METADATAID</td>
             <td>FK</td>
             <td>METADATA-registret har inte angetts</td>
             <td>–</td>
        </tr>
                        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
                        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
                        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
                        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
                        <tr>
             <td>REFERENCEID</td>
             <td>FK</td>
             <td>Variabel, baserad på OBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i OBJCODE-fältet
</td>
        </tr>
                        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
                        <tr>
             <td>SCHEMAID</td>
             <td>FK</td>
             <td>SCHEMA-tabellen har inte angetts. Värdet från den här tabellen anges i SCHEMANAME-kolumnen. SCHEMANAME identifierar den KPI (t.ex. planningHours, stimours och actualHours) som posten är kopplad till.</td>
             <td>–</td>
        </tr>
                                <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
                                <tr>
             <td>STAFFINGPLANID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_CURRENT</td>
             <td>STAFFINGPLANID</td>
        </tr>
                                <tr>
             <td>STAFFINGPLANRESOURCEID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_RESOURCE_CURRENT</td>
             <td>STAFFINGPLANRESOURCEID</td>
        </tr>
                                <tr>
             <td>AKTIVITET</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
                                <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Tidsfördelad KPI-valuta

Begränsad kundtillgänglighet

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tidsfördelad KPI-valuta</td>
            <td>Tidsfasad KPI</td>
            <td>TMPH</td>
            <td>TimePhasedKPI</td>
            <td>TIMEPHASED_CURRENCY_CURRENT<br>TIMEPHASED_CURRENCY_DAILY_HISTORY<br>TIMEPHASED_CURRENCY_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>TILLDELNING</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>TILLDELNING</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LOCATIONID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
                <tr>
             <td>METADATAID</td>
             <td>FK</td>
             <td>METADATA-registret har inte angetts</td>
             <td>–</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>REFERENCEID</td>
             <td>FK</td>
             <td>Variabel, baserad på OBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i OBJCODE-fältet</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SCHEMAID</td>
             <td>FK</td>
             <td>SCHEMA-tabellen har inte angetts. Värdet från den här tabellen anges i SCHEMANAME-kolumnen. SCHEMANAME identifierar den KPI (t.ex. planningRevenueRate, planningCostRate, actualRevenue, osv.) som posten är kopplad till.</td>
             <td>SCHEMAID</td>
        </tr>
        <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
                <tr>
             <td>STAFFINGPLANID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_CURRENT</td>
             <td>STAFFINGPLANID</td>
        </tr>
          <tr>
             <td>STAFFINGPLANRESOURCEID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_RESOURCE_CURRENT</td>
             <td>STAFFINGPLANRESOURCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>AKTIVITET</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
        <tr>
             <td>TIMEPHASEDCURRENCYID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Tidsfasad KPI-varaktighet

Begränsad kundtillgänglighet

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tidsfasad KPI-varaktighet</td>
            <td>Tidsfasad KPI</td>
            <td>TMPH</td>
            <td>TimePhasedKPI</td>
            <td>TIMEPHASED_DURATION_CURRENT<br>TIMEPHASED_DURATION_DAILY_HISTORY<br>TIMEPHASED_DURATION_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>TILLDELNING</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>TILLDELNING</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LOCATIONID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
                <tr>
             <td>METADATAID</td>
             <td>FK</td>
             <td>METADATA-registret har inte angetts</td>
             <td>–</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>REFERENCEID</td>
             <td>FK</td>
             <td>Variabel, baserad på OBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i OBJCODE-fältet</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SCHEMAID</td>
             <td>FK</td>
             <td>SCHEMA-tabellen har inte angetts. Värdet från den här tabellen anges i SCHEMANAME-kolumnen. SCHEMANAME identifierar den KPI (t.ex. planningHours, stimours och actualHours) som posten är kopplad till.</td>
             <td>SCHEMAID</td>
        </tr>
        <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
                <tr>
             <td>STAFFINGPLANID </td>
             <td>FK</td>
             <td>STAFFING_PLAN_CURRENT</td>
             <td>STAFFINGPLANID</td>
        </tr>
           <tr>
             <td>STAFFINGPLANRESOURCEID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_RESOURCE_CURRENT</td>
             <td>STAFFINGPLANRESOURCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>AKTIVITET</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
        <tr>
             <td>TIMEPHASEDDURATIONID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Tidsfasade KPI-nummer

Begränsad kundtillgänglighet

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tidsfasade KPI-nummer</td>
            <td>Tidsfasad KPI</td>
            <td>TMPH</td>
            <td>TimePhasedKPI</td>
            <td>TIMEPHASED_NUMBERS_CURRENT<br>TIMEPHASED_NUMBERS_DAILY_HISTORY<br>TIMEPHASED_NUMBERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>TILLDELNING</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>TILLDELNING</td>
        </tr>
        <tr>
             <td>EVENT_ID</td>
             <td>PK</td>
             <td>Detta är en naturlig nyckel för den tidsfasade KPI-posten</td>
             <td>–</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LOCATIONID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>METADATAID</td>
             <td>FK</td>
             <td>METADATA-registret har inte angetts</td>
             <td>–</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
                <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
                <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
                <tr>
             <td>REFERENCEID</td>
             <td>FK</td>
             <td>Variabel, baserad på OBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i OBJCODE-fältet</td>
        </tr>
                <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
                <tr>
             <td>SCHEMAID</td>
             <td>FK</td>
             <td>SCHEMA-tabellen har inte angetts. Värdet från den här tabellen anges i SCHEMANAME-kolumnen. SCHEMANAME identifierar den KPI (t.ex. planningHours, stimours och actualHours) som posten är kopplad till.</td>
             <td>–</td>
        </tr>
                <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
                <tr>
             <td>STAFFINGPLANID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_CURRENT</td>
             <td>STAFFINGPLANID</td>
        </tr>
                <tr>
             <td>STAFFINGPLANRESOURCEID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_RESOURCE_CURRENT</td>
             <td>STAFFINGPLANRESOURCEID</td>
        </tr>
                <tr>
             <td>AKTIVITET</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
                <tr>
             <td>TIMEPHASEDNUMBERSID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
                <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Tidrapport

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tidrapport</td>
            <td>Tidrapport</td>
            <td>TSTIPSE</td>
            <td>Tidrapport</td>
            <td>TIMESHEETS_CURRENT<br>TIMESHEETS_DAILY_HISTORY<br>TIMESHEETS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GODKÄNNANDE</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>TIDSPEL</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>TIMESHEETPROFILEID</td>
             <td>FK</td>
             <td>TIMESHEETPROFILES_CURRENT</td>
             <td>TIMESHEETPROFILEID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Tidrapportprofil

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tidrapportprofil</td>
            <td>Tidrapportprofil</td>
            <td>TSPRO</td>
            <td>Tidrapportprofil</td>
            <td>TIMESHEETPROFILES_CURRENT<br>TIMESHEETPROFILES_DAILY_HISTORY<br>TIMESHEETPROFILES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GODKÄNNANDE</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>TIMESHEETPROFILEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
    </tbody>
</table>

### Gränssnittsfilter

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Gränssnittsfilter</td>
            <td>Filter</td>
            <td>UIFT</td>
            <td>Filter</td>
            <td>UIFILTERS_CURRENT<br>UIFILTERS_DAILY_HISTORY<br>UIFILTERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på OBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i OBJCODE-fältet</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>FK</td>
             <td>PREFERENCES_CURRENT</td>
             <td>PREFERENCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>UIFILTERID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
    </tbody>
</table>

### Gränssnittsgrupp efter

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Gränssnittsgrupp efter</td>
            <td>Gruppering</td>
            <td>UIGB</td>
            <td>Gruppering</td>
            <td>UIGROUPBYS_CURRENT<br>UIGROUPBYS_DAILY_HISTORY<br>UIGROUPBYS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på OBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i OBJCODE-fältet</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>FK</td>
             <td>PREFERENCES_CURRENT</td>
             <td>PREFERENCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>UIGROUPBYID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
    </tbody>
</table>

### Användargränssnittsmall

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Användargränssnittsmall</td>
            <td>Layoutmall</td>
            <td>UITMPL</td>
            <td>Layoutmall</td>
            <td>UITEMPLATES_CURRENT<br>UITEMPLATES_DAILY_HISTORY<br>UITEMPLATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
    </tbody>
</table>

### Gränssnittsvy

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Gränssnittsvy</td>
            <td>Visa</td>
            <td>UIVIEW</td>
            <td>Visa</td>
            <td>UIVIEWS_CURRENT<br>UIVIEWS_DAILY_HISTORY<br>UIVIEWS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på OBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i OBJCODE-fältet</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>FK</td>
             <td>PREFERENCES_CURRENT</td>
             <td>PREFERENCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>UIVIEWID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
    </tbody>
</table>

### Användare

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Användare</td>
            <td>Användare</td>
            <td>ANVÄNDARE</td>
            <td>Användare</td>
            <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSLEVELID</td>
             <td>FK</td>
             <td>ACCESSLEVELS_CURRENT</td>
             <td>ACCESSLEVELID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DEFAULTHOURTYPEID</td>
             <td>FK</td>
             <td>HOURTYPES_CURRENT</td>
             <td>HOURTYPEID</td>
        </tr>
        <tr>
             <td>DELEGATIONTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EAUTHUSERID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>HOMEGROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>HOMETEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>LASTENTEREDNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LATESTUPDATENOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>–</td>
             <td colspan="2">Layoutmallstabellen stöds inte</td>
        </tr>
        <tr>
             <td>MANAGERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTALPROFILEID</td>
             <td>–</td>
             <td colspan="2">Portalprofiltabellen stöds inte</td>
        </tr>
        <tr>
             <td>PREFUIID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>RESURCEPOOLID</td>
             <td>FK</td>
             <td>RESOURCEPOOLS_CURRENT</td>
             <td>RESURCEPOOLID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>TIMESHEETPROFILEID</td>
             <td>FK</td>
             <td>TIMESHEETPROFILES_CURRENT</td>
             <td>TIMESHEETPROFILEID</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>UUMUSERID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
    </tbody>
</table>

### Användardelegering

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Användardelegering</td>
            <td>Användardelegering</td>
            <td>USRDEL</td>
            <td>Användardelegering</td>
            <td>USERDELEGATIONS_CURRENT<br>USERDELEGATIONS_DAILY_HISTORY<br>USERDELEGATIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>FROMUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>TOUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERDELEGATIONID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
    </tbody>
</table>

### Användargrupp

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Användargrupp</td>
            <td>Andra grupper</td>
            <td>USRGPS</td>
            <td>Användargrupp</td>
            <td>USERSGROUPS_CURRENT<br>USERSGROUPS_DAILY_HISTORY<br>USERSGROUPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERSGROUPID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
    </tbody>
</table>

### Användarplats

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Användarplats</td>
            <td>Användarplats</td>
            <td>USRLOC</td>
            <td>UserLocation</td>
            <td>USERLOCATIONS_CURRENT<br>USERLOCATIONS_DAILY_HISTORY<br>USERLOCATIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CLASSIFIERID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERLOCATIONID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
    </tbody>
</table>

### Användarroll

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Användarroll</td>
            <td>Andra roller</td>
            <td>USRROL</td>
            <td>Användarroll</td>
            <td>USERSROLES_CURRENT<br>USERSROLES_DAILY_HISTORY<br>USERSROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERROLESETID</td>
             <td>FK</td>
             <td>USERROLESET_CURRENT</td>
             <td>USERROLESETID</td>
        </tr>
        <tr>
             <td>USERLOCATIONID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
    </tbody>
</table>

### Värde för användarinställningar

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Värde för användarprefix</td>
            <td>Användarinställningar</td>
            <td>USERPF</td>
            <td>Användarinställningar</td>
            <td>USERPREFVALUES_CURRENT<br>USERPREFVALUES_DAILY_HISTORY<br>USERPREFVALUES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERPREFVALUEID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
    </tbody>
</table>

### Uppsättning med användarroller

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>UserRoleSet</td>
            <td>Uppsättning med användarroller</td>
            <td>URSET</td>
            <td>UserRoleSet</td>
            <td>USERROLESET_CURRENT<br>USERROLESET_DAILY_HISTORY<br>USERROLESET_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PRIMARYROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERROLESETID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
    </tbody>
</table>

### Användarbeslut

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>UsersDecision</td>
            <td>Användarbeslut</td>
            <td>USRDEC</td>
            <td>Användarbeslut</td>
            <td>USERSBESLUT_CURRENT<br>USERSBESLUT_DAILY_HISTORY<br>USERSBESLUT_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>USERAVIONID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Arbetsobjekt

<table>
    <thead>
        <tr>
            <th>Workfront entitetsnamn</th>
            <th>Gränssnittsreferenser</th>
            <th>API-referens</th>
            <th>API-etikett</th>
            <th>Datasjövyer</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>WorkItem</td>
            <td>Arbetsobjekt</td>
            <td>WRKITM</td>
            <td>WorkItem</td>
            <td>WORKITEMS_CURRENT<br>WORKITEMS_DAILY_HISTORY<br>WORKITEMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Primär/extern nyckel</th>
            <th>Typ</th>
            <th>Relaterad tabell</th>
            <th>Relaterat fält</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>TILLDELNING</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>TILLDELNING</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabel, baserad på OBJCODE</td>
             <td>Primärnyckeln / ID för objektet som identifieras i OBJCODE-fältet</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>–</td>
             <td colspan="2">Inte en relation, används för interna programsyften</td>
        </tr>
        <tr>
             <td>AKTIVITET</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>AKTIVITET</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>WORKITEM-ID</td>
             <td>PK</td>
             <td>–</td>
             <td>–</td>
        </tr>
    </tbody>
</table>

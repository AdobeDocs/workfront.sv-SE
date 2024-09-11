---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Connect-dataordlista
description: Den här sidan innehåller information om datastrukturen och innehållet i Workfront Data Connect.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: 57c08a06a57bebfaa81035e4fe801f3077e6a829
workflow-type: tm+mt
source-wordcount: '4295'
ht-degree: 0%

---

# Workfront Data Connect-dataordlista

Den här sidan innehåller information om datastrukturen och innehållet i Workfront Data Connect.

>[!NOTE]
>
>Data i Data Connect uppdateras var fjärde timme, så de senaste ändringarna kanske inte återspeglas direkt.

## Tabelltyper

Det finns ett antal tabelltyper som du kan använda i Data Connect för att visa dina Workfront-data på ett sätt som ger dig den mest insikt.

* **Aktuell tabell**

  I den aktuella tabellen visas data på ungefär samma sätt som i Workfront, alla objekt och det aktuella läget. Den kan navigeras med mycket lägre latens än inom Workfront.

* **Händelsetabell**

  Händelsetabellen spårar alla ändringsposter i Workfront: det vill säga varje gång ett objekt ändras skapas en post som visar när ändringen inträffade, vem som gjorde ändringen och vad som ändrades. Den här tabellen är därför användbar för jämförelser vid olika tidpunkter. Denna tabell innehåller endast poster från de senaste tre åren.

* **Daglig historiktabell**

  Tabellen Daglig historik innehåller en förkortad version av tabellen Event, eftersom den visar varje objekts tillstånd dagligen i stället för när varje enskild händelse inträffade. Den här tabellen är därför användbar för trendanalys.

<!-- Custom table -->

## Enhetsrelationsdiagram

Objekt i Workfront (och därför i Data Connect-datavinen) definieras inte bara av deras individuella värden, utan av deras relationer med andra objekt. I entitetsrelationsdiagrammet nedan finns en mappning på hög nivå av objektrelationer i Data Connect. Diagrammet kan visas och laddas ned via följande länk:

[Relationsdiagram för dataanslutning](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

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

Följande tabell korrelerar objektnamn i Workfront (samt deras namn i gränssnittet och API:t) med deras motsvarande namn i Data Connect.

<table>
  <thead>
    <tr>
        <th>Workfront entitetsnamn</th>
        <th>Gränssnittsreferenser</th>
        <th>API-referens | Etikett</th>
        <th>Data Lake-tabeller</th>
        <th>Alternativ</th>
        <th>Relationsfält</th>
        <th>Relationstabell och fält</th>
    </tr>
  </thead>
  <tbody>
    <tr>
        <td>Åtkomstnivå</td>
        <td>Åtkomstnivå</td>
        <td>ACSLVL | Åtkomstnivå</td>
        <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
        <td></td>
        <td>ACCESSLEVELID (self)<br>APPGLOBALID<br>LASTUPDATEDBYID<br>LEGACYACCESSLEVELID<br>OBJID<br>SYSID</td>
        <td>Självständig<br>Inte en relation, används för interna programsyften<br>USER_CURRENT | USERID<br>Inte en relation; används för interna programsyften<br>ID:t för objektet som identifieras i OBJCODE-fältet<br>Inte en relation; används för interna programsyften</td>
    </tr>
    <tr>
        <td>Åtkomstregel</td>
        <td>Dela</td>
        <td>ACSRUL | Dela</td>
        <td>ACCESSREGLER_CURRENT<br>ACCESSREGLER_DAILY_HISTORY<br>ACCESSREGLER_EVENT</td>
        <td></td>
        <td>ACCESSORID <br>ACCESSRULEID (self) <br>ANCESTORID <br>LASTUPDATEDBYID <br>SECURITYOBJID <br>SYSID</td>
        <td>ID för objektet som identifieras i ACCESSOROBJCODE-fältet<br>Self<br>ID för objektet som identifieras i ANCESTOROBJCODE-fältet<br>USERS_CURRENT | USERID<br>ID:t för objektet som identifieras i fältet SECURITYOBJCODE <br>Inte en relation, används i interna programsyften</td>
    </tr>
    <tr>
        <td>Godkännandesökväg</td>
        <td>Godkännandesökväg</td>
        <td>ARVPTH | Godkännande</td>
        <td>APPROVALPATHS_CURRENT<br>APPROVALPATHS_DAILY_HISTORY<br>APPROVALPATHS_EVENT</td>
        <td></td>
        <td>APPROVALPATHID (self) <br>APPROVALPROCESSID <br>ENTEREDBYID <br>GLOBALPATHID <br>LASTUPDATEDBYID <br>SYSID</td>
        <td>Self<br>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USERS_CURRENT | USERID<br>Inte en relation; används för interna programsyften<br>USERS_CURRENT | USERID<br>Inte en relation; används för interna programsyften</td>
    </tr>
    <tr>
        <td>Godkännandeprocess</td>
        <td>Godkännandeprocess</td>
        <td>ARVPRC | Godkännandeprocess</td>
        <td>APPROVALPROCESSES_CURRENT<br>APPROVALPROCESSES_DAILY_HISTORY<br>APPROVALPROCESSES_EVENT</td>
        <td></td>
        <td>APPROVALPROCESSID (self) <br>ENTEREDBYID <br>LASTUPDATEDBYID<br>SYSID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID<br>Inte en relation; används för interna programsyften</td>
    </tr>
    <tr>
        <td>Godkännandesteg</td>
        <td>Godkännandesteg</td>
        <td>ARVSTP | Godkännandefas</td>
        <td>APPROVALSTEPS_CURRENT<br>APPROVALSTEPS_DAILY_HISTORY<br>APPROVALSTEPS_EVENT</td>
        <td></td>
        <td>GODKÄNNANDEPATHID <br>APPROVALSTEPID (self) <br>SYSID</td>
        <td>APPROVALPATHS_CURRENT | APPROVALPATHID<br>Self<br>Inte en relation; används för interna programsyften</td>
    </tr>
    <tr>
        <td>Godkännarstatus</td>
        <td>Godkännarstatus</td>
        <td>ARVSTS | Godkännarstatus</td>
        <td>APPROVERSTATUSES_CURRENT<br>APPROVERSTATUSES_DAILY_HISTORY<br>APPROVERSTATUSES_EVENT</td>
        <td></td>
        <td>APPROVERSTATUSID (self)<br>APPROVABLEOBJID<br>APPROVALSTEPID<br>APPROVEDBYID <br>DELEGATEUSERID<br>LASTUPDATEDBYID <br>OPTASKID<br>OVERRIDDENUSERID<br>PROJECTID<br>STEPAPPROVERID<br>SYSID<br> <br>TASKIDWILDCARDUSERID</td>
        <td>Själv<br>ID för objektet som identifieras i fältet APPROVABLEOBJCODE <br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID <br>OPTASKS_CURRENT | OPTASKID<br>USERS_CURRENT | USERID<br>PROJECTS_CURRENT | PROJECTID<br>USERS_CURRENT | USERID<br>Inte en relation; används för interna programsyften<br>TASKS_CURRENT | TASKID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Tilldelning</td>
        <td>Tilldelning</td>
        <td>ASSGN | Tilldelning</td>
        <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
        <td></td>
        <td>ASSIGNEDBYID<br>ASSIGNEDTOID<br>ASSIGNMENTID (self)<br>CATEGORYID<br>CLASSIFIERID<br>OPTASKID<br>PRIVATERATECARDID<br>PROJECTID<br>ROLEID<br>TASKID<br>TEAMID</td>
        <td>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>Self<br>CATEGORIES_CURRENT | CATEGORYID<br>Klassificeringstabellen stöds inte för närvarande<br>OPTASK_CURRENT | OPTASKID<br>RATECARD_CURRENT | RATECARDID<br>PROJECT_CURRENT | PROJECTID<br>ROLE_CURRENT | ROLEID<br>TASK_CURRENT | TASKID<br>TEAM_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>Väntar på godkännanden</td>
        <td>Väntar på godkännanden</td>
        <td>AWAPVL | Väntar på godkännande</td>
        <td>AWAITINGAPPROVALS_CURRENT<br>AWAITINGAPPROVALS_DAILY_HISTORY<br>AWAITINGAPPROVALS_EVENT</td>
        <td></td>
        <td>ACCESSREQUESTID<br>APPROVABLEID <br>APPROVERID <br>AWAITINGAPPROVALID (self) <br>DOCUMENTID <br>DOCUMENTVERSIONID<br>OPTASKID <br>PROJECTID <br>ROLEID <br>SUBMITTEDBYID <br>SYSID<br>TASKSKD ID <br> TEAMID <br>TIMESHEETID<br>USERID</td>
        <td>Åtkomstbegärandetabellen stöds inte för närvarande<br>Inte en relation; används för interna programsyften<br>USERS_CURRENT | USERID<br>self<br>DOCUMENTS_CURRENT | DOCUMENTID<br>DOCUMENTVERSIONS_CURRENT | DOCUMENTVERSIONID<br>OPTASKS_CURRENT | OPTASKID<br>PROJECTS_CURRENT | PROJECTID<br>ROLES_CURRENT | ROLEID<br>USERS_CURRENT | USERID<br>Inte en relation; används för interna programsyften<br>TASKS_CURRENT | TASKID<br>TEAMS_CURRENT | TEAMID<br>TIMESHEETS_CURRENT | TIMESHEETID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Baslinje</td>
        <td>Baslinje</td>
        <td>BLIN | Baslinje</td>
        <td>BASELINES_CURRENT<br>BASELINES_DAILY_HISTORY<br>BASELINES_EVENT</td>
        <td></td>
        <td>BASELINEID (self)<br>EXCHANGERATEID <br>PROJECTID <br>SYSID</td>
        <td>Self<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>PROJECTS_CURRENT | PROJECTID<br>Inte en relation; används för interna programsyften</td>
    </tr>
    <tr>
        <td>Originalaktivitet</td>
        <td>Originalaktivitet</td>
        <td>BSTSK | Originalaktivitet</td>
        <td>BASELINETASKS_CURRENT<br>BASELINETASKS_DAILY_HISTORY<br>BASELINETASKS_EVENT</td>
        <td></td>
        <td>BASELINEID<br>BASELINETASKID (self) <br>EXCHANGERATEID <br>PROJECTID <br>SYSID<br>TASKID</td>
        <td>BASELINES_CURRENT | BASELINEID<br>Self<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>PROJECTS_CURRENT | PROJECTID<br>Inte en relation; används för interna programsyften<br>TASKS_CURRENT | AKTIVITET</td>
    </tr>
    <tr>
        <td>Faktureringstakt</td>
        <td>Klassificera eller åsidosätt hastighet</td>
        <td>KURS | Faktureringstakt</td>
        <td>RATES_CURRENT<br>RATES_DAILY_HISTORY<br>RATES_EVENT</td>
        <td></td>
        <td>TILLDELA<br>CLASSIFIERID<br>EXCHANGERATEID<br>NLBRCATEGORYID<br>NONLABORRESOURCEID<br>OBJID<br>PROJECTID <br>RATECARDID<br>RATEID (self)<br>ROLEID <br>SOURCERATECARDID  <br>SYSID <br>TEMPLATEID<br>USERID</td>
        <td>ASSIGNMENTS_CURRENT | ASSIGNMENTID<br>Klassificeringstabellen stöds inte för närvarande<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>Kategoritabellen för icke-arbetsplats stöds inte för närvarande<br>NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID<br>ID för objektet som identifieras i OBJCODE-fältet<br>PROJECTS_CURRENT | PROJECTID <br>RATECARD_CURRENT | RATECARDID<br>Self<br>ROLES_CURRENT | ROLEID <br>RATECARD_CURRENT | RATECARDID <br>Inte en relation, används för interna programsyften <br>TEMPLATES_CURRNT | TEMPLATEID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Faktureringspost</td>
        <td>Faktureringspost</td>
        <td>BILL | Faktureringspost</td>
        <td>BILLINGRECORDS_CURRENT<br>BILLINGRECORDS_DAILY_HISTORY<br>BILLINGRECORDS_EVENT</td>
        <td></td>
        <td>BILLINGRECORDID (self)<br>CATEGORYID<br>EXCHANGERATEID <br>INVOICEID <br>LASTUPDATEDBYID <br>PROJECTID <br>SYSID</td>
        <td>Self<br>CATEGORIES_CURRENT | CATEGORYID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID <br> Fakturatabellen stöds inte för närvarande <br>USERS_CURRENT | USERID <br> PROJECTS_CURRENT | PROJECTID   <br>Inte en relation, används för interna programsyften</td>
    </tr>
    <tr>
        <td>Bokning</td>
        <td>Bokning</td>
        <td>BOOKNG | Bokning</td>
        <td>BOOKINGS_CURRENT<br>BOOKINGS_DAILY_HISTORY<br>BOOKINGS_EVENT</td>
        <td></td>
        <td>BOOKINGID (self)<br>ENTEREDBYID<br>LASTUPDATEDBYID<br>NLBRCATEGORYID<br>NONLABORRESOURCEID<br>OBJID<br>PROJECTID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOID POBJID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID<br>Icke-arbetskategoritabell stöds inte för närvarande<br>NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID<br>ID:t för objektet som identifieras i OBJOBJCODE-fältet<br>PROJECTS_CURRENT | PROJECTID <br>Inte en relation; används för interna programsyften<br>TASKS_CURRENT | AKTIVITET     <br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>ID för objektet som identifieras i TOPOBJCODE-fältet</td>
    </tr>
    <tr>
        <td>Kategori</td>
        <td>Eget formulär</td>
        <td>CTGY | Kategori</td>
        <td>CATEGORIES_CURRENT<br>CATEGORIES_DAILY_HISTORY<br>CATEGORIES_EVENT</td>
        <td></td>
        <td>CATEGORYID (self)<br>ENTEREDBYID<br>GROUPID <br>LASTUPDATEDBYID <br>SYSID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID <br>USERS_CURRENT | USERID <br>Inte en relation; används för interna programsyften</td>
    </tr>
    <tr>
        <td>Kategoriparameter</td>
        <td>Anpassade formulärfält</td>
        <td>CTGYPA | Kategoriparameter</td>
        <td>CATEGORIESPARAMETERS_CURRENT<br>CATEGORIESPARAMETERS_DAILY_HISTORY<br>CATEGORIESPARAMETERS_EVENT</td>
        <td></td>
        <td>CATEGORIESPARAMETERID (self)<br>CATEGORYID<br>PARAMETERGROUPID<br>PARAMETERID    <br>SYSID</td>
        <td>Self<br>CATEGORIES_CURRENT | CATEGORYID<br>Parameter Group-tabellen stöds inte just nu<br>PARAMETERS_CURRENT | PARAMETERID    <br> Inte en relation, används för interna programsyften</td>
    </tr>
    <tr>
        <td>Företag</td>
        <td>Företag</td>
        <td>CMPY | Företag</td>
        <td>COMPANIES_CURRENT<br>COMPANIES_DAILY_HISTORY<br>COMPANIES_EVENT</td>
        <td></td>
        <td>CATEGORYID<br>COMPANYID (self)<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>PRIVATERATECARDID<br>SYSID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>USERS_CURRENT | USERID <br> GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | USERID <br> RATECARD_CURRENT | RATECARDID<br>Inte en relation; används för interna programsyften</td>
    </tr>
    <tr>
        <td>Anpassat kvartal</td>
        <td>Anpassat kvartal</td>
        <td>CSTQRT | Anpassat kvartal</td>
        <td>CUSTOMQUARTERS_CURRENT<br>CUSTOMQUARTERS_DAILY_HISTORY<br>CUSTOMQUARTERS_EVENT</td>
        <td></td>
        <td>ANPASSAD KARTERID (self) <br>SYSID</td>
        <td>Självständig<br>Inte en relation, används för interna programsyften</td>
    </tr>
    <tr>
        <td>CustomEnum</td>
        <td>Villkor, Prioritet, Allvarlighetsgrad, Status</td>
        <td>CSTEM | Anpassad uppräkning</td>
        <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT</td>
        <td>Posttypen identifieras med egenskapen enumClass. Följande typer förväntas:<br>CONDITION_OPTASK<br>CONDITION_PROJ<br>CONDITION_TASK<br>PRIORITY_OPTASK<br>PRIORITY_PROJ<br>PRIORITY_TASK<br>SEVERITY_OPTASK<br>STATUS_OPTASK<br>STATUS_PROJ<br>STATUS_TAUS SK</td>
        <td>ENTEREDBYID<br>GRUPPID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID</td>
    </tr>
    <tr>
        <td>Dokument</td>
        <td>Dokument</td>
        <td>DOCU | Dokument</td>
        <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT<br>DOCUMENTS_CUSTOM_VALUE_CURRENT<br>DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>DOCUMENTS_CUSTOM_VALUE_EVENT</td>
        <td></td>
        <td>CATEGORYID<br>CHECKEDOUTBYID<br>DOCUMENTID<br>DOCUMENTREQUESTID<br>EXCHANGERATEID<br>ITERATIONID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>NOTEID<br>OBJID<br>OPTASKID<br>OWNEUID RID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>RELEASEVERSIONID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID<br>USERID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>Self<br>Tabellen för dokumentbegäran stöds inte just nu<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>ITERATIONS_CURRENT | ITERATIONID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br>Variabel beroende på DOCOBJCODE-värde<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>PORTFOLIO_CURRENT | PORTFOLIOID <br>PROGRAM_CURRENT | PROGRAMID<br>PROJECT_CURRENT | PROJECTID<br>Versionsversionstabellen stöds inte för närvarande<br>TASK_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>Variabel beroende på TOPOBJCODE-värdet<br>USER_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Godkännande av dokument</td>
        <td>Godkännande av dokument</td>
        <td>DOCAPL | Godkännande av dokument</td>
        <td>DOCAPPROVALS_CURRENT<br>DOCAPPROVALS_DAILY_HISTORY<br>DOCAPPROVALS_EVENT</td>
        <td></td>
        <td>APPROVERID<br>DOCAPPROVALID (self)<br>DOCUMENTID<br>NOTEID<br>REQUESTORID<br>SYSID</td>
        <td>USERS_CURRENT | USERID <br>Self<br>DOCUMENTS_CURRENT | DOCUMENTID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID <br>Inte en relation; används för interna programsyften</td>
    </tr>
    <tr>
        <td>Dokumentmapp</td>
        <td>Dokumentmapp</td>
        <td>DOCFLD | DocsFolders</td>
        <td>DOCFOLDERS_CURRENT<br>DOCFOLDERS_DAILY_HISTORY<br>DOCFOLDERS_EVENT</td>
        <td></td>
        <td>DOCFOLDERID (self)<br>ENTEREDBYID<br>ISSUEID<br>ITERATIONID    <br>LINKEDFOLDERID<br>PARENTID<br>PORTFOLIOID <br> PROGRAMID    <br>PROJECTID<br>SYSID<br>TASKID     <br>TEMPLATEID<br>TEMPLATETASKID<br>USERID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>OPTASKS_CURRENT | OPTASKID<br>ITERATIONS_CURRENT | ITERATIONID<br>LINKEDFOLDERS_CURRENT | LINKEDFOLDERID<br>DOCFOLDERS_CURRENT | DOCFOLDERID<br>PORTFOLIO_CURRENT | PORTFOLIOID <br>PROGRAM_CURRENT | PROGRAMID    <br> PROJECTS_CURRENT | PROJECTID <br>Inte en relation; används för interna programsyften<br>TASKS_CURRENT | AKTIVITET     <br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>DokumentAngeMetadata</td>
        <td>Dokumentets metadata</td>
        <td>DOCMET | DocumentProviderMetadata</td>
        <td>DOCPROVIDERMETA_CURRENT<br>DOCPROVIDERMETA_DAILY_HISTORY<br>DOCPROVIDERMETA_EVENT</td>
        <td></td>
        <td>DOCPROVIDERMETAID (self) <br>SYSID</td>
        <td>Självständig<br>Inte en relation, används för interna programsyften</td>
    </tr>
    <tr>
        <td>DocumentProvider</td>
        <td>Dokumentleverantör</td>
        <td>DOCPRO | Dokumentleverantör</td>
        <td>DOCPROVIDERS_CURRENT<br>DOCPROVIDERS_DAILY_HISTORY<br>DOCPROVIDERS_EVENT</td>
        <td></td>
        <td>DOCPROVIDERCONFIGID<br>DOCPROVIDERID (self)<br>OWNERID    <br>SYSID</td>
        <td>DOCPROVIDERCONFIG_CURRENT | DOCPROVIDERCONFIGID<br>Self<br>USERS_CURRENT | USERID    <br> Inte en relation, används för interna programsyften</td>
    </tr>
    <tr>
        <td>Dokumentproviderkonfiguration</td>
        <td>Dokumentproviderkonfiguration</td>
        <td>DOCCFG | Dokumentproviderkonfiguration</td>
        <td>DOCPROVIDERCONFIG_CURRENT<br>DOCPROVIDERCONFIG_DAILY_HISTORY<br>DOCPROVIDERCONFIG_EVENT</td>
        <td></td>
        <td>DOCPROVIDERCONFIGID (self)<br>SYSID</td>
        <td>Självständig<br>Inte en relation, används för interna programsyften</td>
    </tr>
    <tr>
        <td>DocumentVersion</td>
        <td>Dokumentversion</td>
        <td>DOCV | Dokumentversion</td>
        <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
        <td></td>
        <td>DOCUMENTID<br>DOCUMENTPROVIDERID<br>DOCUMENTVERSIONID<br>ENTEREDBYID<br>EXTERNALSTORAGEID<br>PROOFAPPROVALSTATUSID<br>PROOFEDBYUSERID<br>PROOFID<br>PROOFOWNERID<br>PROOFSTAGRIDPROOTAGD EID</td>
        <td>DOCUMENT_CURRENT | DOCUMENTID<br>DOCPROVIDERS_CURRENT | DOCUMENTPROVIDERID<br>self<br>USER_CURRENT | USERID<br>Externt ID<br>Statustabellen för korrektur av godkännande stöds inte för närvarande<br>USER_CURRENT | USERID<br>Korrekturtabell stöds inte för närvarande<br>USER_CURRENT | USERID<br>Korrektur för scentabell stöds inte för närvarande</td>
    </tr>
    <tr>
        <td>Växelkurs</td>
        <td>Växelkurs</td>
        <td>EXRATERA | Växelkurs</td>
        <td>EXCHANGERATES_CURRENT<br>EXCHANGERATES_DAILY_HISTORY<br>EXCHANGERATES_EVENT</td>
        <td></td>
        <td>EXCHANGERATEID (self)<br>PROJECTID<br>SYSID <br>TEMPLATEID  </td>
        <td>Self<br>PROJECTS_CURRENT | PROJECTID <br>Inte en relation; används för interna programsyften <br>TEMPLATES_CURRENT | TEMPLATEID  </td>
    </tr>
    <tr>
        <td>Utgift</td>
        <td>Utgift</td>
        <td>EXPNS | Utgift</td>
        <td>EXPENSES_CURRENT<br>EXPENSES_DAILY_HISTORY<br>EXPENSES_EVENT</td>
        <td></td>
        <td>BILLINGRECORDID<br>CATEGORYID<br>ENTEREDBYID<br>EXCHANGERATEID <br>EXPENSEID (self) <br>EXPENSETYPEID <br>LASTUPDATEDBYID <br>OBJID <br>PROJECTID<br>SYSID<br>TASKID<br>TEMPLATETETETETETE ID<br>TEMPLATETASKID<br>TOPOBJID</td>
        <td>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID <br> Self <br> EXPENSETYPES_CURRENT | EXPENSETYPEID <br>USERS_CURRENT | USERID <br> ID för objektet som identifieras i OBJCODE-fältet <br> PROJECTS_CURRENT | PROJECTID <br>Inte en relation; används för interna programsyften<br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>ID för objektet som identifieras i TOPOBJCODE-fältet</td>
    </tr>
    <tr>
        <td>Utgiftstyp</td>
        <td>Utgiftstyp</td>
        <td>EXPTYP | Utgiftstyp</td>
        <td>EXPENSETYPES_CURRENT<br>EXPENSETYPES_DAILY_HISTORY<br>EXPENSETYPES_EVENT</td>
        <td></td>
        <td>APPGLOBALID<br>EXPENSETYPEID (self)<br>OBJID <br>SYSID  </td>
        <td>Inte en relation; används för interna programsyften<br>Self<br>ID för objektet som identifieras i OBJCODE-fältet <br>Inte en relation; används för interna programsyften  </td>
    </tr>
    <tr>
        <td>Grupp</td>
        <td>Grupp</td>
        <td>GRUPP | Grupp</td>
        <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
        <td></td>
        <td>BUSINESSLEADERID<br>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LAYOUTTEMPLATEID<br>PARENTID<br>ROOTID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>Self<br>Layoutmallstabellen stöds inte<br>GROUP_CURRENT | GROUPID<br>GROUP_CURRENT | GROUPID<br>UITEMPLATES_CURRENT | UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Timme</td>
        <td>Timme</td>
        <td>TIMME | Timme</td>
        <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
        <td></td>
        <td>APPROVEDBYID<br>BILLINGRECORDID<br>CATEGORYID<br>CLASSIFIERID<br>DUPID<br>EXCHANGERATEID<br>EXTERNALTIMESHEETID<br>HOURID<br>HOURTYPEID<br>LASTUPDATEDBYID<br>OPTASKIDID<br>IDID 10}OWNERID<br>PROJECTID<br>PROJECTOVERHEADID<br>ROLEID<br>TASKID<br>TIMESHEETID</td>
        <td>USER_CURRENT | USERID<br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>Klassificeringstabellen stöds inte för närvarande<br>Inte en relation; används för interna programsyften<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>Inte en Workfront-relation; används för integrering med externa system<br>Self<br>HOURTYPE_CURRENT | HOURTYPEID<br>USER_CURRENT | USERID<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>PROJECT_CURRENT | PROJECTID<br>Inte en relation, används för interna programsyften <br>ROLE_CURRENT | ROLEID<br>TASK_CURRENT | TASKID<br>TIMESHEET_CURRENT | TIDSPEL</td>
    </tr>
    <tr>
        <td>Timtyp</td>
        <td>Timtyp</td>
        <td>TID | Timtyp</td>
        <td>HOURTYPES_CURRENT</td>
        <td></td>
        <td>APPGLOBALID<br>HOURTYPEID<br>OBJID</td>
        <td>Inte en relation; används för interna programsyften<br>Själf<br>Inte en relation; används för interna programsyften</td>
    </tr>
    <tr>
        <td>Upprepning</td>
        <td>Upprepning</td>
        <td>ITRN | Upprepning</td>
        <td>ITERATIONS_CURRENT<br>ITERATIONS_DAILY_HISTORY<br>ITERATIONS_EVENT</td>
        <td></td>
        <td>CATEGORYID<br>ENTEREDBYID<br>ITERATIONID (self)<br>LASTUPDATEDBYID<br>OWNERID<br>SYSID<br>TEAMID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID <br>self<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>Inte en relation; används för interna programsyften<br>TEAMS_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>Journalpost</td>
        <td>Journalpost</td>
        <td>JRNLE | Journalpost</td>
        <td>JOURNALENTRIES_CURRENT<br>JOURNALENTRIES_DAILY_HISTORY<br>JOURNALENTRIES_EVENT</td>
        <td></td>
        <td>APPROVERSTATUSID<br>ASSIGNMENTID<br>AUDITRECORDID<br>BASELINEID <br>BILLINGRECORDID<br>COMPANYID <br>DOCUMENTID <br>DOCUMENTSHAREID <br>EDITEDBYID<br>EXPENSEID<br>HOURID<br> INITIATIVEID<br>JOURNALENTRIEID (self)<br>OBJID<br>OPTASKID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>SUBOBJID<br>SUBSCRIBEID<br>SYSID<br>TA. SKID<br>TEMPLATEID<br>TIMESHEETID<br>TOPOBJID<br>USERID</td>
        <td>APPROVERSTATUSES_CURRENT | APPROVERSTATUSID<br>ASSIGNMENTS_CURRENT | ASSIGNMENTID<br>Register för granskningspost stöds inte just nu<br>BASELINES_CURRENT | BASELINEID <br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>COMPANIES_CURRENT | COMPANYID <br>DOCUMENTS_CURRENT | DOCUMENTID <br> Dokumentdelningstabellen stöds inte för närvarande <br>USERS_CURRENT | USERID<br>EXPENSES_CURRENT | UTGITAD<br>HOURS_CURRENT | HOURID<br>Initiative table not supported current<br>Self<br>The ID of the object identify in the OBJCODE field<br>OPTASKS_CURRENT | OPTASKID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECTS_CURRENT | PROJECTID <br>ID:t för objektet som identifieras i SUBOBJCODE-fältet<br>Prenumerationstabellen stöds inte för närvarande<br>Inte en relation, används för interna programsyften<br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TIMESHEETS_CURRENT | TIMESHEETID<br>ID:t för objektet som identifieras i TOPOBJCODE-fältet<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>LinkedFolder</td>
        <td>LinkedFolder</td>
        <td>LNKFDR | LinkedFolder</td>
        <td>LINKEDFOLDERS_CURRENT<br>LINKEDFOLDERS_DAILY_HISTORY<br>LINKEDFOLDERS_EVENT</td>
        <td></td>
        <td>DOCUMENTPROVIDERID<br>EXTERNALSTORAGEID<br>FOLDERID<br>LINKEDBYID<br>LINKEDFOLDERID (self)<br>SYSID</td>
        <td>DOCPROVIDERS_CURRENT | DOCPROVIDERID<br>Externt ID<br>DOCFOLDERS_CURRENT | DOCFOLDERID<br>USERS_CURRENT | USERID <br>Self<br>Not a relationship; used for internal application purposes  </td>
    </tr>
    <tr>
        <td>Milstolpe</td>
        <td>Milstolpe</td>
        <td>MILE | Milstolpe</td>
        <td>MILESTONES_CURRENT<br>MILESTONES_DAILY_HISTORY<br>MILESTONES_EVENT</td>
        <td></td>
        <td>LASTUPDATEDBYID<br>MILESTONEID<br>MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID<br>Self<br>MILESTONEPATH_CURRENT | MILESTONEID</td>
    </tr>
    <tr>
        <td>MilstolpePath</td>
        <td>Sökväg för milstolpe</td>
        <td>MPATH | Sökväg för milstolpe</td>
        <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
        <td></td>
        <td>ENTEREDBYID<br>LASTUPDATEDBYID<br>MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>Self</td>
    </tr>
    <tr>
        <td>NonLaborResource</td>
        <td>Icke-arbetsrelaterad resurs</td>
        <td>NLBR | Icke-arbetsrelaterad resurs</td>
        <td>NONLABORRESOURCES_CURRENT<br>NONLABORRESOURCES_DAILY_HISTORY<br>NONLABORRESOURCES_EVENT</td>
        <td></td>
        <td>CATEGORYID<br>NONLABORRESOURCEID (self)<br>ENTEREDBYID<br>HOMEGROUPID<br>LASTUPDATEDBYID<br>NONLABORRESOURCECATEGORYID <br>SYSID  </td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>USERS_CURRENT | USERID <br> GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | USERID <br>Icke-arbetsrelaterad resurskategoritabell stöds inte för närvarande <br>Inte en relation, används för interna programsyften    </td>
    </tr>
    <tr>
        <td>Ledig dag</td>
        <td>Schemaundantag</td>
        <td>NONWKD | Ledig arbetsdag</td>
        <td>NONWORKDAYS_CURRENT<br>NONWORKDAYS_DAILY_HISTORY<br>NONWORKDAYS_EVENT</td>
        <td></td>
        <td>NONWORKDAYID (self)<br>OBJID <br>SCHEDULEID <br>SYSID <br>USERID  </td>
        <td>Själv<br>ID för objektet som identifieras i OBJCODE-fältet <br>SCHEDULES_CURRENT | SCHEDULEID <br>Inte en relation; används för interna programsyften <br>USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Anteckning</td>
        <td>Anteckning</td>
        <td>ANMÄRKNING | Anteckning</td>
        <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
        <td></td>
        <td>ATTACHDOCUMENTID<br>ATTACHOBJID<br>ATTACHOPTASKID<br>ATTACHWORKID<br>ATTACHWORKUSERID<br>AUDITRECORDID<br>COMPANYID<br>DOCUMENTID<br>EXTERNALSERVICEID<br>ITERATIONID<br>NOTEID{NOTEID 10}OBJID<br>OPTASKID<br>OWNERID<br>PARENTENDORSEMENTID<br>PARENTJOURNALENTRYID<br>PARENTNOTEID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>PROJECTID OFACTIONID<br>PROOFID<br>RICHTEXTNOTEID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TREADID<br>TIMESHEETID<br>TOPOBJID<br>USERID<br></td>
        <td>DOCUMENT_CURRENT | DOCUMENTID<br>Variabel beroende på ATTACHOBJCODE<br>OPTASK_CURRENT | OPTASKID<br>WORKITEMS_CURRENT<br>USER_CURRENT | USERID<br>Registret Granskningspost stöds inte för närvarande<br>COMPANIES_CURRENT | COMPANYID <br>DOCUMENT_CURRENT | DOCUMENTID<br>Inte en Workfront-relation; används för integration med externa system<br>ITERATIONS_CURRENT | ITERATIONID<br>Self<br>Variabel beroende på NOTEOBJCODE<br>OPTASK_CURRENT | OPTASKID <br>USER_CURRENT | USERID<br>Bekräftelsetabellen stöds inte för närvarande<br>JOURNALENTRIES_CURRENT | JOURNALENTRYID<br>NOTE_CURRENT | NOTEID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECT_CURRENT | PROJECTID<br>Korrekturåtgärdstabellen stöds inte för närvarande<br>Korrekturtabellen stöds inte för närvarande<br>RESERVEDTEXTNOTES_CURRENT | RICHTEXTNOTEID<br>TASK_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>NOTE_CURRENT | NOTEID<br>TIMESHEET_CURRENT | TIMESHEETID<br>Variabel beroende på TOPOBJCODE<br>USER_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Objektintegrering</td>
        <td>Objektintegrering</td>
        <td>OBJEKT | ObjectIntegration</td>
        <td>OBJECTINTEGRATION_CURRENT<br>OBJECTINTEGRATION_DAILY_HISTORY<br>OBJECTINTEGRATION_EVENT</td>
        <td></td>
        <td>LINKEDOBJECTID<br>OBJECTINTEGRATIONID   (self)<br>OBJID <br>SYSID  </td>
        <td>ID:t för objektet som identifieras i fältet LINKEDOBJECTCODE <br>Self<br>ID:t för objektet som identifieras i fältet OBJCODE <br>Inte en relation, används i interna programsyften  </td>
    </tr>
    <tr>
        <td>Objektkategori</td>
        <td>Objektkategorier</td>
        <td>OBJCAT | Objektkategori</td>
        <td>OBJECTSCATEGORIES_CURRENT<br>OBJECTSCATEGORIES_DAILY_HISTORY<br>OBJECTSCATEGORIES_EVENT</td>
        <td></td>
        <td>CATEGORYID<br>OBJECTSCATEGORYID (self)<br>OBJID <br>SYSID  </td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>ID:t för objektet som identifieras i OBJCODE-fältet <br>Inte en relation; används för interna programsyften  </td>
    </tr>
    <tr>
        <td>OpTask</td>
        <td>Problem, begäran</td>
        <td>OPTASK | Problem</td>
        <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT<br>OPTASKS_CUSTOM_VALUE_CURRENT<br>OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>OPTASKS_CUSTOM_VALUE_EVENT</td>
        <td></td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>CATEGORYID<br>CURRENTAPPROVALSTEPID<br>ENTEREDBYID<br>EXCHANGERATEID<br>ITERATIONID<br>KANBANBOARDID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDUD ATEDBYID<br>OPTASKID<br>OWNERID<br>PROJECTID<br>QUEUEDEFID<br>QUEUETOPICID<br>RESOLVEOPTASKID<br>RESOLVEPROJECTID<br>RESOLVETASKID<br>RESOLVINGOB. JID<br>ROLEID<br>SOURCEOBJID<br>SOURCETASKID<br>SUBMITTEDBYID<br>TEAMID</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USER_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USER_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>ITERATIONS_CURRENT | ITERATIONID<br>Kanban Board-tabellen stöds inte just nu<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>Self<br>USER_CURRENT | USERID<br>PROJECT_CURRENT | PROJECTID<br>Tabellen Ködefinition stöds inte för närvarande<br>Tabellen Köämne stöds inte för närvarande<br>OPTASK_CURRENT | OPTASKID<br>PROJECT_CURRENT | PROJECTID<br>TASK_CURRENT | TASKID<br>Variabel beroende på RESOLVINGOBJCODE<br>ROLE_CURRENT | ROLEID<br>Variabel beroende på SOURCEOBJCODE<br>TASK_CURRENT | TASKID<br>USER_CURRENT | USERID<br>TEAM_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>Parameter</td>
        <td>Anpassat fält</td>
        <td>PARAM | Parameter</td>
        <td>PARAMETERS_CURRENT<br>PARAMETERS_DAILY_HISTORY<br>PARAMETERS_EVENT</td>
        <td></td>
        <td>LASTUPDATEDBYID<br>PARAMETERFILTERID<br>PARAMETERID (self)<br>SYSID  </td>
        <td>USERS_CURRENT | USERID<br>Parameter Filter-tabellen stöds inte för närvarande<br>Self<br>Inte en relation; används för interna programsyften  </td>
    </tr>
    <tr>
        <td>Parameteralternativ</td>
        <td>Parameteralternativ</td>
        <td>POPT | Parameteralternativ</td>
        <td>PARAMETEROPTIONS_CURRENT<br>PARAMETEROPTIONS_DAILY_HISTORY<br>PARAMETEROPTIONS_EVENT</td>
        <td></td>
        <td>PARAMETERID<br>PARAMETEROPTIONID (self) <br>SYSID  </td>
        <td>PARAMETERS_CURRENT | PARAMETERID <br>Egen <br>Inte en relation; används för interna programsyften  </td>
    </tr>
    <tr>
        <td>Portalavsnitt</td>
        <td>Rapport</td>
        <td>PTLSEC | Rapport</td>
        <td>PORTALSECTIONS_CURRENT<br>PORTALSECTIONS_DAILY_HISTORY<br>PORTALSECTIONS_EVENT</td>
        <td></td>
        <td>APPGLOBALID<br>ENTEREDBYID<br>FILTERID<br>GROUPBYID<br>LASTUPDATEDBYID<br>LASTVIEWEDBYID<br>OBJID<br>PORTALSECTIONID (self)<br>PREFERENCEID<br>PUBLICRUNASUSERID<br>REPORTFOLDERID <br>RUNASUSERID<br>SCHEDULEDREPORTID<br>SYSID<br>VISA</td>
        <td>Inte en relation; används för interna programsyften <br>USERS_CURRENT | USERID <br> UIFILTERS_CURRENT | FILTERID<br>UIGROUPBYS_CURRENT | GROUPBYID<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>ID:t för objektet som identifieras i fältet OBJOBJCODE <br>Self<br>PREFERENCES_CURRENT | PREFERENCEID<br>USERS_CURRENT | USERID <br>REPORTFOLDERS_CURRENT | RAPPORTFOLDERID<br>USERS_CURRENT | USERID  <br>Schemalagd rapporttabell stöds inte för närvarande<br>Inte en relation, används för interna programsyften <br>UIVIEWS_CURRENT | VISA</td>
    </tr>
    <tr>
        <td>Portal Tab</td>
        <td>Kontrollpanel</td>
        <td>PTLTAB | Kontrollpanel</td>
        <td>PORTALTABS_CURRENT<br>PORTALTABS_DAILY_HISTORY<br>PORTALTABS_EVENT</td>
        <td></td>
        <td>DOCID<br>LASTUPDATEDBYID<br>PORTALPROFILEID<br>PORTALTABID (self)<br>SYSID<br>USERID</td>
        <td>Inte en relation; används för interna programsyften <br>USERS_CURRENT | USERID <br>Portal Profile table will not supported <br>Self<br>Not a relationship; used for internal application purposes <br>USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Portal Tab Section</td>
        <td>Instrumentpanelsavsnitt</td>
        <td>PRTBSC | Portal Tab Section</td>
        <td>PORTALTABSPORTALSECTIONS_CURRENT<br>PORTALTABSPORTALSECTIONS_DAILY_HISTORY<br>PORTALTABSPORTALSECTIONS_EVENT</td>
        <td></td>
        <td>CALENDARPORTALSECTIONID<br>EXTERNALSECTIONID<br>INTERNALSECTIONID <br>PORTALSECTIONOBJID <br>PORTALTABID<br>PORTALTABID SECTIONID (self)<br>SYSID</td>
        <td>Kalenderportalavsnittet stöds inte för närvarande<br>Den externa avsnittstabellen stöds inte för närvarande<br>PORTALSECTIONS_CURRENT | PORTALSECTIONID <br> ID:t för objektet som identifieras i fältet PORTALSECTIONOBJCODE <br>PORTALTABS_CURRENT | PORTALTABID<br>Self<br>Not a relationship; used for internal application purposes</td>
    </tr>
    <tr>
        <td>PortalSectionLastViewer</td>
        <td>Rapportera senaste visningsprogram</td>
        <td>PLSLSV | PortalSectionLastViewer</td>
        <td>REPORTLASTVIEWERS_CURRENT<br>REPORTLASTVIEWERS_DAILY_HISTORY<br>REPORTLASTVIEWERS_EVENT</td>
        <td></td>
        <td>RAPPORTERA<br>RAPPORTLASTVIEWERID (self)<br>SYSID<br>VIEWERID</td>
        <td>PORTALSECTIONS_CURRENT | PORTALSECTIONID <br>REPORTLASTVIEWERID (self)<br>Inte en relation; används för interna programsyften<br>USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Portfolio</td>
        <td>Portfolio</td>
        <td>PORT | Portfolio</td>
        <td>PORTFOLIO_CURRENT<br>PORTFOLIO_DAILY_HISTORY<br>PORTFOLIO_EVENT<br>PORTFOLIO_CUSTOM_VALUE_CURRENT<br>PORTFOLIO_CUSTOM_VALUE_DAILY_HISTORY<br>PORTFOLIO_CUSTOM_VALUE_EVENT</td>
        <td></td>
        <td>ALIGNMENTSCORECARDID<br>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>OWNERID<br>PORTFOLIOID</td>
        <td>Styrkortstabellen stöds inte för närvarande<br>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>Self</td>
    </tr>
    <tr>
        <td>Inställningar</td>
        <td>Visa, Filtrera, Gruppera, Rapportdefinition</td>
        <td>PROSET | Inställningar</td>
        <td>PREFERENCES_CURRENT<br>PREFERENCES_DAILY_HISTORY<br>PREFERENCES_EVENT</td>
        <td></td>
        <td>APPGLOBALID<br>PREFERENCEID (self) <br>SYSID  </td>
        <td>Inte en relation; används för interna programsyften<br>Själv <br>Inte en relation; används för interna programsyften  </td>
    </tr>
    <tr>
        <td>Program</td>
        <td>Program</td>
        <td>PRGM | Program</td>
        <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT<br>PROGRAMS_CUSTOM_VALUE_CURRENT<br>PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>PROGRAMS_CUSTOM_VALUE_EVENT</td>
        <td></td>
        <td>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>OWNERID<br>PORTFOLIOID<br>PROGRAMID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>Self</td>
    </tr>
    <tr>
        <td>Projekt</td>
        <td>Projekt</td>
        <td>PROJ | Projekt</td>
        <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT<br>PROJECTS_CUSTOM_VALUE_CURRENT<br>PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>PROJECTS_CUSTOM_VALUE_EVENT</td>
        <td></td>
        <td>AEMNATIVEFOLDERTREESREFID<br>ALIGNMENTSCORECARDID<br>APPROVALPROCESSID<br>ATTACHEDRATECARDID<br>CATEGORYID<br>COMPANYID<br>CONVERTEDOPTASKID<br>CONVERTEDOPTASKORIGINATORID<br>CURRENTAPPROVALSTEPID<br>DELIVERABLESCORECARDID<br>ENTEREDBYID<br>GROUPID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEPATHID<br>OWNERID<br> POPACCOUNTID<br>PORTFOLIOID<br>PRIVATERATECARDID<br>PROGRAMID<br>PROJECTID<br>QUEUEDEFID<br>REJECTIONISSUEID<br>RESOURCEPOOLID<br>SCHEDULEID<br>SPONSORID<br> 26}SUBMITTEDBYID<br>TEAMID<br>TEMPLATEID</td>
        <td>Inte en Workfront-relation; används för integrering med externa system<br>Styrkortstabellen stöds inte för närvarande<br>APPROPROCESSES_CURRENT | APPROVALPROCESSID<br>RATECARD_CURRENT | RATECARDID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID <br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>Styrkortstabell stöds inte för närvarande<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>MILESTONEPATH_CURRENT | MILESTONEPATHID<br>USER_CURRENT | USERID<br>Pop Account table not supported current<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>RATECARD_CURRENT | RATECARDID<br>PROGRAM_CURRENT | PROGRAMID<br>Self<br>Ködefinitionstabellen stöds inte för närvarande<br>OPTASK_CURRENT | OPTASKID<br>RESOURCEPOOLS_CURRENT | RESOURCEPOOLID<br>SCHEDULE_CURRENT | SCHEDULEID<br>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>TEAM_CURRENT | TEAMID<br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>RateCard</td>
        <td>Hastighetskort</td>
        <td>RTCRD |Betygskort</td>
        <td>RATECARD_CURRENT<br>RATECARD_DAILY_HISTORY<br>RATECARD_EVENT</td>
        <td></td>
        <td>CATEGORYID<br>ENTEREDBYID<br>LASTUPDATEDBYID <br>RATECARDID (self) <br>SECURITYROOTID <br>SOURCEID<br>SYSID</td>
        <td>CATEGORYID<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID    <br>Själv<br>ID:t för objektet som identifieras i fältet SECURITYOBJCODE <br>ID:t för objektet som identifieras i fältet SOURCEOBJCODE<br>Inte en relation; används i interna programsyften  </td>
    </tr>
    <tr>
        <td>Rapportmapp</td>
        <td>Rapportmapp</td>
        <td>RPTFDR | Rapportmapp</td>
        <td>REPORTFOLDERS_CURRENT<br>REPORTFOLDERS_DAILY_HISTORY<br>REPORTFOLDERS_EVENT</td>
        <td></td>
        <td>RAPPORTFOLDERID (self) <br>SYSID  </td>
        <td>Själv <br>Inte en relation, används för interna programsyften  </td>
    </tr>
    <tr>
        <td>Reserverad tid</td>
        <td>(Personligt) Tid av</td>
        <td>RESVT | Tid av</td>
        <td>RESERVEDTIMES_CURRENT<br>RESERVEDTIMES_DAILY_HISTORY<br>RESERVEDTIMES_EVENT</td>
        <td></td>
        <td>RESERVEDTIMEID (self) <br>SYSID<br>TASKID<br>USERID  </td>
        <td>Självständig<br>Inte en relation, används för interna programsyften<br>TASKS_CURRENT | TASKID<br>USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Resurspool</td>
        <td>Resurspool</td>
        <td>RSPL | Resurspool</td>
        <td>RSRCPOOLS_CURRENT<br>RSRCPOOLS_DAILY_HISTORY<br>RSRCPOOLS_EVENT</td>
        <td></td>
        <td>ENTEREDBYID<br>LASTUPDATEDBYID <br>RESOURCEPOOLID (self)<br>SYSID  </td>
        <td>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>Self<br>Not a relationship; used for internal application purposes  </td>
    </tr>
    <tr>
        <td>RTF-anteckning</td>
        <td>RTF-anteckning</td>
        <td>RHNOTE | RTF-anteckning</td>
        <td>RESERVEDTEXTNOTES_CURRENT<br>RESERVEDTEXTNOTES_DAILY_HISTORY<br>RESERVEDTEXTNOTES_EVENT</td>
        <td></td>
        <td>RICHTEXTNOTEID (self) <br>SYSID  </td>
        <td>Själv <br>Inte en relation, används för interna programsyften  </td>
    </tr>
    <tr>
        <td>Parametervärde för RTF</td>
        <td>Parametervärde för RTF</td>
        <td>RCHVAL | RichTextParameterValue</td>
        <td>RICHTEXTPARAMETERVALUES_CURRENT<br>RICHTEXTPARAMETERVALUES_DAILY_HISTORY<br>RICHTEXTPARAMETERVALUES_EVENT</td>
        <td></td>
        <td>PARAMETERVALUEID<br>RICHTEXTPARAMETERVALUID (self) <br>SYSID  </td>
        <td>Parametervärdestabellen stöds inte för närvarande<br>Själf <br>Inte en relation; används för interna programsyften  </td>
    </tr>
    <tr>
        <td>risk</td>
        <td>risk</td>
        <td>RISK | risk</td>
        <td>RISKS_CURRENT<br>RISKS_DAILY_HISTORY<br>RISKS_EVENT</td>
        <td></td>
        <td>ENTEREDBYID<br>EXCHANGERATEID<br>LASTUPDATEDBYID <br>PROJECTID <br>RISKID (self)<br>RISKTYPEID<br>SYSID<br>TEMPLATEID</td>
        <td>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>USERS_CURRENT | USERID <br> PROJECTS_CURRENT | PROJECTID   <br> Self<br> RISKTYPES_CURRENT | RISKTYPEID<br>Inte en relation; används för interna programsyften<br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>Risktyp</td>
        <td>Risktyp</td>
        <td>RSKTYP | Risktyp</td>
        <td>RISKTYPES_CURRENT<br>RISKTYPES_DAILY_HISTORY<br>RISKTYPES_EVENT</td>
        <td></td>
        <td>RISKTYPEID<br>SYSID</td>
        <td>Självständig<br>Inte en relation, används för interna programsyften</td>
    </tr>
    <tr>
        <td>Roll</td>
        <td>Jobbroll</td>
        <td>ROLE | Jobbroll</td>
        <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
        <td></td>
        <td>ENTEREDBYID<br>LAYOUTTEMPLATEID<br>PRIVATERATECARDID<br>ROLEID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>Layoutmallstabellen stöds inte<br>RATECARD_CURRENT | RATECARDID<br>Self<br>UITEMPLATES_CURRENT |UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Schema</td>
        <td>Schema</td>
        <td>SCHED | Schema</td>
        <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
        <td></td>
        <td>ENTEREDBYID<br>GROUPID<br>HOMEGROUPID<br>SCHEDULEID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>GROUP_CURRENT | GROUPID<br>Self</td>
    </tr>
    <tr>
        <td>Steggodkännare</td>
        <td>Steggodkännare</td>
        <td>SPAPVR | Scengodkännare</td>
        <td>STEPAPPROVERS_CURRENT<br>STEPAPPROVERS_DAILY_HISTORY<br>STEPAPPROVERS_EVENT</td>
        <td></td>
        <td>APPROVALSTEPID<br>ROLEID<br>STEPAPPROVERID (self)<br>SYSID <br>TEAMID<br>USERID</td>
        <td>APPROVALSTEPS_CURRENT | GODKÄNN<br>ROLES_CURRENT | ROLEID<br>Self<br>Not a relationship; used for internal application purpose <br>TEAMS_CURRENT | TEAMID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Uppgift</td>
        <td>Uppgift</td>
        <td>UPPGIFT | Uppgift</td>
        <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT<br>TASKS_CUSTOM_VALUE_CURRENT<br>TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>TASKS_CUSTOM_VALUE_EVENT</td>
        <td></td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>BILLINGRECORDID<br>CATEGORYID<br>CONVERTEDOPTASKID<br>CONVERTEDOPTASKORIGINATORID<br>CURRENTAPPROVALSTEPID<br>ENTEREDBYID<br>EXCHANGERATEID<br>GROUPUPID ID<br>ITERATIONID<br>KANBANBOARDID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEID<br>PARENTID<br>PROJECTID<br>RECURRENCERULEID<br> 18}REJECTIONISSUEID<br>RESERVEDTIMEID<br>ROLEID<br>SUBMITTEDBYID<br>TASKID<br>TEAMID<br>TEMPLATETASKID</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USER_CURRENT | USERID<br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USER_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>GROUP_CURRENT | GROUPID<br>ITERATIONS_CURRENT | ITERATIONID<br>Tabellen för kanban-tavlan stöds inte för närvarande<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>MILESTONE_CURRENT | MILESTONEID<br>TASK_CURRENT | TASKID<br>PROJECT_CURRENT | PROJECTID<br>Upprepningsregeltabellen stöds inte för närvarande<br>OPTASK_CURRENT | OPTASKID<br>RESERVEDTIMES_CURRENT | RESERVEDTIMEID<br>ROLE_CURRENT | ROLEID<br>USER_CURRENT | USERID<br>Self<br>TEAM_CURRENT | TEAMID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID</td>
    </tr>
    <tr>
        <td>Aktivitetsföregångare</td>
        <td>Föregående</td>
        <td>PRED | Föregående</td>
        <td>PREDECESSORS_CURRENT<br>PREDECESSORS_DAILY_HISTORY<br>PREDECESSORS_EVENT</td>
        <td></td>
        <td>ID (self)<br>PREDECESSORID<br>SUCCESSORID <br>SYSID</td>
        <td>Egendom<br>TASKS_CURRENT | TASKID<br>TASKS_CURRENT | TASKID <br>Inte en relation; används för interna programsyften</td>
    </tr>
    <tr>
        <td>Team</td>
        <td>Team</td>
        <td>TEAMOB | Team</td>
        <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
        <td></td>
        <td>ENTEREDBYID<br>GROUPID<br>LAYOUTTEMPLATEID<br>MYWORKVIEWID<br>OWNERID<br>REQUESTSVIEWID<br>SCHEDULEID<br>TEAMID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>Layoutmallstabellen stöds inte<br>UIVIEWS_CURRENT | UIVIEWID<br>USER_CURRENT | USERID<br>UIVIEWS_CURRENT | UIVIEWID<br>SCHEDULE_CURRENT | SCHEDULEID<br>Self<br>UITEMPLATES_CURRENT |UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Teammedlem</td>
        <td>Andra team, teammedlem</td>
        <td>TEAMMB | Teammedlem</td>
        <td>TEAMMEMBERS_CURRENT<br>TEAMMEMBERS_DAILY_HISTORY<br>TEAMMEMBERS_EVENT</td>
        <td></td>
        <td>SYSID <br>TEAMID<br>TEAMMEMBERID (self)<br>USERID</td>
        <td>Inte en relation; används för interna programsyften <br>TEAMS_CURRENT | TEAMID<br>Self<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>TeamMemberRole</td>
        <td>Teammedlemsroll</td>
        <td>TEAMMR | Teammedlemsroll</td>
        <td>TEAMMEMBERROLES_CURRENT<br>TEAMMEMBERROLES_DAILY_HISTORY<br>TEAMMEMBERROLES_EVENT</td>
        <td></td>
        <td>ROLEID <br>TEAMID<br>TEAMMEMBERROLEID (self)<br>USERID</td>
        <td>ROLES_CURRENT | ROLEID <br>TEAMS_CURRENT | TEAMID<br>Self<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Mall</td>
        <td>Mall</td>
        <td>TMPL | Mall</td>
        <td>TEMPLATES_CURRENT<br>TEMPLATES_DAILY_HISTORY<br>TEMPLATES_EVENT</td>
        <td></td>
        <td>APPROVALPROCESSID<br>CATEGORYID<br>COMPANYID <br>DELIVERABLESCORECARDID <br>ENTEREDBYID<br>GROUPID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEPATHID <br>OWNERID <br>PRIVATERATECARARID DID<br>PROGRAMID<br>QUEUEDEFID<br>SCHEDULEID <br>SYSID <br>TEAMID<br>TEMPLATEID (self)</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID   <br>DELIVERABLESCORECARDID <br>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID<br>MILESTONEPATH_CURRENT | MILESTONEPATHID <br>USERS_CURRENT | USERID <br>RATECARD_CURRENT | RATECARDID<br>PROGRAM_CURRENT | PROGRAMID<br>Ködefinitionstabellen stöds inte för närvarande<br>SCHEDULES_CURRENT | SCHEDULEID <br>Inte en relation, används för interna programsyften <br>TEAMS_CURRENT | TEAMID<br>Self</td>
    </tr>
    <tr>
        <td>Malltilldelning</td>
        <td>Malltilldelning</td>
        <td>TASSGN | Malltilldelning</td>
        <td>TEMPLATEASSIGNMENTS_CURRENT<br>TEMPLATEASSIGNMENTS_DAILY_HISTORY<br>TEMPLATEASSIGNMENTS_EVENT</td>
        <td></td>
        <td>ASSIGNEDTOID<br>CATEGORYID<br>LASTUPDATEDBYID<br>OBJID<br>ROLEID<br>SYSID<br>TEAMID<br>TEAMTIMELINEABLEID<br>TEMPLATEASSIGNMENTID (self)<br>TEMPLATETASKID</td>
        <td>USERS_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>ID:t för objektet som identifieras i OBJCODE-fältet<br>ROLES_CURRENT | ROLEID<br>Inte en relation; används för interna programsyften<br>TEAMS_CURRENT | TEAMID<br>Tidslinjerbar tabell för team stöds inte för närvarande<br>Self<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID</td>
    </tr>
    <tr>
        <td>Malluppgift</td>
        <td>Malluppgift</td>
        <td>TTSK | Malluppgift</td>
        <td>TEMPLATETASKS_CURRENT<br>TEMPLATETASKS_DAILY_HISTORY<br>TEMPLATETASKS_EVENT</td>
        <td></td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>CATEGORYID<br>ENTEREDBYID<br>EXCHANGERATEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEID<br>PARENTID<br>RECURRENCERULEID<br>ROLEID<br>SYSID<br>TEAMID<br>TEAMTIMELINEABLEID<br>TEMPLATEID<br>TEMPLATETASKID (self)</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USERS_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID<br>MILESTONE_CURRENT | MILESTONEID<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID<br>Upprepningsregeltabellen stöds inte just nu<br>ROLES_CURRENT | ROLEID<br>Inte en relation; används för interna programsyften<br>TEAMS_CURRENT | TEAMID<br>Tidslinjerbar tabell för team stöds inte för närvarande<br>TEMPLATES_CURRENT | TEMPLATEID<br>Self</td>
    </tr>
    <tr>
        <td>Föregångare för mallaktivitet</td>
        <td>Mallföregångare</td>
        <td>TPRED | Föregående</td>
        <td>TEMPLATEPREDECESSORS_CURRENT<br>TEMPLATEPREDECESSORS_DAILY_HISTORY<br>TEMPLATEPREDECESSORS_EVENT</td>
        <td></td>
        <td>PREDECESSORID<br>SLUTFÖRSORID <br>TEMPLATEPREDECESSORID (self)<br>SYSID</td>
        <td>TEMPLATETASKS_CURRENT |TEMPLATETASKID<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID <br>Egen<br>Inte en relation; används för interna programsyften</td>
    </tr>
    <tr>
        <td>Tidrapport</td>
        <td>Tidrapport</td>
        <td>TSTIPSE | Tidrapport</td>
        <td>TIMESHEETS_CURRENT<br>TIMESHEETS_DAILY_HISTORY<br>TIMESHEETS_EVENT</td>
        <td></td>
        <td>APPROVERID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>TIMESHEETID<br>TIMESHEETPROFILEID<br>USERID</td>
        <td>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>Self<br>TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID<br>USER_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Tidrapportprofil</td>
        <td>Tidrapportprofil</td>
        <td>TSPRO | Tidrapportprofil</td>
        <td>TIMESHEETPROFILES_CURRENT<br>TIMESHEETPROFILES_DAILY_HISTORY<br>TIMESHEETPROFILES_EVENT</td>
        <td></td>
        <td>APPROVERID<br>ENTEREDBYID <br>GROUPID<br>SYSID<br>TIMESHEETPROFILEID (self)</td>
        <td>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID <br>GROUPS_CURRENT | GROUPID<br>Inte en relation; används för interna programsyften<br>Själv</td>
    </tr>
    <tr>
        <td>Gränssnittsfilter</td>
        <td>Filter</td>
        <td>UIFT | Filter</td>
        <td>UIFILTERS_CURRENT<br>UIFILTERS_DAILY_HISTORY<br>UIFILTERS_EVENT</td>
        <td></td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIFILTERID (self)</td>
        <td>Inte en relation; används för interna programsyften<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br> ID:t för objektet som identifieras i OBJCODE-fältet <br>PREFERENCES_CURRENT | PREFERENCEID<br>Inte en relation; används för interna programsyften <br>Själv</td>
    </tr>
    <tr>
        <td>Gränssnittsgrupp efter</td>
        <td>Gruppering</td>
        <td>UIGB | Gruppering</td>
        <td>UIGROUPBYS_CURRENT<br>UIGROUPBYS_DAILY_HISTORY<br>UIGROUPBYS_EVENT</td>
        <td></td>
        <td>ENTEREDBYID<br>GROUPID <br>LASTUPDATEDBYID <br>SYSID <br>UITEMPLATEID (self)</td>
        <td>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GRUPPID <br>USERS_CURRENT | USERID <br>Inte en relation; används för interna programsyften <br>Själv</td>
    </tr>
    <tr>
        <td>Användargränssnittsmall</td>
        <td>Layoutmall</td>
        <td>UITMPL | Layoutmall</td>
        <td>UITEMPLATES_CURRENT<br>UITEMPLATES_DAILY_HISTORY<br>UITEMPLATES_EVENT</td>
        <td></td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIGROUPBYID (self)</td>
        <td>Inte en relation; används för interna programsyften<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br> ID:t för objektet som identifieras i OBJCODE-fältet <br>PREFERENCES_CURRENT | PREFERENCEID<br>Inte en relation; används för interna programsyften <br>Själv</td>
    </tr>
    <tr>
        <td>Gränssnittsvy</td>
        <td>Visa</td>
        <td>UIVIEW | Visa</td>
        <td>UIVIEWS_CURRENT<br>UIVIEWS_DAILY_HISTORY<br>UIVIEWS_EVENT</td>
        <td></td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIVIEWID (self)</td>
        <td>Inte en relation; används för interna programsyften<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br> ID:t för objektet som identifieras i OBJCODE-fältet <br>PREFERENCES_CURRENT | PREFERENCEID<br>Inte en relation; används för interna programsyften <br>Själv</td>
    </tr>
    <tr>
        <td>Användare</td>
        <td>Användare</td>
        <td>ANVÄNDARE | Användare</td>
        <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT<br>USERS_CUSTOM_VALUE_CURRENT<br>USERS_CUSTOM_VALUE_DAILY_HISTORY<br>USERS_CUSTOM_VALUE_EVENT</td>
        <td></td>
        <td>ACCESSLEVELID<br>CATEGORYID<br>COMPANYID<br>DEFAULTHOURTYPEID<br>DELEGATIONTOID<br>EAUTHUSERID<br>ENTEREDBYID<br>HOMEGROUPID<br>HOMETEAMID<br>LASTENTEREDNOTEID<br>LASTUPDAID TEDBYID<br>LATESTUPDATENOTEID<br>LAYOUTTEMPLATEID<br>MANAGERID<br>PORTALPROFILEID<br>PREFUID<br>PRIVATERATECARDID<br>RESOURCEPOOLID<br>ROLEID<br>SCHEDULEID<br>TIMESHEETPROFILEID<br>UITEMPLATEID<br>USERID<br>UUMUSERID</td>
        <td>ACCESSLEVELS_CURRENT |ACCESSLEVELID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID <br>HOURTYPE_CURRENT | HOURTYPEID<br>USER_CURRENT | USERID<br>Inte en relation; används för interna programsyften<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>TEAM_CURRENT | TEAMID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br>Layoutmallstabellen stöds inte<br>USER_CURRENT | USERID<br>Portal Profile table will not be supported<br>Not a relationship; used for internal application purpose<br>RATECARD_CURRENT | RATECARDID<br>RESOURCEPOOLS_CURRENT | RESOURCEPOOLID<br>ROLE_CURRENT | ROLEID<br>SCHEDULE_CURRENT | SCHEDULEID<br>TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID<br>UITEMPLATES_CURRENT |UITEMPLATEID<br>Egen<br>Inte en relation, används för interna programsyften</td>
    </tr>
    <tr>
        <td>Användardelegering</td>
        <td>Användardelegering</td>
        <td>USRDEL | Användardelegering</td>
        <td>USERDELEGATIONS_CURRENT<br>USERDELEGATIONS_DAILY_HISTORY<br>USERDELEGATIONS_EVENT</td>
        <td></td>
        <td>FROMUSERID<br>SYSID <br>TOUSERID <br>USERDELEGATIONID (self)</td>
        <td>USERS_CURRENT | USERID<br>Inte en relation; används för interna programsyften <br>USERS_CURRENT | USERID <br>Self</td>
    </tr>
    <tr>
        <td>Användargrupp</td>
        <td>Andra grupper</td>
        <td>USRGPS | Användargrupp</td>
        <td>USERSGROUPS_CURRENT<br>USERSGROUPS_DAILY_HISTORY<br>USERSGROUPS_EVENT</td>
        <td></td>
        <td>GRUPPID <br>SYSID<br>USERID <br>USERSGROUPID (self)</td>
        <td>GROUPS_CURRENT | GROUPID <br>Inte en relation; används för interna programsyften<br>USERS_CURRENT | USERID <br>Self</td>
    </tr>
    <tr>
        <td>Användarroll</td>
        <td>Andra roller</td>
        <td>USRROL | Användarroll</td>
        <td>USERSROLES_CURRENT<br>USERSROLES_DAILY_HISTORY<br>USERSROLES_EVENT</td>
        <td></td>
        <td>ROLEID <br>SYSID<br>USERID    <br>USERROLESETID<br>USERSROLEID (self)</td>
        <td>ROLES_CURRENT | ROLEID <br>Inte en relation; används för interna programsyften<br>USERS_CURRENT | USERID    <br> USERROLESET_CURRENT | USERROLESETID<br>Self</td>
    </tr>
    <tr>
        <td>UserPrefValue</td>
        <td>UserPrefValue</td>
        <td>USERPF | Användarinställningar</td>
        <td>USERPREFVALUES_CURRENT<br>USERPREFVALUES_DAILY_HISTORY<br>USERPREFVALUES_EVENT</td>
        <td></td>
        <td>SYSID    <br>USERID <br>USERPREFVALUEID (self)</td>
        <td>Inte en relation; används för interna programsyften<br>USERS_CURRENT | USERID    <br>Själv</td>
    </tr>
    <tr>
        <td>UserRoleSet</td>
        <td>UserRoleSet</td>
        <td>URSET | UserRoleSet</td>
        <td>USERROLESET_CURRENT<br>USERROLESET_DAILY_HISTORY<br>USERROLESET_EVENT</td>
        <td></td>
        <td>PRIMARYROLEID <br>SYSID<br>USERID    <br>USERROLESETID (self)</td>
        <td>ROLES_CURRENT | ROLEID <br>Inte en relation; används för interna programsyften<br>USERS_CURRENT | USERID <br>Self</td>
    </tr>
    <tr>
        <td>UsersDecision</td>
        <td>Användarbeslut</td>
        <td>USRDEC | Användarbeslut</td>
        <td>USERSBESLUT_CURRENT<br>USERSBESLUT_DAILY_HISTORY<br>USERSBESLUT_EVENT</td>
        <td></td>
        <td>USERDECIONID (self)<br>SYSID <br>USERID  </td>
        <td>Självständig<br>Inte en relation, används för interna programsyften <br>USERS_CURRENT | USERID </td>
    </tr>
    <tr>
        <td>WorkItem</td>
        <td>Arbetsobjekt</td>
        <td>WRKITM | WorkItem</td>
        <td>WORKITEMS_CURRENT<br>WORKITEMS_DAILY_HISTORY<br>WORKITEMS_EVENT</td>
        <td></td>
        <td>TILLDELA <br>OBJID<br>OPTASKID    <br> PROJECTID <br>SYSID<br> - AKTIVITET    <br>USERID <br>WORKITEM (self)</td>
        <td>ASSIGNMENTS_CURRENT | ASSIGNMENTID <br>ID för objektet som identifieras i OBJOBJCODE-fältet<br>OPTASK_CURRENT | OPTASKID    <br> PROJECTS_CURRENT | PROJECTID <br>Inte en relation; används för interna programsyften<br>TASKS_CURRENT | AKTIVITET    <br>USERS_CURRENT | USERID    <br>Själv </td>
    </tr>
  </tbody>
</table>

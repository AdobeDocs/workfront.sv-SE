---
content-type: api
navigation-topic: api-navigation-topic
title: Uppdateringar av API-version 8
description: Visa uppdateringarna av API-version 8.
author: Becky
feature: Workfront API
role: Developer
exl-id: c6d7d2d2-cd21-4ca8-a5a0-afe3669dc959
source-git-commit: ae80999fc7ea7e35097560aa99baa435bcd31b74
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Uppdateringar av API-version 8

## Uppdaterade resurser

Följande befintliga resurser har uppdaterats med den här versionen av Adobe Workfront API. Om du vill se vilka resurser som är nya för version 8 går du till [Nyheter i API-version 8](../../wf-api/api/new-api-version-8.md). Ändringar som görs i en resurs anges på följande sätt:

* Tilläggen visas bara i listan
* Borttagningar anges med genomstrykningstext
* Ändringar noteras i anteckningen efter tabellen

### AccessRequest

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| åtgärd<sup>1</sup>  |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Ändringar av möjliga värden

### AccessRule<sup>1</sup> 

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| coreAction<sup>2</sup>  |   |   |   |   |   |   |
| forbiddenActions<sup>2</sup> |   |   |   |   |   |   |
| secondaryActions<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Borttagen flagga: RAPPORTERBAR\
<sup>2</sup> Ändringar av möjliga värden

### Godkännande

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  | resourcePools |   |   |   |   |
| backlogOrder<sup>2</sup> | kanbanBoard  |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Ändringar av möjliga värden\
<sup>2</sup>Tillagda flaggor: DYNAMIC, LAZY_READ och NOT_GROUPABLE

### Tilldelning

|   |   |   |   | Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnTasks | getAssignAssignmentsForTasks  |   |   |   |   |   |
|   |   |   |   | swapUsersOnTasks | getUnassignAssignmentsForTasks |   |   |   |   |   |
|   |   |   |   | unassignUserFromTasks |   |   |   |   |   |   |

{style="table-layout:auto"}

### Kund

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| bizRuleExclusions<sup>1</sup> |   |   |   | getPackagingOptionValue |   |   |
| proofPlan<sup>1</sup> |   |   |   | isPackagingOptionEnabled |   |   |

{style="table-layout:auto"}

<sup>1</sup>Ändringar av möjliga värden

### CustomerPreferences

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| name<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Ändringar av möjliga värden

### DokumentGodkännande

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| ID<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Flagga tillagd: NOT_FILTERABLE

### DocumentVersion

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| activeProofStages |   |   |   |   |   |   |

{style="table-layout:auto"}

### Grupp

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
|   |   | ägare |   |   |   |   |

{style="table-layout:auto"}

### HourType

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| appGlobalID<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Flagga tillagd: NOT_FILTERABLE

### Upprepning

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
|   |   |   |   | moveStories |   |   |

{style="table-layout:auto"}

### Gilla

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |

{style="table-layout:auto"}

### Anteckning

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| auditType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Ändringar av möjliga värden

### OpTask

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  |   |   |   | defaultShownTimesheetIssues  |   |
| backlogOrder | iteration |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| uppskattning |   |   |   |   |   |   |
| iterationID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Ändringar av möjliga värden

### Portfolio

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Ändringar av möjliga värden

### Program

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Ändringar av möjliga värden

### Projekt

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   | resourcePools |   |   | defaultShownTimesheetProjects |   |

{style="table-layout:auto"}

<sup>1</sup>Ändringar av möjliga värden

### KorrekturGodkännande

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| godkännareID | godkännare |   |   |   |   |   |
| documentVersionID | documentVersion |   |   |   |   |   |
| ID<sup>1</sup> |   |   |   |   |   |   |
| proofCreationDate |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Flagga tillagd: NOT_FILTERABLE

### QueueDef

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| requestCoreAction<sup>1</sup> |   |   |   |   |   |   |
| requestForbiddenActions<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Ändringar av möjliga värden

### Hastighet

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| endDate |   |   |   | setRatesForRole  |   |   |
| name |   |   |   |   |   |   |
| startDate |   |   |   |   |   |   |

{style="table-layout:auto"}

### ReservedTime

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| extRefID |   |   |   |   |   |   |

{style="table-layout:auto"}

### ResourceManager

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| projectPriority |   |   |   |   |   |   |

{style="table-layout:auto"}

### Uppgift

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  |   |   |   | allTasksOnIterations  |   |
| backlogParent | kanbanBoard |   |   |   | defaultShownTimesheetTasks |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Ändringar av möjliga värden

### Team

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| agileMethod |   |   |   |   |   |   |
| autoAddNextStory |   |   |   |   |   |   |
| includeIssues |   |   |   |   |   |   |
| teamStoryBoardIssueStatuses |   |   |   |   |   |   |
| wipLimit |   |   |   |   |   |   |

{style="table-layout:auto"}

### Mall

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |

{style="table-layout:auto"}

### TemplateTask

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Ändringar av möjliga värden

Uppdatera

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> | `updateEndorsement` |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Ändringar av möjliga värden

### Användare

|   |   | Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |   |   |
|   |   | userGroups |   |   |   |   |   |   |
|   |   | userRoles |   |   |   |   |   |   |

{style="table-layout:auto"}

### UserNote

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |
| `endorsementShareID` | `endorsementShare` |   |   |   |   |   |
| eventType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Ändringar av möjliga värden

### Arbete

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  |   |   |   |   |   |
| backlogOrder<sup>2</sup> | kanbanBoard  |   |   |   |   |   |
| backlogParent  |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Ändringar av möjliga värden\
<sup>2</sup>Tillagda flaggor: DYNAMIC, LAZY_READ och NOT_GROUPABLE

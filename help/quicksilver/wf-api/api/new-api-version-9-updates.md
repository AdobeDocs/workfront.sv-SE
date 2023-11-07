---
content-type: api
navigation-topic: api-navigation-topic
title: Uppdateringar av API version 9
description: Uppdaterade resurser
author: Becky
feature: Workfront API
role: Developer
exl-id: 51892846-d93f-4363-8416-4118fb2ef84d
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 2%

---

# Uppdateringar av API version 9

## Uppdaterade resurser

Följande befintliga resurser har uppdaterats med den här versionen av Adobe Workfront API. Om du vill se de resurser som är nya för version 9 kan du gå till [Nyheter i API-version 9](../../wf-api/api/new-api-version-9.md) och [Nyheter i API version 9 (forts.)](../../wf-api/api/new-api-version-9-continue.md). Ändringar som görs i en resurs anges på följande sätt:

* Tilläggen visas bara i listan
* Borttagningar anges med genomstrykningstext
* Ändringar noteras i anteckningen efter tabellen

### AgileWork

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| `opTaskID`<sup>2</sup> |  |   |  |   |   |  |
| `taskID`<sup>2</sup> |   |   |  |  |  |  |

{style="table-layout:auto"}

<sup>1</sup> Borttagen flagga: RAPPORTERBAR\
<sup>2</sup> Borttagen flagga: NOT_GROUPABLE

### Godkännande

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| `storyBoardOrder` | `agileWork` |   |   |   |   |   |

{style="table-layout:auto"}

Tilldelning

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| |   |  |  | `assignUserToRoleOnProjects`<sup>1</sup> |   |   |
|   |   |   |   | `assignUserToRoleOnTasks`<sup>1</sup> |   |   |
|   |   |   |   | `swapUsersOnProjects`<sup>1</sup> |   |   |
|   |   |   |   | `swapUsersOnTasks`<sup>1</sup> |   |   |

{style="table-layout:auto"}

<sup>1</sup> Tillagt fält: lockToRole

### CustomerPreferences

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| `name`<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Ändringar av possibleValues

### Timme

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| `days` |   |   |   |   |   |   |
| `workHoursPerDay` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Upprepning

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
|   |   |   |   | `moveIssues` |   |   |

{style="table-layout:auto"}

### LayoutTemplates

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| `groupID` | `group` |   |   |   |   |   |

{style="table-layout:auto"}

### Anteckning

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| `html` |   |   |   |   |   |   |
| `json` |   |   |   |   |   |   |
| `richTextNoteID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### OpTask

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| `color` | `agileWork` |   |   | `convertToProject` |   |   |
| `isReady` |   |   |   | `convertToTask` |   |   |
| `storyBoardOrder` |   |   |   | `linkExternalObject` |   |   |
|   |   |   |   | `unlinkExternalObject` |   |   |

{style="table-layout:auto"}

### ResursBudget

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| `ID` |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Borttagen flagga: RAPPORTERBAR

### Schema

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| `homeGroupID` | `homeGroup` |   |   |   |   |   |

{style="table-layout:auto"}

### Uppgift

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
|   | `agileWork` |   |   | `convertToProject` |   |   |
|   |   |   |   | `linkExternalObject` |   |   |
|   |   |   |   | `unlinkExternalObject` |   |   |

{style="table-layout:auto"}

### Team

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| `includeIssues` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Tidrapportprofil

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| `groupID` | `group` |   |   |   |   |   |

{style="table-layout:auto"}

### UIFilter

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
|   |   |   |   |   | `filtersForObjCode` |   |

{style="table-layout:auto"}

### UIView

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
|   |   |   |   |   | `viewsForObjCode` |   |

{style="table-layout:auto"}

### Användare

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| `logTimeInDays` |   |   |   |   |   |   |
| `workHoursPerDay` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Arbete

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| `storyBoardOrder` | `agileWork` |   |   | `getWFHomeObjects` |   |   |

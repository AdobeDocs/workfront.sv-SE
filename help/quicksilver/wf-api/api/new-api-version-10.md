---
content-type: api
navigation-topic: api-navigation-topic
title: Nyheter i API-version 10
description: Uppdaterade resurser
author: Becky
feature: Workfront API
role: Developer
exl-id: 8ac384ae-5d65-4c0e-98c1-cf38cfbff460
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# Nyheter i API-version 10

* [Nya resurser](#new-resources)
* [Uppdaterade resurser](#updated-resources)
* [Borttagna resurser](#removed-resources)

## Nya resurser {#new-resources}

### ActivityLog

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   | LÄGG TILL |
|   |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | SÖK |

{style="table-layout:auto"}

### CalendarEntry

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | LÄGG TILL |
|   |   |   |   |   |   | COUNT  |
|   |   |   |   |   |   | DELETE  |
|   |   |   |   |   |   | REDIGERA  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | RAPPORT  |
|   |   |   |   |   |   | SÖK |

{style="table-layout:auto"}

### KalenderPostExternReferens

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | RAPPORT  |
|   |   |   |   |   |   | SÖK  |

{style="table-layout:auto"}

### ExternalAuthToken

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | LÄGG TILL |
|   |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | DELETE  |
|   |   |   |   |   |   | REDIGERA  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | RAPPORT  |
|   |   |   |   |   |   | SÖK  |

{style="table-layout:auto"}

### LicenseTypeGroupLimit

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| customerID | kund |   |   |   |   |   |
| groupID | grupp |   |   |   |   |   |
| planLimit |   |   |   |   |   |   |
| usedLicenses |   |   |   |   |   |   |
| arbetsgräns |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

### UserHomeCalendarPreference

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| customerID | kund |   |   |   |   | LÄGG TILL |
| edTime | användare |   |   |   |   | COUNT |
| firstDayOfWeek |   |   |   |   |   | DELETE |
| ID |   |   |   |   |   | REDIGERA |
| showPTO |   |   |   |   |   | GET |
| startTime |   |   |   |   |   | RAPPORT |
| userID |   |   |   |   |   | SÖK |
| workDate |   |   |   |   |   |   |

{style="table-layout:auto"}

**Uppdaterade resurser**

Följande befintliga resurser har uppdaterats med den här versionen av Workfront API. Ändringar som görs i en resurs anges enligt följande:

* Tilläggen visas bara i listan
* Borttagningar anges med genomstrykningstext
* Ändringarna visas i anteckningen efter tabellen

### Godkännande

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval `<sup>1</sup>`   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |
| projectBudgetedCost  |   |   |   |   |   |   |
| projectNetValue  |   |   |   |   |   |   |
| projectRoi  |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost  |   |   |   |   |   |   |

{style="table-layout:auto"}

`<sup>1</sup> Type changed from null to boolean`

### Tilldelning

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| assignPercent `<sup>1</sup>` |   |   |   |   |   |   |
| displayedByAssignedToUser |   |   |   |   |   |   |

{style="table-layout:auto"}

`<sup>1</sup>`added validator LESS_THAN_EQUAL

### BudgeteradTimme

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### CustomerPreferences

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| name `<sup>1</sup>` |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Ändringar av possibleValues

### DocMetadataLinkGroup

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
|   |   |   |   | getMetadataForDocument |   |   |

{style="table-layout:auto"}

### Dokument

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |   |   |   |   |   |

{style="table-layout:auto"}

### DocumentRequest

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

DocumentVersion

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| externalIntegrationType <sup>1</sup> |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Ändringar av possibleValues

Utgift

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Grupp

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
|   | licenseTypeLimit |   |   | addRemoveLicenseTypeLimits  |   |   |
|   |   |   |   | setLicenseTypeLimit |   |   |

{style="table-layout:auto"}

### LinkedFolder

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| externalIntegrationType<sup>1</sup> |  |  |  |  |   |   |

{style="table-layout:auto"}

<sup>1</sup> Ändringar av possibleValues

### OpTask

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| priorityColor |   |  | pendingApproval<sup>1</sup> |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Typen har ändrats från null till boolesk

### PortalSection

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
|   |  |   | groupIDs |   |   |   |

{style="table-layout:auto"}

### Portfolio

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| portfolioNetValue |   |   |   |  |  |   |
| portfolioRoi |   |   |   |   |   |   |

{style="table-layout:auto"}

### Projekt

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| projectBudgetedCost  |   |   |   | linkExternalObject  |   |   |
| projectNetValue |   |   |   | unlinkExternalObject |   |   |
| projectRoi |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost |   |   |   |   |   |   |

{style="table-layout:auto"}

### KorrekturGodkännande

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| godkännareBeslut |   |   |   |   |   |   |

{style="table-layout:auto"}

### Hastighet

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| rateValue <sup>1</sup> |  |  |  |  |  |   |

{style="table-layout:auto"}

<sup>1</sup>tillagd valideringsvaluta

### Uppgift

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| kanbanFlag |   |   |   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### Team

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| hoursPerPoint <sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> added validator LESS_THAN

### TeamAssignment

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### TeamTask

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Tidrapport

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

### Uppdatera

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| updateType `<sup>1</sup>` |   |   |   |   |   | objectUpdatesWithNoteAndJournalEntryIndex  |

{style="table-layout:auto"}

<sup>1</sup> ändringar av possibleValues

### Användare

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
|   | accessLevel  |   |   |   |   |   |

{style="table-layout:auto"}

### UserNote

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| eventType <sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> ändringar av possibleValues

### Arbete

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval <sup>1</sup>  |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Typen har ändrats från null till boolesk

## Borttagna resurser {#removed-resources}

### ResursBudgeteradTimme

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| allokeringsdatum |   |   |   |   |   | LÄGG TILL  |
| BudgeteradTimme |   |   |   |   |   | COUNT  |
| ID |   |   |   |   |   | DELETE  |
| planeradeBudgeteradeTimmar |   |   |   |   |   | REDIGERA  |
| projectID |   |   |   |   |   | GET  |
| roleID |   |   |   |   |   | RAPPORT  |
| userID |   |   |   |   |   | SÖK |

{style="table-layout:auto"}

 

 

 

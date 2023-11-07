---
content-type: api
navigation-topic: api-navigation-topic
title: Nyheter i API-version 6
description: Nyheter i API-version 6
author: Becky
feature: Workfront API
role: Developer
exl-id: e671a881-b8c2-4234-a3a0-76b1fbfafd32
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# Nyheter i API-version 6

## Nya objekt

### Resurshanteraren

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| ID | kund |   |   |   |   | Lägg till |
| customerID | projekt |   |   |   |   | Antal |
| projectID | resourceManager |   |   |   |   | Ta bort |
| resourceManagerID | mall |   |   |   |   | Hämta |
| templateID |   |   |   |   |   | Rapport  |
|   |   |   |   |   |   | Sök  |


### Vattnen

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| fileName |   |   |   |   | ladda upp |   |
| handtag |   |   |   |   |   |   |
| objCode |   |   |   |   |   |   |


### Egen etikett

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| ID |   |   |   | checkDelete | customLabels | Lägg till |
|   |   |   |   | inUseByOtherLayoutTemplate | userCustomLabels | Antal |
|   |   |   |   | removeCustomLabel |   | Ta bort |
|   |   |   |   |   |   | Hämta |
|   |   |   |   |   |   | Rapport |
|   |   |   |   |   |   | Sök |


## Uppdaterade objekt

Ändringar i befintliga objekt: tillägg visas bara, borttagningar har genomstrykning, ändringar i befintliga objekt har en bifogad anteckning efter tabellen

### Uppdatera

 

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> Ändringar av möjliga värden

<sup>2</sup> hasFilters-attributet har ändrats till true

 

### Godkännande

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| completeHours |   | resourceManagers | resourceManagerIDs |   |   |   |
| constraintDate<sup>1</sup> |   |   |   |   |   |   |
| isOriginalPlannedHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Datumvalidering har lagts till

<sup>2</sup> NOT_FILTERABLE-flagga tillagd

 

### Godkännandeprocess

|   | Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|---|
|   |  | `attachedApprovalPaths` |   |   |   |   |   |

{style="table-layout:auto"}

 

### Godkännandesteg

 

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| approvalType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Ändringar av möjliga värden

 

### Godkännandesökväg<sup>1</sup>

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| approvedStatus |   |   |   |   |   | Lägg till |
| approvedStatusLabel |   |   |   |   |   | Antal |
| kommentar |   |   |   |   |   | Ta bort |
| enteredByID |   |   |   |   |   | Redigera |
| entryDate |   |   |   |   |   | Hämta |
| globalPathID |   |   |   |   |   | Rapport |
| isPrivate |   |   |   |   |   | Sök |
| lastUpdateDate |   |   |   |   |   |   |
| lastUpdateByID |   |   |   |   |   |   |
| name<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Ändrad till Rapporteringsbar

<sup>2</sup> Längdvaliderare har lagts till

 

### Arbetstjänstobjekt

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| constraintDate<sup>1</sup> |   |   |   | getMyWorkCountFiltered |   |   |
| workRequired<sup>2</sup> |   |   |   | workItemStatusLabels  |   |   |

{style="table-layout:auto"}

<sup>1</sup> Datumvalidering tillagd

<sup>2</sup> Inte_Filterbar flagga tillagd

 

### Tilldelning

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnProjects |   |   |
|   |   |   |   | swapUsersOnProjects |   |   |
|   |   |   |   | unassignUserFromProjects |   |   |

{style="table-layout:auto"}

 

### Baslinje 

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Inte_Filterbar flagga tillagd

 

### Originalaktivitet

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Inte_Filterbar flagga tillagd

 

### Faktureringspost

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| faktureringsdatum<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> tillagd NO_TIME-fältflagga

### Burndown-händelse 

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| eventInitiator |   |   |   |   |   | `ADD` |
|   |   |   |   |   |   | `DELETE` |

{style="table-layout:auto"}

 

### Kategori 

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
|   |   |   |   | getCascadingRules |   |   |
|   |   |   |   | reorderCategories |   |   |

{style="table-layout:auto"}

 

Anpassad uppräkning 

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
|   |   |   |   | getGroupDefaultProjectStatus | opTaskGroupStatuses |   |
|   |   |   |   | isPossibleToUnlockStatus | projectGroupStatuses |   |
|   |   |   |   |   | taskGroupStatuses |   |

{style="table-layout:auto"}

 

Dokument 

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| `checkedOutByID` | `checkedOutBy`  |   |  isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

Växelkurs 

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| ränta<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> PRECISION-valideraren har ändrats för 8 till 9

 

### Integrering

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| syncBurndownDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### Journalpost

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| changeType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Ändringar av möjliga värden

 

### Optask (Issue)<sup>1</sup> 

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Flaggad som RESTORABLE

<sup>2</sup> Inte_Filterbar flagga tillagd

 

### Projekt<sup>1</sup> 

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| completeHours |   | `openOpTasks` |  openOpTasks |   |   |   |
| isOriginalPlannedHoursSet |   | resourceManagers | resourceManagerIDs  |   |   |   |
| originalWorkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| arbete |   |   |   |   |   |   |
| workRequired |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Flaggas som RESTORABLE och RESOURCE_MANAGEABLE

<sup>2</sup> Inte_Filterbar flagga tillagd

 

### Uppgift<sup>1</sup>

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| constraintDate<sup>2</sup> |   |   |   |   |   |   |
| workRequired<sup>3</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Flaggad som RESTORABLE

<sup>2</sup> AT_DATE_YEAR_BEFORE-valideraren har lagts till

<sup>3</sup> Inte_Filterbar flagga tillagd

 

### Team

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| `myWorkViewID` |  `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style="table-layout:auto"}

 

### Mall<sup>1</sup> 

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
|   |   | resourceManagers | resourceManagerIDs |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Flaggas som RESTORABLE och RESOURCE_MANAGEABLE

### Malluppgift<sup>1</sup> 

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Flaggad som RESTORABLE

<sup>2</sup> Inte_Filterbar flagga tillagd

 

### Användare

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| myInfo<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> MAX_LENGTH-överträdelse

 

### Användaranteckning

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| eventType<sup>1</sup> |   |   |   |   | myNotifications<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> Möjliga värden har ändrats

<sup>2</sup> har filter ändrat till `[true]`

 

### Meddelande

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |

---
content-type: api
navigation-topic: api-navigation-topic
title: Nyheter i API-version 8
description: Det här är en lista över resurser som är nya i API-version 9. En lista över uppdateringar av resurserna i version 8 finns på Uppdateringar till API-version 8
author: Becky
feature: Workfront API
role: Developer
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 1%

---

# Nyheter i API-version 8

## Nya resurser

Det här är en lista över resurser som är nya i API-version 9. En lista över uppdateringar som gjorts för resurserna i version 8 finns på [Uppdateringar av API-version 8](../../wf-api/api/new-api-version-8-updates.md)

**AgileWork**

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| backlogOrder | kund |   |   | bulkCopy  |   | COPY |
| färg | iteration  |   |   |   |   | COUNT |
| customerID | lastUpdatedBy |   |   |   |   | DELETE |
| uppskattning | opTask |   |   |   |   | REDIGERA |
| ID | projekt |   |   |   |   | GET  |
| isReady | storyboardParent |   |   |   |   | RAPPORT |
| iterationID | uppgift |   |   |   |   | SÖK |
| lastUpdateDate | team |   |   |   |   |   |
| lastUpdatedByID |   |   |   |   |   |   |
| name |   |   |   |   |   |   |
| opTaskID |   |   |   |   |   |   |
| parentStoryBoardOrder |   |   |   |   |   |   |
| projectID |   |   |   |   |   |   |
| storyBoardOrder |   |   |   |   |   |   |
| storyBoardParentID |   |   |   |   |   |   |
| taskID  |   |   |   |   |   |   |
| teamID |   |   |   |   |   |   |
| type |   |   |   |   |   |   |
| uiObjCode |   |   |   |   |   |   |
| uiObjectID |   |   |   |   |   |   |

{style="table-layout:auto"}

### APIVersionMetadata

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| deprecationRelease |   |   |   |   |   | COUNT  |
| removalRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | SÖK |

{style="table-layout:auto"}

**KanbanBoard**

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | LÄGG TILL |
| name |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | DELETE |
|   |   |   |   |   |   | REDIGERA |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | SÖK |

{style="table-layout:auto"}

### KorrekturGodkännandestatus

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style="table-layout:auto"}

**KorrekturFilmetadata**

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| documentVersionID | documentVersion |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| fileName |   |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style="table-layout:auto"}

**ResursBudgeteradTimme**

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| allokeringsdatum |   |   |   |   |   | LÄGG TILL |
| BudgeteradTimme |   |   |   |   |   | COUNT |
| planeradeBudgeteradeTimmar |   |   |   |   |   | DELETE |
| projectID |   |   |   |   |   | REDIGERA |
| roleID |   |   |   |   |   | GET |
| userID |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | SÖK |

{style="table-layout:auto"}

### Resursplaneringsfilter

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | LÄGG TILL |
| name |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | DELETE |
|   |   |   |   |   |   | REDIGERA |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | SÖK |

{style="table-layout:auto"}

**RichTextNote**

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | SÖK |

{style="table-layout:auto"}

### Prenumerera

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
|  ID |   |   |   | addSubscribers | prenumeranter | LÄGG TILL |
|   |   |   |   | removeSubscribers |   | COUNT  |
|   |   |   |   | prenumererar |   | DELETE |
|   |   |   |   | avsluta prenumeration |   | GET |
|   |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | SÖK |

{style="table-layout:auto"}

### UserRole

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| roleID | roll |   |   |   |   |   |
| timePercentage | användare |   |   |   |   |   |
| userID |   |   |   |   |   |   |

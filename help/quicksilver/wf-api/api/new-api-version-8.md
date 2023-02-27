---
content-type: api
navigation-topic: api-navigation-topic
title: Nyheter i API-version 8
description: Det här är en lista över resurser som är nya i API-version 9. En lista över uppdateringar av resurserna i version 8 finns på Uppdateringar till API-version 8
author: Becky
feature: Workfront API
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '288'
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

{style=&quot;table-layout:auto&quot;}

### APIVersionMetadata

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| deprecationRelease |   |   |   |   |   | COUNT  |
| removeRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | SÖK |

{style=&quot;table-layout:auto&quot;}

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

{style=&quot;table-layout:auto&quot;}

### KorrekturGodkännandestatus

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**KorrekturFilmetadata**

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| documentVersionID | documentVersion |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| fileName |   |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

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

{style=&quot;table-layout:auto&quot;}

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

{style=&quot;table-layout:auto&quot;}

**RichTextNote**

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | SÖK |

{style=&quot;table-layout:auto&quot;}

### Prenumerera

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
|  ID |   |   |   | addSubscribers | prenumeranter | LÄGG TILL |
|   |   |   |   | removeSubscribers |   | COUNT  |
|   |   |   |   | prenumererar |   | DELETE |
|   |   |   |   | avbeställa |   | GET |
|   |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | SÖK |

{style=&quot;table-layout:auto&quot;}

### UserRole

| Fält | Referenser | Samlingar | Sök | Åtgärder | Frågor | Operationer |
|---|---|---|---|---|---|---|
| roleID | roll |   |   |   |   |   |
| timePercentage | användare |   |   |   |   |   |
| userID |   |   |   |   |   |   |

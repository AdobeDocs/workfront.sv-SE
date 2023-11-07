---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Byta namn på ett dokument eller en mapp (ännu ej implementerad)
description: Byta namn på ett dokument eller en mapp
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 5b1a4a02-a7fd-41f2-9adb-74b40606270b
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '81'
ht-degree: 1%

---


# Byta namn på ett dokument eller en mapp (ännu ej implementerad)

Byter namn på ett dokument eller en mapp med det angivna ID:t i det externa systemet.

**URL**

PUT /rename

## Frågeparametrar

| Namn  | Beskrivning |
|---|---|
| id | Dokument- eller mapp-ID att byta namn på |
| name  | Det nya namnet på dokumentet eller mappen |


## Svar

En JSON-sträng som anger om åtgärden lyckades eller misslyckades, vilket anges i felhanteringsavsnittet nedan.

**Exempel:** PUT https://www.acme.com/api/rename

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

returnerar

```
{status: "success"
 }returns
 {
 status: "failure", error: "Folder cannot be renamed because a folder with that name already exists."
 }
```

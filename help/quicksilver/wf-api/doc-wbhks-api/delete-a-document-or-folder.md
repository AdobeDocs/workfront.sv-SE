---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Ta bort dokument eller mappar
description: Ta bort dokument eller mappar
author: Becky
feature: Workfront API
role: Developer
exl-id: b56ec13a-1ee1-4bef-b39b-e625d00e4952
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '75'
ht-degree: 1%

---


# Ta bort ett dokument eller en mapp (ännu ej implementerad)

Tar bort ett dokument eller en mapp med det angivna ID:t i det externa systemet. Om du tar bort en mapp tas även mappinnehållet bort.

## URL

PUT /delete

## Frågeparametrar

| Namn  | Beskrivning |
|---|---|
| documentId  | Dokument-ID som ska tas bort |
| folderId  |  Mappens ID som ska tas bort |



## Svar

En JSON-sträng som anger om åtgärden lyckades eller misslyckades, vilket anges i felhanteringsavsnittet nedan.

### Exempel

```
PUT https://www.example.com/api/deleteid=1234

* returns `status: "success"`

* returns `status: "failure", error: "File not found"`
```

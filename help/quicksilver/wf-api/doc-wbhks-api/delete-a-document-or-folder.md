---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Ta bort ett dokument eller en mapp
description: Ta bort ett dokument eller en mapp
author: John
feature: Workfront API
exl-id: b56ec13a-1ee1-4bef-b39b-e625d00e4952
source-git-commit: 9de8ee7fad2a3cb67c4fc6bfdff4d6ce50f15afd
workflow-type: tm+mt
source-wordcount: '82'
ht-degree: 0%

---


# Ta bort ett dokument eller en mapp (ännu ej implementerad)

Tar bort ett dokument eller en mapp med angivet ID i det externa systemet. Om du tar bort en mapp tas även mappinnehållet bort.

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

PUT https://www.example.com/api/deleteid=1234
* returnerar `status: “success”`

* returnerar `status: “failure”, error: “File not found”`

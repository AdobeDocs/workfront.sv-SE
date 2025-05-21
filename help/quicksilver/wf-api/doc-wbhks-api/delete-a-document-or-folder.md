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
source-git-commit: 48de4553478fc42d88d81ea953440337f6684e50
workflow-type: tm+mt
source-wordcount: '84'
ht-degree: 0%

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

PUT https://www.example.com/api/deleteid=1234
* returnerar `status: "success"`

* returnerar `status: "failure", error: "File not found"`

---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Hämta en miniatyrbild för ett dokument
description: Hämta en miniatyrbild för ett dokument
author: Becky
feature: Workfront API
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 0%

---


# Hämta en miniatyrbild för ett dokument

Returnerar byte för miniatyrbilder i Raw-format för ett dokument.

**URL**

GET/miniatyrbild

## Frågeparametrar

| Namn  | Beskrivning |
|---|---|
| id  | Dokument-ID. |
| size  |  Bredden på miniatyrbilden. |


## Svar

Byte för miniatyrbilden i Raw-format.

**Exempel:**: https://www.acme.com/api/thumbnail?id=123456

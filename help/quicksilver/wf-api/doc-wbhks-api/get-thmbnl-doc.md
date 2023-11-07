---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Hämta en miniatyrbild för ett dokument
description: Hämta en miniatyrbild för ett dokument
author: Becky
feature: Workfront API
role: Developer
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
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
| size  |  Miniatyrbildens bredd. |


## Svar

Byte till miniatyrbilden för Raw.

**Exempel:**: https://www.acme.com/api/thumbnail?id=123456

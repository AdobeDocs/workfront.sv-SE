---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Skapa en mapp med dokumentwebbhotell
description: Skapa en mapp med dokumentwebbhotell
author: Becky
feature: Workfront API
role: Developer
exl-id: 50905915-58c9-4b50-b8a1-133833884a88
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '66'
ht-degree: 1%

---


# Skapa en mapp med dokumentwebbhotell

Skapar en mapp i en angiven katalog.

## URL

POST /createFolder

## Frågeparametrar

| **Namn** | **Beskrivning** |
|---|---|
| parentId  | Mappens ID som mappen ska skapas i |
| name  | Namnet på den nya mappen |




**Svar**

Metadata för den nyligen skapade mappen, enligt definitionen i /metadata-slutpunkten.

## Exempel

```
POST https://www.acme.com/api/createFolder
­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------
parentId=1234
name=New Folder 
-------------------------------
```

returnerar

```
{title:"New Folder",br /> kind:"folder"
 id":"5678",
 viewLink:"",
 downloadLink:"",
 mimeType:"",
 dateModified:"2014­06­05T17:39:45.251Z"
 size: ""
 }
```

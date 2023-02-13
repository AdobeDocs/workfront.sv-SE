---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Skapa en mapp med dokumentwebbhotell
description: Skapa en mapp med dokumentwebbhotell
author: John
feature: Workfront API
exl-id: 50905915-58c9-4b50-b8a1-133833884a88
source-git-commit: 1b11a4c5f0fdf1987e9f02f7aa06ec6ec36426d3
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
 viewLink:"”,
 downloadLink:"",
 mimeType:"",
 dateModified:"2014­06­05T17:39:45.251Z"
 size: ""
 }
```

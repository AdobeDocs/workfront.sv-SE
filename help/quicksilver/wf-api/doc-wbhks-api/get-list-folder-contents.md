---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Visar metadata för filer eller mappar
description: Visar metadata för filer eller mappar
author: Becky
feature: Workfront API
role: Developer
exl-id: 9c9f9222-59ac-4643-8297-d4939bec7e64
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '96'
ht-degree: 0%

---


# Hämta objektlista med mappinnehåll

Visar metadata för filer och mappar för en viss mapp.

**URL**

GET/filer

## Frågeparametrar

| Namn  | Beskrivning |
|---|---|
| parentId  | Mappens ID. Använd värdet &#39;/&#39; för att hämta metadata för rotkatalogen. |
| max  | Det maximala antalet artiklar som ska returneras. Används för sidnumrering. |
| offset  |  Sidförskjutningen som används tillsammans med max. |


## Svar

JSON som innehåller en lista med filer och mappar. Metadata för varje objekt är samma som returneras av /metadata-slutpunkten.

**Exempel:** https://www.acme.com/api/files?parentId=123456

```
[ 
{
title:"Folder A",
kind:"folder"
id":"2lj23lkj",
viewLink:" https://www.acme.com/viewDocument?id=2lj23lkj ",
downloadLink:"https://www.acme.com/downloadDocument?id=2lj23lkj",
mimeType:"",
dateModified:"2014­06­05T17:39:45.251Z"
size: ""
},
{
title:"My Document",
kind:"file"
id":"da8cj234",
viewLink:" https://www.acme.com/viewDocument?id=da8cj234 ",
downloadLink:"https://www.acme.com/downloadDocument?id=da8cj234",
mimeType:"image/png",
dateModified:"2014­06­05T17:39:45.251Z"
size: "32554694"
}
]
```

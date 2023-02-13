---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Sök via dokumentwebbhotell
description: Sök via dokumentwebbhotell
author: John
feature: Workfront API, Digital Content and Documents
exl-id: 8a3bf0c4-4a20-4311-8c05-15f4ef3a1d42
source-git-commit: 338cc745a7660ffed8e4d44e19dcadfdc13bc345
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---

# Sök via dokumentwebbhotell

Returnerar metadata för de filer och mappar som returneras från en sökning. Detta kan implementeras som en fulltextsökning eller som en vanlig databasfråga. Adobe Workfront anropar slutpunkten /search när användaren utför en sökning från den externa filläsaren.

## URL

GET/sökning

## Frågeparametrar

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Namn </th> 
   <th>Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>fråga</td> 
   <td>Sökordet eller frasen.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(valfritt) Mappens ID som sökningen utfördes från. Obs! Detta är en platshållare för en framtida funktion i Workfront. För närvarande skickas inte den här parametern av arbetsfronten. </p> </td> 
  </tr> 
  <tr> 
   <td>max</td> 
   <td>Det maximala antalet artiklar som ska returneras. Används för sidnumrering.</td> 
  </tr> 
  <tr> 
   <td>offset</td> 
   <td> Sidförskjutningen som används tillsammans med"max".</td> 
  </tr> 
 </tbody> 
</table>

 

## Svar

JSON innehåller en lista med metadata för filer och mappar som matchar frågan. Vad som utgör en matchning bestäms av webbkrokleverantören. Helst ska det göras en textsökning. Det går också att göra en filnamnsbaserad sökning.

**Exempel:**

Exempel:  `https://www.acme.com/api/search?query=test-query`

```
[ 
{ File/Folder Metadata },
{ File/Folder Metadata } 
]
```

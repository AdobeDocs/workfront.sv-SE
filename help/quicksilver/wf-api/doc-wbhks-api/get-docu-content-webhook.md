---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Hämta dokumentinnehåll via webbhotell
description: Returnerar oformaterade byte för ett dokument
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '43'
ht-degree: 0%

---

# Hämta dokumentinnehåll via webbhotell

Returnerar oformaterade byte för ett dokument

## URL

GET/nedladdning

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
   <td> <p>id</p> </td> 
   <td> Dokument-ID.</td> 
  </tr> 
 </tbody> 
</table>

## Svar

Dokumentets raw-byte.

**Exempel**:  `https://www.acme.com/api/download?id=123456`

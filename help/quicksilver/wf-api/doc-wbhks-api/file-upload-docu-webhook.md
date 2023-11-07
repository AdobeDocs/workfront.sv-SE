---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Filöverföring via webbhotell för dokument
description: Filöverföring via webbhotell för dokument
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c5727ee-bf8f-4664-a9b1-c5da356d94f5
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---


# Filöverföring via webbhotell för dokument

Att överföra en fil till en dokumentlagringsleverantör är en tvåstegsprocess som kräver två separata API-slutpunkter. Adobe Workfront påbörjar överföringen genom att anropa /uploadInit. Den här slutpunkten returnerar ett dokument-ID som sedan skickas till /upload när dokumentbyte överförs. Beroende på det underliggande dokumentlagringssystemet kan det vara nödvändigt att skapa ett dokument med längden noll och sedan uppdatera innehållet i dokumentet senare.

Dokument-ID och dokumentversions-ID kan läggas till i version 1.1 av den här specifikationen för att hämta extra information från Workfront.

**Exempel:** Om dokumenthanteringssystemet vill ha extra information om dokumentet, kan webhochimplementeringskoden använda dokument-ID:t för att hämta informationen med Workfront RESTful API. Som en god vana kan den här informationen komma från anpassade datafält i dokumentet och innehålla uppgifter, problem eller projekt.

## POST

**URL**

POST /uploadInit

### Frågeparametrar

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
   <td>parentId </td> 
   <td>Det överordnade mapp-ID:t som webbkrokprovidern refererar till.</td> 
  </tr> 
  <tr> 
   <td>filnamn </td> 
   <td>Dokumentets namn</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>Workfront dokument-ID (lades till i version 1.1)</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>Version-ID för Workfront-dokument (lades till i version 1.1) </td> 
  </tr> 
 </tbody> 
</table>

## Svar

Metadata för filen, enligt definitionen i /metadata-slutpunkten. Detta inkluderar det dokument-ID som används av providern.

**Exempel:**

```
https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&documentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b
```

## PUT-metod

Överför byte i ett dokument till webbholleverantören.

**URL**

PUT /upload

## Frågeparametrar

| Namn  | Beskrivning |
|---|---|
| id  |  Dokument-ID, som precis skapades. |


**Begärandetext**

Dokumentets byte med Raw-innehåll.

**Svar**

```
{
result: "success"
}
```

eller

```
{
result: "fail"
}
```

**Exempel**

`https://www.acme.com/api/upload?id=1234 [document bytes included in update stream]`

svar

```
{
result:"success"
}
```

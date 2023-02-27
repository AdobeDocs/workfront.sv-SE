---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Utför en anpassad åtgärd
description: Utför en anpassad åtgärd
author: Becky
feature: Workfront API
exl-id: a18b6b97-ee1e-4ad2-a4e1-00a644a0f4f2
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---


# Utför en anpassad åtgärd (ännu inte implementerad)

Den här slutpunkten gör att en Adobe Workfront-användare (eller en automatiserad arbetsflödeshändelse) kan utföra en åtgärd i det externa systemet. Slutpunkten /customAction accepterar en name-parameter, som gör att webkrok-providern kan implementera flera anpassade åtgärder.

Webbholleverantören registrerar anpassade åtgärder med Workfront genom att inkludera åtgärderna i svaret /serviceInfo under customActions. Workfront läser in den här listan när du konfigurerar eller uppdaterar webkrokprovidern under Inställningar > Dokument > Anpassade integreringar.

Användarna kan aktivera den anpassade åtgärden genom att markera avsnittet under Dokumentåtgärder

**URL**

GET /customAction

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
   <td> <p>name</p> </td> 
   <td> <p>Identifieraren som anger vilken typ av åtgärd som ska utföras. Det här värdet motsvarar ett av de customAction-värden som anges av slutpunkten /serviceInfo.</p> </td> 
  </tr> 
  <tr> 
   <td>documentId </td> 
   <td>Det dokument-ID för arbetsytan som åtgärden utförs för.</td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td> Version-ID för arbetsfrontdokumentet som åtgärden utförs för.</td> 
  </tr> 
 </tbody> 
</table>

 

## Svar

En JSON-sträng som anger om åtgärden lyckades eller misslyckades, vilket anges i felhanteringsavsnittet nedan. Vid fel (d.v.s. status = &quot;error&quot;) visas det angivna felmeddelandet för användaren i Workfront.

**Exempel:**

```
https://sample.com/webhooks/customName?name=archive&documentId=5502082c003a4f30 ddec2fb2b739cb7c&documentVersionId=54b598a700e2342d6971597a5df1a8d3
```

svar

```
{
status: “success”
}
```

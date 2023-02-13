---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Hämta information om tjänsten
description: Hämta information om tjänsten
author: John
feature: Workfront API
exl-id: a3a423ff-29a6-466e-a568-f64e02dcb484
source-git-commit: 5cb65c3a0c3ffd374c4002867c9c48985378e03c
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---


# Hämta information om tjänsten (ännu inte implementerad)

>[!NOTE]
>
>Utgivningsdatumet för den här funktionen har ännu inte fastställts.

Returnerar information om tjänsten, t.ex. funktioner. Adobe Workfront använder den här informationen för att anpassa användargränssnittet i Workfront. Om webkromimplementeringen till exempel innehåller vissa anpassade åtgärder, ska JSON visa dessa åtgärder i JSON. Användarna kan sedan aktivera dessa åtgärder från Workfront.

**URL**

GET /serviceInfo

## Frågeparametrar

Ingen. Dessutom ska anrop till den här slutpunkten inte kräva autentisering.

## Svar

JSON som innehåller information om den här tjänsten

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Namn</th> 
   <th>Typ </th> 
   <th>Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>webkrokVersion </td> 
   <td>Sträng </td> 
   <td>Den webkrosversion som implementeras av den här tjänsten. Det här är versionsnumret som visas högst upp i den här specifikationen.</td> 
  </tr> 
  <tr> 
   <td>version </td> 
   <td>Sträng </td> 
   <td>Det interna versionsnumret för den här tjänsten. Detta nummer bestäms av webbkroktjänstleverantören och används endast i informationssyfte.<br><br></td> 
  </tr> 
  <tr> 
   <td>utgivare </td> 
   <td>Sträng </td> 
   <td>Namnet på det företag som tillhandahåller webbkrokimplementeringen.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>Sträng </td> 
   <td>En lista som innehåller API-slutpunkterna som implementeras av den här tjänsten. Detta kan användas för att säkerställa att användargränssnittet i Workfront återspeglar funktionerna som erbjuds av webkrokprovidern. Varje objekt i listan måste innehålla slutpunktens namn (till exempel "sök").</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>Sträng</td> 
   <td>  <p>En lista som innehåller de anpassade åtgärder som implementeras av den här webbocken. Varje listobjekt innehåller ett namn och ett visningsnamn. Visningsnamnet visas i listrutan Dokumentåtgärder i Workfront. Om du klickar på objektet i listrutan anropas åtgärden i webkroken genom att slutpunkten /customAction anropas.</p></td> 
  </tr> 
 </tbody> 
</table>

**Exempel:** `https://www.acme.com/api/serviceInfo`

returnerar

```
{
webhook version: “1.2”, version: “1.0”, publisher: “Acme, LLC”, availableEndpoints: [“files”, “metadata”, “search”, “download”
“thumbnail”, “uploadInit”, “upload” ], customActions [
{
name: “archive”, displayName: “Archive” 
}, 
{name: “doSomethingElse”, displayName: “Do Something” }, 
] 
}
```

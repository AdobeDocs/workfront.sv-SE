---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Hämta metadata för en fil eller mapp
description: Hämta metadata för en fil eller mapp
author: John
feature: Workfront API
exl-id: 7b594df5-c87f-45d4-b84a-cae17171e906
source-git-commit: 492361028e7cf0d886c1f84f437ce9c55bc6603e
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---


# Hämta metadata för en fil eller mapp

Returnerar metadata för den angivna filen eller mappen.

**URL**

GET /metadata?id=[dokument- eller mapp-ID]

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
   <td>id</td> 
   <td>Fil- eller mappens ID, som webbkrokprovidern refererar till. Detta skiljer sig från Adobe Workfront dokument-ID. Använd värdet "/" för att hämta metadata för rotkatalogen.
   <p>Obs! ID:t får innehålla högst 255 tecken.</p></td> 
  </tr> 
 </tbody> 
</table>

 

## Svar

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Namn </th> 
   <th>Typ </th> 
   <th>Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>title </td> 
   <td>Sträng </td> 
   <td>Namnet på dokumentet eller mappen</td> 
  </tr> 
  <tr> 
   <td>sort </td> 
   <td>Sträng </td> 
   <td>Anger om det här objektet är en fil eller mapp ("fil" eller"mapp")</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>Sträng </td> 
   <td>ID för filen eller mappen.</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>Sträng </td> 
   <td> <p>Den URL-sökväg som en användare använder för att visa dokumentet i ett webbläsarfönster. URL:en kan finnas hos antingen dokumentprovidern eller den interna externa lagringsprovidern.</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>Sträng </td> 
   <td> <p>Den URL-sökväg som en användare använder för att hämta dokumentet i ett webbläsarfönster. URL:en kan finnas hos antingen dokumentprovidern eller den interna externa lagringsprovidern.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>Sträng </td> 
   <td>Filens MIME-typ. (valfritt)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>Sträng </td> 
   <td>Senaste gången den här filen ändrades (RFC 339-tidsstämpel formateras)</td> 
  </tr> 
  <tr> 
   <td>size</td> 
   <td>Lång</td> 
   <td> Filens storlek i byte. (valfritt)</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>Boolean</td> 
   <td> Anger om den här filen eller mappen är skrivskyddad för den autentiserade användaren.(valfritt) </td> 
  </tr> 
 </tbody> 
</table>

**Exempel:** https://www.acme.com/api/metadata?id=12345
<pre>{<br>title:"Mitt dokument",<br>sort:"file"<br>id":"12345",<br>viewLink:"https://www.acme.com/viewDocument?id=12345",<br>downloadLink:"https://www.acme.com/downloadDocument?id=12345",<br>mimeType:"image/png",<br>dateModified:"20140605T17:39:45,251Z",<br>storlek: "32554694"<br>}</pre>

>[!NOTE]
>
>Felhanteringen bör vara konsekvent för alla API-anrop. Mer information finns i avsnittet Felhantering nedan.

---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Registrera en webbkrosintegrering
description: Registrera en webbkrosintegrering
author: Becky
feature: Workfront API
role: Developer
exl-id: 9a4f8dbe-967f-4a41-a42c-8e3acb604972
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---


# Registrera en webbkrosintegrering

Adobe Workfront-administratörer kan lägga till en anpassad webbkrokintegrering för sitt företag genom att gå till Inställningar > Dokument > Anpassade integreringar i Workfront. På sidan Anpassad integrering i installationsprogrammet kan administratörer visa en lista över befintliga webkrok-integreringar för dokument. Från den här sidan kan integreringar läggas till, redigeras, aktiveras och inaktiveras.

Om du vill lägga till en integrering klickar du på **Lägg till anpassad integrering**.

![Lägg till anpassad integrering](assets/webhooks-integration-2-350x220.png)

## Tillgängliga fält

När du lägger till en integrering anger administratören värden för följande fält.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Fältnamn</th> 
   <th>Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Namn</td> 
   <td>Namnet på den här integreringen.</td> 
  </tr> 
  <tr> 
   <td>Bas-API-URL</td> 
   <td> <p>Plats för återanrops-API:t. När du anropar det externa systemet lägger Workfront bara till slutpunktsnamnet till den här adressen. Om administratören t.ex. angav Bas-API-URL:en, https://www.mycompany.com/api/v1, använder Workfront följande URL för att hämta ett dokuments metadata: https://www.mycompany.com/api/v1/metadata?id=1234.</p> </td> 
  </tr> 
  <tr> 
   <td>Begär parametrar</td> 
   <td> <p>Valfria värden som ska läggas till i frågesträngen för varje API-anrop. Till exempel access_type=offline. </p> </td> 
  </tr> 
  <tr> 
   <td>Autentiseringstyp</td> 
   <td>OAuth2 eller ApiKey</td> 
  </tr> 
  <tr> 
   <td>Autentiserings-URL</td> 
   <td> <p>(Endast OAuth2) Den fullständiga URL som används för användarautentisering. Workfront kommer att navigera användare till den här adressen som en del av OAuth-etableringsprocessen. Obs! Workfront lägger till en state-parameter i frågesträngen. Providern måste skicka tillbaka detta till Workfront genom att lägga till det till Workfront omdirigerings-URI.</p> </td> 
  </tr> 
  <tr> 
   <td>URL för tokenslutpunkt</td> 
   <td> <p>(Endast OAuth2) Den fullständiga API-URL som används för att hämta OAuth2-token. Detta hanteras av webbkrokprovidern eller den externa dokumentprovidern</p> </td> 
  </tr> 
  <tr> 
   <td>Klient-ID</td> 
   <td>(Endast OAuth2) Klient-ID för OAuth2 för den här integreringen</td> 
  </tr> 
  <tr> 
   <td>Klienthemlighet</td> 
   <td> <p>(Endast OAuth2) OAuth2-klienthemlighet för den här integreringen</p> </td> 
  </tr> 
  <tr> 
   <td>Workfront Omdirigerings-URI</td> 
   <td>(Endast OAuth2) Detta är ett skrivskyddat fält som genereras av Workfront. Det här värdet används för att registrera integreringen med den externa dokumentprovidern. Obs! Som beskrivs ovan för autentiserings-URL måste providern lägga till parametern "state" och dess värde i frågesträngen när den utför omdirigeringen.</td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td> <p>(Endast ApiKey) Används för att göra auktoriserade API-anrop till webbkrokprovidern. Den API-nyckel som utfärdas av webbkrokprovidern.</p> </td> 
  </tr> 
 </tbody> 
</table>

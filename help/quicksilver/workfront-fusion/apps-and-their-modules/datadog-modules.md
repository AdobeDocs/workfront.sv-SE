---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: koppling
navigation-topic: apps-and-their-modules
title: Datadogmoduler
description: I en [!DNL Adobe Workfront Fusion] kan du automatisera arbetsflöden som använder Datadog, samt ansluta det till flera tredjepartsprogram och -tjänster.
author: Becky
feature: Workfront Fusion
exl-id: a0b4352d-a1ce-4459-a58e-71de860b8a90
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '721'
ht-degree: 0%

---

# [!DNL Datadog] moduler

I en [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder [!DNL Datadog], samt ansluta till flera tredjepartsprogram och -tjänster.

Om du behöver instruktioner om hur du skapar ett scenario kan du läsa [Skapa ett scenario i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Mer information om moduler finns i [Moduler i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] eller högre</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licens**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Förutsättningar

Används [!DNL Datadog] moduler, du måste ha en [!DNL Datadog] konto.

## Anslut [!DNL Datadog] till [!DNL Workfront Fusion] {#connect-datadog-to-workfront-fusion}

### Hämta API-nyckeln och programnyckeln {#retrieve-your-api-key-and-application-key}

Koppla samman [!DNL Datadog] konto till [!DNL Workfront Fusion] du behöver hämta en API-nyckel och en programnyckel från [!DNL Datadog] konto.

1. Logga in på [!DNL Datadog] konto.
1. Klicka på **[!UICONTROL Integrations]** och sedan klicka **[!UICONTROL APIs]**.
1. På huvudskärmen klickar du på **[!UICONTROL API Keys]**.
1. Hovra över det lila fältet för att visa API-nyckeln.
1. Kopiera API-nyckeln till en säker plats.
1. På huvudskärmen klickar du på **[!UICONTROL Application Keys]**.
1. Hovra över det lila fältet för att visa programnyckeln.
1. Kopiera programnyckeln till en säker plats.

### Skapa en anslutning till [!DNL Datadog] in [!DNL Workfront Fusion]

Du kan skapa en anslutning till [!DNL Datadog] direkt inifrån [!UICONTROL Datadog] -modul.

1. I alla [!UICONTROL Datadog] modul, klicka på **[!UICONTROL Add]** bredvid [!UICONTROL Connection] fält.
1. Fyll i modulens fält enligt följande:

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection Type]</td> 
      <td> <p> Välj [!UICONTROL [!DNL Datadog] Application] option to get full access to [!DNL Datadog] API.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection Name]</td> 
      <td> <p> Ange ett namn för anslutningen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Domain] </td> 
      <td> <p>Välj den domän du vill ansluta till (USA eller EU).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL API Key]</td> 
      <td> <p> Ange [!DNL Datadog] API-nyckel. </p> <p>Instruktioner om hur du hämtar API-nyckeln finns i <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">Hämta API-nyckeln och programnyckeln</a> i den här artikeln.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Application Key]</td> 
      <td> <p> Ange [!DNL Datadog] programnyckel. </p> <p>Instruktioner om hur du hämtar programnyckeln finns i <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">Hämta API-nyckeln och programnyckeln</a> i den här artikeln.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **[!UICONTROL Continue]** för att skapa anslutningen och gå tillbaka till modulen.

## [!DNL Datadog] moduler och deras fält

När du konfigurerar [!DNL Datadog] moduler, [!DNL Workfront Fusion] visar fälten som listas nedan. Tillsammans med dessa finns ytterligare [!DNL Datadog] fält kan visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Åtgärder

* [[!UICONTROL Post Timeseries Points]](#post-timeseries-points)
* [[!UICONTROL Make an API Call]](#make-an-api-call)

#### [!UICONTROL Post Timeseries Points]

Med modulen kan du bokföra data från tidsserier som kan graderas [!DNL Datadog]Det är kontrollpaneler.

Gränsen för komprimerade nyttolaster är 3,2 megabyte (3200000) och 62 megabyte (62914560) för dekomprimerade nyttolaster.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Datadog] konto till [!DNL Workfront Fusion], se <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Datadog] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Series]</td> 
   <td> <p>Lägg till tidsserie som du vill skicka till [!DNL Datadog].</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Metric]</strong> </p> <p>Ange namnet på tidsserierna.</p> </li> 
     <li> <p><strong>[!UICONTROL Type]</strong> </p> <p>Välj typ av mätvärde.</p> </li> 
     <li> <p><strong>[!UICONTROL Interval]</strong> </p> <p> Om måttets typ är hastighet eller antal definierar du motsvarande intervall.</p> </li> 
     <li> <p><strong>[!UICONTROL Points]</strong> </p> <p>Lägg till punkter som hör till ett mätvärde.</p> <p>Detta är en JSON-array med punkter. Varje punkt har följande format: <code>[[POSIX_timestamp, numeric_value], ...] </code></p> <p>Obs!  <p>Tidsstämpeln måste vara i sekunder.</p> <p>Tidsstämpeln måste vara aktuell. Aktuell definieras som inte mer än 10 minuter i framtiden eller mer än 1 timme tidigare.</p> <p> Det numeriska värdeformatet ska vara ett flyttal.</p> </p> <p>Det här fältet måste innehålla minst 1 objekt.</p> </li> 
     <li> <p><strong>[!UICONTROL Host]</strong> </p> <p>Ange namnet på värden som genererade måttet.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Make an API Call]

Med den här åtgärdsmodulen kan du utföra ett anpassat API-anrop.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Datadog] konto till [!DNL Workfront Fusion], se <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Datadog] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Ange en sökväg som är relativ till <code>https://api.datadoghq.com/api/</code>. Exempel:<code> /v1/org</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-förfrågningsmetoder i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Lägg till rubrikerna för begäran i form av ett standard-JSON-objekt.</p> <p>Exempel: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion lägger till auktoriseringsrubrikerna åt dig.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Lägg till frågan för API-anropet i form av ett standard-JSON-objekt.</p> <p>Exempel: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Lägg till brödinnehållet för API-anropet i form av ett standard-JSON-objekt.</p> <p>Obs!  <p>När du använder villkorssatser som <code>if</code> i JSON placerar citattecknen utanför villkorssatsen.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Exempel:** Följande API-anrop returnerar alla instrumentpaneler i [!DNL Datadog] konto:

URL: `/v1/dashboard`

Metod: `GET`

![](assets/datadog-api-example.png)

Resultatet finns i modulens utdata under Paket > Brödtext > kontrollpaneler.

I vårt exempel returnerades tre kontrollpaneler:

![](assets/datadog-api-response-example.png)

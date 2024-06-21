---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: apps-and-their-modules
title: Adobe Firefly-moduler
description: I en [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder [!DNL Adobe Firefly], samt ansluta till flera tredjepartsprogram och -tjänster.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 1e131c27-571d-4099-9243-69572bdb3f5a
source-git-commit: f1821568ea69d370dc5b2e4cbaaf6b0a72f9fe7f
workflow-type: tm+mt
source-wordcount: '1154'
ht-degree: 0%

---

# [!DNL Adobe Firefly] moduler

I en [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder [!DNL Adobe Firefly], samt ansluta till flera tredjepartsprogram och -tjänster.

Om du behöver instruktioner om hur du skapar ett scenario kan du läsa [Skapa ett scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

Mer information om moduler finns i [Moduler i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td> <p>Nytt: [!UICONTROL Standard]</p><p>eller</p><p>Aktuell: [!UICONTROL Work] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licens**</td> 
   <td>
   <p>Aktuell: Nej [!DNL Workfront Fusion] krav på licens.</p>
   <p>eller</p>
   <p>Äldre: Alla </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Nytt:</p> <ul><li>[!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Workfront] Plan: Din organisation måste köpa [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan: [!DNL Workfront Fusion] ingår.</li></ul>
   <p>eller</p>
   <p>Aktuell: Din organisation måste köpa [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Förutsättningar

Innan du kan använda [!DNL Adobe Firefly] måste du se till att följande krav uppfylls:

* Du måste ha en aktiv [!DNL Adobe Firefly] konto.

## Skapa en anslutning till [!DNL Adobe Firefly]

Skapa en anslutning för [!DNL Adobe Firefly] moduler:

1. Klicka **[!UICONTROL Add]** bredvid rutan Anslutning.

1. Fyll i följande fält:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[!UICONTROL Connection name]</td>
        <td>
          <p>Ange ett namn för anslutningen.</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Environment]</td>
        <td>Ange om du ansluter till en produktionsmiljö eller icke-produktionsmiljö.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Type]</td>
        <td>Ange om du ansluter till ett tjänstkonto eller ett personligt konto.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Ange [!UICONTROL Adobe] [!UICONTROL Client ID]. Detta finns i [!UICONTROL Credentials] informationsdelen av [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Ange [!DNL Adobe] [!UICONTROL Client Secret]. Detta finns i [!UICONTROL Credentials] informationsdelen av [!DNL Adobe Developer Console]</td>
        </tr>
      </tbody>
    </table>

1. Klicka **[!UICONTROL Continue]** för att spara anslutningen och återgå till modulen.

## [!DNL Adobe Firefly] moduler och deras fält

När du konfigurerar [!DNL Adobe Firefly] moduler, [!DNL Workfront Fusion] visar fälten som listas nedan. Tillsammans med dessa finns ytterligare [!DNL Adobe Firefly] fält kan visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Göra ett anpassat API-anrop

Den här åtgärdsmodulen gör ett anpassat anrop till Firefly API.

Specifika tillgängliga API:er finns på [ADOBE FIREFLY API](https://developer.adobe.com/firefly-services/docs/firefly-api/) i Adobe Developer-dokumentationen.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Firefly], se <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Firefly]</a> i den här artikeln.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Ange en sökväg i förhållande till <code>https://firefly-api-enterprise-stage.adobe.io/</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
   <td> <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-förfrågningsmetoder i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Lägg till rubrikerna för begäran i form av ett standard-JSON-objekt.</p>
        <p>Exempel: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] lägger till auktoriseringshuvuden automatiskt.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Lägg till brödinnehållet för API-anropet i form av ett standard-JSON-objekt.</p> <p>Obs!  <p>När du använder villkorssatser som <code>if</code> i JSON placerar citattecknen utanför villkorssatsen.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

### Expandera en bild

Den här åtgärdsmodulen expanderar en bild, eventuellt med innehåll från en fråga som du anger.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Campaign], se <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Firefly]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prompt]</td> 
   <td>Ange eller mappa en fråga för innehållet som du vill expandera bilden med. Om ingen fråga visas kommer bilden att expanderas med innehåll som matchar originalbilden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number of variations]</td> 
   <td>Ange ett tal mellan 1 och 4. Modulen genererar detta antal expanderade bildvariationer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expanded image format]</td> 
   <td>Välj det filformat som den expanderade bilden ska sparas som.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>  <p>Välj en källfil från en tidigare modul eller mappa källfilens bildfilnamn och bildfil (data).</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Size]</td> 
   <td>Välj den storlek som du vill att den expanderade bilden ska ha.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seed]</td> 
   <td>Ange eller mappa ett heltal. Du kan använda samma startvärde i en annan expanderingsmodul om du vill generera en liknande bild med olika format. </td> 
  </tr> 
 </tbody> 
</table>

## Fylla en bild

Den här åtgärdsmodulen fyller det maskerade området i en bild, eventuellt med innehåll från en uppmaning som du anger.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Campaign], se <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Firefly]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prompt]</td> 
   <td>Ange eller mappa en fråga för innehållet som du vill fylla bilden med. Om ingen uppmaning visas fylls bilden med innehåll som matchar originalbilden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number of variations]</td> 
   <td>Ange ett tal mellan 1 och 4. Modulen genererar det här antalet fyllda bildvariationer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filled image format]</td> 
   <td>Välj det filformat som den ifyllda bilden ska sparas som.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Image]</td> 
   <td>  <p> Klicka <b>Lägga till en bild</b>. Välj en källfil från en tidigare modul eller mappa källfilens bildfilnamn och bilddata.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mask]</td> 
   <td>  <p> Klicka <b>Lägga till en mask</b>. Välj en källfil från en tidigare modul eller mappa källfilens maskfilnamn och maskdata. Maskfilen representerar den anpassade mask som ska fyllas med genererat innehåll.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Size]</td> 
   <td>Välj den storlek som du vill att den fyllda bilden ska ha.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seed]</td> 
   <td>Ange eller mappa ett heltal. Du kan använda samma startvärde i en annan expanderingsmodul om du vill generera en liknande bild med olika format. </td> 
  </tr> 
 </tbody> 
</table>

## Generera en bild

Den här åtgärdsmodulen genererar en bild som baseras på en fråga som du anger. Du kan också ange en valfri referensbild så matchar den genererade bilden stilen för referensbilden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Campaign], se <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Firefly]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prompt]</td> 
   <td>Ange eller mappa en fråga för den bild du vill skapa. Mer detaljskärpa ger dig större kontroll över vad som visas i bilden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number of variations]</td> 
   <td>Ange ett tal mellan 1 och 4. Modulen genererar detta antal bildvariationer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Generated image format]</td> 
   <td>Välj det filformat som den expanderade bilden ska sparas som. Om du väljer standardformat kommer filformatet att vara JPEG om ingen referensbild finns. Om en referensbild anges kommer den genererade bildens filformat att vara detsamma som referensbilden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>  <p>Välj en källfil från en tidigare modul eller mappa källfilens namn på referensbildfilen och referensbildfilen (data). Den genererade bilden skapas så att den matchar referensbildens format.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Presets]</td> 
   <td>Om du vill använda ett förinställt format klickar du på Lägg till objekt och anger eller mappar det format som du vill använda.<p>En lista med förinställda stilar finns på <a href="https://developer.adobe.com/firefly-services/docs/firefly-api/guides/concepts/styles/" >Bildmodellformat</a> i dokumentationen för utvecklaren av Adobe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Negative prompt]</td> 
   <td>Ange eller mappa de ord som du vill undvika i det genererade innehållet. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content class]</td> 
   <td>Välj om du vill att den genererade bilden ska vara mer lik ett foto eller mer lik en skapad bild. <ul><li><b>Foto</b><p>Ange värden för Aperture, Slutarhastighet (i sekunder) och visningsfält (i millimeter).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seed]</td> 
   <td>Ange eller mappa ett heltal. Du kan använda samma startvärde i en annan expanderingsmodul om du vill generera en liknande bild med olika format. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Size]</td> 
   <td>Välj den storlek som du vill att den genererade bilden ska ha.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Strength]</td> 
   <td>Ange eller mappa ett heltal som representerar intensiteten som den genererade bilden ska matcha stilen för den förinställda stilen eller referensbilden med. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visual intensity]</td> 
   <td>Ange eller mappa ett heltal som representerar den övergripande intensiteten för fotots befintliga visuella egenskaper. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Locale]</td> 
   <td>Om en språkinställning anges genererar modulen innehåll som är mer relevant för den angivna språkinställningen. <p>Språk måste anges i ISO 639-1-språkkoden och ISO 3166-1-regionen.</p><p> Exempel: <code>en-US</code></p></td> 
  </tr> 
 </tbody> 
</table>

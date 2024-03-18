---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: apps-and-their-modules
title: Adobe Photoshop moduler
description: Med Adobe Photoshop-modulerna kan du starta ett Adobe Workfront Fusion-scenario baserat på händelser i ditt Adobe Photoshop-konto, skapa, läsa eller uppdatera avtal och andra poster, söka efter poster med villkor som du anger och överföra dokument.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
source-git-commit: 8d6f8217a58459539c9e4f4faa43e01d17d6ecee
workflow-type: tm+mt
source-wordcount: '1319'
ht-degree: 0%

---

# [!DNL Adobe Photoshop] moduler

I en [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder [!DNL Adobe Photoshop], samt ansluta till flera tredjepartsprogram och -tjänster.


Om du behöver instruktioner om hur du skapar ett scenario kan du läsa [Skapa ett scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

Mer information om moduler finns i [Moduler i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
      <td>
        <p>[!UICONTROL Pro] eller högre</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] licens*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] licens**</td>
      <td >
        <p>[!UICONTROL Workfront Fusion for Work Automation and Integration]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Produkt</td>
      <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td>
    </tr>
    </tr>
  </tbody>
</table>


&#42;Kontakta din [!DNL Workfront] administratör.

&#42;&#42;För information om [!DNL Adobe Workfront Fusion] licenser, se [!DNL [Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Förutsättningar

Innan du kan använda [!DNL Adobe Photoshop] måste du se till att följande krav uppfylls:

* Du måste ha en aktiv [!DNL Adobe Photoshop] konto.

## Skapa en anslutning till [!DNL Adobe Photoshop]

Skapa en anslutning för [!DNL Adobe Photoshop] moduler:

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
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Ange [!UICONTROL Adobe] [!UICONTROL Client ID]. Detta finns i [!UICONTROL Credentials] informationsdelen av [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Ange [!DNL Adobe] [!UICONTROL Client Secret]. Detta finns i [!UICONTROL Credentials] informationsdelen av [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Technical account ID]</td>
        <td>Ange [!DNL Adobe] [!UICONTROL Technical account ID]. Detta finns i [!UICONTROL Credentials] informationsdelen av [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Organization ID]</td>
        <td>Ange [!DNL Adobe] [!UICONTROL Organization ID]. Detta finns i [!UICONTROL Credentials] informationsdelen av [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Private key]</td>
        <td>
          <p>Ange den privata nyckel som skapades när dina autentiseringsuppgifter skapades i [!DNL Adobe Developer Console]. </p>
          <p>Så här extraherar du din privata nyckel eller ditt certifikat:</p>
          <ol>
            <li value="1">
              <p>Klicka på <b>[!UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>Välj vilken typ av fil du extraherar.</p>
            </li>
            <li value="3">
              <p>Markera filen som innehåller den privata nyckeln eller certifikatet.</p>
            </li>
            <li value="4">
              <p>Ange lösenordet för filen.</p>
            </li>
            <li value="5">
              <p>Klicka <b>Spara</b> extrahera filen och gå tillbaka till[!UICONTROL ]e-anslutningsinställningar.</p>
            </li>
          </ol>
        </td>
        </tr>
      </tbody>
    </table>

1. Klicka **[!UICONTROL Continue]** för att spara anslutningen och återgå till modulen.

## [!DNL Adobe Photoshop] moduler och deras fält

När du konfigurerar [!DNL Adobe Photoshop] moduler, [!DNL Workfront Fusion] visar fälten som listas nedan. Tillsammans med dessa finns ytterligare [!DNL Adobe Photoshop] fält kan visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


### Åtgärder

* [Skapa en ny PSD](#create-a-new-psd)
* [Redigera textlager](#edit-text-layers)
* [Kör djuposkärpa](#execute-depth-blur)
* [Utför Photoshop-åtgärder](#execute-photoshop-actions)
* [Kör produktbeskärning](#execute-product-crop)
* [Hämta lagerinformation](#get-layer-info)
* [Göra ett anpassat API-anrop](#make-a-custom-api-call)

#### Skapa en ny PSD

Den här åtgärdsmodulen skapar ett nytt PSD med valfria lager och genererar återgivningar eller sparar som PSD.

Om du vill se fält som hör till den här modulen går du till [Skapa en ny PSD](https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/documentCreate) i Adobe Photoshop-dokumentationen.

#### Redigera textlager

Den här åtgärdsmodulen redigerar textlager i en Photoshop-fil.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Photoshop], se <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Photoshop]</a> i den här artikeln.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Input file storage]</td>
      <td>
        <p>Välj den filtjänst där filen som du vill redigera lagras.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Ange eller mappa URL:en eller sökvägen till filen som du vill redigera. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Manage missing fonts]</td>
      <td>
        <p>Välj den åtgärd som ska utföras om det finns ett eller flera saknade teckensnitt i dokumentet. Om teckensnittet inte anges används standardteckensnittet.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Default font]  </td>
      <td>
        <p>Ange det fullständiga postscript-namnet för det teckensnitt som ska användas som dokumentets globala standard. Det här teckensnittet används för alla textlager som saknar teckensnitt och inget annat teckensnitt har angetts specifikt för det lagret. Om det här teckensnittet saknas börjar det alternativ som anges i Hantera saknade teckensnitt gälla.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Layers]</td>
   <td> <p>Mer information om lageralternativ finns i <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/text">Redigera textlager</a> i Adobe Photoshop-dokumentationen.</p>  </td>     </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Output file storage]</td>
      <td>
        <p>Välj den filtjänst där du vill att den redigerade filen ska lagras.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file URL]</p>
      </td>
   <td> Ange eller mappa URL:en eller sökvägen där den redigerade filen ska lagras. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file type]</p>
      </td>
   <td> Välj filtyp för den redigerade filen. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Välj om den nyligen redigerade filen ska skriva över alla utdatafiler som redan finns.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> Välj komprimeringsnivå för utdatafilen. </td> 
    </tr>
  </tbody>
</table>

#### Kör djuposkärpa

Den här åtgärdsmodulen kör djuposkärpa på den markerade filen.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Photoshop], se <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Photoshop]</a> i den här artikeln.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Input file storage]</td>
      <td>
        <p>Välj den filtjänst där filen som du vill redigera lagras.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Ange eller mappa URL:en eller sökvägen till filen som du vill redigera. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Output file storage]</td>
      <td>
        <p>Välj den filtjänst där du vill att den redigerade filen ska lagras.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file URL]</p>
      </td>
   <td> Ange eller mappa URL:en eller sökvägen där den redigerade filen ska lagras. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file type]</p>
      </td>
   <td> Välj filtyp för den redigerade filen. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Other fields]</td>
      <td>
        <p>Mer information om andra alternativ för djuposkärpa finns i <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/depthBlur">Kör djuposkärpa </a>i Adobe Photoshop API-dokumentationen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Välj om den nyligen redigerade filen ska skriva över alla utdatafiler som redan finns.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> Välj komprimeringsnivå för utdatafilen. </td> 
    </tr>
  </tbody>
</table>

#### Utför Photoshop-åtgärder

Den här åtgärdsmodulen kör en Photoshop-åtgärd på den markerade bilden.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Photoshop], se <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Photoshop]</a> i den här artikeln.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Input file storage]</td>
      <td>
        <p>Välj den filtjänst där filen som du vill redigera lagras.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Ange eller mappa URL:en eller sökvägen till filen som du vill redigera. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Actions file storage]</td>
      <td>
        <p>Välj filtjänsten där åtgärdsfilen lagras.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Actions file URL]</p>
      </td>
   <td> Ange eller mappa URL:en eller sökvägen för åtgärdsfilen. </td> 
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Action name]</p>
      </td>
   <td> Om du bara vill köra en viss åtgärd kan du ange vilken åtgärd som ska spelas upp från ActionSet. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Font / Pattern / Brush storage]</td>
      <td>
        <p>Välj den filtjänst där filen som du vill använda lagras.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Font / Pattern / Brush file URL]</p>
      </td>
   <td> Ange eller mappa URL:en eller sökvägen till filen som du vill använda. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Output file storage]</td>
      <td>
        <p>Välj den filtjänst där du vill att den redigerade filen ska lagras.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file URL]</p>
      </td>
   <td> Ange eller mappa URL:en eller sökvägen där den redigerade filen ska lagras. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file type]</p>
      </td>
   <td> Välj filtyp för den redigerade filen. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Välj om den nyligen redigerade filen ska skriva över alla utdatafiler som redan finns.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> Välj komprimeringsnivå för utdatafilen. </td> 
    </tr>
  </tbody>
</table>

#### Kör produktbeskärning

Den här åtgärdsmodulen kör produktbeskärning på den valda bilden.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Photoshop], se <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Photoshop]</a> i den här artikeln.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Input file storage]</td>
      <td>
        <p>Välj den filtjänst där filen som du vill beskära lagras.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Ange eller mappa URL-adressen eller sökvägen till filen som du vill beskära. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Unit]</p>
      </td>
   <td> Välj om du vill beskriva justeringen av höjd och bredd i pixlar eller i procent. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Width]</p>
      </td>
   <td> Ange eller mappa den mängd breddutfyllnad som du vill lägga till. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Height]</p>
      </td>
   <td> Ange eller mappa den höjd som du vill lägga till. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Output file storage]</td>
      <td>
        <p>Välj den filtjänst där du vill att den redigerade filen ska lagras.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file URL]</p>
      </td>
   <td> Ange eller mappa URL:en eller sökvägen där den redigerade filen ska lagras. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file type]</p>
      </td>
   <td> Välj filtyp för den redigerade filen. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Välj om den nyligen redigerade filen ska skriva över alla utdatafiler som redan finns.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> Välj komprimeringsnivå för utdatafilen. </td> 
    </tr>
  </tbody>
</table>

#### Hämta lagerinformation

Den här åtgärdsmodulen hämtar lagerinformation från den angivna PSD-filen.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Photoshop], se <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Photoshop]</a> i den här artikeln.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Input file storage]</td>
      <td>
        <p>Välj den filtjänst där filen som du vill hämta lagerinformation från lagras.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Ange eller mappa URL:en eller sökvägen till filen som du vill hämta lagerinformation från. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Thumbnails]</p>
      </td>
   <td> </td> 
    </tr>
  </tbody>
</table>

#### Göra ett anpassat API-anrop

Den här åtgärdsmodulen gör ett anpassat anrop till Photoshop API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Photoshop], se <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Photoshop]</a> i den här artikeln.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Ange en sökväg i förhållande till <code>https://image.adobe.io/pie/psdService</code>. Exempel: <code>/photoshopActions</code></p>
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
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>Ange frågesträngen för begäran.</p>
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


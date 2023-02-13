---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: koppling
navigation-topic: apps-and-their-modules
title: Gränssnittsmoduler
description: I en [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder [!DNL Bynder], samt ansluta till flera tredjepartsprogram och -tjänster.
author: Becky
feature: Workfront Fusion
exl-id: e4dc9588-334a-41a3-85d1-996cb819c3fa
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1367'
ht-degree: 0%

---

# [!DNL Bynder] moduler

I en [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder [!DNL Bynder], samt ansluta till flera tredjepartsprogram och -tjänster.

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

Används [!DNL Bynder] moduler, du måste ha en [!DNL Bynder] konto.

## Anslut [!DNL Bynder] till Workfront Fusion  {#connect-bynder-to-workfront-fusion}

* [Skapa en anslutning till [!DNL Bynder] från [!DNL Workfront Fusion]](#create-a-connection-to-bynder-from-workfront-fusion)
* [Generera en [!UICONTROL Client ID] och [!UICONTROL Client Secret] in [!DNL Bynder] (Valfritt)](#generate-a-client-id-and-client-secret-in-bynder-optional)

### Skapa en anslutning till [!DNL Bynder] från [!DNL Workfront Fusion]

Du kan skapa en anslutning från [!DNL Workfront Fusion] till [!DNL Bynder] direkt inifrån [!DNL Bynder] -modul.

1. I alla [!DNL Bynder] modul, klicka på **[!UICONTROL Add]** bredvid [!UICONTROL Connection] fält.
1. Välj [!DNL Bynder] domän som du vill ansluta till.
1. (Valfritt) Klicka på **[!UICONTROL Advanced settings]** anger du [!UICONTROL Client ID] och [!UICONTROL Client Secret].

   Instruktioner om hur du genererar klient-ID och klienthemlighet finns i [Generera ett klient-ID och klienthemlighet i [!DNL Bynder] (Valfritt)](#generate-a-client-id-and-client-secret-in-bynder-optional) i den här artikeln.

1. I [!UICONTROL login] anger du ditt användarnamn (e-postadress) och lösenord.
1. Klicka **[!UICONTROL Continue]** för att skapa anslutningen och gå tillbaka till modulen.

### Generera en [!UICONTROL Client ID] och [!UICONTROL Client Secret] in [!DNL Bynder] (Valfritt)

Om du vill skapa en anslutning med klient-ID och klienthemlighet kan du generera dem från din [!DNL Bynder] konto. Klient-ID och klienthemlighet genereras när du skapar ett program i [!DNL Bynder].

Instruktioner för hur du skapar ett program i [!DNL Bynder], se [Oauth 2.0-appar](https://developer-docs.bynder.com/api/authentication-oauth2-oauth-apps/) i [!DNL Bynder] dokumentation.

>[!NOTE]
>
>När du skapar programmet i [!DNL Bynder]anger du följande som `redirect uri`:
>
>`https://app.workfrontfusion.com/oauth/cb/workfront-bynder`

## [!DNL Bynder] moduler och deras fält

När du konfigurerar [!DNL Bynder] moduler, [!DNL Workfront Fusion] visar fälten som listas nedan. Tillsammans med dessa finns ytterligare [!DNL Bynder] fält kan visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Åtgärder](#actions)
* [Sökningar](#searches)
* [Utlösare](#triggers)

### Åtgärder

* [[!UICONTROL Custom API Call]](#custom-api-call)
* [[!UICONTROL Read asset metadata]](#read-asset-metadata)
* [[!UICONTROL Update asset metadata]](#update-asset-metadata)
* [[!UICONTROL Add assets to a collection]](#add-assets-to-a-collection)
* [[!UICONTROL Remove assets from collection]](#remove-assets-from-collection)
* [[!UICONTROL Add a tag to assets]](#add-a-tag-to-assets)
* [[!UICONTROL Remove a tag] från resurser](#remove-a-tag-from-assets)
* [[!UICONTROL Download asset]](#download-asset)
* [[!UICONTROL Upload asset]](#upload-asset)

#### [!UICONTROL Custom API Call]

Med den här åtgärdsmodulen kan du göra ett anpassat autentiserat anrop till [!DNL Bynder] API. På så sätt kan du skapa en dataflödesautomatisering som inte kan uppnås av andra [!DNL Bynder] moduler.

När du konfigurerar den här modulen visas följande fält.

Modulen returnerar en statuskod tillsammans med rubrikerna och brödtexten för API-anropet.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Bynder] konto till [!DNL Workfront Fusion], se <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Bynder] till [!DNL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Ange en sökväg som är relativ till <code>https://{your-bynder-domain}/api/{api-version}/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-förfrågningsmetoder i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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

#### [!UICONTROL Read asset metadata]

Den här åtgärdsmodulen läser metadata för en resurs.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Bynder] konto till [!DNL Workfront Fusion], se <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Bynder] till [!DNL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td>Ange eller mappa ID:t för resursen som du vill hämta metadata för.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Välj den information som du vill inkludera i utdatapaketet för den här modulen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update asset metadata]

Den här åtgärdsmodulen uppdaterar metadata för en befintlig resurs.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Bynder] konto till [!DNL Workfront Fusion], se <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Bynder] till [!DNL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td>Ange eller mappa ID:t för resursen som du vill uppdatera metadata för.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td> <p>Markera de fält som du vill ange information för och ange eller mappa sedan den information som du vill uppdatera metadata med till dessa fält. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Metaproperties]</p> </td> 
   <td>Välj de alternativ som du vill uppdatera och ange eller mappa sedan informationen till dessa egenskaper. Metaegenskaper är information om resursen som inte representerar specifika fält i resursen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Add assets to a collection]

Den här åtgärdsmodulen lägger till en eller flera resurser i en samling.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Bynder] konto till [!DNL Workfront Fusion], se <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Bynder] till [!DNL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collection ID]</td> 
   <td> <p>Ange eller mappa ID:t för samlingen där du vill lägga till resurser.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset IDs]</td> 
   <td> <p>För varje resurs som du vill lägga till i samlingen klickar du på <strong>[!UICONTROL Add item]</strong>anger eller mappar sedan resurs-ID:t.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remove assets from collection]

Den här åtgärdsmodulen tar bort en eller flera resurser från en samling.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Bynder] konto till [!DNL Workfront Fusion], se <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Bynder] till [!DNL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collection ID]</td> 
   <td> <p>Ange eller mappa ID:t för samlingen där du vill ta bort resurser.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset IDs]</td> 
   <td> <p>För varje resurs som du vill ta bort från samlingen klickar du på <strong>[!UICONTROL Add item]</strong>anger eller mappar sedan resurs-ID:t.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Add a tag to assets]

Lägga till en tagg i en eller flera resurser

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Bynder] konto till [!DNL Workfront Fusion], se <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Bynder] till [!DNL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tag ID]</td> 
   <td> <p>Ange eller mappa ID:t för taggen som du vill lägga till i resurser.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset IDs]</td> 
   <td> <p>För varje resurs som du vill tagga klickar du på <strong>[!UICONTROL Add item]</strong>anger eller mappar sedan resurs-ID:t.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remove a tag from assets]

Ta bort en tagg från en eller flera resurser

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Bynder] konto till [!DNL Workfront Fusion], se <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Bynder] till [!DNL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tag ID]</td> 
   <td> <p>Ange eller mappa ID:t för taggen som du vill ta bort från resurserna.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset IDs]</td> 
   <td> <p>För varje resurs som du vill ta bort en tagg från klickar du på <strong>[!UICONTROL Add item]</strong>anger eller mappar sedan resurs-ID:t.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Download asset]

Den här åtgärdsmodulen hämtar en enskild resurs.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Bynder] konto till [!DNL Workfront Fusion], se <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Bynder] till [!DNL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td>Ange eller mappa ID:t för resursen som du vill hämta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset version]</td> 
   <td> <p>Ange eller mappa den version av resursen som du vill hämta. Om du vill hämta den senaste versionen av resursen lämnar du fältet tomt.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Upload asset]

Den här åtgärdsmodulen överför en enskild resurs.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Bynder] konto till [!DNL Workfront Fusion], se <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Bynder] till [!DNL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Save as]</td> 
   <td> <p>Välj hur du vill spara filen som du överför.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL New asset]</strong> </p> <p>Markera de fält och metaegenskaper som du vill ange information för och ange sedan informationen i fälten.</p> <p>Ange eller mappa ID:t för det varumärke som du vill använda för den överförda resursen.</p> </li> 
     <li> <p><strong>[!UICONTROL New asset version]</strong> </p> <p>Ange ID:t för resursen som du överför en ny version för.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</td> 
  </tr> 
 </tbody> 
</table>

### Sökningar

* [[!UICONTROL List record]](#list-record)
* [[!UICONTROL Search for assets]](#search-for-assets)

#### [!UICONTROL List record]

Den här sökmodulen hämtar alla objekt av en viss typ.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Bynder] konto till [!DNL Workfront Fusion], se <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Bynder] till [!DNL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Välj den typ av post som du vill visa.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Read all collections]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Read information about all tags]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Read all assets of a collection]</strong> </p> <p>Ange eller mappa ID:t för samlingen som du vill visa resurser för.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Markera de fält som du vill inkludera i modulens utdata.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ange eller mappa det maximala antalet resurser som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Search for assets]

Den här sökmodulen söker efter resurser baserat på de villkor du anger.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Bynder] konto till [!DNL Workfront Fusion], se <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Bynder] till [!DNL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Criteria]</td> 
   <td> <p>Ange sökvillkoren. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Field]</strong> </p> <p>Markera fältet som du vill använda i sökningen</p> </li> 
     <li> <p><strong>[!UICONTROL Logical Operator]</strong> </p> <p>Välj den operator som du vill använda i sökningen.</p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>Ange eller mappa värdet som du vill söka efter i det markerade fältet. Värdetypen ska vara densamma som datatypen för det markerade fältet. </p> <p>Mer information om datatyper finns i <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Artikeldatatyper i [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Result set]</td> 
   <td>Välj om du vill returnera den första matchande resursen eller alla matchande resurser.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort by]</td> 
   <td> <p>Markera fältet som du vill sortera efter.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort Direction]</td> 
   <td> <p>Välj om du vill sortera stigande eller fallande.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Markera de fält som du vill inkludera i modulens utdata.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ange eller mappa det maximala antalet resurser som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Utlösare

#### [!UICONTROL Watch assets]

Den här utlösarmodulen startar ett scenario när en resurs skapas eller uppdateras.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Bynder] konto till [!DNL Workfront Fusion], se <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Bynder] till [!DNL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Event type</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select whether you want to start the scenario when a new asset is created or when an existing asset is updated.</td>
   --> 
  </tr> 
  <tr>
     <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Collections]</td>
   <td> <p>Välj den samling som du vill bevaka för nya resurser. Om du vill bevaka alla samlingar lämnar du det här fältet tomt.</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Outputs</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the fields that you want to include in the output.</td>
   --> 
  </tr> 
  <tr> 
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Limit]</td>

<td> <p>Ange det högsta antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

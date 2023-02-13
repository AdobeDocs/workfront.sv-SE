---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: apps-and-their-modules
title: Allocadia-moduler
description: I en [!DNL Adobe Workfront Fusion] kan du automatisera arbetsflöden som använder Allocadia och ansluta det till flera tredjepartsprogram och -tjänster.
author: Becky
feature: Workfront Fusion
exl-id: f1edefd1-9fe0-48fc-bea2-c3f9facf7363
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1245'
ht-degree: 0%

---

# [!DNL Allocadia] moduler

I en [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder [!DNL Allocadia], samt ansluta till flera tredjepartsprogram och -tjänster.

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

Används [!DNL Allocadia] moduler, du måste ha en [!DNL Allocadia] konto.

## Anslut [!DNL Allocadia] till [!DNL Workfront Fusion]

Du kan skapa en anslutning till [!DNL Allocadia] direkt inifrån ett [!DNL Allocadia] -modul.

1. I alla [!DNL Allocadia] modul, klicka på **[!UICONTROL Add]** bredvid [!UICONTROL Connection] fält.
1. Välj om du vill använda den nordamerikanska servern eller den europeiska servern.
1. Ange ditt användarnamn och lösenord.
1. Klicka **[!UICONTROL Continue]** för att skapa anslutningen och gå tillbaka till modulen.

## [!DNL Allocadia] moduler och deras fält

När du konfigurerar [!DNL Allocadia] moduler, [!DNL Workfront Fusion] visar fälten som listas nedan. Tillsammans med dessa finns ytterligare [!DNL Allocadia] fält kan visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Utlösare](#triggers)
* [Åtgärder](#actions)
* [Sökningar](#searches)

### Utlösare

#### [!UICONTROL Watch Record]

Den här utlösarmodulen kör ett scenario när objekt av en viss typ läggs till, uppdateras eller både och. Modulen returnerar alla standardfält som är associerade med posten eller posterna, tillsammans med anpassade fält och värden som anslutningen har åtkomst till. Du kan mappa den här informationen i efterföljande moduler i scenariot.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto"> <table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter ditt Allocadia-konto till [!DNL Workfront Fusion], se <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Allocadia] till Workfront Fusion</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filter</td> 
   <td> <p>Välj om du vill att scenariot bara ska visa nya poster [!UICONTROL Updated Records Only]eller Nya och uppdaterade poster.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Enhetstyp</td> 
   <td>Välj posttypen Allocadia som du vill att modulen ska bevaka.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Utdata</td> 
   <td> <p>Markera de fält som du vill inkludera i modulens utdata. Vilka fält som är tillgängliga beror på vilken enhetstyp du har valt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Gräns</td> 
   <td> <p>Ange eller mappa det maximala antalet poster som modulen ska bevaka under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Åtgärder

* [Anpassat API-anrop](#custom-api-call)
* [Läs post](#read-record)
* [Skapa post](#create-record)
* [Ta bort post](#delete-record)
* [Uppdatera post](#update-record)

#### [!UICONTROL Custom API Call]

Med den här åtgärdsmodulen kan du göra ett anpassat autentiserat anrop till [!DNL Allocadia] API. På så sätt kan du skapa en dataflödesautomatisering som inte kan uppnås av andra [!DNL Allocadia] moduler.

Åtgärden baseras på den entitetstyp (Allocadia-objekttyp) som du anger.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Allocadia] konto till [!DNL Workfront Fusion], se <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Allocadia] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Ange en sökväg som är relativ till <code>https://api-na.allocadia.com/{version}</code> eller <code>https://api-eu.allocadia.com/{version}</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-förfrågningsmetoder i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Lägg till rubrikerna för begäran i form av ett standard-JSON-objekt.</p> <p>Exempel: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] lägger till auktoriseringsrubrikerna åt dig.</p> </td> 
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

#### [!UICONTROL Read Record]

Den här åtgärdsmodulen läser data från en enda post i [!DNL Allocadia].

Du anger postens ID.

Modulen returnerar alla standardfält som är associerade med posten, tillsammans med eventuella anpassade fält och värden som anslutningen har åtkomst till. Du kan mappa den här informationen i efterföljande moduler i scenariot.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Allocadia] konto till [!DNL Workfront Fusion], se <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Allocadia] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Välj typ av [!DNL Allocadia] som du vill att modulen ska läsa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Markera de fält som du vill inkludera i modulens utdata. Vilka fält som är tillgängliga beror på [!UICONTROL Entity Type] du markerade.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Ange eller mappa det unika [!DNL Allocadia] ID för den post som du vill att modulen ska läsa.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create Record]

Den här åtgärdsmodulen skapar en post.

Modulen returnerar postens ID och eventuella associerade fält, tillsammans med eventuella anpassade fält och värden som anslutningen har åtkomst till. Du kan mappa den här informationen i efterföljande moduler i scenariot.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Allocadia] konto till [!DNL Workfront Fusion], se <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Allocadia] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Välj om du vill skapa en ny post baserat på radartikel eller kolumnval.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Budgets]</td> 
   <td> <p>Välj den budget där du vill skapa en post.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Column choices]</td> 
   <td>Markera den kolumn som du vill använda för att skapa en ny post.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Label]</td> 
   <td>Ange eller mappa en etikett för den nya posten</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete Record]

Den här åtgärdsmodulen tar bort en viss post.

Du anger postens ID.

Modulen returnerar postens ID och eventuella associerade fält, tillsammans med eventuella anpassade fält och värden som anslutningen har åtkomst till. Du kan mappa den här informationen i efterföljande moduler i scenariot.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Allocadia] konto till [!DNL Workfront Fusion], se <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Allocadia] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td> <p>Välj den typ av enhet som du vill ta bort.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Line item]</strong> </p> <p>Ange radartikel-ID</p> </li> 
     <li> <p><strong>[!UICONTROL Column Choice]</strong> </p> <p>Välj den budget som du vill ta bort en post från och ange sedan kolumn-ID och alternativ-ID.</p> </li> 
     <li> <p><strong>[!UICONTROL Forecast Tags]</strong> </p> <p>Välj den budget som du vill ta bort en post från och ange sedan tagg-ID:t.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update Record]

Den här åtgärdsmodulen uppdaterar en post, t.ex. ett radobjekt, en användare eller ett kolumnval.

Du anger postens ID.

Modulen returnerar postens ID och eventuella associerade fält, tillsammans med eventuella anpassade fält och värden som anslutningen har åtkomst till. Du kan mappa den här informationen i efterföljande moduler i scenariot.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!UICONTROL Allocadia] konto till [!DNL Workfront Fusion], se <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Allocadia] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Välj typ av [!DNL Allocadia] som du vill att modulen ska uppdatera. Andra fält visas baserat på den enhetstyp du väljer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Budgets]</td> 
   <td> <p>Välj den budget där du vill uppdatera en post. </p> </td> 
  </tr> 
 </tbody> 
</table>

### Sökningar

#### [!UICONTROL Search Record]

Den här sökmodulen söker efter poster i ett objekt i [!DNL Allocadia] som matchar den sökfråga du anger.

Du kan mappa den här informationen i efterföljande moduler i scenariot.

Du anger vilken typ av poster du vill använda.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Allocadia] konto till [!DNL Workfront Fusion], se <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Allocadia] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Välj typ av [!DNL Allocadia] poster som du vill att modulen ska söka efter. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Budgets]</td> 
   <td> <p>Välj den budget som du vill söka i. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Result set]</td> 
   <td>Välj om du vill att modulen ska returnera alla matchande poster eller endast den första matchande posten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximal count of records]</td> 
   <td> <p>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search criteria]</td> 
   <td>Markera fältet som du vill söka efter, markera åtgärden och ange eller mappa värdet som du vill söka efter. Du kan lägga till [!DNL AND] eller [!DNL OR] regler för att ytterligare filtrera sökningen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Markera de fält som du vill inkludera i modulens utdata. Vilka fält som är tillgängliga beror på vilken enhetstyp du har valt.</p> </td> 
  </tr> 
 </tbody> 
</table>

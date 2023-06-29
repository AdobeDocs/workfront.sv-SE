---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: apps-and-their-modules
title: Frame.io-moduler
description: The [!DNL Adobe Workfront Fusion Frame].io modules enable you to monitor, create, update, retrieve, or delete assets and comments in your [!DNL Frame.io] konto.
author: Becky
feature: Workfront Fusion
exl-id: 373a86f6-fbba-4914-b08d-a3a035ac0ae4
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1927'
ht-degree: 0%

---

# [!DNL Frame.io] moduler

The [!DNL Adobe Workfront Fusion] [!DNL Frame.io] kan du övervaka, skapa, uppdatera, hämta eller ta bort resurser och kommentarer i [!DNL Frame.io] konto.

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
   <td>
   <p>Aktuellt licenskrav: Nej [!DNL Workfront Fusion] krav på licens.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuellt produktbehov: Om du har [!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Adobe Workfront] Planera, din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln. [!DNL Workfront Fusion] ingår i [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>eller</p>
   <p>Krav för äldre produkt: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Förutsättningar

Används [!DNL Frame.io] moduler, du måste ha en [!DNL Frame.io] konto

## Anslut [!DNL Frame.io] till [!UICONTROL Adobe Workfront Fusion]

Du kan ansluta till [!DNL Frame.io] med en API-token, eller med OAuth 2.0.

[Anslut till [!DNL Frame.io] använda en API-token](#connect-to-frameio-using-an-api-token)

[Anslut till [!DNL Frame.io] med OAuth 2.0 PKCE](#connect-to-frameio-using-oauth-20-pkce)

### Anslut till [!DNL Frame.io] använda en API-token

Koppla samman [!DNL Frame.io] konto till [!DNL Workfront Fusion] med en API-token måste du skapa API-token i [!DNL Frame.io] konto och infoga det i [!DNL Workfront Fusion] [!DNL Frame.io] [!UICONTROL Create a connection] -dialogrutan.

1. Logga in på [!DNL Frame.io] konto.
1. Gå till **[!UICONTROL Tokens]** sidan i [!DNL Frame.io] Utvecklare.
1. Klicka på **[!UICONTROL New]**.
1. Ange namnet på variabeln, markera de omfång du vill använda och klicka på **[!UICONTROL Create]**.
1. Kopiera angiven token.
1. Gå till [!DNL Workfront Fusion] och öppna [!DNL Frame.io] modulens **[!UICONTROL Create a connection]** -dialogrutan.
1. I **[!UICONTROL Connection type]** fält, markera **[!DNL Frame.io]**.
1. Ange den token som du har kopierat i steg 5 till **[!UICONTROL Your [!DNL Frame.io] API Key]** fält och klicka **[!UICONTROL Continue]** för att upprätta anslutningen.

Anslutningen har upprättats. Du kan fortsätta med att konfigurera modulen.

### Anslut till [!DNL Frame.io] med OAuth 2.0 PKCE

Du kan skapa en anslutning till [!DNL Frame.io] med OAuth 2.0 PKCE och ett valfritt klient-ID. Om du vill inkludera ett klient-ID i anslutningen måste du skapa en OAuth 2.0-app i din [!DNL Frame.io] konto.

* [Anslut till [!DNL Frame.io] med OAuth 2.0 PKCE (utan klient-ID)](#connect-to-frameio-using-using-oauth-20-pkce-without-client-id)
* [Anslut till [!DNL Frame.io] med OAuth 2.0 PKCE (med klient-ID)](#connect-to-frameio-using-using-oauth-20-pkce-with-client-id)

#### Anslut till [!DNL Frame.io] med OAuth 2.0 PKCE (utan klient-ID)

1. Gå till [!DNL Workfront Fusion] och öppna [!DNL Frame.io] modulens **[!UICONTROL Create a connection]** -dialogrutan.
1. I **[!UICONTROL Connection type]** fält, markera **[!UICONTROL [!DNL Frame.io] OAuth 2.0 PKCE]**.
1. Ange ett namn för den nya anslutningen i dialogrutan **[!UICONTROL Connection name]** fält.
1. Klicka **[!UICONTROL Continue]** för att upprätta anslutningen.

Anslutningen har upprättats. Du kan fortsätta med att konfigurera modulen.

#### Anslut till [!DNL Frame.io] med OAuth 2.0 PKCE (med klient-ID)

1. Skapa en OAuth 2.0-app i [!DNL Frame.io]. Instruktioner finns i [!DNL Frame.io] dokumentation om [!UICONTROL OAuth 2.0 Code Authorization Flow].

   >[!IMPORTANT]
   >
   >När du skapar OAuth 2.0-appen i [!DNL Frame.io]:
   >
   >* Ange följande som omdirigerings-URI:
   >   
   >  Amerika/APAC `https://app.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >  EMEA `https://app-eu.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >* Aktivera alternativet PCKE.


1. Kopiera den angivna `client_id`.
1. Gå till [!DNL Workfront Fusion] och öppna [!DNL Frame.io] modulens **[!UICONTROL Create a connection]** -dialogrutan.
1. I **[!UICONTROL Connection type]** fält, markera **[!UICONTROL [!DNL Frame.io] OAuth 2.0 PKCE]**.
1. Ange ett namn för den nya anslutningen i dialogrutan **[!UICONTROL Connection name]** fält.
1. Klicka på **[!UICONTROL Show advanced settings]**.
1. Ange `client_id` du kopierade i steg 2 till **[!UICONTROL Client ID]** fält.
1. Klicka **[!UICONTROL Continue]** för att upprätta anslutningen.

Anslutningen har upprättats. Du kan fortsätta med att konfigurera modulen.

## [!DNL Frame.io] moduler och deras fält

När du konfigurerar [!DNL Frame.io] moduler, [!DNL Workfront Fusion] visar fälten som listas nedan. Tillsammans med dessa finns ytterligare [!DNL Frame.io] fält kan visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Resurser](#assets)
* [Kommentarer](#comments)
* [Projekt](#projects)
* [Övriga](#other)

### Resurser

* [[!UICONTROL Create an Asset]](#create-an-asset)
* [[!UICONTROL Delete an Asset]](#delete-an-asset)
* [[!UICONTROL Get an Asset]](#get-an-asset)
* [[!UICONTROL List Assets]](#list-assets)
* [[!UICONTROL Update an Asset]](#update-an-asset)
* [[!UICONTROL Watch Asset Deleted]](#watch-asset-deleted)
* [[!UICONTROL Watch Asset Label Updated]](#watch-asset-label-updated)
* [[!UICONTROL Watch New Asset]](#watch-new-asset)

#### [!UICONTROL Create an Asset]

Den här åtgärdsmodulen skapar en ny resurs.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Frame.io], se <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Frame.io] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Välj eller mappa teamet som äger projektet som du vill skapa en resurs för.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>Markera projektet eller mappa ID:t för projektet som du vill skapa en resurs för.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>Markera mappen eller mappa ID:t för mappen som du vill skapa en resurs i.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type] </td> 
   <td> <p>Välj om du vill skapa en mapp eller fil.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Ange namnet på den nya filen eller mappen.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">File Type </td> 
    <td> <p>Select the type of file you want to upload.</p> </td> 
   </tr>
  --> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">File Size </td> 
    <td> <p>The file size in bytes.</p> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source URL] </td> 
   <td> <p>Ange URL-adressen till filen som du vill överföra.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description] </td> 
   <td> <p>Ange en kort beskrivning av resursen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete an Asset]

Den här åtgärdsmodulen tar bort en angiven resurs.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Frame.io], se <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Frame.io] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Markera eller mappa teamet som äger projektet som innehåller resursen som du vill ta bort.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p> Markera projektet eller det som innehåller resursen som du vill ta bort.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>Markera mappen som innehåller resursen som du vill ta bort</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>Markera eller mappa resursen som du vill ta bort.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get an Asset]

Den här åtgärdsmodulen hämtar resursinformation.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Frame.io], se <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Frame.io] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Välj eller mappa det team som äger projektet som innehåller resursen som du vill hämta information om.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p> Välj det projekt som innehåller resursen som du vill hämta information om.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>Välj den mapp som innehåller resursen som du vill hämta information om.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>Markera resursen eller mappa ID:t för resursen som du vill hämta information om.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List Assets]

Den här sökmodulen hämtar alla resurser i det angivna projektets mapp.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Frame.io], se <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Frame.io] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Välj eller mappa det team som äger projektet som innehåller mappen som du vill hämta resurser från.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p> Välj det projekt som innehåller mappen som du vill hämta resurser från.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>Välj den mapp som du vill visa resurser från.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Ange maximalt antal resurser [!DNL Workfront Fusion] returneras under en körningscykel.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### `[!UICONTROL Update an Asset]`

Med den här åtgärdsmodulen kan du uppdatera en befintlig resurs namn, beskrivning eller anpassade fält.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Frame.io], se <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Frame.io] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Välj eller mappa teamet som äger projektet som du vill uppdatera en resurs för.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>Markera projektet eller mappa ID:t för projektet som du vill uppdatera en resurs för.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>Markera mappen eller mappa ID:t för mappen som du vill uppdatera en resurs i.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Ange namnet på den uppdaterade filen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description] </td> 
   <td> <p>Ange en kort beskrivning av den uppdaterade resursen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch Asset Deleted]

Den här utlösarmodulen startar ett scenario när en resurs tas bort.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p> Ange namnet på webkroken, t.ex. resurs borttagen.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Frame.io], se <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Frame.io] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Välj teamet som den här webboken skapas för.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch Asset Label Updated]

Den här utlösarmodulen startar ett scenario när en resurs status anges, ändras eller tas bort.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p> Ange namnet på webkroken, t.ex. uppdaterad resursstatus.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Frame.io], se <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Frame.io] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Välj teamet som den här webboken skapas för.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch New Asset]

Den här utlösarmodulen startar ett scenario när en ny resurs skapas.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p> Ange namnet på webkroken, t.ex. Skapad resurs.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Frame.io], se <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Frame.io] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Välj teamet som den här webboken skapas för.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Kommentarer

* [[!UICONTROL Create a Comment]](#create-a-comment)
* [[!UICONTROL Delete a Comment]](#delete-a-comment)
* [[!UICONTROL Get a Comment]](#get-a-comment)
* [[!UICONTROL List Comments]](#list-comments)
* [[!UICONTROL Update a Comment]](#update-a-comment)
* [[!UICONTROL Watch Comment Updated]](#watch-comment-updated)
* [[!UICONTROL Watch New Comment]](#watch-new-comment)

#### [!UICONTROL Create a Comment]

Den här åtgärdsmodulen lägger till en ny kommentar eller ett nytt svar till resursen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Frame.io], se <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Frame.io] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type] </td> 
   <td> <p>Välj om du vill skapa en kommentar eller svara på en kommentar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Markera eller mappa teamet som äger projektet som innehåller resursen som du vill lägga till en kommentar i.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>Markera projektet eller mappa ID:t för projektet som innehåller resursen som du vill lägga till en kommentar i.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>Markera mappen eller mappa ID:t för mappen som innehåller resursen som du vill lägga till en kommentar i.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>Markera eller mappa resursen som du vill lägga till en kommentar i.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment ID] </td> 
   <td> <p>Markera eller mappa kommentaren som du vill lägga till ett svar i.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text]</td> 
   <td> <p> Ange textinnehållet i kommentaren eller svaret.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timestamp] </td> 
   <td> <p>Ange bildrutenumret i videon som kommentaren ska länkas till.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a Comment]

Den här åtgärdsmodulen tar bort en befintlig kommentar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Frame.io], se <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Frame.io] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID]</td> 
   <td> <p> Markera eller mappa teamet som äger projektet som innehåller resursen som du vill ta bort en kommentar från.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p> Markera projektet eller mappa ID:t för projektet som innehåller resursen som du vill ta bort en kommentar från.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID]</td> 
   <td> <p> Markera mappen som innehåller resursen som du vill ta bort en kommentar från.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>Markera resursen som innehåller kommentaren som du vill ta bort.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment ID] </td> 
   <td> <p>Markera den kommentar som du vill ta bort.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a Comment]

Den här åtgärdsmodulen hämtar information om den angivna kommentaren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Frame.io], se <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Frame.io] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Välj eller mappa teamet som äger projektet som innehåller mappen som du vill hämta resurser från.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>Välj det projekt som innehåller mappen som du vill hämta resurser från.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>Välj den mapp som du vill visa resurser från.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>Markera resursen som innehåller kommentaren som du vill hämta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment ID] </td> 
   <td> <p>Markera kommentaren som du vill hämta information om.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List Comments]

Den här sökmodulen hämtar alla kommentarer för den angivna resursen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Frame.io], se <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Frame.io] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Markera eller mappa det team som äger projektet som innehåller mappen som du vill hämta kommentarer från.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>Välj det projekt som innehåller mappen som du vill hämta kommentarer från.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>Markera den mapp som innehåller resursen som du vill visa kommentarer från.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>Markera den resurs som du vill visa kommentarer för.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Ange maximalt antal kommentarer [!DNL Workfront Fusion] returneras under en körningscykel.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update a Comment]

Den här åtgärdsmodulen redigerar en befintlig kommentar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Frame.io], se <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Frame.io] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Markera eller mappa teamet som äger projektet som innehåller resursen som du vill uppdatera en kommentar för.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>Markera projektet \ som innehåller resursen som du vill uppdatera en kommentar för.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>Markera mappen som innehåller resursen som du vill uppdatera en kommentar för.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>Markera den resurs som du vill uppdatera en kommentar på.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment ID] </td> 
   <td> <p>Markera den kommentar som du vill uppdatera.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text]</td> 
   <td> <p> Ange textinnehållet i kommentaren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timestamp] </td> 
   <td> <p>Ange bildrutenumret i videon som kommentaren är länkad till.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch Comment Updated]

Den här utlösarmodulen startar ett scenario när en kommentar redigeras.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name] </td> 
   <td> <p>Ange namnet på webkroken, t.ex. Redigerad kommentar.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Frame.io], se <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Frame.io] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Välj teamet som den här webboken skapas för.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch New Comment]

Den här utlösarmodulen startar ett scenario när en ny kommentar eller ett nytt svar skapas.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name] </td> 
   <td> <p>Ange namnet på webkroken, t.ex. Ny kommentar.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Frame.io], se <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Frame.io] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Välj teamet som den här webboken skapas för.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Projekt

#### [!UICONTROL List Projects]

Den här sökmodulen hämtar alla projekt för det angivna teamet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Frame.io], se <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Frame.io] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Välj eller mappa teamet som du vill hämta projekt för.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Ange maximalt antal projekt [!DNL Workfront Fusion] returneras under en körningscykel.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Övriga

#### [!UICONTROL Make an API Call]

Med den här modulen kan du utföra ett anpassat API-anrop.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Frame.io], se <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Frame.io] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Ange en sökväg som är relativ till <code>https://api.frame.io</code>. Exempel: <code> /v2/teams</code></p> <p>Obs! En lista över tillgängliga slutpunkter finns i [!DNL Frame.io] API-referens.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-förfrågningsmetoder i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Lägg till rubrikerna för begäran i form av ett standard-JSON-objekt.</p> <p>Exempel: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] lägger till auktoriseringshuvuden automatiskt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String] </td> 
   <td> <p>Ange frågesträngen för begäran. För varje parameter som du vill ta med i frågesträngen klickar du på <b>[!UICONTROL Add item]</b> och ange fältets namn och det önskade värdet.</p> </td> 
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

**Exempel:** Följande API-anrop returnerar alla team och dess information i ditt [!DNL Frame.io] konto:

URL: `/v2/teams`

Metod: `GET`

![](assets/api-call-example.png)

Resultatet finns i modulens Utdata under Paket > Brödtext.

I vårt exempel returnerades information om 1 team:

![](assets/api-call-output.png)

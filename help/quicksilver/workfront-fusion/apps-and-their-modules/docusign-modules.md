---
title: DocuSign-moduler
description: The [!DNL Adobe Workfront Fusion DocuSign] kan du övervaka och hämta kuvertstatus, söka efter och hämta kuvert eller ladda ned och skicka ett dokument för signering [!DNL DocuSign] konto.
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: a6ebfe6f-dc3f-41f7-8129-bbc5775cff33
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '1647'
ht-degree: 0%

---

# DocuSign-moduler

The [!DNL Adobe Workfront Fusion] [!DNL DocuSign] kan du övervaka och hämta kuvertstatus, söka efter och hämta kuvert eller ladda ned och skicka ett dokument för signering [!DNL DocuSign] konto.

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

Används [!DNL DocuSign] moduler, du måste ha en [!DNL DocuSign] konto.

## Anslut [!DNL DocuSign] till [!DNL Workfront Fusion] {#connect-docusign-to-workfront-fusion}

Skapa en anslutning för [!DNL DocuSign] moduler:

1. Klicka **[!UICONTROL Add]** bredvid [!UICONTROL Connection] när du börjar konfigurera den första [!DNL DocuSign] -modul.
1. Ange följande:

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td>Ange ett namn för den nya [!DNL DocuSign] anslutning</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Account type]</td> 
      <td>Välj om du vill ansluta till kontot är ett produktionskonto eller ett demokonto.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fortsätt enligt beskrivningen i [Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner](../../workfront-fusion/connections/connect-to-fusion-general.md#connect).

## [!DNL DocuSign] moduler och deras fält

När du konfigurerar [!DNL DocuSign] moduler, [!DNL Workfront Fusion] visar fälten som listas nedan. Tillsammans med dessa finns ytterligare [!DNL DocuSign] fält kan visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Utlösare](#triggers)
* [Åtgärder](#actions)

### Utlösare

#### [!UICONTROL Watch envelopes]

Den här utlösarmodulen startar ett scenario när ett kuvert skickas, levereras, signeras, slutförs eller avvisas.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL DocuSign] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Anslut modulens app eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>Välj det konto som innehåller de poster som du vill bevaka.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event type]</td> 
   <td> <p> Välj vilken typ av händelse du vill bevaka.</p> 
    <ul> 
     <li>[!UICONTROL Document completed]</li> 
     <li>[!UICONTROL Document declined]</li> 
     <li>[!UICONTROL Document sent]</li> 
     <li>[!UICONTROL Document signed]</li> 
     <li>[!UICONTROL New document in Inbox]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Output fields]</p> </td> 
   <td> <p>Markera de fält som du vill inkludera i modulutdata.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Ange eller mappa det maximala antal poster som du vill att modulen ska arbeta med under varje körningscykel för scenario.</td> 
  </tr> 
 </tbody> 
</table>

### Åtgärder

* [[!UICONTROL Custom API Call]](#custom-api-call)
* [[!UICONTROL Download a document]](#download-a-document)
* [[!UICONTROL Read an envelope]](#read-an-envelope)
* [[!UICONTROL Upload a file to an envelope]](#upload-a-file-to-an-envelope)
* [[!UICONTROL Create a new envelope]](#create-a-new-envelope)
* [[!UICONTROL Add Recipient to Envelope]](#add-recipient-to-envelope)
* [[!UICONTROL Add custom field]](#add-custom-field)
* [[!UICONTROL Modify custom field]](#modify-custom-field)
* [[!UICONTROL Send envelope]](#send-envelope)

#### [!UICONTROL Custom API Call]

Med den här åtgärdsmodulen kan du utföra ett anpassat API-anrop.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL DocuSign] konto till [!DNL Workfront Fusion], se <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Anslut [!DNL DocuSign] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Account]</td> 
   <td>Ange eller mappa kontot som du vill använda för att få åtkomst till [!DNL DocuSign] API.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>Skriv adressen på webbservern som du vill att modulen ska interagera med.</p> <p>Du kan ange en relativ URL-adress, vilket betyder att du inte behöver inkludera protokollet (till exempel <code>http://</code>) i början. Detta tyder på för webbservern att interaktionen sker på servern.</p> <p>Exempel: <code>[!DNL /api/conversations].create</code></p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Method]</td> 
   <td> <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-förfrågningsmetoder i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Headers]</td> 
   <td> <p>Lägg till rubrikerna för begäran i form av ett standard-JSON-objekt. Detta avgör begärans innehållstyp.</p> <p>Exempel:<code> {"Content-type":"application/json"}</code></p> <p>Obs! Om du får felmeddelanden och det är svårt att fastställa deras ursprung bör du överväga att ändra rubrikerna baserat på [!DNL Workfront] dokumentation. Om ditt anpassade API-anrop returnerar ett 422 HTTP-begärandefel kan du försöka med att använda rubriken"Content-Type":"text/plain".</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query String]</td> 
   <td> <p>Lägg till frågan för API-anropet i form av ett standard-JSON-objekt.</p> <p>Exempel: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body]</td> 
   <td> <p>Lägg till brödinnehållet för API-anropet i form av ett standard-JSON-objekt.</p> <p>Obs!  <p>När du använder villkorssatser som <code>if</code> i JSON placerar citattecknen utanför villkorssatsen.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td>Ange eller mappa det maximala antalet resultat som ska bearbetas under en körningscykel.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exempel:** Listkuvert
>
>Följande API-anrop returnerar kuvert från det angivna datumet i [!DNL DocuSign] konto:
>
>**URL**: `/v2.1/accounts/{accountId}/envelopes/`
>
>**Metod**: `GET`
>
>**Frågesträng**:
>
>* **Nyckel**: `from_date`
>
>* **Värde**: `YYYY-MM-DD`
>
>Anger när begäran börjar söka efter statusändringar för kuvert i kontot.
>
>![](assets/example-docusign-setup-350x770.png)
>
>Resultatet finns i modulens Utdata under Paket > Brödtext > Omslag.
>
>I vårt exempel returnerades 6 kuvert:
>
>![](assets/docusign-example-output-350x677.png)

#### [!UICONTROL Download a document]

Den här åtgärdsmodulen hämtar ett enstaka dokument.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL DocuSign] konto till [!DNL Workfront Fusion], se <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Anslut [!DNL DocuSign] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>Välj det konto som innehåller dokumentet som du vill hämta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> Ange eller mappa ID:t för kuvertet som du vill hämta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Document ID]</p> </td> 
   <td> <p>Ange eller mappa ID:t för dokumentet som du vill hämta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Certificate]</td> 
   <td>Välj <strong>[!UICONTROL Yes]</strong> om du vill inkludera kuvertsigneringscertifikatet i hämtningen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Documents by User ID]</td> 
   <td>Välj <strong>[!UICONTROL Yes]</strong> om du vill tillåta mottagarna att hämta dokument efter användar-ID. Om en användare till exempel ingår i två olika routningsordningar med olika synligheter, returnerar det här alternativet alla dokument från båda routningarna.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encrypt]</td> 
   <td>Välj <strong>[!UICONTROL Yes]</strong> om du vill att PDF byte som returneras i svaret ska krypteras för alla nyckelhanterare som konfigurerats på din [!DNL DocuSign] konto.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Language]</td> 
   <td>Välj språk.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show Changes]</td> 
   <td>När inställt på <strong>[!UICONTROL Yes]</strong>, markeras alla ändrade fält för det returnerade PDF i gult och valfria signaturer eller initialer i rött.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watermark]</td> 
   <td> <p>Välj <strong>[!UICONTROL No]</strong> om du vill ta bort vattenstämpeln från PDF-dokumenten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Read an envelope]

Den här åtgärdsmodulen läser information om ett omslag i [!DNL DocuSign] med kuvert-ID.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL DocuSign] konto till [!DNL Workfront Fusion], se <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Anslut [!DNL DocuSign] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>Välj det konto som innehåller dokumentet som du vill läsa information från.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> Ange eller mappa ID:t som innehåller dokumentet som du vill läsa information från.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Markera de egenskaper som du vill ska visas i modulens utdata. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Upload a file to an envelope]

Den här modulen överför en angiven fil till ett befintligt kuvert i DocuSign.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL DocuSign] konto till [!DNL Workfront Fusion], se <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Anslut [!DNL DocuSign] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>Välj det konto som innehåller kuvertet där du vill överföra en fil.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> Ange eller mappa ID:t för kuvertet där du vill överföra en fil.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Välj en källfil från en tidigare modul eller ange källfilens namn och data.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create a new envelope]

Den här åtgärdsmodulen skapar ett nytt kuvert från en mall. Det returnerar det nya kuvertets ID samt statusen för det nya kuvertet.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td>

<td> <p>Instruktioner om hur du ansluter ditt DocuSign-konto till Workfront Fusion finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app eller webbtjänst till Workfront Fusion</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Account] </td>
   <td> <p>Välj det konto som innehåller kuvertet där du vill överföra en fil.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Template]</td>
   <td> <p> Välj den mall som du vill skapa det nya kuvertet från. Mallar är tillgängliga baserat på [!UICONTROL Account] du markerade.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">
     [!UICONTROL After creation]
   </td> 
   <td> <p>Välj om du vill spara kuvertet som ett utkast eller skicka det för signering.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Template recipients]</td>
    <td>Välj mottagare av kuvertet</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Add Recipient to Envelope]

Den här åtgärdsmodulen lägger till en eller flera mottagare i ett befintligt kuvert. Om kuvertet redan har skickats skickas ett e-postmeddelande till mottagaren. Den här modulen är inte giltig för kuvert som redan har slutförts.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Connection] </td>
   <td> <p>Instruktioner om hur du ansluter ditt DocuSign-konto till Workfront Fusion finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app eller webbtjänst till Workfront Fusion</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Account] </td>
   <td> <p>Välj det konto som innehåller kuvertet där du vill lägga till mottagare.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Envelope ID]</td>
    <td>Markera eller mappa ID:t för kuvertet där du vill lägga till mottagaren.</td>
  </tr> 
  <tr data-mc-conditions="">
    <td role="rowheader">[!UICONTROL Recipient type]</td>
   <td> <p> Välj den typ av mottagare som du vill lägga till i kuvertet.</p> 
    <ul> 
     <li> <p>[!UICONTROL Agent]</p> </li> 
     <li> <p>[!UICONTROL Carbon copy]</p> </li> 
     <li> <p>[!UICONTROL Certified delivery]</p> </li> 
     <li> <p>[!UICONTROL In-person signer]</p> </li> 
     <li> <p>[!UICONTROL Intermediary]</p> </li> 
     <li> <p>[!UICONTROL Signer]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Email]</td>
   <td> <p>Ange eller mappa e-postadressen till mottagaren som du vill lägga till i kuvertet.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Name]</td>
   <td>Ange eller mappa namnet på mottagaren som du vill lägga till i kuvertet.</td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Routing order]</td>
   <td> <p>Ange eller mappa routningsnumret för mottagaren. Routningsnummer avgör i vilken ordning mottagarna tar emot och signerar dokumenten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Email body]</td>
   <td>Ange eller mappa e-postmeddelandets brödtext (innehåll) till mottagaren.</td> 
  </tr> 
  <tr>
    <td role="rowheader">[!UICONTROL Email subject]</td>
   <td>Ange eller mappa ämnet för det e-postmeddelande som skickas till mottagaren.</td> 
  </tr> 
    <td role="rowheader">[!UICONTROL Private message]</td>
   <td> <li> <p>Det är bara den valda mottagaren som ser det privata meddelandet samt det allmänna meddelandet. Det privata meddelandet får innehålla högst 1 000 tecken.</p> </li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Authentication]</td> 
   <td> <p>Välj den autentiseringsmetod som du vill använda för att bekräfta mottagarens identitet.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL None]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Access code]</strong> </p> <p>Ange eller mappa åtkomstkoden.</p> </li> 
     <li> <p><strong>[!UICONTROL Phone]</strong> </p> <p>Ange eller mappa telefonnumret</p> </li> 
     <li> <p><strong>[!UICONTROL SMS]</strong> </p> <p>Ange eller mappa telefonnumret</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Add custom field]

Den här åtgärdsmodulen lägger till ett anpassat fält i dokumentet

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL DocuSign] konto till [!DNL Workfront Fusion], se <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Anslut [!DNL DocuSign] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>Välj det konto som innehåller dokumentet där du vill lägga till ett anpassat fält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> Ange eller mappa ID:t för kuvertet som innehåller dokumentet där du vill lägga till ett anpassat fält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Field name]</td> 
   <td>Ange eller mappa ett namn för det nya fältet som du vill lägga till.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Required]</td> 
   <td>Aktivera det här alternativet om du vill att det tillagda fältet ska vara ett obligatoriskt fält.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show field]</td> 
   <td>Aktivera det här alternativet om du vill att fältet ska vara synligt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Value]</td> 
   <td>Ange eller mappa värdet (innehållet) för det tillagda fältet. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Modify custom field]

Den här åtgärdsmodulen ändrar ett anpassat fält med fältnamnet.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL DocuSign] konto till [!DNL Workfront Fusion], se <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Anslut [!DNL DocuSign] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>Välj det konto som innehåller dokumentet där du vill ändra ett anpassat fält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> Ange eller mappa ID:t för kuvertet som innehåller dokumentet där du vill ändra ett anpassat fält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Field ID]</td> 
   <td>Ange eller mappa ID:t för fältet som du vill ändra.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Field name]</td> 
   <td>Ange eller mappa namnet på fältet som du vill ändra.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Required]</td> 
   <td>Aktivera det här alternativet om du vill att det ändrade fältet ska vara ett obligatoriskt fält.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show field]</td> 
   <td>Aktivera det här alternativet om du vill att fältet ska vara synligt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Value]</td> 
   <td>Ange eller mappa värdet (innehållet) för det ändrade fältet. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Send envelope]

Den här åtgärdsmodulen skickar ett utkast till mottagarna.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL DocuSign] konto till [!DNL Workfront Fusion], se <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Anslut [!DNL DocuSign] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>Markera det konto som innehåller det utkast som du vill skicka till mottagarna.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> Ange eller mappa ID:t för det utkast som du vill skicka till mottagarna.</p> </td> 
  </tr> 
 </tbody> 
</table>

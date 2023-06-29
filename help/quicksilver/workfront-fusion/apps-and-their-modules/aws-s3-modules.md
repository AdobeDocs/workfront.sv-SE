---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: apps-and-their-modules
title: AWS S3-moduler
description: The [!DNL Adobe Workfront Fusion AWS] Med S3-moduler kan du utföra åtgärder på dina S3-bucket.
author: Becky
feature: Workfront Fusion
exl-id: 33623b5d-d9ff-4d41-b938-33378f50539e
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1254'
ht-degree: 0%

---

# AWS S3-moduler

The [!DNL Adobe Workfront Fusion AWS] Med S3-moduler kan du utföra åtgärder på dina S3-bucket.

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

Används [!UICONTROL AWS S3] moduler, du måste ha en [!DNL Amazon Web Service] konto.

## Anslut [!DNL AWS] till [!DNL Workfront Fusion] {#connect-aws-to-workfront-fusion}

Ansluta [!DNL AWS S3] till [!DNL Workfront Fusion] du måste koppla din [!DNL AWS] konto till [!DNL Workfront Fusion]. För att göra det måste du först skapa en API-användare i [!DNL AWS] [!UICONTROL IAM].

1. Logga in på [!DNL AWS] [!UICONTROL IAM] konto.
1. Navigera till **[!UICONTROL Identity and Access Management]** > **[!UICONTROL Access Management]** > **[!UICONTROL Users]**.

1. Klicka på **[!UICONTROL Add User]**.
1. Ange namnet på den nya användaren och välj **[!UICONTROL Programmatic access]** i [!UICONTROL Access type] -avsnitt.
1. Klicka **[!UICONTROL Attach existing policies directly]** och sedan söka efter **[!UICONTROL AmazonS3FullAccess]** i sökfältet. Klicka på den när den visas och klicka sedan på **[!UICONTROL Next]**.

1. Gå igenom de andra dialogrutorna och klicka sedan på **[!UICONTROL Create User]**.
1. Kopiera den angivna **[!UICONTROL Access key ID]** och **[!UICONTROL Secret access key]**.

1. Gå till [!DNL Workfront Fusion] och öppna [!DNL AWS S3] modulens **[!UICONTROL Create a connection]** -dialogrutan.
1. Ange [!UICONTROL Access key ID] och [!UICONTROL Secret access key] från steg 7 till respektive fält och klicka **[!UICONTROL Continue]** för att upprätta anslutningen.

Anslutningen har upprättats. Du kan fortsätta med att konfigurera modulen.

## [!DNL AWS S3] moduler och deras fält

När du konfigurerar [!DNL AWS S3] moduler, [!DNL Workfront Fusion] visar fälten som listas nedan. Tillsammans med dessa finns ytterligare [!DNL AWS S3] fält kan visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Åtgärder](#actions)
* [Sökningar](#searches)

### Åtgärder

* [[!UICONTROL Create Bucket]](#create-bucket)
* [[!UICONTROL Get File]](#get-file)
* [[!UICONTROL Upload File]](#upload-file)
* [[!UICONTROL Make an API Call]](#make-an-api-call)

#### [!UICONTROL Create Bucket]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL AWS] konto till [!DNL Workfront Fusion], se <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Anslut [!DNL AWS] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Ange namnet på den nya bucket.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Välj regional slutpunkt. Mer information finns i diskussionen om <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">regionala slutpunkter</a> i AWS-dokumentationen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get File]

Hämtar en fil från en hink.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL AWS] konto till [!DNL Workfront Fusion], se <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Anslut [!DNL AWS] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Välj regional slutpunkt. Mer information finns i diskussionen om <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">regionala slutpunkter</a> i [!DNL AWS] dokumentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>Markera den hink du vill hämta filen från.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Path]</p> </td> 
   <td> <p>Ange sökvägen till filen. Exempel: <code>/photos/2019/February/image023.jpg</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Upload File]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL AWS] konto till [!DNL Workfront Fusion], se <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Anslut [!DNL AWS] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Välj regional slutpunkt. Mer information finns i diskussionen om <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">regionala slutpunkter</a> i [!DNL AWS] dokumentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Folder] (valfritt) </p> </td> 
   <td> <p>Ange målmappen som du vill överföra en fil till.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Headers] (valfritt)</p> </td> 
   <td> <p> Infoga begäranderubriker. Tillgängliga rubriker finns i <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html">[!DNL AWS S3] dokumentation - [!UICONTROL PUT] object</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Make an API Call]

En detaljerad diskussion om [!DNL Amazon S3] API, se [[!DNL Amazon S3] [!UICONTROL REST] API-introduktion](https://docs.aws.amazon.com/AmazonS3/latest/API/Welcome.html).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL AWS] konto till [!DNL Workfront Fusion], se <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Anslut [!DNL AWS] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Region] </td> 
   <td> <p>Välj regional slutpunkt. Mer information finns i diskussionen om <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">regionala slutpunkter</a> i [!DNL AWS] dokumentation.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>URL Ange en värd-URL. Sökvägen måste vara relativ till<code> https://s3.&lt;selected-region>.amazonaws.com/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Method]</td> 
   <td> <p>Välj [!UICONTROL HTTP] begärandemetod som du måste konfigurera API-anropet. Mer information finns i <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">[!UICONTROL HTTP] förfrågningsmetoder i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Headers]</td> 
   <td> <p>Lägg till en begäranderubrik. Du kan använda följande vanliga begärandehuvuden. För fler begäranderubriker se <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTCommonRequestHeaders.html">[!DNL AWS S3] API-dokumentation</a>.</p> <p>[!DNL Workfront Fusion] lägger till auktoriseringshuvuden automatiskt.</p> 
    <table style="table-layout:auto">
     <col> 
     <col> 
     <thead> 
      <tr> 
       <th>Rubriknamn</th> 
       <th> <p> Beskrivning</p> </th> 
      </tr> 
     </thead> 
     <tbody> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Length]</p> </td> 
       <td> <p>Meddelandets längd (utan rubriker) enligt RFC 2616. Den här rubriken krävs för [!UICONTROL PUT]och åtgärder som läser in XML, till exempel loggning och åtkomstkontrollistor.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Type]</p> </td> 
       <td> <p>Resursens innehållstyp om begärandeinnehållet finns i brödtexten. Exempel: <code>text/plain</code>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-MD5]</p> </td> 
       <td> <p>Base64-kodade 128-bitars MD5-meddelandet (utan rubriker) enligt RFC 1864. Den här rubriken kan användas som en meddelandeintegritetskontroll för att verifiera att data är samma data som ursprungligen skickades. Även om det är valfritt rekommenderar vi att du använder [!UICONTROL Content-MD5] som en helhetskontroll. Mer information om [!UICONTROL REST] autentiseringsbegäran, gå till <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/RESTAuthentication.html?r=1821">[!UICONTROL REST] Autentisering</a> i <i>[!DNL Amazon] Utvecklarhandbok för enkel lagringstjänst</i>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Date]</p> </td> 
       <td> <p>Aktuellt datum och aktuell tid enligt den som gjorde begäran. Exempel: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. När du anger <code>Authorization </code>måste du ange antingen <code>x-amz-date</code> eller <code>Date </code>header.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Expect]</p> </td> 
       <td> <p>När ditt program använder [!UICONTROL 100-continue]skickar den inte begärandetexten förrän den får en bekräftelse. Om meddelandet avvisas baserat på rubrikerna skickas inte meddelandets brödtext. Den här rubriken kan bara användas om du skickar en text.</p> <p>Giltiga värden: [!UICONTROL 100-continue]</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Host]</p> </td> 
       <td> <p>För sökvägsbegäranden är värdet <code>s3.amazonaws.com</code>. För virtuella begäranden är värdet <code>BucketName.s3.amazonaws.com</code>. Mer information finns i <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/VirtualHosting.html">Virtuellt värdskap</a> i <i>[!DNL Amazon] Utvecklarhandbok för enkel lagringstjänst</i>.</p> <p>Detta huvud krävs för HTTP 1.1 (de flesta verktygslådor lägger till detta huvud automatiskt); valfritt för HTTP/1.0-begäranden.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-content-sha256]</p> </td> 
       <td> <p>När du använder signaturversion 4 för att autentisera begäran ger det här huvudet en hash av nyttolasten för begäran. När du överför ett objekt i segment anger du värdet till <code>STREAMING-AWS4-HMAC-SHA256-PAYLOAD</code> för att ange att signaturen endast omfattar rubriker och att det inte finns någon nyttolast. Mer information finns i <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-streaming.html">Signaturberäkningar för auktoriseringshuvudet: Överför nyttolast i flera segment (uppladdning i segment) ([!DNL AWS] Signatur version 4)</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-date]</p> </td> 
       <td> <p>Aktuellt datum och aktuell tid enligt den som gjorde begäran. Exempel: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. När du anger <code>Authorization </code>måste du ange antingen <code>x-amz-date</code> eller <code>Date </code>header. Om du anger båda anges värdet för <code>x-amz-date</code> har företräde.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-security-token]</p> </td> 
       <td> <p>Den här rubriken kan användas i följande scenarier:</p> 
        <ul> 
         <li>Ange säkerhetstoken för [!DNL Amazon DevPay] åtgärder. Varje begäran som använder [!DNL Amazon DevPay] kräver två <code>x-amz-security-token</code> sidhuvuden: en för produkttoken och en för användartoken. När [!DNL Amazon S3] tar emot en autentiserad begäran, jämför den beräknade signaturen med den angivna signaturen. Felaktigt formaterade flervärdesrubriker som används för att beräkna en signatur kan orsaka autentiseringsproblem.</li> 
         <li>Ange en säkerhetstoken när du använder temporära säkerhetsuppgifter. När du gör begäranden med temporära säkerhetsuppgifter som du fått från IAM (InDesign) måste du ange en säkerhetstoken med den här rubriken. Om du vill veta mer om tillfälliga säkerhetsbehörigheter går du till Göra förfrågningar.</li> 
        </ul> <p>Den här rubriken krävs för begäranden som använder [!DNL Amazon DevPay] och begäranden som signeras med temporära säkerhetsuppgifter.</p> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query String]</td> 
   <td> <p>Lägg till önskade frågesträngar, t.ex. parametrar eller formulärfält.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body]</td> 
   <td> <p>Lägg till brödinnehållet för API-anropet i form av ett standard-JSON-objekt.</p> <p>Obs!   <p>När du använder villkorssatser som <code>if</code> i JSON placerar citattecknen utanför villkorssatsen.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### Sökningar

* [[!UICONTROL List Files]](#list-files)
* [[!UICONTROL List Folders]](#list-folders)

#### [!UICONTROL List Files]

Returnerar en lista med filer från en angiven plats.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL AWS] konto till [!DNL Workfront Fusion], se <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Anslut [!DNL AWS] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Välj regional slutpunkt. Mer information finns i diskussionen om <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">regionala slutpunkter</a> i [!DNL AWS] dokumentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>Välj [!DNL Amazon S3] som du vill söka efter filer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefix] (valfritt)</p> </td> 
   <td> <p> Sökväg till en mapp där filer ska slås upp, t.ex. <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List Folders]

Returnerar en lista med mappar från en angiven plats.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL AWS] konto till [!DNL Workfront Fusion], se <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Anslut [!DNL AWS] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Välj regional slutpunkt. Mer information finns i diskussionen om <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">regionala slutpunkter</a> i AWS-dokumentationen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>Välj [!DNL Amazon S3] som du vill söka efter mappar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefix] (valfritt)</p> </td> 
   <td> <p> Sökväg till en mapp där du kan söka efter mappar, t.ex. <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

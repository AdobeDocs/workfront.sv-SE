---
title: Adobe PDF Services
description: Adobe PDF Services
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: e0a5736b-dbdb-43c6-83ff-e88a5625a5bf
source-git-commit: b43ea012d7c649c94011f72f010ae24895e6ef4b
workflow-type: tm+mt
source-wordcount: '3108'
ht-degree: 0%

---

# [!DNL Adobe PDF Services]

Med [!DNL Adobe Workfront Fusion] [!DNL Adobe PDF Services]kan du extrahera data från en PDF-fil eller generera en ny PDF-fil från data du anger. Dessutom kan du konvertera en mängd olika filtyper till PDF eller PDF till andra filtyper. Med PDF Services kan du även kombinera, komprimera och läsa metadata för en PDF-fil samt styra lösenordsskyddet för filen.

Om du behöver instruktioner om hur du skapar ett scenario kan du läsa [Skapa ett scenario i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Mer information om moduler finns i [Moduler i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

Mer information om API:t för PDF Services finns i [Adobe-API för dokumentgenerering](https://www.adobe.io/apis/documentcloud/dcsdk/doc-generation.html).

## Säkerhetsaspekter vid användning [!DNL Adobe PDF Services]

<!--

* [You do not need an [!DNL Adobe] account](#you-do-not-need-an-adobe-account) 
* [[!DNL Workfront Fusion] does not store your files](#workfront-fusion-does-not-store-your-files)

### You do not need an [!DNL Adobe] account 

Because [!DNL Workfront Fusion] is part of the [!DNL Adobe] product suite, you don't need a separate [!DNL Adobe] account to use these tools. Each tool accesses [!DNL Adobe] PDF functionality without using a connection.

Although [!DNL Workfront Fusion] does not require an [!DNL Adobe] account to use the PDF Services, the modules do require a connection. There are no credentials involved in this connection, and you provide only a name for the connection itself.

### [!DNL Workfront Fusion] does not store your files 

-->

The [!DNL Adobe PDF Services] kan läsa, konvertera eller ändra filer, men varken [!DNL Adobe] eller [!DNL Workfront Fusion] lagra filer eller data. Detta innebär att

* Du behåller kontrollen över dina filer, inklusive deras säkerhet
* Du behöver inte ha en [!UICONTROL Adobe] lagringskonto eller molnlagringskonto för användning av PDF-tjänster.

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
   <p>Krav för äldre produkter: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta din [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Förutsättningar

Om du vill skapa en OAuth Server-till-server måste du lägga till API:t för Adobe PDF Services i Adobe Developers Console. När du lägger till API:t väljer du alternativet OAuth Server-till-server.

Instruktioner finns i [Lägg till API i projekt med OAuth](https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/) I dokumentationen för utvecklaren av Adobe.

## Skapa en anslutning till [!DNL Adobe PDF Services]

Skapa en anslutning för [!DNL Adobe PDF Services] moduler:

1. I alla [!DNL Adobe PDF Services] modul, klicka på **[!UICONTROL Add]** bredvid rutan Anslutning.

1. Fyll i följande fält:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Connection type]</td>
          <td>
            <p>Välj om du vill skapa en server-till-server-anslutning eller en JWT-anslutning.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Connection name]</td>
          <td>
            <p>Ange ett namn för anslutningen.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client ID]</td>
          <td>Ange [!DNL Adobe] [!UICONTROL Client ID]. Detta finns i [!UICONTROL Credentials details] i [!DNL Adobe Developer Console].<p>Instruktioner om hur du hittar inloggningsuppgifter finns i <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >Referenser</a> i dokumentationen för utvecklaren av Adobe.</p></td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client Secret]</td>
          <td>Ange [!DNL Adobe] [!UICONTROL Client Secret]. Detta finns i [!UICONTROL Credentials details] i [!DNL Adobe Developer Console].<p>Instruktioner om hur du hittar inloggningsuppgifter finns i <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >Referenser</a> i dokumentationen för utvecklaren av Adobe.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Technical account ID] (endast JWT)</td>
          <td>Ange [!DNL Adobe] [!UICONTROL Technical account ID]. Detta finns i [!UICONTROL Credentials details] i [!DNL Adobe Developer Console].<p>Instruktioner om hur du hittar inloggningsuppgifter finns i <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >Referenser</a> i dokumentationen för utvecklaren av Adobe.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Organization ID] (endast JWT)</td>
          <td>Ange [!DNL Adobe] [!UICONTROL Organization ID]. Detta finns i [!UICONTROL Credentials details] i [!DNL Adobe Developer Console].<p>Instruktioner om hur du hittar inloggningsuppgifter finns i <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >Referenser</a> i dokumentationen för utvecklaren av Adobe.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Meta scopes] (endast JWT)</td>
          <td>
            Ange eventuella metaomfång som behövs för anslutningen.
          </td>
        </tr>
       </tbody>
    </table>
1. Klicka **[!UICONTROL Continue]** för att spara anslutningen och återgå till modulen.


## [!DNL Adobe PDF Services] moduler och deras fält

När du konfigurerar [!DNL PDF Services], [!DNL Workfront Fusion] visar fälten som listas nedan. Dessutom kan ytterligare fält visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En fetstilt titel i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Generate document]](#generate-document)
* [[!UICONTROL Extract Text / Table]](#extract-text--table)
* [[!UICONTROL Combine PDF files]](#combine-pdf-files)
* [[!UICONTROL Compress PDF files]](#compress-pdf-files)
* [[!UICONTROL Convert document to PDF file]](#convert-document-to-pdf-file)
* [[!UICONTROL Convert HTML to PDF file]](#convert-html-to-pdf-file)
* [[!UICONTROL Convert image to PDF file]](#convert-image-to-pdf-file)
* [[!UICONTROL Convert PDF to document]](#convert-pdf-to-document)
* [[!UICONTROL Convert PDF to image]](#convert-pdf-to-image)
* [[!UICONTROL Linearize a PDF file]](#linearize-a-pdf-file)
* [[!UICONTROL OCR for PDF file]](#ocr-for-pdf-file)
* [[!UICONTROL Page manipulation]](#page-manipulation)
* [[!UICONTROL PDF accessibility auto-tag]](#pdf-accessibility-auto-tag)
* [[!UICONTROL PDF file properties]](#pdf-file-properties)
* [[!UICONTROL Protect PDF file]](#protect-pdf-file)
* [[!UICONTROL Remove protection of a PDF file]](#remove-protection-of-a-pdf-file)
* [Dela en PDF-fil](#split-a-pdf-file)

### [!UICONTROL Generate document]

The [!UICONTROL Generate document] är ett kraftfullt sätt att skapa ett PDF som innehåller de data du väljer. Du kan formatera den med en [!DNL Microsoft Word] eller genom att tillhandahålla data i JSON-format.

Mer information om [!UICONTROL [!DNL Adobe PDF Services] Generate document] finns i [Översikt över dokumentgenerering](https://www.adobe.io/apis/documentcloud/dcsdk/docs.html) i [!DNL Adobe Document Services] dokumentation.

* [Använd [!UICONTROL Generate document] modul med [!DNL Microsoft Word] mall](#use-the-generate-document-module-with-a-microsoft-word-template)
* [Använd [!UICONTROL Generate document] modul med JSON](#use-the-generate-document-module-with-json)

#### Använd [!UICONTROL Generate document] modul med [!DNL Microsoft Word] mall

<!--
>[!NOTE]
>
>For a discussion of Microsoft Word templates, see [Microsoft Word Template modules](../../workfront-fusion/apps-and-their-modules/microsoft-word-templates-modules.md). 
>
>You do not need to use Microsoft Word template modules to use a Microsoft Word template with the PDF Services Generate document module.
-->

Använd [!UICONTROL Generate document] modul med [!UICONTROL Microsoft Word] måste du först skapa mallen. Sök efter&quot;Skapa en mall&quot; i dialogrutan [!DNL Microsoft Office] dokumentation.

Fyll i [!UICONTROL Generate document] modulfält enligt följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Markera anslutningen som ska användas för den här modulen.</p> Instruktioner om hur du skapar en anslutning till [!DNL Adobe PDF Services], se <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe PDF Services]</a> i den här artikeln. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source File]</td> 
   <td> <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</p> <p>Den här källfilen är [!DNL Microsoft Word ]som används i modulen för att generera det nya PDF.</p> <p>Vi rekommenderar att du skapar ett projekt i [!DNL Workfront] för [!DNL Microsoft Word] mallar som du använder i [!DNL Workfront Fusion]. Du kan sedan använda [!DNL Workfront] &gt; [!UICONTROL Download document] för att dra in rätt mall i ditt scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Format]</td> 
   <td> <p>Välj format för det genererade dokumentet.</p> 
    <ul> 
     <li> <p>PDF</p> </li> 
     <li> <p>DOCX</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data for merge]</td> 
   <td> <p>Fyll i följande för varje värdetagg i mallen som du vill ersätta med text:</p> 
    <ul> 
     <li> <p>[!UICONTROL Key]</p> <p>Ange en tangent. I mallen är nyckeln texten som visas i värdetaggen. Om du till exempel vill montera text i värdetaggen <code>&#123;&#123;name&#125;&#125;</code>, ange <code>name </code>i nyckelfältet.</p> </li> 
     <li> <p>Värdetyp</p> <p>Ange om data i värdefältet är ett värde, ett objekt eller en array med objekt.</p> </li> 
     <li> <p>[!UICONTROL Value]</p> <p>Ange eller mappa texten som du vill ska visas i det genererade dokumentet i stället för värdetaggen.</p> </li> 
    </ul> <p> <img src="assets/generate-with-template-350x241.png" style="width: 350;height: 241;"> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Använd [!UICONTROL Generate document] modul med JSON

Använd [!UICONTROL Generate document] med JSON, fyll i fälten enligt följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Markera anslutningen som ska användas för den här modulen.</p> Instruktioner om hur du skapar en anslutning till [!DNL Adobe PDF Services], se <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe PDF Services]</a> i den här artikeln. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source File]</td> 
   <td> <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Format]</td> 
   <td> <p>Välj format för det genererade dokumentet.</p> 
    <ul> 
     <li> <p>PDF</p> </li> 
     <li> <p>DOCX</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data for merge]</td> 
   <td> <p>Om du vill använda JSON i den här modulen måste du aktivera mappning för det här fältet.</p> <p>Ange eller mappa det JSON-objekt som dokumentet ska skapas från. </p> <p>Du kan skriva JSON direkt i det här fältet eller mappa JSON-utdata från en JSON-modul.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Extract Text / Table]

Med den här åtgärdsmodulen kan du extrahera data från en PDF-fil. Modulen matar ut enskilda textelement, t.ex. ett stycke eller texten i en enda cell i en tabell.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Markera anslutningen som ska användas för den här modulen.</p> Instruktioner om hur du skapar en anslutning till [!DNL Adobe PDF Services], se <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe PDF Services]</a> i den här artikeln. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elements that should be extracted as JSON]</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Text]</p> </li> 
     <li> <p>[!UICONTROL Tables]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Extract Bounding boxes?]</td> 
   <td>Aktivera det här alternativet om du vill extrahera data om textens begränsningsram.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include styling information for output?]</td> 
   <td>Aktivera det här alternativet om du vill lägga till formatinformation i JSON-utdata.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Combine PDF files]

Den här åtgärdsmodulen tar flera PDF-filer och kombinerar dem i en enda PDF-fil. Den här modulen kan till exempel kombinera alla dokument i en [!UICONTROL Workfront] till ett enda PDF när projektet är klart.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Markera anslutningen som ska användas för den här modulen.</p> Instruktioner om hur du skapar en anslutning till [!DNL Adobe PDF Services], se <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe PDF Services]</a> i den här artikeln. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Documents]</td> 
   <td> <p>Du kan använda en aggregeringsmodul för att samla dokument som ska kombineras till ett PDF, eller så kan du lägga till dokumenten manuellt. </p> <p>Vi rekommenderar att du [!UICONTROL Array Aggregator] för att samla utdata från en tidigare modul. Genom att använda en aggregator behöver du inte känna till namn, plats eller antal filer som ska kombineras. Att använda en aggregator är därför mycket flexiblare och mer skalbart än att manuellt ange de dokument som ska kombineras.</p> <p>Använd [!UICONTROL Combine PDF] filmodulen med en aggregator måste du aktivera mappning på [!UICONTROL Documents] fält. </p> <p>I det här exemplet [!UICONTROL Read Related Records] -modulen identifierar dokument som är kopplade till ett projekt och [!UICONTROL Download Documents] för nedladdning. Alla PDF samlas i en array som skickas till [!UICONTROL Combine PDF] filmodulen.</p> <p> <img src="assets/combine-example-350x104.png" style="width: 350;height: 104;"> </p> <p>Du kan också ange dokument manuellt.</p> <p>För varje dokument som ska inkluderas i den kombinerade PDF:</p> 
    <ol> 
     <li value="1"> <p>Klicka på [!UICONTROL Add a Document]</p> </li> 
     <li value="2"> <p>I [!UICONTROL Source file] markerar du modulen som matar ut dokumentet som du vill inkludera, eller mappar källfilens namn och data. </p> </li> 
     <li value="3"> <p>(Valfritt) Om du bara vill inkludera vissa sidor från källfilen, för varje sidintervall som du vill lägga till, klickar du på <strong>[!UICONTROL Add item]</strong> i [!UICONTROL Pages] och sedan ange den första och sista sidan i det sidintervall som ska inkluderas. Klicka på <strong>[!UICONTROL Add]</strong>. Du kan inkludera mer än ett sidintervall från ett enstaka dokument.</p> </li> 
     <li value="4"> <p>Klicka på <strong>[!UICONTROL Add]</strong>. </p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Compress PDF files]

Den här åtgärdsmodulen tar en PDF-fil och komprimerar den. Detta kan vara användbart för att spara bandbredd eller minne.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Markera anslutningen som ska användas för den här modulen.</p> Instruktioner om hur du skapar en anslutning till [!DNL Adobe PDF Services], se <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe PDF Services]</a> i den här artikeln. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</p> <p>Källfilen måste vara i PDF-format. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compression level]</td> 
   <td>Välj den komprimeringsnivå som du vill använda.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convert document to PDF file]

Det här verktyget konverterar ett dokument till en PDF-fil. Källfilen måste ha något av följande dokumentformat:

* DOC
* XLS
* PPT
* TXT
* RTF

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Markera anslutningen som ska användas för den här modulen.</p> Instruktioner om hur du skapar en anslutning till [!DNL Adobe PDF Services], se <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe PDF Services]</a> i den här artikeln. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</p> <p>Källfilen måste ha något av följande format:</p> 
    <ul> 
     <li> <p>DOC</p> </li> 
     <li> <p>XLS</p> </li> 
     <li> <p>PPT</p> </li> 
     <li> <p>TXT</p> </li> 
     <li> <p>RTF</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Language]</td> 
   <td> <p>Välj standardspråk för källdokumentet. Detta gör att modulen kan välja ett lämpligt teckensnitt, om det inte finns något teckensnitt i källfilen.</p> <p>Välj bland följande språk:</p> 
    <ul> 
     <li> <p>en-US (standard): engelska (USA)</p> </li> 
     <li> <p>ca-ES: Katalanska (Spanien)</p> </li> 
     <li> <p>cs-CZ: Tjeckiska (Tjeckien)</p> </li> 
     <li> <p>da-DK: danska (Danmark)</p> </li> 
     <li> <p>de-DE: German (Germany)</p> </li> 
     <li> <p>en-AE: Engelska (Förenade Arabemiraten)</p> </li> 
     <li> <p>en-GB: Engelska (Storbritannien)</p> </li> 
     <li> <p>en-IL: Engelska (Israel)</p> </li> 
     <li> <p>en-US: Engelska (USA)</p> </li> 
     <li> <p>es-ES: Spanska (Spanien)</p> </li> 
     <li> <p>es-MX: Spanska (Mexiko)</p> </li> 
     <li> <p>eu-ES: Baskiska (Spanien)</p> </li> 
     <li> <p>fi-FI: Finska (Finland)</p> </li> 
     <li> <p>fr-CA: Franska (Kanada)</p> </li> 
     <li> <p>fr-FR: Franska (Frankrike)</p> </li> 
     <li> <p>fr-MA: Franska (Marocko)</p> </li> 
     <li> <p>hr-HR: Kroatiska (Kroatien)</p> </li> 
     <li> <p>hu-HU: Ungerska (Ungern)</p> </li> 
     <li> <p>IT-IT: Italienska (Italien)</p> </li> 
     <li> <p>ja-JP: Japanska (Japan)</p> </li> 
     <li> <p>kr-KR: Koreanska (Sydkorea)</p> </li> 
     <li> <p>Anm. NO: Norska bokmål (Norge)</p> </li> 
     <li> <p>nl-NL: Nederländska (Nederländerna)</p> </li> 
     <li> <p>pl-PL: Polska (Polen)</p> </li> 
     <li> <p>pt-BR: Portugisiska (Brasilien)</p> </li> 
     <li> <p>pt-PT: Portugisiska (Portugal)</p> </li> 
     <li> <p>ro-RO: Rumänska (Rumänien)</p> </li> 
     <li> <p>RU: Ryska (Ryssland)</p> </li> 
     <li> <p>sk-SK: Slovakiska (Slovakien)</p> </li> 
     <li> <p>sl-SI: Slovenska (Slovenien)</p> </li> 
     <li> <p>sv-SE: Swedish (Sweden)</p> </li> 
     <li> <p>tr-TR: Turkiska (Turkiet)</p> </li> 
     <li> <p>uk-UA: Ukrainska (Ukraina)</p> </li> 
     <li> <p>zh-CN: Kinesiska (fastlandet Kina)</p> </li> 
     <li> <p>zh-TW: Kinesiska (Taiwan)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convert HTML to PDF file]

Det här verktyget konverterar en HTML-fil till en PDF-fil.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Markera anslutningen som ska användas för den här modulen.</p> Instruktioner om hur du skapar en anslutning till [!DNL Adobe PDF Services], se <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe PDF Services]</a> i den här artikeln. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</p> <p>Viktigt! Källfilen måste vara i HTML- eller ZIP-format. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON]</td> 
   <td> <p>Om HTML refererar till JavaScript-variabler kan du ta med dessa variabler här. </p> <p>För varje variabel klickar du på <strong>[!UICONTROL Add item]</strong> och innehåller variabelns nyckel och värde.</p> <p>Obs!   
     <ul> 
      <li> <p>När du skapar ett PDF från en ZIP-fil måste källmaterialet innehålla ett skriptelement som: <code> &lt;script src='./json.js' type='text/javascript'&gt;&lt;/script&gt;</code> </p> </li> 
      <li> <p>När du skapar ett PDF från en URL, injiceras innehållet i det här JSON-objektet i den virtuella webbläsaren innan sidan återges. </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include header and footer]</td> 
   <td> <p>Aktivera det här alternativet om du vill skapa sidhuvuden och sidfötter för PDF-dokumentet.</p> 
    <ul> 
     <li> <p>Rubriken innehåller ett datum och dokumenttiteln.</p> </li> 
     <li> <p>Sidfoten innehåller filnamnet och ett sidnummer.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Page width]</td> 
   <td>Ange papperets bredd i tum. I modulen används den här informationen för att formatera sidorna i den skapade PDF-filen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Page height]</td> 
   <td>Ange papperets höjd i tum. I modulen används den här informationen för att formatera sidorna i den skapade PDF-filen.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convert image to PDF file]

Med det här verktyget kan du konvertera en bild till en PDF-fil.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Markera anslutningen som ska användas för den här modulen.</p> Instruktioner om hur du skapar en anslutning till [!DNL Adobe PDF Services], se <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe PDF Services]</a> i den här artikeln. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och bildfil.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convert PDF to document]

Det här verktyget konverterar en PDF-fil till ett dokument. Du kan välja något av följande format för utdatafilen.

* DOC
* DOCX
* PPTX
* XSX
* RTF

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Markera anslutningen som ska användas för den här modulen.</p> Instruktioner om hur du skapar en anslutning till [!DNL Adobe PDF Services], se <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe PDF Services]</a> i den här artikeln. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</p> <p>Källfilen måste vara i PDF-format. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Files Format]</td> 
   <td> <p>Välj det format som du vill att filerna ska skrivas ut som:</p> 
    <ul> 
     <li> <p>DOC</p> </li> 
     <li> <p>DOCX</p> </li> 
     <li> <p>PPTX</p> </li> 
     <li> <p>XSX</p> </li> 
     <li> <p>RTF</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convert PDF to image]

Det här verktyget konverterar en PDF till en bild i PNG- eller JPEG-format, som sedan skrivs ut som en ZIP-fil. PDF konverteras till en bild per sida och varje bild avslutas med sidnumret. Bildfilerna kombineras sedan till en ZIP-fil.

En fil med namnet&quot;TestFile&quot; med 8 sidor ger till exempel 8 bilder med namnet&quot;TestFile_1&quot; till&quot;TestFile_8&quot;. Modulens utdata är en ZIP-fil som innehåller de 8 bilderna.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Markera anslutningen som ska användas för den här modulen.</p> Instruktioner om hur du skapar en anslutning till [!DNL Adobe PDF Services], se <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe PDF Services]</a> i den här artikeln. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</p> <p>Källfilen måste vara i PDF-format. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Files Format]</td> 
   <td> <p>Välj det format som du vill att filerna ska skrivas ut som:</p> 
    <ul> 
     <li>PNG</li> 
     <li>JPEG</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Linearize a PDF file]

Med det här verktyget linjäriserar du ett PDF-dokument och skapar ett webboptimerat PDF-dokument. Ett linjärt PDF-dokument kan visas sida vid sida utan att hela dokumentet behöver hämtas.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Markera anslutningen som ska användas för den här modulen.</p> Instruktioner om hur du skapar en anslutning till [!DNL Adobe PDF Services], se <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe PDF Services]</a> i den här artikeln. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL OCR for PDF file]

Det här verktyget utför optisk teckenigenkänning (OCR) på en fil och skapar en PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Markera anslutningen som ska användas för den här modulen.</p> Instruktioner om hur du skapar en anslutning till [!DNL Adobe PDF Services], se <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe PDF Services]</a> i den här artikeln. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL OCR type]</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Modified original image] text ser till att texten är sökbar och markeringsbar, men ändrar den ursprungliga bilden under rensningsprocessen (till exempel skevar den) innan ett osynligt textlager placeras över den. Den här typen tar bort oönskade artefakter och kan i vissa fall leda till ett mer läsbart dokument. </p> </li> 
     <li> <p>[!UICONTROL Unchanged original image] text lägger också över ett sökbart textlager över originalbilden, men i det här fallet ändras inte originalbilden. Den här typen ger maximal återgivning av originalbilden.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Language]</td> 
   <td>Välj språk för det här dokumentet.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Page manipulation]

I den här modulen kan du välja mellan att rotera eller ta bort sidor i ett PDF-dokument. Du kan till exempel ändra stående till liggande eller ta bort vissa sidor från dokumentet PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Markera anslutningen som ska användas för den här modulen.</p> Instruktioner om hur du skapar en anslutning till [!DNL Adobe PDF Services], se <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe PDF Services]</a> i den här artikeln. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td> <p>Välj den åtgärd som du vill utföra på filen.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Delete]</b> </p> <p>Välj det här alternativet om du vill ta bort sidor från dokumentet.</p> </li> 
     <li> <p><b>[!UICONTROL Rotate]</b> </p> <p>Välj det här alternativet om du vill rotera sidor och sedan ange vinkeln, i grader medsols, som du vill rotera dokumentsidorna i förhållande till deras startorientering.</p> <p>Rotera sidan 90 eller 270 grader om du vill rotera från stående till liggande eller tvärtom.</p> <p>Om en sida är upp och ned roterar du den 180 grader.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pages]</td> 
   <td> <p>För varje sidintervall som du vill ta bort klickar du på <strong>[!UICONTROL Add]</strong> och ange sedan sidintervallets första och sista sida. </p> <p>Obs!   
     <ul> 
      <li> <p>Du kan använda negativa tal för att räkna tillbaka från slutet av dokumentet. Den sista sidan i ett dokument är -1, den andra till den sista sidan är -2 och så vidare.</p> </li> 
      <li> <p>Om du vill ta bort en enstaka sida anger du samma sidnummer som både början och slutet av intervallet.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ange eller mappa det maximala antal poster som du vill att modulen ska arbeta med under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDF accessibility auto-tag]

Den här åtgärdsmodulen skapar ett PDF som är taggat för att skapa hjälpmedelsfall. Den skapar också en valfri Microsoft Excel-rapport med felmeddelanden och förslag på korrigeringar.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Markera anslutningen som ska användas för den här modulen.</p> Instruktioner om hur du skapar en anslutning till [!DNL Adobe PDF Services], se <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe PDF Services]</a> i den här artikeln. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Shift Headings]</td> 
   <td> <p>Aktivera det här alternativet om du vill flytta rubriker i dokumentet.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Generate Report]</b> </p> <p>Aktivera det här alternativet om du vill generera en rapport som listar tillgänglighetsproblem i PDF tillsammans med deras plats, och ger förslag på hur du kan åtgärda dessa problem.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDF file properties]

Det här verktyget extraherar grundläggande information om dokumentet, till exempel:

* Antal sidor
* PDF version
* Om filen är krypterad
* Om filen är linjär
* Om filen innehåller inbäddade filer

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Markera anslutningen som ska användas för den här modulen.</p> Instruktioner om hur du skapar en anslutning till [!DNL Adobe PDF Services], se <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe PDF Services]</a> i den här artikeln. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Protect PDF file]

Det här verktyget skyddar ett PDF-dokument med ett användar- eller ägarlösenord. Den anger även begränsningar för vissa funktioner som utskrift, redigering och kopiering i PDF-dokumentet. Du väljer vilken typ av innehåll som ska krypteras och krypteringsalgoritmen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Markera anslutningen som ska användas för den här modulen.</p> Instruktioner om hur du skapar en anslutning till [!DNL Adobe PDF Services], se <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe PDF Services]</a> i den här artikeln. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</p> <p>Källfilen måste vara i PDF-format. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Password Protection Type]</td> 
   <td> <p>Aktivera det här alternativet om du vill använda lösenord för att kryptera det inmatade PDF-dokumentet. Om du aktiverar det här alternativet måste du ange och ange ett värde för ett eller båda av följande: </p> 
    <ul> 
     <li> <p>[!UICONTROL userPassword]</p> </li> 
     <li> <p>[!UICONTROL ownerPassword] </p> </li> 
    </ul> <p>Lösenordet kan innehålla upp till 128 tecken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encryption Algorithm]</td> 
   <td> <p>Välj krypteringsalgoritm. </p> 
    <ul> 
     <li> <p>[!UICONTROL AES-128 encryption]</p> <p>Lösenordet stöder endast LATIN-I-tecken. </p> </li> 
     <li> <p>[!UICONTROL AES-256 encryption]</p> <p>Lösenordet stöder Unicode-teckenuppsättningen</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content to Encrypt]</td> 
   <td> <p>Välj vilken typ av innehåll som ska krypteras.</p> 
    <ul> 
     <li> <p>[!UICONTROL All content]</p> </li> 
     <li> <p>[!UICONTROL All content except metadata]</p> </li> 
     <li> <p>[!UICONTROL Only embedded data] </p> </li> 
    </ul> <p>Markera[!UICONTROL Only embedded data]"ger alla angivna åtkomstbehörigheter ogiltiga.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Permissions]</td> 
   <td> <p>Välj de behörigheter du vill inkludera för utskrift, redigering eller kopiering av innehåll.</p> <p>Behörighetsinställningar används bara om [!UICONTROL ownerPassword] är inställd i [!UICONTROL Password Protection Type] fält.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Remove protection of a PDF file]

Det här verktyget tar bort skydd (lösenord) från ett PDF-dokument.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Markera anslutningen som ska användas för den här modulen.</p> Instruktioner om hur du skapar en anslutning till [!DNL Adobe PDF Services], se <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe PDF Services]</a> i den här artikeln. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</p> <p>Källfilen måste vara i PDF-format.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Password]</td> 
   <td>Ange lösenordet som skyddar filen.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Split a PDF file]

Den här åtgärdsmodulen delar upp ett PDF-dokument i flera mindre dokument. Du anger om du vill dela upp den efter antal filer, sidor per fil eller sidintervall.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Markera anslutningen som ska användas för den här modulen.</p> Instruktioner om hur du skapar en anslutning till [!DNL Adobe PDF Services], se <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe PDF Services]</a> i den här artikeln. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</p> <p>Källfilen måste vara i PDF-format.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split option]</td> 
   <td>Välj hur du vill dela filen. 
   <ul>
   <li><p><b>Sidintervall</b></p><p>För varje sidintervall som du vill dela upp i ett separat dokument klickar du på <b>Lägg till</b> och ange den sida där du vill börja och den sida där du vill avsluta.</p></li>
   <li><p><b>Antal sidor</b></p><p>Ange antalet sidor som du vill inkludera i de nya dokumenten.</p></li>
   <li><p><b>Antal filer</b></p><p>Ange antalet filer i samma storlek som du vill dela dokumentet i.</p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>


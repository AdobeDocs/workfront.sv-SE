---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: apps-and-their-modules
title: Microsoft Office 365-e-post
description: I en [!DNL Adobe Workfront Fusion] kan du automatisera arbetsflöden som använder e-post i Microsoft Office 365 samt ansluta det till flera tredjepartsprogram och -tjänster.
author: Becky
feature: Workfront Fusion
exl-id: 29b69e8c-a889-441e-a052-287f1db2052d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1460'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Email]

I en [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder [!UICONTROL Microsoft Office 365 Email], samt ansluta till flera tredjepartsprogram och -tjänster.

För att kunna använda [!UICONTROL Office 365 Email] med [!DNL Adobe Workfront Fusion]måste du ha en [!UICONTROL Office 365 account]. Du kan skapa en på www.office.com.

Instruktioner om hur du ansluter [!UICONTROL Office 365] konto till [!DNL Workfront Fusion], se [Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner](../../workfront-fusion/connections/connect-to-fusion-general.md)

När du har gett ditt samtycke omdirigeras du tillbaka till [!UICONTROL Workfront Fusion] administrationssida där du kan fortsätta att skapa ditt scenario.

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

Används [!DNL Microsoft Office 365 Email] moduler, du måste ha en [!DNL Microsoft Office 365 Email] konto.

## [!DNL Microsoft Office 365 Email] moduler och deras fält

När du konfigurerar [!DNL Microsoft Office 365 Email] moduler, [!DNL Workfront Fusion] visar fälten som listas nedan. Tillsammans med dessa finns ytterligare [!DNL Microsoft Office 365 Email] fält kan visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Meddelande](#message)
* [Utkastmeddelande](#draft-message)
* [Bifogad fil](#attachment)
* [Övriga](#other)

### Meddelande

* [[!UICONTROL Watch Messages]](#watch-messages)
* [[!UICONTROL Search messages]](#search-messages)
* [[!UICONTROL Get a message]](#get-a-message)
* [[!UICONTROL Create and Send a Message]](#create-and-send-a-message)
* [[!UICONTROL Move a Message]](#move-a-message)
* [[!UICONTROL Delete a Message]](#delete-a-message)

#### [!UICONTROL Watch Messages]

Utlöses när ett nytt e-postmeddelande skickas eller tas emot.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Office 365] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Watch Messages]</p> </td> 
   <td> <p>Markera de meddelanden som du vill bevaka:</p> 
    <ul> 
     <li>[!UICONTROL Only Unread]</li> 
     <li>[!UICONTROL Only read]</li> 
     <li>[!UICONTROL All]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mail Folder]</td> 
   <td> <p>Markera den mapp som innehåller de meddelanden som du vill bevaka.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>Ange din sökfråga. Mer information om hur du skriver en sökfråga finns i [!DNL Microsoft] supportartikel <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">Sök efter e-post och personer i [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Ange maximalt antal meddelanden [!DNL Workfront Fusion] ska returneras under en körningscykel.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Search messages]

Söker efter meddelanden baserat på specifika kriterier.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Office 365] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mail Folder]</td> 
   <td> <p>Markera mappen som innehåller de meddelanden som du vill söka i.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>Ange din sökfråga. Mer information om hur du skriver en sökfråga finns i [!DNL Microsoft] supportartikel <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">Sök efter e-post och personer i [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
   <td> <p>Välj hur du vill ordna resultaten:</p> 
    <ul> 
     <li>[!UICONTROL Subject (Ascending or descending)]</li> 
     <li>[!UICONTROL Created Date Time (Ascending or descending)]</li> 
     <li>[!UICONTROL Last Modified Date Time (Ascending or descending)]</li> 
     <li>[!UICONTROL Received Date Time (Ascending or descending)]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ange maximalt antal meddelanden [!DNL Workfront Fusion] ska returneras under en körningscykel.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a message]

Hämtar metadata för ett visst meddelande

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Office 365] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Markera eller mappa ID:t för meddelandet som du vill hämta metadata för.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Get MIME contents]</td> 
   <td>Aktivera det här alternativet om du vill hämta data om MIME-innehållet i meddelandet. [!UICONTROL MIME] kan innehålla bilder, ljud, video eller andra typer av filer.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create and Send a Message]

Skapar och skickar ett e-postmeddelande.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Office 365] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Ange eller mappa ämnesraden för meddelandet.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Body Content Type]</td> 
   <td>Ange om meddelandets brödtext är HTML eller Text.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content]</td> 
   <td> <p>Ange eller mappa meddelandetexten i e-postmeddelandet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Välj e-postmeddelandets betydelse</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL To Recipients]</p> </td> 
   <td> <p>Lägg till den e-postadress som du vill skicka meddelandena till:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Ange kontaktens namn</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Ange kontaktens e-postadress.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Lägg till de mottagare som du vill ska få en kopia av meddelandet:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Ange kontaktens namn</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Ange kontaktens e-postadress.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Bcc Recipients]</p> </td> 
   <td> <p>Lägg till de mottagare som du vill kopiera i meddelandet, utan att tillåta andra mottagare att se sina namn eller e-postadresser:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Ange kontaktens namn</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Ange kontaktens e-postadress.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>Lägg till de bifogade filerna i e-postmeddelandet:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>Ange filnamnet. Exempel: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Ange fildata i fältet eller mappa filens källa.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Internet Message Headers]</td> 
   <td> <p>Lägg till meddelanderubriker för e-postmeddelandet.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Ange namnet på rubriken</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Ange ett värde för rubriken.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Move a Message]

Flyttar ett e-postmeddelande till en markerad mapp i postlådan.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Office 365] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Markera eller mappa ID:t för meddelandet som du vill flytta till en annan mapp.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mail Folder] </td> 
   <td> <p>Markera eller mappa ID:t för mappen där du vill flytta meddelandet.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a Message]

Tar bort ett befintligt e-postmeddelande.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Office 365] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Markera eller mappa ID:t för meddelandet som du vill ta bort.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Utkastmeddelande

* [Skapa ett utkast](#create-a-draft-message)
* [Skicka ett utkast](#send-a-draft-message)
* [Uppdatera ett meddelande](#update-a-message)

#### [!UICONTROL Create a Draft Message]

Skapar ett nytt e-postmeddelande.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Office 365] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Ange ämnesraden för meddelandet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body Content Type]</td> 
   <td>Ange om meddelandets brödtext är HTML eller Text.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content]</td> 
   <td> <p>Ange meddelandetexten i e-postmeddelandet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Välj e-postmeddelandets betydelse</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL To Recipients]</p> </td> 
   <td> <p>Lägg till mottagarna som du vill skicka meddelandena till:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Ange kontaktens namn</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Ange kontaktens e-postadress.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Lägg till mottagarna Du vill få en kopia av meddelandet:</p> 
    <ul> 
     <li> <p><strong>Namn</strong> </p> <p>Ange kontaktens namn</p> </li> 
     <li> <p><strong>E-postadress</strong> </p> <p>Ange kontaktens e-postadress.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Hemlig kopia-mottagare</p> </td> 
   <td> <p>Lägg till de mottagare som du vill kopiera i meddelandet, utan att tillåta andra mottagare att se sina namn eller e-postadresser:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Ange kontaktens namn</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Ange kontaktens e-postadress.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>Lägg till de bifogade filerna i e-postmeddelandet:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>Ange filnamnet. Exempel: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Ange fildata i fältet eller mappa filens källa.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Send a Draft Message]

Skickar ett e-postmeddelande som är i utkast.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Office 365] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Draft Message ID]</td> 
   <td> <p> Markera eller mappa meddelande-ID:t för utkastet som du vill skicka.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update a Message]

Uppdaterar ett befintligt meddelande.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Office 365] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a message ID]</td> 
   <td> <p>Välj hur du vill identifiera meddelandet som ska uppdateras:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter Manually]</strong> </p> <p>Ange eller mappa meddelande-ID:t.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Markera mappen som innehåller meddelandet som du vill uppdatera och markera sedan meddelandet</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Ange ämnesraden för meddelandet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content]</td> 
   <td> <p>Ange meddelandetexten i e-postmeddelandet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Välj e-postmeddelandets betydelse</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL To Recipients]</p> </td> 
   <td> <p>Lägg till den e-postadress som du vill skicka meddelandena till:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Ange kontaktens namn</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Ange kontaktens e-postadress.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Lägg till mottagarna Du vill få en kopia av meddelandet:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Ange kontaktens namn</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Ange kontaktens e-postadress.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Bcc Recipients]</p> </td> 
   <td> <p>Lägg till de mottagare som du vill kopiera i meddelandet, utan att tillåta andra mottagare att se sina namn eller e-postadresser:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Ange kontaktens namn</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Ange kontaktens e-postadress.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>Lägg till de bifogade filerna i e-postmeddelandet:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>Ange filnamnet. Exempel: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Ange fildata i fältet eller mappa filens källa.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mark it as Read]</td> 
   <td>Aktivera det här alternativet om du vill markera det uppdaterade meddelandet som läst.</td> 
  </tr> 
 </tbody> 
</table>

### Bifogad fil

* [[!UICONTROL List Attachments]](#list-attachments)
* [[!UICONTROL Download an Attachment]](#download-an-attachment)

#### [!UICONTROL List Attachments]

Den här modulen hämtar en lista med bilagor som tillhör det angivna meddelandet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Office 365] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Markera eller mappa ID:t för meddelandet som du vill hämta bilagor från.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ange eller mappa det maximala antalet bilagor som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Download an Attachment]

Den här modulen hämtar den angivna bifogade filen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Office 365] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Markera eller mappa ID:t för meddelandet som innehåller den bifogade filen som du vill hämta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Attachment ID]</td> 
   <td> <p>Ange eller mappa ID:t för den bifogade fil som du vill hämta.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Övriga

* [[!UICONTROL Make an API Call]](#make-an-api-call)
* [[!UICONTROL Add an Attachment]](#add-an-attachment)

#### [!UICONTROL Make an API Call]

Med den här modulen kan du utföra ett anpassat API-anrop.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Office 365] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Ange en sökväg som är relativ till <code>https://graph.microsoft.com</code>. Exempel:<code> /v1.0/me/messages</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   td&gt; <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-förfrågningsmetoder i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Lägg till rubrikerna för begäran i form av ett standard-JSON-objekt.Till exempel <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] lägger till auktoriseringsrubrikerna åt dig.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Lägg till frågan för API-anropet i form av ett standard-JSON-objekt.</p> </td> 
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

#### [!UICONTROL Add an Attachment]

Den här modulen lägger till en stor bifogad fil i ett meddelande.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Office 365] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Markera eller mappa ID:t för meddelandet som du vill lägga till en bifogad fil i.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Välj en fil från en tidigare modul eller mappa källfilens namn och data.</p> </td> 
  </tr> 
 </tbody> 
</table>

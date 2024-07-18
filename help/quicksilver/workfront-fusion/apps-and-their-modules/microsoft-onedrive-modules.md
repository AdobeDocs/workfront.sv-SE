---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: koppling
navigation-topic: apps-and-their-modules
title: Microsoft OneDrive-moduler
description: I ett [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder OneDrive samt ansluta det till flera tredjepartsprogram och -tjänster.
author: Becky
feature: Workfront Fusion
exl-id: 13a25c6c-bdf1-467d-bd90-ebd763c59235
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '3263'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive] moduler

I ett [!DNL Adobe Workfront Fusion]-scenario kan du automatisera arbetsflöden som använder [!DNL OneDrive] samt ansluta det till flera tredjepartsprogram och -tjänster.

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
   <p>Aktuellt licenskrav: Inget [!DNL Workfront Fusion]-licenskrav.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för Automatisering och integrering av arbetet] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuellt produktkrav: Om du har planen [!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Adobe Workfront] måste din organisation köpa både [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln. [!DNL Workfront Fusion] ingår i planen [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>eller</p>
   <p>Äldre produktkrav: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Förutsättningar

Du måste ha ett [!DNL Microsoft OneDrive]-konto för att kunna använda [!DNL OneDrive]-moduler.




## Ansluter tjänsten [!DNL OneDrive] till [!DNL Workfront Fusion]

Instruktioner om hur du ansluter ditt [!DNL OneDrive]-konto till [!UICONTROL Workfront Fusion] finns i [Skapa en anslutning till [!UICONTROL Adobe Workfront Fusion] - grundläggande instruktioner](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Vissa Microsoft-program använder samma anslutning, som är kopplad till individuella användarbehörigheter. När du skapar en anslutning visas därför alla behörigheter som tidigare har beviljats användarens anslutning, förutom de nya behörigheter som krävs för det aktuella programmet.
>
>Om en användare till exempel har behörighet att läsa tabell som beviljats via Excel-anslutningen och sedan skapar en anslutning i Outlook-anslutningen för att läsa e-post, visar tillståndsskärmen både den behörighet som redan har beviljats för att läsa tabell och den behörighet som nyligen har krävts för att skriva e-post.

## [!DNL Microsoft OneDrive]-moduler och deras fält

När du konfigurerar [!DNL OneDrive] moduler visar [!DNL Workfront Fusion] fälten som listas nedan. Dessutom kan ytterligare [!DNL OneDrive] fält visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Fil/mapp](#filefolder)
* [Övriga](#other)

### Fil/mapp

* [[!UICONTROL Watch Files/Folders]](#watch-filesfolders)
* [[!UICONTROL Search Files/Folders]](#search-filesfolders)
* [[!UICONTROL Get a file]](#get-a-file)
* [[!UICONTROL Download a file]](#download-a-file)
* [[!UICONTROL Upload a file]](#upload-a-file)
* [[!UICONTROL Create a Folder]](#create-a-folder)
* [[!UICONTROL Get a Share Link]](#get-a-share-link)
* [[!UICONTROL Move a File/Folder]](#move-a-filefolder)
* [[!UICONTROL Copy a File]](#copy-a-file)
* [[!UICONTROL Delete a File/Folder]](#delete-a-filefolder)

#### [!UICONTROL Watch Files/Folders]

Den här utlösarmodulen startar ett scenario när en fil eller mapp skapas eller uppdateras.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Instruktioner om hur du ansluter ditt [!DNL OneDrive]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch Files/Folders]</td> 
   <td> <p>Välj hur du vill bevaka filer och mappar:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL By Created Time]</b> </p> <p>Leta efter nya filer eller mappar.</p> </li> 
     <li> <p><b>[!UICONTROL By Updated Time]</b> </p> <p>Håll utkik efter uppdaterade befintliga filer eller mappar.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose your [!DNL OneDrive] plats]</td> 
   <td> <p>Välj den plats som du vill bevaka:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Välj om modulen ska aktiveras för att ange ett enhets-ID.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>Ange ID:t för den enhet som du vill att modulen ska bevaka.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> <p>Navigera till mappen som du vill att modulen ska bevaka. Du kan också ange en fråga för att filtrera de returnerade resultaten.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Shared With Me]</b> </p> <p>Modulen bevakar filer som har delats med enhetens ägare.</p> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Markera den SharePoint-webbplats som du vill att modulen ska titta på. Tillgängliga platser är platser följt av den inloggade användaren.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Markera den grupp vars enhet du vill att modulen ska bevaka.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose an Item Type]</td> 
   <td> <p>Välj om du vill bevaka filer, mappar eller båda.</p> <p>Obs! Du kan inte bevaka mappar i en [!UICONTROL Shared With Me]-enhet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>



#### [!UICONTROL Search Files/Folders]

Den här sökmodulen returnerar filer och mappar baserat på de villkor du anger.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Instruktioner om hur du ansluter ditt [!DNL OneDrive]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose your [!DNL OneDrive] plats]</td> 
   <td> <p>Välj den plats som du vill söka efter:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Välj om modulen ska aktiveras för att ange ett enhets-ID.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>Ange ID:t för den enhet som du vill att modulen ska söka efter.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> <p>Navigera till mappen som du vill att modulen ska söka i. Du kan också ange en fråga för att filtrera de returnerade resultaten.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Shared With Me]</b> </p> <p>Modulen söker efter filer som har delats med enhetens ägare.</p> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Välj den [!DNL SharePoint]-plats som du vill att modulen ska söka i. Tillgängliga platser är platser följt av den inloggade användaren.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Markera gruppen vars enhet du vill att modulen ska söka i.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose an Item Type]</td> 
   <td> <p>Välj om du vill söka efter filer, mappar eller både och.</p> <p>Obs! Du kan inte söka efter mappar i en [!UICONTROL Shared With Me]-enhet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a file]

Den här åtgärdsmodulen hämtar metadata för en angiven fil.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Instruktioner om hur du ansluter ditt [!DNL OneDrive]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter (File ID & File Path)]</td> 
   <td>Välj om du vill identifiera filen med fil-ID eller filsökväg.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a File ID] / [!UICONTROL File Path]</td> 
   <td> <p>Välj hur du vill ange fil-ID eller filsökväg:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Enter Manually]</b> </p> <p>Välj det här alternativet om du vill ange ID:t eller sökvägen direkt, eller mappa det från en tidigare modul.</p> </li> 
     <li> <p><b>[!UICONTROL Select from a list]</b> </p> <p>Välj det här alternativet om du vill välja i en lista över tillgängliga filer eller sökvägar. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose your [!DNL OneDrive] plats]</td> 
   <td> <p>Välj den plats som du vill söka efter:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Välj om modulen ska aktiveras för att ange ett enhets-ID.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>Ange ID:t för den enhet som innehåller filen som du vill hämta.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Markera den SharePoint-webbplats som innehåller filen som du vill hämta. Tillgängliga platser är platser följt av den inloggade användaren.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Markera gruppen vars enhet innehåller filen som du vill hämta.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Markera eller mappa den enhet som innehåller filen som du vill hämta. Det här fältet är inte tillgängligt om du har markerat [!UICONTROL No] i fältet [!UICONTROL Enable to Enter a Drive ID].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td> 
   <td> <p>Om du har markerat [!UICONTROL Enter Manually] anger eller mappar du fil-ID:t eller sökvägen till filen som du vill hämta.</p> <p>Om du har markerat [!UICONTROL Select from the list] markerar du filen som du vill hämta.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Download a file]

Den här åtgärdsmodulen hämtar den angivna filen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Instruktioner om hur du ansluter ditt [!DNL OneDrive]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter (File ID & File Path)]</td> 
   <td>Välj om du vill identifiera filen med fil-ID eller filsökväg.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ange ett fil-ID/Filsökväg</td> 
   <td> <p>Välj hur du vill ange fil-ID eller filsökväg:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Enter Manually]</b> </p> <p>Välj det här alternativet om du vill ange ID:t eller sökvägen direkt, eller mappa det från en tidigare modul.</p> </li> 
     <li> <p><b>[!UICONTROL Select from a list]</b> </p> <p>Välj det här alternativet om du vill välja i en lista över tillgängliga filer eller sökvägar. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose your [!DNL OneDrive] plats]</td> 
   <td> <p>Välj den plats som innehåller filen som du vill hämta:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Välj om modulen ska aktiveras för att ange ett enhets-ID.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>Ange ID:t för den enhet som innehåller filen som du vill hämta.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Markera den SharePoint-webbplats som innehåller filen som du vill hämta. Tillgängliga platser är platser följt av den inloggade användaren.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Markera gruppen vars enhet innehåller filen som du vill hämta.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Markera eller mappa enheten som innehåller filen som du vill hämta. Det här fältet är inte tillgängligt om du har markerat [!UICONTROL No] i fältet [!UICONTROL Enable to Enter a Drive ID].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td>
   <td> <p>Om du valde [!UICONTROL Enter Manually] anger eller mappar du fil-ID:t eller sökvägen till filen som du vill hämta.</p> <p>Om du valde [!UICONTROL Select from the list] markerar du filen som du vill hämta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Convert to PDF]</td> 
   <td> <p>Aktivera det här alternativet om du vill konvertera filen till en PDF-fil. Du kan konvertera från följande filtyper:</p> 
    <table style="table-layout:auto"> 
     <col> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td> 
        <ul> 
         <li> <p> <p>CSV</p> </p> </li> 
         <li> <p> <p>DOC</p> </p> </li> 
         <li> <p> <p>DOCX</p> </p> </li> 
         <li> <p> <p>ODP</p> </p> </li> 
         <li> <p> <p>ODS</p> </p> </li> 
         <li> <p> <p>ODT</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p> <p>POT</p> </p> </li> 
         <li> <p> <p>POTM</p> </p> </li> 
         <li> <p> <p>POTX</p> </p> </li> 
         <li> <p> <p>PPS</p> </p> </li> 
         <li> <p> <p>PPSX</p> </p> </li> 
         <li> <p> <p>PPSXM</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p>PPT</p> </li> 
         <li> <p>PPTM</p> </li> 
         <li> <p>PPTX</p> </li> 
         <li> <p>RTF</p> </li> 
         <li> <p>XLS</p> </li> 
         <li> <p>XSX</p> </li> 
        </ul> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Upload a file]

Den här åtgärdsmodulen överför en fil till den angivna mappen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Instruktioner om hur du ansluter ditt [!DNL OneDrive]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ange (mapplats-ID och -sökväg)</td> 
   <td>Välj om du vill identifiera målmappen med hjälp av ID eller en sökväg.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose your [!DNL OneDrive] plats]</td> 
   <td> <p>Välj den plats där du vill överföra en fil:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Välj om modulen ska aktiveras för att ange ett enhets-ID.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>Välj den enhet som innehåller filen som du vill hämta.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Välj den [!DNL SharePoint]-plats som innehåller mappen dit du vill överföra en fil. Tillgängliga platser är platser följt av den inloggade användaren.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Markera den grupp vars enhet innehåller mappen dit du vill överföra en fil.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Välj den enhet som innehåller mappen dit du vill överföra en fil. Det här fältet är inte tillgängligt om du har markerat [!UICONTROL No] i fältet [!UICONTROL Enable to Enter a Drive ID].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL If the File with the Same Name Exists]</td> 
   <td>Välj hur du vill fortsätta om det redan finns en fil med samma namn.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Lägg till en beskrivning till den överförda filen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create a Folder]

Den här åtgärdsmodulen skapar en ny mapp på den angivna enheten.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Instruktioner om hur du ansluter ditt [!DNL OneDrive]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose your [!DNL OneDrive] plats]</td> 
   <td> <p>Välj den plats där du vill skapa en mapp:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Välj om modulen ska aktiveras för att ange ett enhets-ID.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>Välj den enhet där du vill skapa en mapp.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Välj den [!DNL SharePoint]-plats där du vill skapa en mapp. Tillgängliga platser är platser följt av den inloggade användaren.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Markera gruppen som äger enheten där du vill skapa en mapp.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Välj den enhet där du vill skapa en mapp. Det här fältet är inte tillgängligt om du har markerat [!UICONTROL No] i fältet [!UICONTROL Enable to Enter a Drive ID].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Om du vill att den nya mappen ska vara en undermapp går du till den mapp där du vill att den ska vara en undermapp.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL New Folder Name]</td> 
   <td> <p>Ange eller mappa ett namn för den nya mappen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL If the Folder with the Same Name Exists]</td> 
   <td>Välj hur du vill fortsätta om det redan finns en fil med samma namn.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a Share Link]

Den här åtgärdsmodulen returnerar en delningslänk för den angivna filen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Instruktioner om hur du ansluter ditt [!DNL OneDrive]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter (File ID & File Path)]</td> 
   <td>Välj om du vill identifiera filen med fil-ID eller filsökväg.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a File ID] / [!UICONTROL File Path]</td> 
   <td> <p>Välj hur du vill ange fil-ID eller filsökväg:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Enter Manually]</b> </p> <p>Välj det här alternativet om du vill ange ID:t eller sökvägen direkt, eller mappa det från en tidigare modul.</p> </li> 
     <li> <p><b>[!UICONTROL Select from a list]</b> </p> <p>Välj det här alternativet om du vill välja i en lista över tillgängliga filer eller sökvägar. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose your [!DNL OneDrive] plats]</td> 
   <td> <p>Välj den plats där du vill hämta en delningslänk för:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Välj om modulen ska aktiveras för att ange ett enhets-ID.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>Ange ID:t för den enhet som innehåller filen som du vill hämta en delningslänk för.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Markera den SharePoint-webbplats som innehåller den fil som du vill hämta en delningslänk för. Tillgängliga platser är platser följt av den inloggade användaren.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Markera gruppen vars enhet innehåller filen som du vill hämta en delningslänk för.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Markera eller mappa enheten som innehåller filen som du vill hämta en delningslänk för. Det här fältet är inte tillgängligt om du har markerat [!UICONTROL No] i fältet [!UICONTROL Enable to Enter a Drive ID].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td> 
   <td> <p>Om du valde [!UICONTROL Enter Manually] anger eller mappar du fil-ID:t eller sökvägen för filen som du vill hämta en delningslänk för.</p> <p>Om du valde [!UICONTROL Select] i listan markerar du filen som du vill hämta en delningslänk för.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Permission Type]</td> 
   <td> <p>Välj om du vill att personer med länken ska kunna läsa och skriva till filen eller om de ska vara skrivskyddade.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scope]</td> 
   <td>Välj om du vill att filen ska vara tillgänglig för alla som har länken eller bara för medlemmar i organisationen som har länken.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Move a File/Folder]

Den här åtgärdsmodulen flyttar en fil eller mapp till en ny mapp

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Instruktioner om hur du ansluter ditt [!DNL OneDrive]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter (File ID & File Path)]</td> 
   <td>Välj om du vill identifiera filen med fil-ID eller filsökväg.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a File ID / File Path]</td> 
   <td> <p>Välj hur du vill ange fil-ID eller filsökväg:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Enter Manually]</b> </p> <p>Välj det här alternativet om du vill ange ID:t eller sökvägen direkt, eller mappa det från en tidigare modul.</p> </li> 
     <li> <p><b>[!UICONTROL Select from a list]</b> </p> <p>Välj det här alternativet om du vill välja i en lista över tillgängliga filer eller sökvägar. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose your [!DNL OneDrive] plats]</td> 
   <td> <p>Välj den plats som innehåller filen eller mappen som du vill flytta:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Välj om modulen ska aktiveras för att ange ett enhets-ID.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>Ange ID:t för den enhet som innehåller filen eller mappen som du vill flytta.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Markera platsen [!DNL SharePoint] som innehåller filen eller mappen som du vill flytta. Tillgängliga platser är platser följt av den inloggade användaren.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Markera gruppen vars enhet innehåller filen eller mappen som du vill flytta.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Markera eller mappa den enhet som innehåller filen eller mappen som du vill flytta. Det här fältet är inte tillgängligt om du har markerat [!UICONTROL No] i fältet [!UICONTROL Enable to Enter a Drive ID].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Välj [!UICONTROL File/Folder]</td> 
   <td>Välj om du vill flytta en fil eller en mapp.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</p> <p role="rowheader">[!UICONTROL Folder] / [!UICONTROL Folder ID] / [!UICONTROL Folder Path]</p> </td> 
   <td> <p>Om du markerade [!UICONTROL Enter Manually] anger eller mappar du ID:t eller sökvägen för filen eller mappen som du vill flytta.</p> <p>Om du markerade [!UICONTROL Select] i listan markerar du filen eller mappen som du vill flytta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a New Folder Location]</td> 
   <td> <p>Välj hur du vill ange platsen som du vill flytta filen eller mappen till:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Enter Manually]</b> </p> <p>Välj det här alternativet om du vill ange ID:t eller sökvägen direkt, eller mappa det från en tidigare modul.</p> </li> 
     <li> <p><b>[!UICONTROL Select from a list]</b> </p> <p>Välj det här alternativet om du vill välja i en lista över tillgängliga filer eller sökvägar. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose your [!DNL OneDrive] plats]</td> 
   <td> <p>Välj den plats där du vill flytta filen eller mappen:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Välj om modulen ska aktiveras för att ange ett enhets-ID.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>Ange ID:t för den enhet där du vill flytta filen eller mappen.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Välj den [!DNL SharePoint]-plats där du vill flytta filen eller mappen. Tillgängliga platser är platser följt av den inloggade användaren.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Markera gruppen som du vill flytta filen eller mappen till.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Markera eller mappa enheten som innehåller mappen som du vill flytta filen eller mappen till. Det här fältet är inte tillgängligt om du har markerat [!UICONTROL No] i fältet [!UICONTROL Enable to Enter a Drive ID].</p> <p>Om du lämnar detta tomt kan filen eller mappen bara flyttas inom samma [!DNL OneDrive].</p> <p>Du kan flytta filer och mappar från [!UICONTROL My Drive] till en [!UICONTROL Site's Drive] eller en [!UICONTROL Group's Drive]. </p> <p>Du kan bara flytta filer från en [!UICONTROL Site's Drive] till samma enhet på samma plats.</p> <p>Du kan bara flytta filer från en [!UICONTROL Group's Drive] till samma enhet i samma grupp.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Ange eller mappa den mapp där du vill flytta filen eller mappen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copy a File]

Den här åtgärdsmodulen kopierar en fil till en ny mapp

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Instruktioner om hur du ansluter ditt [!DNL OneDrive]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter (File ID & File Path)]</td> 
   <td>Välj om du vill identifiera filen med fil-ID eller filsökväg.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a File ID] / [!UICONTROL File Path]</td> 
   <td> <p>Välj hur du vill ange fil-ID eller filsökväg:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Enter Manually]</b> </p> <p>Välj det här alternativet om du vill ange ID:t eller sökvägen direkt, eller mappa det från en tidigare modul.</p> </li> 
     <li> <p><b>[!UICONTROL Select from a list]</b> </p> <p>Välj det här alternativet om du vill välja i en lista över tillgängliga filer eller sökvägar. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose your [!DNL OneDrive] plats]</td> 
   <td> <p>Välj den plats som innehåller filen som du vill kopiera:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Välj om modulen ska aktiveras för att ange ett enhets-ID.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>Ange ID:t för den enhet som innehåller filen eller mappen som du vill kopiera.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Markera den SharePoint-plats som innehåller filen som du vill flytta. Tillgängliga platser är platser följt av den inloggade användaren.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Markera gruppen vars enhet innehåller filen som du vill kopiera.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Markera eller mappa den enhet som innehåller filen som du vill kopiera. Det här fältet är inte tillgängligt om du har markerat [!UICONTROL No] i fältet [!UICONTROL Enable to Enter a Drive ID].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</p> </td> 
   <td> <p>Om du markerade [!UICONTROL Enter Manually] anger eller mappar du ID:t eller sökvägen för filen som du vill kopiera.</p> <p>Om du markerade [!UICONTROL Select] i listan markerar du filen som du vill kopiera.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a New Folder Location]</td> 
   <td> <p>Välj hur du vill ange platsen som du vill kopiera filen till:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Enter Manually]</b> </p> <p>Välj det här alternativet om du vill ange ID:t eller sökvägen direkt, eller mappa det från en tidigare modul.</p> </li> 
     <li> <p><b>[!UICONTROL Select from a list]</b> </p> <p>Välj det här alternativet om du vill välja i en lista över tillgängliga mappar. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL New OneDrive location]</td> 
   <td> <p>Välj den plats där du vill kopiera filhanteraren. Det här alternativet är tillgängligt om du väljer att välja den nya mapplatsen i en lista.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Välj om modulen ska aktiveras för att ange ett enhets-ID.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>Ange ID:t för den enhet där du vill kopiera filen.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Välj den [!DNL SharePoint]-plats där du vill kopiera filen. Tillgängliga platser är platser följt av den inloggade användaren.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Markera gruppen som du vill kopiera filen till.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Markera eller mappa enheten som innehåller mappen som du vill kopiera filen till. Det här fältet är inte tillgängligt om du har markerat [!UICONTROL No] i fältet [!UICONTROL Enable to Enter a Drive ID].</p> <p>Om du lämnar detta tomt kan filen eller mappen bara kopieras inom samma [!UICONTROL OneDrive].</p> <p>Du kan kopiera filer och mappar från [!UICONTROL My Drive] till en [!UICONTROL Site's Drive] eller en [!UICONTROL Group's Drive]. </p> <p>Du kan bara kopiera filer från en [!UICONTROL Site's Drive] till samma enhet på samma plats.</p> <p>Du kan bara kopiera filer från en [!UICONTROL Group's Drive] till samma enhet i samma grupp.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Ange eller mappa den mapp där du vill flytta kopian eller mappen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL New Copied File Name]</td> 
   <td> <p>Ange eller mappa ett namn för den nya kopian av filen. Du kan lämna detta tomt om du inte vill ändra det ursprungliga filnamnet.</p> <p>Namnet måste innehålla filtillägget. Exempel:<code> file.txt</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a File/Folder]

Den här åtgärdsmodulen tar bort den markerade filen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Instruktioner om hur du ansluter ditt [!DNL OneDrive]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter (File/Folder ID & Path)]</td> 
   <td>Välj om du vill identifiera filen med fil-ID eller filsökväg.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a File/Folder ID /Enter a File/Folder Path]</td> 
   <td> <p>Välj hur du vill ange fil-ID eller filsökväg:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Enter Manually]</b> </p> <p>Välj det här alternativet om du vill ange ID:t eller sökvägen direkt, eller mappa det från en tidigare modul.</p> </li> 
     <li> <p><b>[!UICONTROL Select from a list]</b> </p> <p>Välj det här alternativet om du vill välja i en lista över tillgängliga filer eller sökvägar. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose your [!DNL OneDrive] plats]</td> 
   <td> <p>Välj den plats som du vill söka efter:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Välj om modulen ska aktiveras för att ange ett enhets-ID.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>Ange ID:t för den enhet som innehåller filen eller mappen som du vill ta bort.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Markera platsen [!DNL SharePoint] som innehåller filen eller mappen som du vill ta bort. Tillgängliga platser är platser följt av den inloggade användaren.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Markera gruppen vars enhet innehåller filen eller mappen som du vill ta bort.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Markera eller mappa den enhet som innehåller filen eller mappen som du vill ta bort. Det här fältet är inte tillgängligt om du har markerat [!UICONTROL No] i fältet [!UICONTROL Enable to Enter a Drive ID].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Välj [!UICONTROL File/Folder]</td> 
   <td>Välj om du vill ta bort en fil eller en mapp.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td>
   <td> <p>Om du har markerat [!UICONTROL Enter Manually] anger eller mappar du fil-ID:t eller sökvägen till filen som du vill ta bort.</p> <p>Om du markerade [!UICONTROL Select] i listan markerar du filen som du vill ta bort.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Övriga

#### [!UICONTROL Make an API Call]

Denna modul utför ett anpassat API-anrop.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Instruktioner om hur du ansluter ditt [!DNL OneDrive]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Ange en relativ sökväg till <code>https://graph.microsoft.com</code>. Exempel:<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metoder för HTTP-begäran i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td> <p>Lägg till brödinnehållet för API-anropet i form av ett standard-JSON-objekt.</p> <p>Obs!  <p>När du använder villkorssatser som <code>if</code> i JSON placerar du citattecknen utanför villkorssatsen.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>



## Om du inte kan överföra eller uppdatera en fil

Det finns flera möjliga problem när det inte går att överföra eller uppdatera en fil:

* Den överförda filen är för stor och överskrider maxgränsen för filstorlek för din [!DNL OneDrive]-plan, eller så har du använt hela lagringskvoten för ditt [!DNL OneDrive]-konto. Om du vill ha mer lagringsutrymme tar du bort befintliga filer från [!DNL OneDrive] eller uppgraderar ditt [!DNL OneDrive]-konto.
* Det går inte att överföra två filer med samma namn till en enda mapp med OneDrive. Om målmappen innehåller en fil med samma namn som den fil som överförs avslutas scenariot med ett fel. Lösningen är att byta namn på filen som överförs. Om du vill uppdatera en fil använder du åtgärden [!UICONTROL Update a file].
* Den tidigare markerade mappen, som filen överförs till, finns inte längre. Scenariot stoppas och du måste välja målmappen igen.

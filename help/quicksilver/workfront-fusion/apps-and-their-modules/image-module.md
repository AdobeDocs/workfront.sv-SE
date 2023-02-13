---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Bildmoduler
description: Med Adobe Workfront Fusion Image-modulerna kan du hämta information om en viss bild (mått, typ o.s.v.), konvertera en bild till ett annat filformat och direkt ändra bildens storlek.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 89efa9d5-00c9-4bb5-97b3-2b2f9d73721d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 0%

---

# Bildmoduler

[!DNL Adobe Workfront Fusion] [!UICONTROL Image] Med -moduler kan du få information om en viss bild (dimensioner, typ o.s.v.), konvertera en bild till ett annat filformat och direkt ändra storlek på bilden.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p>  <p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Image] moduler och deras fält

När du konfigurerar den här modulen visas följande fält. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

* [[!UICONTROL Resize]](#resize)
* [[!UICONTROL Convert a format]](#convert-a-format)
* [[!UICONTROL Extract metadata]](#extract-metadata)

### [!UICONTROL Resize]

Den här transformerarmodulen ändrar en bilds höjd och bredd enligt de villkor du anger.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Välj källan till den bild som du vill konvertera. Du kan välja utdata från en tidigare modul eller mappa datafilen och filnamnet. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data]</td> 
   <td>Mappa filen som du vill konvertera. Det här fältet är tillgängligt om du har valt [!UICONTROL Map] i [!UICONTROL Source file] fält.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>Ange ett namn för den konverterade filen. Det här fältet är tillgängligt om du har valt [!UICONTROL Map] i [!UICONTROL Source file] fält.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL I want to]</td> 
   <td>Välj om du vill behålla förhållandet mellan höjd och bredd eller ändra dimensionerna till en angiven höjd och bredd.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL According to]</td> 
   <td> <p>Välj hur du vill att modulen ska avgöra bildens nya storlek. Det här fältet visas om du har valt att behålla förhållandet mellan höjd och bredd i fältet Jag vill. Andra fält visas baserat på valet i det här fältet.</p> 
    <ul> 
     <li> <p>[!UICONTROL Maximum width]</p> <p>Minskar en bild till en bredd som du anger. Höjden beräknas automatiskt.</p> </li> 
     <li> <p>[!UICONTROL Maximum height]</p> <p>Förminskar en bild till en höjd som du anger. Bredden beräknas automatiskt.</p> </li> 
     <li> <p>[!UICONTROL Maximum height or width]</p> <p>Minskar en bild så att dess höjd och bredd inte överskrider de värden du anger. Eftersom det här alternativet behåller förhållandet mellan höjd och bredd kan en av dimensionerna vara mindre än den angivna. Om till exempel både höjd och bredd anges som 40, kommer en bild på 400x300 att minskas till 40x30.</p> </li> 
     <li> <p>[!UICONTROL Minimum width]</p> <p>Förstorar en bild till en bredd som du anger. Höjden beräknas automatiskt.</p> </li> 
     <li> <p>[!UICONTROL Minimum height]</p> <p>Förstorar en bild till en höjd som du anger. Bredden beräknas automatiskt.</p> </li> 
     <li> <p>[!UICONTROL Minimum height or width]</p> <p>Förstorar en bild så att dess höjd och bredd inte är mindre än de värden du anger. Eftersom detta alternativ bevarar förhållandet mellan höjd och bredd kan en av dimensionerna vara större än angivet. Om till exempel både höjd och bredd anges som 300 förstoras en bild på 40x30 till 400x300.</p> </li> 
     <li> <p>[!UICONTROL Percent]</p> <p>Ändrar bildstorleken med ett procentvärde baserat på det värde du anger. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Width]</td> 
   <td>Ange eller mappa önskad bredd för den storleksändrade bilden i pixlar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Height]</td> 
   <td>Ange eller mappa den önskade höjden på den storleksändrade bilden i pixlar.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convert a format]

Den här transformatormodulen ändrar formatet för en bildfil. Den här modulen är kompatibel med följande format:

* PNG
* JPG
* GIF
* BMP

Både källfilen och utdata måste ha något av dessa format. Till exempel [!UICONTROL Image] >[!UICONTROL Convert a format] kan omvandla en PNG-fil till en BMP-fil eller en BMP till en JPG.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Välj källan till den bild som du vill konvertera. Du kan välja utdata från en tidigare modul eller mappa datafilen och filnamnet. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data]</td> 
   <td>Mappa filen som du vill konvertera. Det här fältet är tillgängligt om du har valt [!UICONTROL Map] i [!UICONTROL Source file] fält.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>Ange ett namn för den konverterade filen. Det här fältet är tillgängligt om du har valt [!UICONTROL Map] i [!UICONTROL Source file] fält.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output format]</td> 
   <td>Välj det format som du vill att modulen ska konvertera källfilen till. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Extract metadata]

Den här transformatormodulen returnerar grundläggande information om en modul.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Välj källan till den bild som du vill konvertera. Du kan välja utdata från en tidigare modul eller mappa datafilen och filnamnet. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data]</td> 
   <td>Mappa filen som du vill konvertera. Det här fältet är tillgängligt om du har valt Karta i [!UICONTROL Source file] fält.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>Ange ett namn för den konverterade filen. Det här fältet är tillgängligt om du har valt Karta i [!UICONTROL Source file] fält.</td> 
  </tr> 
 </tbody> 
</table>

## Möjliga problem

### Åtgärden avslutades med ett fel

Det finns tre fall då en åtgärd kan avslutas med ett fel:

* Mottagna data fanns inte i formatet JPG/GIF/PNG/BMP
* Gränsen för maximal bredd/höjd har överskridits när bildens dimensioner ändrades. Bildstorleken får inte överstiga bredden 3 840 px och höjden 2 160 px
* Den största tillåtna storleken för en bild har överskridits när bildens dimensioner eller format ändrades.

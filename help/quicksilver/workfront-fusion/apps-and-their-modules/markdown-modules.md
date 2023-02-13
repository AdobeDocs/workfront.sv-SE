---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Markeringsmoduler
description: I en [!DNL Adobe Workfront Fusion] kan du använda Markdown-modulerna för att konvertera Markdown till HTML och HTML till Markdown.
author: Becky
feature: Workfront Fusion
exl-id: 9e810302-4897-494a-9b50-667d87ce9cb7
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# [!UICONTROL Markdown] moduler

I en [!DNL Adobe Workfront Fusion] scenario kan du använda [!UICONTROL Markdown] för att konvertera Markdown till HTML och HTML till Markdown.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p>  <p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr>
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Markdown to HTML]

I den här modulen konverteras Markdown till HTML.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Markdown]</td> 
   <td> <p>Ange markeringsformaterad oformaterad text.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL GitHub Flavored Markdown] </td> 
   <td> <p>Aktivera det här alternativet om du vill konvertera GitHub Flavsted Markdown till HTML.</p> <p>Mer information finns i mars[!DNL ]nedåtkalkylblad i [!DNL GitHub] dokumentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sanitize]</td> 
   <td>Välj ett alternativ som anger om du vill ta bort HTML-taggar från texten eller Esc-HTML.</td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL HTML to Markdown]

Den här modulen konverterar HTML-kod till Markdown.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Markdown]</td> 
   <td> <p>Ange den HTML-kod som du vill konvertera till Markdown.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL GitHub Flavored Markdown] </td> 
   <td> <p>Aktivera det här alternativet för att konvertera HTML till [!DNL GitHub Flavored Markdown].</p> <p>Mer information finns i markeringsdatabladet i [!DNL GitHub] dokumentation.</p> </td> 
  </tr> 
 </tbody> 
</table>

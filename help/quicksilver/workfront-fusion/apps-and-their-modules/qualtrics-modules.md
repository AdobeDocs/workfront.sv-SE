---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: apps-and-their-modules
title: Qualtrics-moduler
description: I en [!DNL Adobe Workfront Fusion] kan du automatisera arbetsflöden som använder Qualtrics, samt ansluta det till flera tredjepartsprogram och -tjänster.
author: Becky
feature: Workfront Fusion
exl-id: 146802cd-b863-4c93-b767-50e05892c4de
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Qualtrics-moduler

I en [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder [!DNL Qualtrics], samt ansluta till flera tredjepartsprogram och -tjänster.

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

Används [!DNL Qualtrics] moduler, du måste ha en [!UICONTROL Qualtrics] konto.

## Ansluter [!DNL Qualtrics] till [!DNL Workfront Fusion]

Du kan skapa en anslutning till [!DNL Qualtrics] direkt inifrån [!UICONTROL Qualtrics] -modul.

1. I alla [!UICONTROL Qualtrics] modul, klicka på **[!UICONTROL Add]** bredvid [!UICONTROL Connection] fält.
1. Ange följande information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td> <p>Ange ett namn för den nya anslutningen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Data Center ID] </td> 
      <td>Använd formatet <code>&lt;Data Center ID>.qualtrics.com</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL API Key]</td> 
      <td>Information om hur du hittar API-nyckeln finns i <a href="https://api.qualtrics.com/instructions/docs/Instructions/api-key-authentication.md">API-tokenautentisering</a> i [!DNL Qualtrics] dokumentation.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **[!UICONTROL Continue]** för att skapa anslutningen och gå tillbaka till modulen.

## [!DNL Qualtrics] moduler och deras fält

Följande moduler är tillgängliga för [!DNL Qualtrics] koppling:

* [!UICONTROL Watch New Survey Response]
* [!UICONTROL Create a Directory Contact]
* [!UICONTROL Delete a Directory Contact]
* [!UICONTROL Get a Directory Contact]
* [!UICONTROL Update a Directory Contact]
* [!UICONTROL Create a New Survey Distribution via SMS]
* [!UICONTROL Distribute a Survey via Email]
* [!UICONTROL Make an API call]
* [!UICONTROL List Directory Contacts]

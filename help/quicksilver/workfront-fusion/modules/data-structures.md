---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Datastrukturer i [!DNL Adobe Workfront Fusion]
description: En datastruktur är ett dokument som i detalj beskriver formatet på de data som överförs till Adobe Workfront Fusion. Baserat på det här dokumentet kan scenarioredigeraren ta reda på vilken datatyp som returneras eller tas emot. Datastrukturdokumenten används oftast för serialisering/tolkning av dataformat som JSON, XML, CSV med flera.
author: Becky
feature: Workfront Fusion
exl-id: 35a7e906-7ca2-433d-87a9-bbb01babffb0
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Datastrukturer i [!DNL Adobe Workfront Fusion]

En datastruktur är ett dokument som i detalj beskriver formatet på de data som överförs till [!DNL Adobe Workfront Fusion]. Baserat på det här dokumentet kan scenarioredigeraren ta reda på vilken datatyp som returneras eller tas emot. Datastrukturdokumenten används oftast för serialisering/tolkning av dataformat som JSON, XML, CSV med flera.

Du kan skapa en datastruktur genom att klicka på [!UICONTROL Create a new data structure] i [!UICONTROL Data structure overview] eller i inställningarna för modulen som kräver datastruktursspecifikation.

Datatyper som stöds beskrivs i [[!UICONTROL Types of modules]](../../workfront-fusion/modules/module-types.md) artikel.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] eller högre</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licens**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Datastrukturgenerator

Datastrukturer behöver inte alltid skapas. Du kan göra det enklare genom att använda en mall från vår inbyggda generator. Genom att tillhandahålla ett dataexempel kommer generatorn automatiskt att skapa en datastruktur baserat på det dataexempel du har angett. Den datastruktur som skapas kan sedan ändras manuellt.

![](assets/data-structure-generator-350x341.jpg)

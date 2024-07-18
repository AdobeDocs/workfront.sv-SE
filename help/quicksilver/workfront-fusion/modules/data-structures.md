---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Datastrukturer i  [!DNL Adobe Workfront Fusion]
description: En datastruktur är ett dokument som i detalj beskriver formatet på de data som överförs till Adobe Workfront Fusion. Baserat på det här dokumentet kan scenarioredigeraren ta reda på vilken datatyp som returneras eller tas emot. Datastrukturdokumenten används oftast för serialisering/tolkning av dataformat som JSON, XML, CSV med flera.
author: Becky
feature: Workfront Fusion
exl-id: 35a7e906-7ca2-433d-87a9-bbb01babffb0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# Datastrukturer i [!DNL Adobe Workfront Fusion]

En datastruktur är ett dokument som i detalj beskriver formatet på de data som överförs till [!DNL Adobe Workfront Fusion]. Baserat på det här dokumentet kan scenarioredigeraren ta reda på vilken datatyp som returneras eller tas emot. Datastrukturdokumenten används oftast för serialisering/tolkning av dataformat som JSON, XML, CSV med flera.

Du kan skapa en datastruktur genom att klicka på knappen [!UICONTROL Create a new data structure] i avsnittet [!UICONTROL Data structure overview] eller i inställningarna för modulen som kräver en datastrukturspecifikation.

Datatyper som stöds beskrivs i artikeln [[!UICONTROL Types of modules]](../../workfront-fusion/modules/module-types.md).

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

## Datastrukturgenerator

Datastrukturer behöver inte alltid skapas. Du kan göra det enklare genom att använda en mall från vår inbyggda generator. Genom att tillhandahålla ett dataexempel kommer generatorn automatiskt att skapa en datastruktur baserat på det dataexempel du har angett. Den datastruktur som skapas kan sedan ändras manuellt.

![](assets/data-structure-generator-350x341.jpg)

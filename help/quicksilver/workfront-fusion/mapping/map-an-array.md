---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Mappa en array i [!DNL Adobe] Workfront Fusion
description: Du kan mappa en array till ett modulfält i Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# Mappa en matris i [!DNL Adobe Workfront Fusion]

En array är en speciell typ av objekt som kan innehålla följande:

* Ett eller flera textvärden (enkel array)
* En eller flera samlingar av samma typ (komplex array)

>[!INFO]
>
>**Exempel:** Modulen [!UICONTROL Watch emails] returnerar en array med bilagor för varje e-postmeddelande. Alla bilagor representerar en samling som kan innehålla namn, innehåll, storlek och så vidare.

Mer information finns i [Objektdatatyper i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

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

## Mappa en array

1. Klicka på knappen i målfältet.

   >[!INFO]
   >
   >  **Exempel:** I exemplet ovan klickar du på knappen [!UICONTROL Add an attachment] för ett e-postmeddelande.
   >
   >![](assets/add-an-attachment-button-350x152.jpg)

1. Ange objektet i rutan som visas.

   På panelen kan du mappa fält på samma sätt som andra typer av objekt. Om du inte vill fylla i varje objekt separat, men vill mappa en annan array till målfältet, använder du knappen [!UICONTROL Map]. I det här fallet måste du se till att båda arrayerna (källarrayen och målarrayen) har samma struktur.

   Du kan lägga till valfritt antal objekt i en array.

Du kan dela upp en array i enskilda paket med hjälp av en iterator. Mer information finns i modulen [[!UICONTROL Iterator] i  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

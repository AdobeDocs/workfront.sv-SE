---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Mappa en array i [!DNL Adobe] Workfront Fusion
description: Du kan mappa en array till ett modulfält i Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# Mappa en array i [!DNL Adobe Workfront Fusion]

En array är en speciell typ av objekt som kan innehålla följande:

* Ett eller flera textvärden (enkel array)
* En eller flera samlingar av samma typ (komplex array)

>[!INFO]
>
>**Exempel:** The [!UICONTROL Watch emails] returnerar en array med bilagor för varje e-post. Varje bifogad fil representerar en samling som kan innehålla namn, innehåll, storlek och så vidare.

Mer information finns i [Artikeldatatyper i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

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

## Mappa en array

1. Klicka på knappen i målfältet.

   >[!INFO]
   >
   >  **Exempel:** I exemplet ovan klickar du på [!UICONTROL Add an attachment] för ett e-postmeddelande.
   >
   >![](assets/add-an-attachment-button-350x152.jpg)

1. Ange objektet i rutan som visas.

   På panelen kan du mappa fält på samma sätt som andra typer av objekt. Om du inte vill fylla i varje objekt separat, men vill mappa en annan array till målfältet, använder du [!UICONTROL Map] -knappen. I det här fallet måste du se till att båda arrayerna (källarrayen och målarrayen) har samma struktur.

   Du kan lägga till valfritt antal objekt i en array.

Du kan dela upp en array i enskilda paket med hjälp av en iterator. Mer information finns i [[!UICONTROL Iterator] modulen i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

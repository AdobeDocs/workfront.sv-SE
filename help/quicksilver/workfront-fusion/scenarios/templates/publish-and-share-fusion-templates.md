---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Publish och dela [!DNL Adobe Workfront Fusion] mallar
description: När du skapar en mall blir mallen tillgänglig för alla dina teammedlemmar. Om du vill dela mallen med någon utanför ditt team måste du först publicera den.
author: Becky
feature: Workfront Fusion
exl-id: aaa59a1e-aa16-41f5-9f56-ce0615c1b685
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 0%

---

# Publish och dela [!DNL Adobe Workfront Fusion] mallar

När du skapar en mall blir mallen tillgänglig för alla dina teammedlemmar. Om du vill dela mallen med någon utanför ditt team måste du först publicera den.

Mer information om hur du skapar en mall finns i [Skapa nya mallar i Adobe Workfront Fusion](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

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
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för Automatisering och integrering av arbetet], [!UICONTROL [!DNL Workfront Fusion] för Automatisering av arbete]</p>
   </td>    </tr> 
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

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Förutsättningar

En mall måste skapas innan den kan delas.

## Publish och en [!DNL Adobe Workfront Fusion]-mall

1. Klicka på **[!UICONTROL Templates]** i den vänstra navigeringspanelen.
1. Klicka på fliken **[!UICONTROL Team templates]**.
1. Klicka på mallens namn.
1. Klicka på knappen **[!UICONTROL Publish]** i skärmens övre högra hörn.

## Dela en [!DNL Workfront Fusion]-mall

När du har publicerat en mall kan du dela den.

1. (Villkorligt) Om du vill ha en delbar länk klickar du på **[!UICONTROL Share public link]**.

   >[!NOTE]
   >
   >Du kan dela den här länken med vem du vill. Själva mallen finns kvar på fliken [!UICONTROL Team templates] och är inte offentlig.

1. (Villkorligt) Om du vill att mallen ska vara offentlig skickar du den till administratören för godkännande genom att klicka på **[!UICONTROL Request Approval]**.

   >[!NOTE]
   >
   >* När mallen har godkänts blir den offentlig. [!UICONTROL Public templates] visas på fliken [!UICONTROL Public templates] för alla [!DNL Workfront Fusion]-användare, oavsett organisation eller team.
   >* Din administratör har inte informerats om att han eller hon får mallen för granskning via e-post. Kontakta administratören direkt om godkännandet är brådskande.


## Mallstatus

Du kan kontrollera mallsidans status under mallnamnet

Följande statusar är tillgängliga:

* **[!UICONTROL Private]**: Den här mallen visas bara för mallskaparen och deras team.
* **[!UICONTROL Published]**: Den här mallen visas bara för mallskaparen och deras team. Du kan skicka publicerade mallar för godkännande och kopiera en delbar länk.
* **[!UICONTROL Approved]**: Den här mallen visas för alla Workfront Fusion-användare på fliken [!UICONTROL Public templates]. Du kan kopiera en delbar länk genom att klicka på [!UICONTROL Options] i skärmens övre högra hörn.

Du kan även kontrollera statusen på fliken [!UICONTROL Team templates]. Om en mall publiceras visas en ikon till höger om mallnamnet.

* **Ögonikon**: Mallen publiceras, den visas bara för gruppen och godkännandebegäran skickades inte.
* **Gula bockmarkeringsikonen**: Mallen publiceras, den visas bara för teamet och godkännandebegäran skickades.
* **Grön bockmarkeringsikon**: Mallen är publicerad och offentlig. Den är synlig för alla Workfront Fusion-användare på fliken [!UICONTROL Public templates]. Den visas även på fliken [!UICONTROL Team templates] och mallskaparen eller teammedlemmen kan fortfarande redigera den.

Mallar utan ikoner har statusen [!UICONTROL Private]. De publiceras inte och är bara synliga för teamet.

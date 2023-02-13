---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Publicera och dela [!DNL Adobe Workfront Fusion] mallar
description: När du skapar en mall blir mallen tillgänglig för alla dina teammedlemmar. Om du vill dela mallen med någon utanför ditt team måste du först publicera den.
author: Becky
feature: Workfront Fusion
exl-id: aaa59a1e-aa16-41f5-9f56-ce0615c1b685
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Publicera och dela [!DNL Adobe Workfront Fusion] mallar

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p><p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Förutsättningar

En mall måste skapas innan den kan delas.

## Publicera en [!DNL Adobe Workfront Fusion] mall

1. Klicka på **[!UICONTROL Templates]**.
1. Klicka på **[!UICONTROL Team templates]** -fliken.
1. Klicka på mallens namn.
1. Klicka på **[!UICONTROL Publish]** i skärmens övre högra hörn.

## Dela en [!DNL Workfront Fusion] mall

När du har publicerat en mall kan du dela den.

1. (Villkorligt) Om du vill ha en delbar länk klickar du på **[!UICONTROL Share public link]**.

   >[!NOTE]
   >
   >Du kan dela den här länken med vem du vill. Själva mallen finns kvar i [!UICONTROL Team templates] och är inte offentlig.

1. (Villkorligt) Om du vill att mallen ska vara offentlig skickar du den till administratören för godkännande genom att klicka på **[!UICONTROL Request Approval]**.

   >[!NOTE]
   >
   >* När mallen har godkänts blir den offentlig. [!UICONTROL Public templates] är synliga i [!UICONTROL Public templates] tabb för alla [!DNL Workfront Fusion] -användare, oavsett organisation eller team.
   >* Din administratör har inte informerats om att han eller hon får mallen för granskning via e-post. Kontakta administratören direkt om godkännandet är brådskande.



## Mallstatus

Du kan kontrollera mallsidans status under mallnamnet

Följande statusar är tillgängliga:

* **[!UICONTROL Private]**: Den här mallen visas bara för mallskaparen och deras team.
* **[!UICONTROL Published]**: Den här mallen visas bara för mallskaparen och deras team. Du kan skicka publicerade mallar för godkännande och kopiera en delbar länk.
* **[!UICONTROL Approved]**: Den här mallen är synlig för alla Workfront Fusion-användare i [!UICONTROL Public templates] -fliken. Du kan kopiera en delbar länk genom att klicka på [!UICONTROL Options] i skärmens övre högra hörn.

Du kan även kontrollera statusen på [!UICONTROL Team templates] -fliken. Om en mall publiceras visas en ikon till höger om mallnamnet.

* **Ögonikon**: Mallen publiceras, visas bara för teamet och godkännandebegäran skickades inte.
* **Gula bockmarkeringsikon**: Mallen publiceras, visas bara för teamet och godkännandebegäran skickades.
* **Grön bockmarkeringsikon**: Mallen är publicerad och offentlig. Den är synlig för alla Workfront Fusion-användare i [!UICONTROL Public templates] -fliken. Den visas även i [!UICONTROL Team templates] och mallskaparen eller teammedlemmen kan fortfarande redigera den.

Mallar utan ikoner har [!UICONTROL Private] status. De publiceras inte och är bara synliga för teamet.

---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Ta emot en webkrok från en webbtjänst
description: Om en webbtjänst inte är implementerad som en app i [!DNL Adobe Workfront Fusion], men det har stöd för att skicka webhooks, kan du lägga till tjänsten i ett scenario med hjälp av den anpassade webkrokmodulen som en direktutlösare.
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Ta emot en webkrok från en webbtjänst

Om en webbtjänst inte är implementerad som en app i [!DNL Adobe Workfront Fusion], men det har stöd för att skicka webhooks, kan du lägga till tjänsten i ett scenario med hjälp av den anpassade webkrokmodulen som en direktutlösare.

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

## Ta emot en webkrok

1. Lägg till **[!UICONTROL Webhooks]>[!UICONTROL Custom webhook]** till ditt scenario.
1. Klicka **[!UICONTROL Add]**, skriv en **[!UICONTROL Webhook name]** i rutan som visas och sedan klickar du **[!UICONTROL Save]**.

1. Klicka **[!UICONTROL Copy address to clipboard]** och sedan klicka **[!UICONTROL OK]**.

1. Logga in på webbtjänsten och gör följande:

   1. I [!UICONTROL Settings] för webbtjänsten, skapa en webkrok.
   1. Klistra in adressen som du kopierade till Urklipp i steg 3.
   1. Välj den händelse som ska utlösa webkroken.

1. I [!DNL Workfront Fusion] scenario, ange händelsen eller händelserna som du vill utlösa [!UICONTROL Custom webhook] -modul.
1. Kör scenariot.

   När en eller flera händelser inträffar [!UICONTROL Custom webhook] modulutlösare och scenariot körs.

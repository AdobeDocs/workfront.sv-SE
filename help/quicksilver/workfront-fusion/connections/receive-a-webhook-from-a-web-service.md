---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Ta emot en webkrok från en webbtjänst
description: Om en webbtjänst inte är implementerad som en app i  [!DNL Adobe Workfront Fusion], men den har stöd för att skicka webbhooks, kan du lägga till tjänsten i ett scenario med hjälp av den anpassade webbkrokmodulen som en direktutlösare.
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# Ta emot en webkrok från en webbtjänst

Om en webbtjänst inte är implementerad som en app i [!DNL Adobe Workfront Fusion], men den har stöd för att skicka webbhooks, kan du lägga till tjänsten i ett scenario med hjälp av den anpassade webbkrokmodulen som en direktutlösare.

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

## Ta emot en webkrok

1. Lägg till modulen **[!UICONTROL Webhooks]>[!UICONTROL Custom webhook]** i ditt scenario.
1. Klicka på **[!UICONTROL Add]**, skriv **[!UICONTROL Webhook name]** i rutan som visas och klicka sedan på **[!UICONTROL Save]**.

1. Klicka på **[!UICONTROL Copy address to clipboard]** och sedan på **[!UICONTROL OK]**.

1. Logga in på webbtjänsten och gör följande:

   1. Skapa en webkrok i området [!UICONTROL Settings] för webbtjänsten.
   1. Klistra in adressen som du kopierade till Urklipp i steg 3.
   1. Välj den händelse som ska utlösa webkroken.

1. I scenariot [!DNL Workfront Fusion] anger du händelsen eller händelserna som du vill ska utlösa modulen [!UICONTROL Custom webhook].
1. Kör scenariot.

   När händelsen eller händelserna inträffar utlöses modulen [!UICONTROL Custom webhook] och scenariot körs.

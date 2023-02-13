---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Skapa en [!DNL Adobe Workfront] förfrågan från ett Outlook-e-postmeddelande
description: Du kan skapa en [!DNL Adobe Workfront] förfrågan från ett e-postmeddelande i Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4ecfe632-5f2e-4dc2-8c88-6a8229887f53
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# Skapa en [!DNL Adobe Workfront] begäran från en [!UICONTROL Outlook] e-post

Du kan skapa en [!DNL Adobe Workfront] förfrågan från ett e-postmeddelande i Outlook.

När du skapar en [!DNL Workfront] begäran som baseras på ett e-postmeddelande, inkluderas innehållet i e-postmeddelandet (inklusive ämnet och brödtexten) som standard i begäran.

>[!NOTE]
>
>Du kan inte skapa en [!DNL Workfront] begäran från en delad [!UICONTROL Outlook] postlåda.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Förutsättningar

Dina [!DNL Workfront] administratör måste aktivera [!DNL Outlook for Office] med [!DNL Workfront] innan du kan använda den här integreringen.

## Skapa en begäran från en [!DNL Outlook] e-post

Skapa en [!DNL Workfront] Begär från [!DNL Outlook]:

1. Markera det e-postmeddelande som innehåller den information du vill inkludera i en [!DNL Workfront] begäran.
1. Klicka på **[!DNL Workfront]** i det övre högra hörnet av e-postmeddelandet för att visa Workfront-tillägget.\
   Du kan behöva klicka på den nedåtriktade pilen i det övre högra hörnet av ditt e-postmeddelande för att komma åt [!DNL Workfront] ikon.

1. Klicka på **[!UICONTROL Menu]** ikon för att visa listan över tillgängliga [!DNL Workfront] alternativ.

   ![o365_addin_menu2_icon.png](assets/o365-addin-menu2-icon.png)

1. Klicka på **[!UICONTROL Submit Request]**.
1. I **[!UICONTROL Select a Request Type]** markerar du den begärandekö där du vill skicka begäran.

   ![o365_addin_submitRequest.png](assets/o365-addin-submitrequest.png)

1. Ange följande information:\
   Beroende på hur frågekö konfigurerades kan tillgängliga fält variera. En fullständig lista och en beskrivning av möjliga fält finns på [Skapa och skicka [!DNL Adobe Workfront] förfrågningar](../../manage-work/requests/create-requests/create-submit-requests.md) artikel.

   * **[!UICONTROL Subject]:** Ange ett ämne för begäran. Som standard används e-postmeddelandets ämne.
   * **[!UICONTROL Description]:** Ange en beskrivning för begäran. Som standard används e-postbrödtexten.
   * **[!UICONTROL Documents]:** Bifoga alla dokument som du vill inkludera i begäran. Du kan bifoga dokument genom att dra och släppa eller genom att klicka **[!UICONTROL Select File]** och bläddra till och markera dokumentet.\

      Som standard inkluderas alla dokument som är bifogade till e-postmeddelandet i begäran.

1. Klicka på **[!UICONTROL Submit Request]**.\
   Begäran skickas till [!DNL Workfront], i den angivna begärandekön.

1. (Valfritt) Navigera tillbaka till [!DNL Outlook]och välj det ursprungliga e-postmeddelandet.\
   Överst på [!DNL Workfront] lägg till en länk till bekräftelsen om att e-postmeddelandet har lagts till i Workfront som en begäran. Länken innehåller datumet då den konverterades.\
   ![outlook_skickad_as_a_request.png](assets/outlook-submitted-as-a-request-350x130.png)

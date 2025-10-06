---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Skapa en [!DNL Adobe Workfront] begäran från ett Outlook-e-postmeddelande
description: Du kan skapa en [!DNL Adobe Workfront] begäran från ett e-postmeddelande i Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4ecfe632-5f2e-4dc2-8c88-6a8229887f53
source-git-commit: 793c8c940c8cb7ac53169edf21ddf28af2554120
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# Skapa en [!DNL Adobe Workfront]-förfrågan från ett [!UICONTROL Outlook]-e-postmeddelande



>[!IMPORTANT]
>
>[Microsoft har inaktiverat stöd för äldre Exchange-onlinetoken](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) som användes av Workfront Outlook-tillägget för autentisering. Denna ändring av Microsoft har stegvis genomförts och är klar den 1 oktober 2025.
>
>**Eftersom Microsoft har inaktiverat dessa token fungerar inte längre integreringen i Workfront för Microsoft Outlook.**

Du kan skapa en [!DNL Adobe Workfront]-begäran från ett e-postmeddelande i Outlook.

När du skapar en [!DNL Workfront]-begäran baserat på ett e-postmeddelande inkluderas innehållet i e-postmeddelandet (inklusive ämnet och brödtexten) som standard i begäran.

>[!NOTE]
>
>Du kan inte skapa en [!DNL Workfront]-begäran från en delad [!UICONTROL Outlook]-postlåda.

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

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

[!DNL Workfront]-administratören måste aktivera [!DNL Outlook for Office] med [!DNL Workfront] innan du kan använda den här integreringen.

## Skapa en begäran från ett [!DNL Outlook]-e-postmeddelande

Så här skapar du en [!DNL Workfront]-begäran från [!DNL Outlook]:

1. Markera det e-postmeddelande som innehåller den information som du vill inkludera i en [!DNL Workfront]-begäran.
1. Klicka på ikonen **[!DNL Workfront]** i det övre högra hörnet av e-postmeddelandet för att visa Workfront-tillägget.\
   Du kan behöva klicka på den nedåtriktade pilen i det övre högra hörnet av ditt e-postmeddelande för att komma åt ikonen [!DNL Workfront].

1. Klicka på ikonen **[!UICONTROL Menu]** ![&#x200B; o365_addin_menu2_icon.png](assets/o365-addin-menu2-icon.png) för att visa listan med tillgängliga [!DNL Workfront]-alternativ.

1. Klicka på **[!UICONTROL Submit Request]**.
1. I fältet **[!UICONTROL Select a Request Type]** väljer du den begärandekö där du vill skicka begäran.

1. Ange följande information:\
   Beroende på hur frågekö konfigurerades kan tillgängliga fält variera. En fullständig lista och en beskrivning av möjliga fält finns i artikeln [Skapa och skicka [!DNL Adobe Workfront] förfrågningar](../../manage-work/requests/create-requests/create-submit-requests.md) .

   * **[!UICONTROL Subject]:** Ange ett ämne för begäran. Som standard används e-postmeddelandets ämne.
   * **[!UICONTROL Description]:** Ange en beskrivning för begäran. Som standard används e-postbrödtexten.
   * **[!UICONTROL Documents]:** Bifoga alla dokument som du vill inkludera i begäran. Du kan bifoga dokument genom att dra och släppa eller genom att klicka på **[!UICONTROL Select File]** och bläddra till och markera dokumentet.\

     Som standard inkluderas alla dokument som är bifogade till e-postmeddelandet i begäran.

1. Klicka på **[!UICONTROL Submit Request]**.\
   Begäran skickas till [!DNL Workfront] i den angivna begärandekön.

1. (Valfritt) Navigera tillbaka till [!DNL Outlook] och markera det ursprungliga e-postmeddelandet.\
   Längst upp på tilläggspanelen [!DNL Workfront] kan du se bekräftelsen med en länk att e-postmeddelandet har lagts till i Workfront som en begäran. Länken innehåller datumet då den konverterades.\

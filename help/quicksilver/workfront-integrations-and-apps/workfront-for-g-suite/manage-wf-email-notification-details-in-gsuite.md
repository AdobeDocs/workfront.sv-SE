---
product-area: workfront-integrations
keywords: google,doc,dokument,ark,bild
navigation-topic: workfront-for-g-suite
title: Hantera [!DNL Adobe Workfront] meddelandeinformation från Google Workspace
description: När du öppnar ett e-postmeddelande som har skickats från Adobe [!DNL Workfront]  i Google Workspace kan du visa den associerade arbetsuppgiftens information och svara utan att lämna inkorgen. Om det finns tillgängliga åtgärder, till exempel godkännande av en begäran, kan du utföra dessa åtgärder direkt från Workfront för Google Workspace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# Hantera meddelandeinformation för [!DNL Adobe Workfront] från [!DNL Google Workspace]

>[!IMPORTANT]
>
>För att kunna leverera mer stabila och skalbara integreringar går vi över till en modern, flexibel integrationsstrategi med hjälp av Workfront Automation and Integration (Fusion). Under den här övergångsprocessen kommer följande Workfront för Google Workspace-funktioner inte att vara tillgängliga efter **28 februari 2026**:
>
>* Åtkomst till Google Workspace-funktioner inifrån Workfront
>
>* Visa och hantera Workfront-uppgifter från Gmail eller Google Calendar-webbplatspanelen
>
>Vi rekommenderar att du använder Workfront Automation and Integration för din organisations integreringsbehov med Google Workspace.
>
>En översikt över Workfront Automation and Integration finns i [Adobe Workfront Fusion - översikt](https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Mer information om de specifika funktionerna i Workfront Automation and Integration-modulerna för Google Workspace finns i [Gmail-moduler](https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) och [Google Calendar-moduler](https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

När du öppnar ett e-postmeddelande som [!DNL Google Workspace] har skickat i [!DNL Adobe Workfront] kan du visa den associerade arbetsuppgiftens information och svara utan att lämna din [!UICONTROL Inbox]. Om det finns tillgängliga åtgärder, till exempel godkännande av en begäran, kan du utföra dessa åtgärder direkt från [!DNL Workfront for Google Workspace].

>[!NOTE]
>
> [!DNL Workfront for Google Workspace] stöder nästan alla typer av e-postmeddelanden som du kan ta emot från [!DNL Workfront] (ungefär 120 olika typer). [!UICONTROL Daily digest] e-postmeddelanden som skickas från [!DNL Workfront] visas inte i [!DNL Workfront for Google Workspace]. Mer information om meddelandetyperna [!DNL Workfront] finns i [Ändra dina egna e-postmeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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

Innan du kan hantera meddelandeinformation från [!DNL Google Workspace] måste du

* Installera [!DNL Workfront for Google Workspace]\
   Instruktioner finns i [Installera [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Hantera meddelandeinformation för [!DNL Adobe Workfront] från [!DNL Google Workspace]

1. Om panelen [!DNL Workfront for Google Workspace] inte visas klickar du på ikonen [!DNL Workfront] ![Workfront ](assets/wf-lion-icon.png) i sidofältet för [!DNL Google Workspace]-tillägg längst till höger på sidan.
1. Öppna ett [!DNL Google Workspace]-meddelande i [!DNL Workfront].
1. Klicka på **[!UICONTROL View all updates]** om den visas nära panelens övre del.
1. Klicka på **[!UICONTROL Details]**.
1. Klicka på eventuella tillgängliga alternativ.

   De alternativ som kan visas gäller den typ av e-postmeddelanden som du har öppnat. Om det till exempel är ett e-postmeddelande där du ombeds godkänna en uppgift, visas **[!UICONTROL Approve]** och **[!UICONTROL Reject]** i stället för alternativ som **[!UICONTROL Work on It]** eller **[!UICONTROL Done]**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Typ av e-postmeddelande</th> 
      <th>Åtgärd</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>Aktivitet eller problem</td> 
      <td><strong>[!UICONTROL Approve]</strong> den, <strong>[!UICONTROL Reject]</strong> den, <strong>[!UICONTROL Grant]</strong> åtkomst till den, <strong>[!UICONTROL Ignore]</strong> en begäran om åtkomst till den, <strong>[!UICONTROL Work on it]</strong> eller klicka på ett alternativ som anger att du är <strong>[!UICONTROL Done]</strong> med den</td> 
     </tr> 
     <tr> 
      <td>Projekt</td> 
      <td><strong>[!UICONTROL Approve]</strong> den, <strong>[!UICONTROL Reject]</strong> den, <strong>[!UICONTROL Grant]</strong> åtkomst till den eller <strong>[!UICONTROL Ignore]</strong> en begäran om åtkomst till den</td> 
     </tr> 
     <tr> 
      <td>Dokument</td> 
      <td><strong>[!UICONTROL Approve]</strong> den, <strong>[!UICONTROL Reject]</strong> den, <strong>[!UICONTROL Grant]</strong> åtkomst till den eller <strong>[!UICONTROL Ignore]</strong> en begäran om åtkomst till den</td> 
     </tr> 
     <tr> 
      <td>Uppdatera </td> 
      <td> <p>Visa en del av hela listan med uppdateringar för objektet så att du har den kontext du behöver för att <strong>[!UICONTROL Post]</strong> en ny uppdatering eller en <strong>[!UICONTROL Reply]</strong>. Du kan klicka på <strong>[!UICONTROL Notify]</strong> om du vill varna vissa användare om ditt svar. </p> <p>Mer information finns i <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">Svara på ett [!DNL Adobe Workfront] uppdateringsmeddelande från [!DNL Google Workspace]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Godkännandebegäran</td> 
      <td><strong>[!UICONTROL Approve]</strong> eller <strong>[!UICONTROL Reject]</strong> det (du kan ändra dig genom att klicka på det andra alternativet), hämta det, visa dess ägare eller visa dess referensnummer</td> 
     </tr> 
     <tr> 
      <td>En ändring av ett projekts status</td> 
      <td> Visa all aktuell information om projektet, inklusive eventuella anpassade formulär. </td> 
     </tr> 
    </tbody> 
   </table>

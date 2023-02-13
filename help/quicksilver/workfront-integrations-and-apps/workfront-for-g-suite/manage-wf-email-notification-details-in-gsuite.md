---
product-area: workfront-integrations
keywords: google,doc,dokument,ark,bild
navigation-topic: workfront-for-g-suite
title: Hantera [!DNL Adobe Workfront] meddelandeinformation från G Suite
description: I G Suite när du öppnar ett e-postmeddelande Adobe [!DNL Workfront] har skickat kan du visa den associerade arbetsuppgiftens information och svara utan att lämna Inkorgen. Om det finns tillgängliga åtgärder, till exempel godkännande av en begäran, kan du utföra dessa åtgärder direkt från Workfront för G Suite.
author: Becky
feature: Workfront Integrations and Apps
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: 3143e5a4988b7234d8225da442f5af1d756d461d
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Hantera [!DNL Adobe Workfront] meddelandeinformation från [!DNL G Suite]

I [!DNL G Suite]när du öppnar ett e-postmeddelande [!DNL Adobe Workfront] har skickat kan du visa den associerade arbetsuppgiftens information och svara utan att lämna [!UICONTROL Inbox]. Om det finns tillgängliga åtgärder, till exempel att godkänna en begäran, kan du utföra dessa åtgärder direkt från [!DNL Workfront for G Suite].

>[!NOTE]
>
> [!DNL Workfront for G Suite] har stöd för nästan alla typer av e-postmeddelanden som du kan få från [!DNL Workfront] (ungefär 120 olika typer). [!UICONTROL Daily digest] e-postmeddelanden skickade från [!DNL Workfront] visas inte i [!DNL Workfront for G Suite]. Mer information om [!DNL Workfront] e-postmeddelandetyper, se [Aktivera eller inaktivera egna händelsemeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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

Innan du kan hantera meddelandeinformation från [!DNL G Suite]måste du

* Installera [!DNL Workfront for G suite]\
   Instruktioner finns i [Installera [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Hantera [!DNL Adobe Workfront] meddelandeinformation från [!DNL G Suite]

1. Om [!DNL Workfront for G Suite] visas inte, klicka på [!DNL Workfront] icon ![](assets/wf-lion-icon.png) i [!DNL G Suite] sidofältet för tillägg längst till höger på sidan.
1. I [!DNL G Suite], öppna en [!DNL Workfront] e-postmeddelande.
1. Klicka **[!UICONTROL View all updates]** om den visas nära panelens övre del.
1. Klicka på **[!UICONTROL Details]**.
1. Klicka på eventuella tillgängliga alternativ.

   De alternativ som kan visas gäller den typ av e-postmeddelanden som du har öppnat. Om det till exempel är ett e-postmeddelande där du uppmanas att godkänna en uppgift visas **[!UICONTROL Approve]** och **[!UICONTROL Reject]** i stället för alternativ som **[!UICONTROL Work on It]** eller **[!UICONTROL Done]**:

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
      <td><strong>[!UICONTROL Approve]</strong> den, <strong>[!UICONTROL Reject]</strong> den, <strong>[!UICONTROL Grant]</strong> tillgång till den, <strong>[!UICONTROL Ignore]</strong> en begäran om tillgång till den, <strong>[!UICONTROL Work on it]</strong>eller klicka på ett alternativ som anger att du <strong>[!UICONTROL Done]</strong> med</td> 
     </tr> 
     <tr> 
      <td>Projekt</td> 
      <td><strong>[!UICONTROL Approve]</strong> den, <strong>[!UICONTROL Reject]</strong> den, <strong>[!UICONTROL Grant]</strong> tillgång till den, eller <strong>[!UICONTROL Ignore]</strong> en begäran om åtkomst</td> 
     </tr> 
     <tr> 
      <td>Dokument</td> 
      <td><strong>[!UICONTROL Approve]</strong> den, <strong>[!UICONTROL Reject]</strong> den, <strong>[!UICONTROL Grant]</strong> tillgång till den, eller <strong>[!UICONTROL Ignore]</strong> en begäran om åtkomst</td> 
     </tr> 
     <tr> 
      <td>Uppdatera </td> 
      <td> <p>Visa en del av hela listan med uppdateringar för objektet så att du har den kontext du behöver <strong>[!UICONTROL Post]</strong> en ny uppdatering eller en <strong>[!UICONTROL Reply]</strong>. Du kan klicka <strong>[!UICONTROL Notify]</strong> om du vill varna vissa användare om ditt svar. </p> <p>Mer information finns i <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">Svara på en [!DNL Adobe Workfront] uppdateringsmeddelande från [!DNL G Suite]</a>.</p> </td> 
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

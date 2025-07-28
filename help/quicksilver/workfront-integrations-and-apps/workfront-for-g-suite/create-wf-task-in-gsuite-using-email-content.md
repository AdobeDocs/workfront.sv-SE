---
product-area: workfront-integrations;projects
keywords: google,doc,dokument,ark,bild
navigation-topic: workfront-for-g-suite
title: Skapa en [!DNL Adobe Workfront] aktivitet i Google Workspace med e-postinnehåll
description: Du kan konvertera ett externt e-postmeddelande (som inte har genererats av Adobe [!DNL Workfront]) till en Workfront-uppgift.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 6bbb4301-2791-4d72-bad8-fef63d6e892a
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 0%

---

# Skapa en [!DNL Adobe Workfront]-uppgift i [!DNL Google Workspace] med e-postinnehåll

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

Du kan konvertera ett externt e-postmeddelande (som inte har genererats av [!DNL Adobe Workfront]) till en [!DNL Workfront]-åtgärd.

Du kan också konvertera ett externt e-postmeddelande till en uppdatering för en befintlig uppgift. Mer information finns i [Uppdatera ett [!DNL Adobe Workfront] objekt från [!DNL Google Workspace] med e-postinnehåll](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

Mer information om hur du använder [!DNL Google Workspace] för att arbeta med e-postmeddelanden som skickas av [!DNL Workfront] finns i [Hantera [!DNL Adobe Workfront] meddelandeinformation från [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

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

Innan du kan skapa en [!DNL Workfront]-uppgift i [!DNL Google Workspace] måste du

* Installera [!DNL Workfront for Google Workspace]\
   Instruktioner finns i [Installera [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Skapa en [!DNL Adobe Workfront]-uppgift i [!DNL Google Workspace] med e-postinnehåll

1. Om panelen [!UICONTROL Workfront for Google Workspace] inte visas klickar du på ikonen [!DNL Workfront] ![Workfront ](assets/wf-lion-icon.png) i sidofältet för [!DNL Google Workspace]-tillägg längst till höger på sidan.
1. Öppna e-postmeddelandet i [!DNL Google Workspace] och klicka på ett alternativ i [!DNL Workfront for Google Workspace] för att konvertera e-postmeddelandet till en ny [!DNL Workfront]-åtgärd.

1. Välj ett **[!UICONTROL Create new]**-alternativ för att ange om aktiviteten ska vara en del av ett projekt eller en personlig uppgift som är oberoende av ett projekt.
1. Om du vill bifoga aktiviteten till ett överordnat projekt klickar du på **[!UICONTROL Project name]**, skriver namnet på projektet där du vill ha aktiviteten och klickar sedan på projektnamnet när det visas i listan nedan.
1. Gör någon av dessa ändringar:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Task name]</td> 
      <td>Redigera valfri del av den här texten, som hämtas från e-postmeddelandets ämnesrad.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Redigera valfri del av den här texten, som hämtas från e-postmeddelandet.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Assign To]</td> 
      <td>Klicka på <strong>[!UICONTROL Assign To]</strong>, klicka på alternativet <strong>[!UICONTROL Assign this to]</strong> som visas och börja sedan skriva in personens namn och klicka på det när det visas i listan nedan. Upprepa detta för varje person som du vill lägga till och klicka sedan på <strong>[!UICONTROL Save]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Planned duration]</td> 
      <td> <p>Klicka på <strong>[!UICONTROL Planned duration]</strong> och ange sedan det antal dagar som du vill att uppgiften ska ta. </p> <p>Obs! Det här alternativet kan konfigureras för din organisation på olika sätt. För din organisation kan du till exempel behöva ange ett antal timmar i stället för dagar. Kontakta [!DNL Workfront]-administratören om du behöver mer information. Om du vill ange en annan tidsperiod än den konfigurerade standardperioden skriver du <strong>m</strong>, <strong>h</strong>, <strong>d</strong>, <strong>w</strong> eller <strong>mo</strong> efter talet för att ange minuter, timmar, dagar, veckor eller månader.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Priority]</td> 
      <td>Klicka på listrutepilen och klicka sedan på den prioritet du vill ha för uppgiften.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email attachments]</td> 
      <td> <p>(Endast tillgängligt om e-postmeddelandet innehåller minst en bifogad fil.) Klicka på det här alternativet om du vill spara bifogade filer i e-postmeddelandet i [!UICONTROL Documents]-området för uppgiften. </p> <p>Om du inte vill spara en bifogad fil klickar du på krysset till höger om namnet. </p> <p>Om e-postmeddelandet innehåller länkar till dokument i [!DNL Google Drive] sparas de på fliken [!UICONTROL Overview] för den uppgift du skapar. </p> <p>Viktigt! För att detta ska fungera måste [!DNL Workfront]-administratören godkänna [!DNL Google Drive] att arbeta med dokument i [!DNL Workfront], vilket beskrivs i avsnittet <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">Konfigurera integreringar för att hantera dokument</a> i artikeln <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">Konfigurera dokumentintegreringar</a>.</p> <p>Om du aktiverar det här alternativet förblir det aktiverat för andra e-postmeddelanden som du konverterar till uppgifter, utgåvor och uppdateringar.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email file]</td> 
      <td> <p>Klicka på det här alternativet om du vill spara det ursprungliga e-postmeddelandet som en EML-fil <span> i [!UICONTROL Documents] området </span> för uppgiften. Därifrån kan du dubbelklicka på filen för att öppna e-postmeddelandet i ditt e-postprogram.</p> <p>Om du aktiverar det här alternativet förblir det aktiverat för andra e-postmeddelanden som du konverterar till uppgifter, utgåvor och uppdateringar.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **[!UICONTROL Create Task]**.

   Fliken **[!UICONTROL Details]** för den nya aktiviteten visas på panelen [!DNL Workfront for Google Workspace]. Du kan klicka på **[!UICONTROL Updates]** och börja kommunicera med medarbetare direkt utan att lämna din inkorg.

   Längst ned på fliken **[!UICONTROL Details]** kan du även klicka på **[!UICONTROL View in [!DNL Workfront]]** för att gå till den nya aktiviteten i Workfront.

   När du uppdaterar webbläsaren bekräftar ett meddelande med en länk längst ned på panelen [!DNL Workfront for Google Workspace] att du har konverterat e-postmeddelandet till en åtgärd:

   Du kan klicka på länken för att gå till detaljvyn på panelen [!DNL Workfront for Google Workspace] för den uppgift du har skapat.

   Du kan upprepa de här stegen om du vill konvertera samma e-post till flera åtgärder. När du uppdaterar webbläsaren eller återgår till e-postmeddelandet vid ett senare tillfälle visas alla länkar som du har skapat för e-postmeddelandet längst ned på panelen [!UICONTROL Workfront for Google Workspace].

1. (Valfritt) Fortsätt att arbeta med uppgiften på panelen [!DNL Workfront for Google Workspace] genom att göra något av följande:

   * Om du vill lägga till en uppdatering på fliken **[!UICONTROL Updates]** klickar du på **[!UICONTROL Start a new update]** och skriver uppdateringen.

   * Om du vill svara på en uppdatering på fliken **[!UICONTROL Updates]** klickar du på **[!UICONTROL Reply]** och skriver in ditt svar.

     För båda ovanstående åtgärder kan du meddela vissa användare om din kommentar. Klicka på **[!UICONTROL Notify]**, börja skriva namnet på en användare och klicka sedan på namnet när det visas i listrutan. Upprepa den här processen för andra användare som du vill meddela och klicka sedan på **[!UICONTROL Post]**.

   * Klicka på fliken **[!UICONTROL Documents]** om du vill visa dokument som har sparats med uppgiften.

Du kan upprepa de här stegen om du vill konvertera samma e-post till flera åtgärder. När du uppdaterar webbläsaren eller återgår till e-postmeddelandet vid ett senare tillfälle visas alla länkar som du har skapat för e-postmeddelandet längst ned på panelen [!DNL Workfront for Google Workspace].

---
product-area: workfront-integrations;projects
keywords: google,doc,dokument,ark,bild
navigation-topic: workfront-for-g-suite
title: Skapa ett [!DNL Adobe Workfront] problem i Google Workspace med e-postinnehåll
description: Du kan konvertera en extern e-postadress (som inte har genererats av  [!DNL Adobe Workfront)] ) till en [!DNL Workfront] utgåva.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7a15f557-67d8-4be8-8538-4bce06536c0a
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 0%

---

# Skapa ett [!DNL Adobe Workfront]-problem i [!DNL Google Workspace] med e-postinnehåll

>[!NOTE]
>
>Den senaste versionen av Adobe Workfront-pluginprogrammet för Google släpptes den 26 juni 2023.

Du kan konvertera en extern e-postadress (som inte har genererats av [!DNL Adobe Workfront]) till ett [!DNL Workfront]-problem.

Du kan också konvertera ett externt e-postmeddelande till en uppdatering om ett befintligt problem. Mer information finns i [Uppdatera ett [!DNL Adobe Workfront] objekt från [!DNL Google Workspace] med e-postinnehåll](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

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

Innan du kan skapa ett problem från [!DNL Google Workspace] måste du

* Installera [!DNL Workfront for Google Workspace]\
   Instruktioner finns i [Installera [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Skapa ett [!DNL Adobe Workfront]-problem i [!DNL Google Workspace] med e-postinnehåll

1. Om panelen [!UICONTROL Workfront for Google Workspace] inte visas klickar du på ikonen [!DNL Workfront] ![](assets/wf-lion-icon.png) i sidofältet för [!DNL Google Workspace] tillägg längst till höger på sidan.
1. Öppna e-postmeddelandet i [!DNL Google Workspace] och klicka på ett alternativ i [!DNL Workfront for Google Workspace] för att konvertera e-postmeddelandet till ett nytt [!DNL Workfront]-problem.

   ![](assets/convert-email-task-issue-update.png)

1. Om du vill bifoga utgåvan till ett överordnat projekt klickar du på **[!UICONTROL Project name]**, börjar skriva namnet på projektet där du vill ha utgåvan och klickar sedan på projektnamnet när det visas i listan nedan.
1. Gör någon av dessa ändringar:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Issue Name]</td> 
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
      <td role="rowheader">[!UICONTROL Priority]</td> 
      <td>Klicka på listrutepilen och klicka sedan på den prioritet du vill ha för problemet.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email attachments]</td> 
      <td> <p>(Endast tillgängligt om e-postmeddelandet innehåller minst en bifogad fil.) Klicka på det här alternativet om du vill spara bifogade filer i e-postmeddelandet i problemområdet [!UICONTROL Documents]. </p> <p>Om du inte vill spara en bifogad fil klickar du på krysset till höger om namnet. </p> <p>Om e-postmeddelandet innehåller länkar till dokument i [!DNL Google Drive] sparas de på fliken [!UICONTROL Overview] i det problem du skapar. </p> <p>Viktigt! För att detta ska fungera måste [!DNL Workfront]-administratören godkänna [!DNL Google Drive] att arbeta med dokument i [!DNL Workfront], vilket beskrivs i avsnittet <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">Konfigurera integreringar för att hantera dokument</a> i artikeln <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">Konfigurera dokumentintegreringar</a>.</p> <p>Om du aktiverar det här alternativet förblir det aktiverat för andra e-postmeddelanden som du konverterar till uppgifter, utgåvor och uppdateringar.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Inkludera e-postfil</td> 
      <td> <p>Klicka på det här alternativet om du vill spara det ursprungliga e-postmeddelandet som en EML-fil (e-post) <span> i [!UICONTROL Documents] området </span> för problemet. Därifrån kan du dubbelklicka på filen för att öppna e-postmeddelandet i ditt e-postprogram.</p> <p>Om du aktiverar det här alternativet förblir det aktiverat för andra e-postmeddelanden som du konverterar till uppgifter, utgåvor och uppdateringar.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **[!UICONTROL Create Issue]**.

   Fliken **[!UICONTROL Details]** för den nya utgåvan visas på panelen [!DNL Workfront for Google Workspace]. Du kan klicka på **[!UICONTROL Updates]** och börja kommunicera med medarbetare direkt utan att lämna din inkorg.

   Längst ned på fliken **[!UICONTROL Details]** kan du även klicka på **[!UICONTROL View in Workfront]** för att gå till den nya utgåvan i Workfront.

   När du uppdaterar webbläsaren bekräftar ett meddelande med en länk längst ned på panelen [!UICONTROL Workfront for Google Workspace] att du har konverterat e-postmeddelandet till ett problem:

   Du kan klicka på länken för att gå till detaljvyn på panelen [!DNL Workfront for Google Workspace] för det problem du har skapat.

   Du kan upprepa de här stegen för att konvertera samma e-post till flera utgåvor. När du uppdaterar webbläsaren eller återgår till e-postmeddelandet vid ett senare tillfälle visas alla länkar som du har skapat för e-postmeddelandet längst ned på panelen [!UICONTROL Workfront for Google Workspace].

1. (Valfritt) Fortsätt att arbeta med problemet på panelen [!DNL Workfront for Google Workspace] genom att göra något av följande:

   * Om du vill lägga till en uppdatering på fliken **[!UICONTROL Updates]** klickar du på **[!UICONTROL Start a new update]** och skriver uppdateringen.

   * Om du vill svara på en uppdatering på fliken **[!UICONTROL Updates]** klickar du på **[!UICONTROL Reply]** och skriver in ditt svar.

     För båda ovanstående åtgärder kan du meddela vissa användare om din kommentar. Klicka på **[!UICONTROL Notify]**, börja skriva namnet på en användare och klicka sedan på namnet när det visas i listrutan. Upprepa den här processen för andra användare som du vill meddela och klicka sedan på **[!UICONTROL Post]**.

   * Klicka på fliken **[!UICONTROL Documents]** om du vill visa dokument som har sparats med problemet.

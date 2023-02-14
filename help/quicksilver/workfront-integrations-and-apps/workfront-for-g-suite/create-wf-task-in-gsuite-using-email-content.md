---
product-area: workfront-integrations;projects
keywords: google,doc,dokument,ark,bild
navigation-topic: workfront-for-g-suite
title: Skapa en [!DNL Adobe Workfront] i G Suite med e-postinnehåll
description: Du kan konvertera ett externt e-postmeddelande (som inte genererats av Adobe) [!DNL Workfront]) till en Workfront-uppgift.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 6bbb4301-2791-4d72-bad8-fef63d6e892a
source-git-commit: 0934ae23a8e80dd18872efef7d274bd57d227647
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Skapa en [!DNL Adobe Workfront] uppgift i [!DNL G Suite] använda e-postinnehåll

>[!NOTE]
>
>Det finns en [känt problem](https://experienceleague.adobe.com/docs/workfront-known-issues/issues/new-workfront-experience/wf-current/wf-integrations-error-when-opening-wf-for-gsuite.html?lang=en) med den aktuella versionen av [!DNL Workfront for G Suite] fungerar inte som förväntat. Vi arbetar med en ny version och förväntar oss att den ska släppas på [!DNL Google Marketplace] inom den närmaste framtiden.

Du kan konvertera ett externt e-postmeddelande (som inte genererats av [!DNL Adobe Workfront]) till [!DNL Workfront] uppgift.

Du kan också konvertera ett externt e-postmeddelande till en uppdatering för en befintlig uppgift. Mer information finns i [Uppdatera en [!DNL Adobe Workfront] objekt från [!DNL G Suite] med e-postinnehåll](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

Mer information om hur du använder [!DNL G Suite] att arbeta med e-postmeddelanden som skickas av [!DNL Workfront], se [Hantera [!DNL Adobe Workfront] meddelandeinformation från [!DNL G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

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

Innan du kan skapa en [!DNL Workfront] uppgift i [!DNL G Suite]måste du

* Installera [!DNL Workfront for G suite]\
   Instruktioner finns i [Installera [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Skapa en [!DNL Adobe Workfront] uppgift i [!DNL G Suite] använda e-postinnehåll

1. Om [!UICONTROL Workfront for G Suite] visas inte, klicka på [!DNL Workfront] icon ![](assets/wf-lion-icon.png) i [!DNL G Suite] sidofältet för tillägg längst till höger på sidan.
1. Med e-postmeddelandet öppet i [!DNL G Suite]klickar du på ett alternativ i [!DNL Workfront for G Suite] konvertera e-postmeddelandet till ett nytt [!DNL Workfront] uppgift.

   ![](assets/convert-email-task-issue-update.png)

1. Välj en **[!UICONTROL Create new]** för att ange om uppgiften ska ingå i ett projekt eller en personlig uppgift som är oberoende av ett projekt.
1. Om du vill bifoga uppgiften till ett överordnat projekt klickar du på **[!UICONTROL Project name]** börjar du skriva namnet på det projekt där du vill ha uppgiften och klickar sedan på projektnamnet när det visas i listan nedan.
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
      <td>Redigera valfri del av den här texten, som hämtas från e-postmeddelandets brödtext.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Assign To]</td> 
      <td>Klicka <strong>[!UICONTROL Assign To]</strong>klickar du på <strong>[!UICONTROL Assign this to]</strong> som visas börjar du skriva personens namn och klickar på det när det visas i listan nedan. Upprepa detta för varje person som du vill lägga till och klicka sedan på <strong>[!UICONTROL Save]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Planned duration]</td> 
      <td> <p>Klicka <strong>[!UICONTROL Planned duration]</strong>skriver du sedan det antal dagar som du vill att uppgiften ska utföras. </p> <p>Obs! Det här alternativet kan konfigureras för din organisation på olika sätt. För din organisation kan du till exempel behöva ange ett antal timmar i stället för dagar. Om du behöver mer information kan du läsa [!DNL Workfront] administratör. Om du vill ange en annan tidsperiod än den konfigurerade standardperioden skriver du <strong>m</strong>, <strong>h</strong>, <strong>d</strong>, <strong>w</strong>, eller <strong>mån</strong> efter numret för att ange minuter, timmar, dagar, veckor eller månader.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Priority]</td> 
      <td>Klicka på listrutepilen och klicka sedan på den prioritet du vill ha för uppgiften.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email attachments]</td> 
      <td> <p>(Endast tillgängligt om e-postmeddelandet innehåller minst en bifogad fil.) Klicka på det här alternativet om du vill spara bilagor i e-postmeddelandet i [!UICONTROL Documents] aktivitetens område. </p> <p>Om du inte vill spara en bifogad fil klickar du på krysset till höger om namnet. </p> <p>Om e-postmeddelandet innehåller länkar till dokument i [!DNL Google Drive], sparas de i [!UICONTROL Overview] -fliken för uppgiften som du skapar. </p> <p>Viktigt: För att det ska fungera [!DNL Workfront] administratören måste auktorisera [!DNL Google Drive] arbeta med dokument i [!DNL Workfront], enligt beskrivningen i avsnittet <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">Konfigurera integreringar för att hantera dokument</a> i artikeln <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">Konfigurera dokumentintegreringar</a>.</p> <p>Om du aktiverar det här alternativet förblir det aktiverat för andra e-postmeddelanden som du konverterar till uppgifter, utgåvor och uppdateringar.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email file]</td> 
      <td> <p>Klicka på det här alternativet om du vill spara det ursprungliga e-postmeddelandet som en EML-fil <span>till [!UICONTROL Documents] area</span> för uppgiften. Därifrån kan du dubbelklicka på filen för att öppna e-postmeddelandet i ditt e-postprogram.</p> <p>Om du aktiverar det här alternativet förblir det aktiverat för andra e-postmeddelanden som du konverterar till uppgifter, utgåvor och uppdateringar.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **[!UICONTROL Create Task]**.

   The **[!UICONTROL Details]** -fliken för den nya uppgiften visas i [!DNL Workfront for G Suite] -panelen. Du kan klicka **[!UICONTROL Updates]** och börja kommunicera med medarbetarna direkt utan att behöva lämna kartongen.

   Längst ned på **[!UICONTROL Details]** kan du även klicka på **[!UICONTROL View in [!DNL Workfront]]** för att gå till den nya uppgiften i Workfront.

   När du uppdaterar webbläsaren visas ett meddelande med en länk längst ned i [!DNL Workfront for G Suite] bekräftar att du har konverterat e-postmeddelandet till en uppgift:

   ![](assets/email-was-converted.png)

   Du kan klicka på länken för att gå till vyn Detaljer, i dialogrutan [!DNL Workfront for G Suite] för den uppgift du har skapat.

   Du kan upprepa de här stegen om du vill konvertera samma e-post till flera åtgärder. När du uppdaterar webbläsaren eller återgår till e-postmeddelandet vid ett senare tillfälle visas alla länkar som du har skapat för e-postmeddelandet längst ned i [!UICONTROL Workfront for G Suite] -panelen.

1. (Valfritt) Fortsätt att arbeta med uppgiften i [!DNL Workfront for G Suite] gör något av följande:

   * Lägga till en uppdatering på **[!UICONTROL Updates]** flik, klicka **[!UICONTROL Start a new update]** och skriv uppdateringen.

   * Svara på en uppdatering på **[!UICONTROL Updates]** flik, klicka **[!UICONTROL Reply]** och skriv in ditt svar.

      För båda ovanstående åtgärder kan du meddela vissa användare om din kommentar. Klicka **[!UICONTROL Notify]** börjar du skriva namnet på en användare och klickar sedan på namnet när det visas i listrutan. Upprepa den här processen för andra användare som du vill meddela och klicka sedan på **[!UICONTROL Post]**.

   * Klicka på **[!UICONTROL Documents]** om du vill visa dokument som har sparats med uppgiften.

Du kan upprepa de här stegen om du vill konvertera samma e-post till flera åtgärder. När du uppdaterar webbläsaren eller återgår till e-postmeddelandet vid ett senare tillfälle visas alla länkar som du har skapat för e-postmeddelandet längst ned i [!DNL Workfront for G Suite] -panelen.

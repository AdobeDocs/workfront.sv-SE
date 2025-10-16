---
product-area: workfront-integrations;projects
keywords: google,doc,dokument,ark,bild
navigation-topic: workfront-for-g-suite
title: Uppdatera ett [!DNL Adobe Workfront] objekt från Google Workspace med e-postinnehåll
description: Du kan uppdatera ett befintligt projekt, en uppgift eller ett problem med information från ett e-postmeddelande som inte kommer från Adobe Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 1e5b3c7d087c34870ccb0f4e65021358f08b81bf
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 0%

---

# Uppdatera ett [!DNL Adobe Workfront]-objekt från [!DNL Google Workspace] med e-postinnehåll

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
>En översikt över Workfront Automation and Integration finns i [Adobe Workfront Fusion - översikt](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Mer information om de specifika funktionerna i Workfront Automation and Integration-modulerna för Google Workspace finns i [Gmail-moduler](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) och [Google Calendar-moduler](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

Du kan uppdatera ett befintligt projekt, en uppgift eller ett problem med information från ett e-postmeddelande som inte är [!DNL Adobe Workfront].

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Standard</p><p>Arbeta eller högre</p>
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Innan du kan uppdatera ett [!DNL Workfront]-objekt med e-postinnehåll från [!DNL Google Workspace] måste du

* Installera [!DNL Workfront for Google Workspace]\
   Instruktioner finns i [Installera [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Uppdatera ett [!DNL Workfront]-objekt med e-postinnehåll från [!DNL Google Workspace]

1. Om panelen [!UICONTROL Workfront for Google Workspace] inte visas klickar du på Workfront-ikonen ![ Workfront-ikonen ](assets/wf-lion-icon.png) i sidofältet för [!DNL Google Workspace] tillägg längst till höger på sidan.
1. Öppna e-postmeddelandet i [!DNL Google Workspace] och klicka på **[!UICONTROL Post as a new update]** på panelen [!DNL Google Workspace].
1. Klicka på listrutepilen under **[!UICONTROL Type]** och klicka sedan på den typ av objekt där du vill lägga till uppdateringen.
1. Klicka på alternativet **[!UICONTROL Search for]**, börja skriva namnet på objektet där du vill lägga till uppdateringen och markera sedan objektet när det visas i listan nedan.

   Det här alternativet varierar beroende på vad du valde i steg 3. Det kan vara **[!UICONTROL Search for a project]**, **[!UICONTROL Search for a task]** eller **[!UICONTROL Search for an issue]**.

   >[!NOTE]
   >
   >När du skriver namnet på en uppgift tas personliga uppgifter inte med i namnlistan som visas nedan.

1. Gör någon av dessa valfria ändringar:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Update]</td> 
      <td>Redigera valfri del av den här texten, som hämtas från e-postmeddelandets ämnesrad och brödtext.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email attachments]</td> 
      <td><p>(Endast tillgängligt om e-postmeddelandet innehåller minst en bifogad fil.) Klicka på det här alternativet om du vill spara bifogade filer på fliken [!UICONTROL Documents] för uppgiften eller problemet. </p><p>Om du inte vill spara en bifogad fil klickar du på krysset till höger om namnet. </p><p>Om e-postmeddelandet innehåller länkar till dokument i [!DNL Google Drive] sparas länkarna på fliken [!UICONTROL Overview] för den uppgift eller det problem som du skapar. </p><p>Viktigt: <span style="color: #ff1493;"><span style="color: #000000;">För att det här ska fungera måste </span></span>[!DNL Workfront]-administratören<span style="color: #ff1493;"><span style="color: #000000;"> godkänna att [!DNL Google Drive] arbetar med [!DNL Workfront]</span></span></p>
      <p>Om du aktiverar det här alternativet förblir det aktiverat för andra e-postmeddelanden som du konverterar till uppgifter, utgåvor och uppdateringar.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Meddela</td> 
      <td>Klicka på <strong>[!UICONTROL Notify]</strong>, klicka på alternativet <strong>[!UICONTROL Search for a user or team]</strong> som visas och börja sedan skriva namnet på personen eller teamet och klicka på det när det visas i listan nedan. Upprepa detta för varje person och team som du vill lägga till och klicka sedan på <strong>[!UICONTROL Save]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **[!UICONTROL Update]**.

   När du uppdaterar webbläsaren bekräftar ett meddelande med en länk längst ned på panelen [!DNL Workfront for Google Workspace] att du har konverterat e-postmeddelandet till en uppdatering:

   Du kan klicka på länken för att gå till fliken [!UICONTROL Updates] i [!DNL Workfront] för objektet som du angav i steg 4.

   Du kan upprepa de här stegen för att konvertera samma e-post till uppdateringar, uppgifter och utgåvor (se [Skapa ett Adobe Workfront-problem i [!DNL Google Workspace] med e-postinnehåll](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md)). När du uppdaterar webbläsaren eller återgår till e-postmeddelandet vid ett senare tillfälle visas alla länkar som du har skapat för e-postmeddelandet längst ned på panelen [!UICONTROL Workfront for Google Workspace].

1. (Valfritt) Fortsätt att arbeta med uppdateringen på tilläggspanelen [!DNL Workfront] genom att göra något av följande:

   * Om du vill lägga till en ny uppdatering på fliken **[!UICONTROL Updates]** klickar du på **[!UICONTROL Start a new update]** och skriver informationen.

   * Om du vill svara på en uppdatering på fliken **[!UICONTROL Updates]** klickar du på **[!UICONTROL Reply]** och skriver in ditt svar.

     För båda alternativen ovan kan du klicka på **[!UICONTROL Notify]** för att ange mottagare för svaret som i steg 5. När du är klar klickar du på **[!UICONTROL Post]** för att lägga till uppdateringen eller svaret.

   * Klicka på fliken **[!UICONTROL Details]** om du vill visa information om det nya projektet, aktiviteten eller problemet.

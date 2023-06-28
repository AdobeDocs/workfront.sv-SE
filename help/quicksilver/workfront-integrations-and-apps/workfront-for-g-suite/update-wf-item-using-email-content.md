---
product-area: workfront-integrations;projects
keywords: google,doc,dokument,ark,bild
navigation-topic: workfront-for-g-suite
title: Uppdatera en [!DNL Adobe Workfront] objekt från G Suite med e-postinnehåll
description: Du kan uppdatera ett befintligt projekt, en uppgift eller ett problem med information från ett e-postmeddelande som inte kommer från Adobe Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 4b95828dc3e6a67c4dbefb46f173303c519643a9
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 0%

---

# Uppdatera en [!DNL Adobe Workfront] objekt från [!DNL G Suite] använda e-postinnehåll

>[!NOTE]
>
>Den senaste versionen av Adobe Workfront-pluginprogrammet för Google släpptes den 26 juni 2023.

Du kan uppdatera ett befintligt projekt, en befintlig uppgift eller ett befintligt problem med information från en icke-[!DNL Adobe Workfront] e-post.

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

Innan du kan uppdatera en [!DNL Workfront] objekt med e-postinnehåll från [!DNL G Suite]måste du

* Installera [!DNL Workfront for G suite]\
   Instruktioner finns i [Installera [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Uppdatera en [!DNL Workfront] objekt med e-postinnehåll från [!DNL G Suite]

1. Om [!UICONTROL Workfront for G Suite] visas inte. Klicka på Workfront-ikonen ![](assets/wf-lion-icon.png) i [!DNL G Suite] sidofältet för tillägg längst till höger på sidan.
1. Med e-postmeddelandet öppet i [!DNL G Suite], klicka **[!UICONTROL Post as a new update]** i [!DNL G Suite] -panelen.
1. Under **[!UICONTROL Type]** klickar du på listrutepilen och sedan på den typ av objekt där du vill lägga till uppdateringen.
1. Klicka på **[!UICONTROL Search for]** börjar du skriva namnet på objektet där du vill lägga till uppdateringen och markerar sedan objektet när det visas i listan nedan.

   Det här alternativet varierar beroende på vad du valde i steg 3. Det kan vara **[!UICONTROL Search for a project]**, **[!UICONTROL Search for a task]**, eller **[!UICONTROL Search for an issue]**.

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
      <td><p>(Endast tillgängligt om e-postmeddelandet innehåller minst en bifogad fil.) Klicka på det här alternativet om du vill spara bilagor i [!UICONTROL Documents] för uppgiften eller problemet. </p><p>Om du inte vill spara en bifogad fil klickar du på krysset till höger om namnet. </p><p>Om e-postmeddelandet innehåller länkar till dokument i [!DNL Google Drive], sparas länkarna i [!UICONTROL Overview] -fliken för den uppgift eller det problem som du skapar. </p><p>Viktigt: <span style="color: #ff1493;"><span style="color: #000000;">För att det ska fungera</span></span>[!DNL Workfront] administratör<span style="color: #ff1493;"><span style="color: #000000;"> måste auktorisera [!DNL Google Drive] att arbeta med [!DNL Workfront]</span></span></p>
      <p>Om du aktiverar det här alternativet förblir det aktiverat för andra e-postmeddelanden som du konverterar till uppgifter, utgåvor och uppdateringar.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Meddela</td> 
      <td>Klicka <strong>[!UICONTROL Notify]</strong>klickar du på <strong>[!UICONTROL Search for a user or team]</strong> som visas börjar du skriva namnet på personen eller teamet och klickar på det när det visas i listan nedan. Upprepa detta för varje person och team som du vill lägga till och klicka sedan på <strong>[!UICONTROL Save]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **[!UICONTROL Update]**.

   När du uppdaterar webbläsaren visas ett meddelande med en länk längst ned i [!DNL Workfront for G Suite] bekräftar du att du har konverterat e-postmeddelandet till en uppdatering:

   Du kan klicka på länken för att gå till [!UICONTROL Updates] tabba in [!DNL Workfront] för det objekt som du angav i steg 4.

   Du kan upprepa de här stegen för att konvertera samma e-post till uppdateringar, uppgifter och problem (se [Skapa ett Adobe Workfront-problem i [!DNL G Suite] med e-postinnehåll](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md)). När du uppdaterar webbläsaren eller återgår till e-postmeddelandet vid ett senare tillfälle visas alla länkar som du har skapat för e-postmeddelandet längst ned i [!UICONTROL Workfront for G Suite] -panelen.

1. (Valfritt) Fortsätt arbeta med uppdateringen i dialogrutan [!DNL Workfront] tilläggspanelen på något av följande sätt:

   * Lägga till en ny uppdatering på **[!UICONTROL Updates]** flik, klicka **[!UICONTROL Start a new update]** och ange informationen.

   * Svara på en uppdatering på **[!UICONTROL Updates]** flik, klicka **[!UICONTROL Reply]** och skriv in ditt svar.

     För båda alternativen ovan kan du klicka **[!UICONTROL Notify]** för att ange mottagare för svaret som i steg 5. När du är klar klickar du på **[!UICONTROL Post]** för att lägga till uppdateringen eller svaret.

   * Klicka på **[!UICONTROL Details]** för att visa information om det nya projektet, uppgiften eller utgåvan.

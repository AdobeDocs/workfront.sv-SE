---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Skicka [!DNL Adobe Workfront] förfrågningar från [!DNL Microsoft] team
description: När teamägaren har installerat Adobe Workfront för Microsoft Teams kan du skicka in Workfront-förfrågningar från ditt Microsoft Teams-konto. För att kunna göra det måste du ha ett Workfront-konto med tillgång till förfrågningar. Mer information om hur du installerar Workfront för Microsoft Teams finns i Installera Workfront för Microsoft Teams.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5975d773-eae6-44ae-8296-2013504da3a8
source-git-commit: 75c4baf5ceca53f7ba85ffcc34876bca1238c9de
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# Skicka [!DNL Adobe Workfront] förfrågningar från [!DNL Microsoft] team

>[!IMPORTANT]
>
>När Microsoft går över till New Teams-klienten är Classic Teams-klienten inte längre tillgänglig efter 1 juli 2025. Vi håller på att utveckla en ny version av Microsoft Teams-integreringen som är helt kompatibel med nya Teams-klienten och som är tillgänglig före 1 juli för att säkerställa en smidig övergång.
>
>Instruktioner om hur du hämtar och installerar integreringen i New Teams-klienten visas här när integreringen är tillgänglig.

När teamägaren har installerat [!DNL Adobe Workfront for Microsoft Teams] kan du skicka [!DNL Workfront] förfrågningar från ditt [!DNL Microsoft Teams]-konto. För att kunna göra det måste du ha ett Workfront-konto med tillgång till förfrågningar. Mer information om hur du installerar [!DNL Workfront for Microsoft Teams] finns i [Installera [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

>[!NOTE]
>
>[!DNL Microsoft Teams] stöder inte längre [!DNL Internet Explorer]. Om du vill använda [!DNL Adobe Workfront for Microsoft Teams integration] måste du använda en annan webbläsare än [!DNL Internet Explorer].


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
   <td> <p>Arbete, Planera, Granska, Begäran</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Din [!DNL Microsoft Teams]-teamägare måste installera [!DNL Workfront] för [!DNL Microsoft Teams] innan du kan använda det.

## Skicka [!DNL Workfront] förfrågningar från [!DNL Microsoft Teams]

1. Klicka på ikonen **[!UICONTROL More added apps]** (tre punkter) i det vänstra navigeringsfältet i [!DNL Microsoft Teams].

1. Klicka på **[!DNL Workfront]** i listan som visas.
1. Klicka på fliken **[!UICONTROL Requests]**.
1. Klicka på **[!UICONTROL New Request]**.
1. I rutan **[!UICONTROL Select a Request Type]** väljer du den begärandekö där du vill skicka begäran.
1. (Valfritt) Välj en ämnesgrupp eller ett ämne i kön om de är tillgängliga i kön.
1. Ange följande information:

   (Beroende på hur kön med begäranden har konfigurerats kan alternativen och rutorna som visas variera. En fullständig lista och beskrivning av möjliga fält finns i [Skapa och skicka [!DNL Adobe Workfront] förfrågningar](../../manage-work/requests/create-requests/create-submit-requests.md).)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ämne</td> 
      <td>Skriv ett ämnesnamn för begäran.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>Ange en beskrivning för begäran.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> <p>Bifoga alla dokument som du vill inkludera i begäran. Du kan bifoga dokument genom att dra och släppa eller genom att klicka på [!UICONTROL Select file] och bläddra till och markera dokumentet i filsystemet.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Om administratören av [!DNL Workfront] kopplade anpassade formulär till kön med förfrågningar anger du informationen i fälten som är tillgängliga för anpassade formulär.
1. De anpassade formulären visas längst ned i den nya begäran.
1. Klicka på **[!UICONTROL Submit]**.

   Begäran visas i [!DNL Workfront] i den angivna begärandekön. Du får en bekräftelse på att begäran har skickats.

## Visa [!DNL Workfront] förfrågningar som du har skickat in [!DNL Microsoft Teams]

1. Klicka på ikonen **[!UICONTROL More added apps]** (tre punkter) i det vänstra navigeringsfältet i [!DNL Microsoft Teams].

1. Klicka på **[!DNL Workfront]** i listan som visas.
1. Klicka på fliken **[!UICONTROL Requests]**.

   Begäranden som du har skickat visas i området [!UICONTROL My submitted requests] på fliken [!UICONTROL Requests]. Du kan inte konfigurera den information som visas på den här fliken om de begäranden som du har skickat.

   Du kan visa följande information om dina skickade begäranden i [!UICONTROL My submitted requests]-området på fliken [!UICONTROL Requests]:

   * **[!UICONTROL Subject]**: Namnet på begäran
   * **[!UICONTROL Reference number]**
   * **[!UICONTROL Request type]**: Namnet på den begärandekö där du skickade begäran
   * **[!UICONTROL Status]**
   * **[!UICONTROL Submitted on]**: Datumet då du skickade begäran
   * **[!UICONTROL Assigned to]**

1. (Valfritt) Klicka på rubriken för någon av kolumnerna i listan för att sortera listan efter den kolumnen. Som standard sorterar [!DNL Workfront] listan efter datumet [!UICONTROL Submitted on], med början vid den senast skickade begäran.

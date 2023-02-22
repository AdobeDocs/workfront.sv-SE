---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Skicka [!DNL Adobe Workfront] förfrågningar från [!DNL Microsoft] Team
description: När teamägaren har installerat Adobe Workfront för Microsoft Teams kan du skicka in Workfront-begäranden från ditt Microsoft Teams-konto. För att kunna göra det måste du ha ett Workfront-konto med tillgång till förfrågningar. Mer information om hur du installerar Workfront för Microsoft Teams finns i Installera Workfront för Microsoft Teams.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5975d773-eae6-44ae-8296-2013504da3a8
source-git-commit: 473a1fe3cb7e247749d9b540e3e5556cbe17a1dd
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 0%

---

# Skicka [!DNL Adobe Workfront] förfrågningar från [!DNL Microsoft] Team

När teamägaren har installerat [!DNL Adobe Workfront for Microsoft Teams]kan du skicka in [!DNL Workfront] förfrågningar från [!DNL Microsoft Teams] konto. För att kunna göra det måste du ha ett Workfront-konto med tillgång till förfrågningar. Mer information om installation [!DNL Workfront for Microsoft Teams], se [Installerar [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

>[!NOTE]
>
>[!DNL Microsoft Teams] stöder inte längre [!DNL Internet Explorer]. Så här använder du [!DNL Adobe Workfront for Microsoft Teams integration]måste du använda en annan webbläsare än [!DNL Internet Explorer].


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
   <td> <p>Arbete, Planera, Granska, Begär</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Förutsättningar

Dina [!DNL Microsoft Teams] teamägaren måste installera [!DNL Workfront] for [!DNL Microsoft Teams] innan du kan använda den.

## Skicka [!DNL Workfront] förfrågningar från [!DNL Microsoft Teams]

1. Klicka på **[!UICONTROL More added apps]** (tre punkter) ikon i det vänstra navigeringsfältet i [!DNL Microsoft Teams].

1. Klicka **[!DNL Workfront]** i listan som visas.
1. Klicka på **[!UICONTROL Requests]** -fliken.
1. Klicka på **[!UICONTROL New Request]**.
1. I **[!UICONTROL Select a Request Type]** markerar du den begärandekö där du vill skicka begäran.
1. (Valfritt) Välj en ämnesgrupp eller ett ämne i kön om de är tillgängliga i kön.
1. Ange följande information:

   (Beroende på hur kön med begäranden har konfigurerats kan alternativen och rutorna som visas variera. En fullständig lista och en beskrivning av möjliga fält finns på [Skapa och skicka [!DNL Adobe Workfront] förfrågningar](../../manage-work/requests/create-requests/create-submit-requests.md).)

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
      <td> <p>Bifoga alla dokument som du vill inkludera i begäran. Du kan bifoga dokument genom att dra och släppa eller genom att klicka [!UICONTROL Select file] och bläddra till och markera dokumentet i filsystemet.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Om [!DNL Workfront] administratör kopplade anpassade formulär till begärandekön. Ange informationen i fälten som finns i de anpassade formulären.
1. De anpassade formulären visas längst ned i den nya begäran.
1. Klicka på **[!UICONTROL Submit]**.

   Begäran visas i [!DNL Workfront], i den angivna begärandekön. Du får en bekräftelse på att begäran har skickats.

## Visa [!DNL Workfront] du skickade in [!DNL Microsoft Teams]

1. Klicka på **[!UICONTROL More added apps]** (tre punkter) ikon i det vänstra navigeringsfältet i [!DNL Microsoft Teams].

1. Klicka **[!DNL Workfront]** i listan som visas.
1. Klicka på **[!UICONTROL Requests]** -fliken.

   Begäranden du har skickat visas i [!UICONTROL My submitted requests] området på [!UICONTROL Requests] -fliken. Du kan inte konfigurera den information som visas på den här fliken om de begäranden som du har skickat.

   Du kan visa följande information om dina skickade förfrågningar i [!UICONTROL My submitted requests] området på [!UICONTROL Requests] tab:

   * **[!UICONTROL Subject]**: Namnet på begäran
   * **[!UICONTROL Reference number]**
   * **[!UICONTROL Request type]**: Namnet på den begärandekö där du skickade begäran
   * **[!UICONTROL Status]**
   * **[!UICONTROL Submitted on]**: Datumet då du skickade din begäran
   * **[!UICONTROL Assigned to]**

1. (Valfritt) Klicka på rubriken för någon av kolumnerna i listan för att sortera listan efter den kolumnen. Som standard [!DNL Workfront] sorterar listan efter [!UICONTROL Submitted on] datum, med början från den senast skickade begäran.

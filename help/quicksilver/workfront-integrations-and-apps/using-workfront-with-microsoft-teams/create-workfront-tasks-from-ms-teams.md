---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Skapa [!DNL Adobe Workfront] aktiviteter från [!DNL Microsoft] team
description: Du kan skapa personliga uppgifter i Adobe [!DNL Workfront]  från Microsoft Teams om en teamägare har installerat och konfigurerat  [!DNL Workfront]  för Microsoft Teams för ditt team och du är inloggad på Workfront från Microsoft Teams.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 31b86c8d-967a-446a-86f2-3d38e44c45e1
source-git-commit: 1f2655c0e88a5cc918501e2a0ef830758111ded8
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Skapa [!DNL Adobe Workfront] aktiviteter från [!DNL Microsoft Teams]

>[!NOTE]
>
>Integreringen av Adobe Workfront för Microsoft Teams stöds för närvarande bara för den klassiska Microsoft Teams.

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

Du kan skapa personliga uppgifter i [!DNL Adobe Workfront] från [!DNL Microsoft Teams] om följande villkor uppfylls:

* En teamägare har installerat och konfigurerat [!DNL Workfront for Microsoft Teams] för ditt team.
* Du är inloggad på [!DNL Workfront] från [!DNL Microsoft Teams].

>[!NOTE]
>
>[!DNL Microsoft Teams] stöder inte längre [!DNL Internet Explorer]. Om du vill använda integreringen av [!DNL Adobe Workfront for Microsoft Teams] måste du använda en annan webbläsare än [!DNL Internet Explorer].

Information om hur du installerar [!DNL Workfront for Microsoft Teams] och loggar in på [!UICONTROL Workfront] från [!DNL Microsoft Teams] finns i [Installera [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## Skapa personliga uppgifter från [!DNL Microsoft Teams]

1. Logga in på [!DNL Workfront] från [!DNL Microsoft Teams].

   Mer information om hur du loggar in på [!DNL Workfront] finns i [Installera [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. Så här öppnar du ett **[!UICONTROL New task]**-kort:

   * Om du befinner dig i den [!DNL Workfront] båda chattkanalen skriver du **[!UICONTROL New task]** i fältet [!UICONTROL conversation] för att skapa en ny uppgift.
   * Om du befinner dig i en annan chattkanal än [!DNL Workfront]-chattkanalen:

      * Börja skriva **[!DNL @workfront]** i fältet [!UICONTROL conversation] och välj sedan den [!DNL Workfront]-robotkanal du vill använda.
      * Fortsätt skriva **[!UICONTROL New task]** i fältet [!UICONTROL conversation] för att skapa en ny uppgift.

        Kortet [!UICONTROL New task] visas i robotkanalen [!DNL Workfront].

        ![ms_teams_new_task_card.png](assets/ms-teams-new-task-card-350x181.png)

1. Ange följande information på [!UICONTROL New task]-kortet i [!UICONTROL Workfront]-robotkanalen:

   * Uppgiftsnamn i fältet **[!UICONTROL Write the task's title]**.
   * Uppgiftsbeskrivning i fältet **[!UICONTROL Write the tasks's description]**.
   * Det datum då aktiviteten måste slutföras av, i fältet **[!UICONTROL Due Date]**.

1. Klicka på **[!UICONTROL Save].**

   Den nya personliga aktiviteten skapas i [!DNL Workfront]. Ett [!UICONTROL Reference Number] har tilldelats det och är synligt på kortet [!UICONTROL new task].

   Mer information om referensnummer finns i avsnittet [[!UICONTROL Reference Numbers] av objekt ](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-reference-numbers-of-objects) i artikeln [Förstå objekt i [!DNL Adobe Workfront]](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Valfritt) Klicka på **[!UICONTROL Edit]** om du vill redigera aktivitetsinformationen ytterligare.
1. (Valfritt) Klicka på **[!UICONTROL View in [!DNL Workfront]]** om du vill öppna uppgiften på en ny flik i [!DNL Workfront] och redigera aktiviteten ytterligare, flytta den till ett projekt eller tilldela den till någon annan.

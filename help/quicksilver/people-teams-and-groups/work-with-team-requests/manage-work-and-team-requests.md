---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Hantera arbets- och teamförfrågningar
description: En begäran representerar en väntande aktivitet eller utleverans. Arbetsförfrågningar görs till enskilda personer, och teamförfrågningar görs till team.
author: Lisa
feature: People Teams and Groups, Work Management
exl-id: ef96e520-0d5f-4180-a27a-1fbbffff8f2b
source-git-commit: 9693ac3792fec3eca6218a228f2067519ed433ac
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---

# Hantera arbets- och teamförfrågningar

En begäran representerar en väntande aktivitet eller utleverans. Arbetsförfrågningar görs till enskilda personer, och teamförfrågningar görs till team.

>[!NOTE]
>
>Agile-team har inga teamförfrågningar.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>Granska eller senare för att tilldela eller arbeta med en begäran. Arbeta eller senare för att tilldela om en begäran</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Om du vill ta reda på vilken plan eller licenstyp du har kontaktar du [!DNL Workfront] administratör.

## Tilldela en förfrågan till ett team {#assign-a-request-to-a-team}

Projektledare och begärande kan tilldela team arbete när de inte vet vilken resurs som är rätt att utföra arbetet eller när det inte spelar någon roll vem som slutför arbetet.

Uppgifter som tilldelats teamet finns kvar på [!UICONTROL Team Requests] tills en användare i teamet kan arbeta med begäran.

När en begäran har tilldelats både ett team och en användare som inte är medlem i teamet visas begäran i båda [!UICONTROL Team Requests] -fliken och i användarens arbetsförfrågningsområde. Om den användare som inte är medlem i teamet arbetar med uppgiften är uppgiften fortfarande kvar i [!UICONTROL Team Requests] tills en användare i teamet kan arbeta med det.

Team kan tilldelas till uppgifter och ärenden på något av följande sätt:

* Via [!UICONTROL Gantt Chart]
* Från en aktivitet eller en utleveranslista (individuellt eller gruppvis)
* När en uppgift eller ett problem skapas eller ändras
* Genom routningsregler för en begäran (endast utgåvor)

Du kan manuellt tilldela en begäran till ett team från teamsidan, enligt beskrivningen i det här avsnittet.

Så här tilldelar du en förfrågan till ett team manuellt från teamsidan:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Teams]**.

1. Klicka på **[!UICONTROL Switch team]** icon ![Byt ikon för team](assets/switch-team-icon.png)väljer du sedan ett nytt team i listrutan eller söker efter ett team i sökfältet.

1. Klicka på **[!UICONTROL More]** icon ![](assets/more-icon.png)väljer **[!UICONTROL Send work request]**.

   ![](assets/edit-team-settings-350x205.png)

1. Fyll i informationen i rutan som öppnas.
1. Klicka på **[!UICONTROL Send Request]**.\
   Teamet har nu tilldelats en ny uppgift som visas på fliken Teamförfrågningar. Den här aktiviteten är för närvarande inte kopplad till ett projekt, men den kan flyttas enligt beskrivningen i [Flytta uppgifter](../../manage-work/tasks/manage-tasks/move-tasks.md).

## Tilldela om begäranden {#reassign-requests}

Du kan tilldela om begäranden som har tilldelats ditt team:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Teams]**.
1. Klicka på **[!UICONTROL Switch team]** icon ![Byt ikon för team](assets/switch-team-icon.png)väljer du sedan ett nytt team i listrutan eller söker efter ett team i sökfältet.
1. Välj **[!UICONTROL Team Requests]**.
1. Klicka på **[!UICONTROL Reassign]** ikon.

1. Börja skriva namnet på den användare, grupp eller team som du vill tilldela om begäran till och klicka sedan på **[!UICONTROL Assign]**.\
   Begäran har omtilldelats.

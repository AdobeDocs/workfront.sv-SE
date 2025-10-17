---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Hantera arbets- och teamförfrågningar
description: En begäran representerar en väntande aktivitet eller utleverans. Arbetsförfrågningar görs till enskilda personer, och teamförfrågningar görs till team.
author: Jenny
feature: People Teams and Groups, Work Management
exl-id: ef96e520-0d5f-4180-a27a-1fbbffff8f2b
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Hantera arbets- och teamförfrågningar

En begäran representerar en väntande aktivitet eller utleverans. Arbetsförfrågningar görs till enskilda personer, och teamförfrågningar görs till team.

>[!NOTE]
>
>Agile-team har inga teamförfrågningar.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p>Så här tilldelar du eller arbetar med en begäran:
   <p>Ljus eller högre</p>
  <p>Granska eller högre</p>
   <p>Så här tilldelar du om en begäran:
   <p>Standard</p>
   <p>Arbeta eller högre</p></td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tilldela en förfrågan till ett team {#assign-a-request-to-a-team}

Projektledare och begärande kan tilldela team arbete när de inte vet vilken resurs som är rätt att utföra arbetet eller när det inte spelar någon roll vem som slutför arbetet.

Uppgifter som tilldelats teamet finns kvar på fliken [!UICONTROL Team Requests] tills en användare i teamet kan arbeta med begäran.

När en begäran har tilldelats både ett team och en användare som inte är medlem i teamet, visas begäran både på fliken [!UICONTROL Team Requests] och i användarens arbetsförfrågningsområde. Om användaren som inte är medlem i teamets frivilliga för att arbeta med uppgiften, finns uppgiften kvar på fliken [!UICONTROL Team Requests] tills en användare i teamets frivilliga för att arbeta med den.

Team kan tilldelas till uppgifter och ärenden på något av följande sätt:

* Genom [!UICONTROL Gantt Chart]
* Från en aktivitet eller en utleveranslista (individuellt eller gruppvis)
* När en uppgift eller ett problem skapas eller ändras
* Genom routningsregler för en begäran (endast utgåvor)

Du kan manuellt tilldela en begäran till ett team från teamsidan, enligt beskrivningen i det här avsnittet.

Så här tilldelar du en förfrågan till ett team manuellt från teamsidan:

{{step1-to-team}}

1. Klicka på ikonen **[!UICONTROL Switch team]** ![Byt ikon för team](assets/switch-team-icon.png) och välj sedan ett nytt team i listrutan eller sök efter ett team i sökfältet.

1. Klicka på ikonen **[!UICONTROL More]** ![](assets/more-icon.png) och välj sedan **[!UICONTROL Send work request]**.

   ![](assets/edit-team-settings-350x205.png)

1. Fyll i informationen i rutan som öppnas.
1. Klicka på **[!UICONTROL Send Request]**.\
   Teamet har nu tilldelats en ny uppgift som visas på fliken Teamförfrågningar. Den här aktiviteten är för närvarande inte associerad med ett projekt, men den kan flyttas enligt beskrivningen i [Flytta aktiviteter](../../manage-work/tasks/manage-tasks/move-tasks.md).

## Tilldela om begäranden {#reassign-requests}

Du kan tilldela om begäranden som har tilldelats ditt team:

{{step1-to-team}}

1. Klicka på ikonen **[!UICONTROL Switch team]** ![Byt ikon för team](assets/switch-team-icon.png) och välj sedan ett nytt team i listrutan eller sök efter ett team i sökfältet.
1. Välj **[!UICONTROL Team Requests]** i den vänstra navigeringspanelen.
1. Klicka på ikonen **[!UICONTROL Reassign]**.

1. Börja skriva namnet på den användare, grupp eller det team som du vill tilldela om begäran till och klicka sedan på **[!UICONTROL Assign]**.\
   Begäran har omtilldelats.

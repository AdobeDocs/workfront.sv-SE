---
product-area: agile-and-teams
navigation-topic: work-in-an-agile-environment
title: Hantera den flexibla eftersläpningen
description: Uppgifter och ärenden kan tilldelas ett smidigt team och läggas till i teamets eftersläpning som berättelser, beroende på den flexibla metod teamet använder.
author: Lisa
feature: Agile
exl-id: 59660840-7ab8-482e-8b43-96b4a1ecc538
source-git-commit: b855f032b24079ff27435fb833cd3ed8a382a77c
workflow-type: tm+mt
source-wordcount: '1283'
ht-degree: 0%

---

# Hantera den flexibla eftersläpningen

Följande arbetsuppgifter kan tilldelas ett smidigt team och läggas till i teamets eftersläpning som artiklar, beroende på den flexibla metod teamet använder:

* **[!UICONTROL Scrum agile teams]:** Uppgifter och ärenden kan tilldelas det flexibla teamet och läggas till i eftersläpningen.
* **[!UICONTROL Kanban agile teams]:** Uppgifter kan tilldelas det flexibla teamet och läggas till i eftersläpningen. Användare kan visa eftersläpningen direkt från den flexibla artikelpanelen enligt beskrivningen i [[!UICONTROL Add the backlog] till Kanban-tavlan](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md). Teamet använder denna eftersläpning för att prioritera och hantera sin arbetskö.

Uppgifter eller problem kan tilldelas teamet (och sedan läggas till i teamets eftersläpning) var som helst i [!DNL Adobe Workfront]. Ett team kan till exempel tilldelas arbetsuppgifter från flera projekt.

>[!NOTE]
>
>Om du lägger till flera team i ett eftersläpningsobjekt visas uppgiften eller problemet endast i det primära teamets eftersläpning. Det primära teamet är det som först tilldelats.

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
   <td> <p>[!UICONTROL Work] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>[!UICONTROL Worker] eller högre</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>[!UICONTROL Manage] åtkomst till det projekt som artikeln är på</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Skapa och hantera artiklar i efterloggen

* [Ordna om artiklar](#reorder-stories)
* [[!UICONTROL Break] ned berättelser](#break-down-stories)
* [Redigera artiklar](#edit-stories)
* [Skapa nya artiklar i eftersläpningen](#create-new-stories-on-the-backlog)
* [Flytta artiklar från eftersläpningen till en iteration eller en kanban-panel](#move-stories-from-the-backlog-to-an-iteration-or-kanban-board)

### Ordna om artiklar {#reorder-stories}

Du kan ändra ordning på artiklarna i eftersläpningslistan genom att dra och släppa.

1. Gå till den flexibla eftersläpningen där du vill ändra ordning på artiklarna.
1. I **[!UICONTROL View]** väljer du **[!UICONTROL Backlog]** eller en anpassad vy som innehåller **[!UICONTROL Order]** kolumn.

   >[!NOTE]
   >
   >Om en uppgift eller ett ärende har tilldelats ett rörligt team och projektet inte har en status som motsvarar Aktuell, visas de inte i eftersläpningen. De påverkar dock fortfarande antalet eftersläpningar i kolumnen Ordning.

1. Markera en eller flera artiklar och dra dem sedan till den ordning som du vill att de ska visas i eftersläpningen.\
   ![Dra och släpp eftersläpningsobjekt](assets/agile-backlog-drag-and-drop.png)

### Dela upp artiklar {#break-down-stories}

Eftersom artiklar i en eftersläpning varierar i storlek kan användarna dela upp dem i användbara storlekar för en upprepning. När du delar upp en artikel skapas underuppgifter för den uppgift som artikeln representerar och den ursprungliga uppgiften ersätts i eftersläpningen. Du kan ha en överordnad uppgift eller dess underaktiviteter tilldelade till ett smidigt team, men du kan inte ha båda samtidigt tilldelade till ett team.

>[!NOTE]
>
>Tänk på följande begränsningar när du delar upp artiklar:
>
>* Endast artiklar som representerar uppgifter kan delas upp. Du kan inte dela upp artiklar som representerar problem.
>* Artiklar kan bara delas upp om de är kopplade till ett projekt.



Så här bryter du ned en artikel:

1. Gå till den eftersläpning som innehåller artikeln som du vill bryta ned.
1. Markera artikeln som du vill dela upp och klicka sedan på **[!UICONTROL Breakdown Story]**.\
   The [!UICONTROL Breakdown Story] visas.\
   ![Dialogrutan Detaljerad artikel](assets/backlog-breakdown-dialog.png)

1. Ange ett namn och en uppskattning för artikeln och välj om artikeln är klar.
1. Klicka **[!UICONTROL Add Story]** om du vill skapa en ny artikel från originalartikeln.
1. Klicka på **[!UICONTROL Save]**.

### Redigera artiklar {#edit-stories}

Du kan redigera artiklar direkt från [!UICONTROL Stories] eller [!UICONTROL Issues] -flikar i eftersläpningen på samma sätt som du redigerar uppgifter eller problem i ett projekt i grupp, enligt beskrivningen i [Redigera flera uppgifter samtidigt](../../manage-work/tasks/manage-tasks/edit-tasks.md#editing-tasks-in-bulk) in [Redigera uppgifter](../../manage-work/tasks/manage-tasks/edit-tasks.md) och [Redigera problem](../../manage-work/issues/manage-issues/edit-issues.md#bulk-editing-issues) in [Redigera problem](../../manage-work/issues/manage-issues/edit-issues.md).

## Skapa nya artiklar i eftersläpningen {#create-new-stories-on-the-backlog}

Du kan skapa nya artiklar i eftersläpningen genom att skapa artikeln direkt från eftersläpningen eller genom att tilldela en befintlig uppgift eller utgåva till ett smidigt team.

* [Skapa en artikel från eftersläpningen](#create-a-story-from-the-backlog)
* [Tilldela en uppgift eller ett problem till ett smidigt team](#assign-a-task-or-issue-to-an-agile-team)

### Skapa en artikel från eftersläpningen {#create-a-story-from-the-backlog}

När du skapar en artikel från en eftersläpning skapas artikeln som en uppgift eller ett problem i ett projekt. Du kan inte skapa en artikel från eftersläpningen som ett problem.

Så här skapar du en artikel från en eftersläpning:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Teams]**.

1. (Valfritt) Klicka på **[!UICONTROL Switch team]** icon ![Byt ikon för team](assets/switch-team-icon.png)väljer du sedan ett nytt Scrum-team i listrutan eller söker efter ett team i sökfältet.

1. Välj **[!UICONTROL Backlog]** från den vänstra panelen.
1. Gör något av följande, beroende på om du vill skapa en uppgift eller ett problem:

   * **Så här skapar du en uppgift:** Klicka **[!UICONTROL Stories]**.

   * **Så här skapar du en utgåva:** Klicka **[!UICONTROL Issues]**.

1. Klicka **[!UICONTROL New Story]** eller **[!UICONTROL New Issue]**.

1. Ange följande information:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Story Name]</strong></td>
      <td> Ange ett namn för artikeln.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td>
      <td>(Valfritt) Skriv en beskrivning för artikeln.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td> Välj om artikeln är klar att läggas till i en iteration. Den här inställningen är endast informativ. Det går att lägga till artiklar i en iteration oavsett den här inställningens status.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimate]</strong></td>
      <td>Ange en punkt eller timuppskattning för artikeln. Uppskattningar påverkar nedladdningsdiagrammet. Nedbrytningsdiagrammet för en iteration är endast korrekt om varje artikel innehåller en korrekt uppskattning. (Om du anger en punktuppskattning måste du i gruppinställningarna ha angett hur många timmar varje punkt representerar.)</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Project]</strong></td>
      <td>Börja skriva namnet på det projekt där artikeln ska skapas och klicka sedan på namnet när det visas i listrutan.<br>Projektets status måste anges till [!UICONTROL Current]. Om projektets status är något annat än [!UICONTROL Current]visas den inte i listrutan.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Task]</strong></td>
      <td>(Valfritt) Börja skriva namnet på den överordnade uppgift som den här artikeln är underordnad för och klicka sedan på namnet när den visas i listrutan.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td> (Valfritt) Markera de anpassade formulär som du vill lägga till i artikeln.</td>
     </tr>
    </tbody>
   </table>

1. Klicka på **[!UICONTROL Save Story]**.

### Tilldela en uppgift eller ett problem till ett smidigt team {#assign-a-task-or-issue-to-an-agile-team}

Du kan tilldela en uppgift eller ett ärende till ett smidigt team. När uppgiften eller utgåvan har tilldelats visas den som en ny artikel i teamets eftersläpning.

Så här tilldelar du en uppgift eller ett ärende till ett smidigt team:

1. Gå till det projekt som innehåller uppgiften som du vill tilldela om.
1. Markera uppgiften eller utgåvan i listan.
1. Klicka på **[!UICONTROL Edit]**.
1. Klicka på **[!UICONTROL Assignments]**.
1. (Valfritt) Ta bort alla befintliga tilldelningar.
1. Klicka på **[!UICONTROL Add Assignee]**.
1. Börja skriva namnet på det flexibla team som du vill ska tilldelas uppgiften eller utgåvan och klicka sedan på teamnamnet när det visas i listrutan.
1. Klicka på **[!UICONTROL Save Changes]**.\
   Uppgiften eller utgåvan är nu tillgänglig i teamets eftersläpning.

## Flytta artiklar från eftersläpningen till en iteration eller + board {#move-stories-from-the-backlog-to-an-iteration-or-kanban-board}

* [Flytta befintliga artiklar till eftersläpningen](#move-existing-stories-to-the-backlog)
* [Exportera artiklar från eftersläpningen](#export-stories-from-the-backlog)

1. Gå till eftersläpningen i det flexibla teamet.
1. Markera de artiklar som du vill flytta till en iteration eller en kanban-panel och klicka sedan på **[!UICONTROL More]** > **[!UICONTROL Move to]**.\
   Om du flyttar artikeln till en [!UICONTROL Kanban] bräda [!UICONTROL Move Story to the Kanban] Kort visas.\
   Om du flyttar en artikel till en iteration [!UICONTROL Move Story to an Iteration] visas.\
   ![Dialogrutan Flytta artikel](assets/agile-backlog-addtoiteration.png)

1. Gör något av följande:

   * **För Scrum-team:** I **[!UICONTROL Select Iteration]** markerar du den iteration där du vill flytta artiklarna.

   * **För Kanban-team:** I **[!UICONTROL Select Kanban Board]** fält, välj ditt team [!UICONTROL Kanban] bräda. (Kanban-team kan bara ha ett [!UICONTROL Kanban] bräda.)

1. Klicka på **[!UICONTROL Move Story]**.

### Flytta befintliga artiklar till eftersläpningen {#move-existing-stories-to-the-backlog}

Om du bestämmer dig för att ditt team inte är redo att arbeta med en artikel kan du flytta artikeln till eftersläpningen.

Mer information finns i [Flytta en flexibel artikel](../../agile/work-in-an-agile-environment/move-an-agile-story.md).

### Exportera artiklar från eftersläpningen {#export-stories-from-the-backlog}

Du kan exportera en eller flera artiklar (inklusive uppgifter och ärenden) direkt från eftersläpningen.

Du exporterar artiklar från en eftersläpning på samma sätt som du exporterar andra data i [!DNL Workfront], enligt beskrivningen i [Exportera data](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

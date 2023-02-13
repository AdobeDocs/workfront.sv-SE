---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Skapa en flexibel artikel
description: Du kan skapa en flexibel artikel om en iteration på olika sätt. När du har skapat en flexibel artikel kan du lägga till underuppgifter i artikeln.
author: Lisa
feature: Agile
exl-id: d16ee940-3551-44da-8fe6-093f4fcac070
source-git-commit: 11009f24cd482e83319ed9f1ecf3f7a2f4e79d52
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 0%

---

# Skapa en flexibel artikel

Du kan skapa en flexibel artikel om en iteration på olika sätt. När du har skapat en flexibel artikel kan du lägga till underuppgifter i artikeln.

När du lägger till en artikel eller underuppgift i en iteration anges varaktighetstypen till [!UICONTROL Simple] och aktivitetsbegränsningen är inställd på Fasta datum, med datumen låsta i iteration. Du kan inte ändra varaktighetstypen eller aktivitetsbegränsningen i en iteration. Aktivitetens varaktighet måste också vara längre än 0 minuter.

Mer information om hur du hanterar artikeln när den har lagts till i den finns i [Iterationer](../../agile/use-scrum-in-an-agile-team/iterations/iterations.md).

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

## Skapa en flexibel artikel i en iteration

1. Gå till den smidiga upprepningen där du vill skapa artikeln:

   1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Teams]**.

   1. (Valfritt) Klicka på **[!UICONTROL Switch team]** icon ![Byt ikon för team](assets/switch-team-icon.png)väljer du sedan ett nytt Scrum-team i listrutan eller söker efter ett team i sökfältet.

   1. Välj **[!UICONTROL Iterations]** om du vill välja en viss upprepning, eller markera **[!UICONTROL Current Iteration]**.
   1. Klicka på namnet på den specifika upprepning där du vill skapa en artikel.

   ![Lägg till ny artikel i upprepning](assets/iteration-add-story.png)

1. Klicka på **[!UICONTROL New Story].**
1. Ange följande information:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Story Name]</strong></td>
      <td>Ange ett namn för artikeln.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td>
      <td>Skriv en beskrivning för artikeln.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td>Välj det här alternativet om artikeln är klar att läggas till i en iteration. När det här alternativet är markerat visar det för användarna vilka artiklar i efterloggen som är klara att läggas till i en iteration.<br>En artikel kan läggas till i en iteration oavsett om den är markerad eller inte <strong>[!UICONTROL Ready].</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimate] (punkter)</strong></td>
      <td>Ange uppskattningen för artikeln. Om ditt flexibla team är konfigurerat att uppskatta artiklar i poäng är standardvärdet 1 poäng 8 timmar. Beräkningar läggs till som [!UICONTROL Planned Hours] på storyn.<br>Om du till exempel beräknar att en artikel har tre punkter blir standardbeteendet att lägga till 24 [!UICONTROL Planned Hours] till historien.<br>Om en artikel innehåller underuppgifter måste du komma ihåg att den sammanlagda uppskattningen för alla underuppgifter avgör den överordnade artikelns uppskattning. Mer information finns i <a href="../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md" class="MCXref xref">Lägga till artiklar i en befintlig upprepning</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Project]</strong></td>
      <td>Börja skriva namnet på det projekt som den här artikeln ska kopplas till.<br>Som standard visas artikelfärgen som samma färg som andra artiklar i det här projektet.<br>Projektets status måste anges till [!UICONTROL Current]. Om projektets status är något annat än [!UICONTROL Current]visas den inte i listrutan.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Task]</strong></td>
      <td>När du har valt ett överordnat projekt kan du välja en överordnad uppgift. När du väljer en överordnad uppgift skapas artikeln som en underuppgift till den överordnade uppgiften i det projekt som du valde.<br>Börja skriva namnet på den överordnade uppgiften för artikeln och klicka sedan på den när den visas i listrutan.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td>Välj vilka anpassade formulär som ska läggas till i artikeln.</td>
     </tr>
    </tbody>
   </table>

1. Klicka på **[!UICONTROL Save Story]**.

## Skapa en flexibel artikel i eftersläpningen

Du kan skapa en smidig artikel utifrån den flexibla eftersläpningen enligt beskrivningen i avsnittet [Skapa nya artiklar i eftersläpningen](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#creating-new-stories) i artikeln [[!UICONTROL Manage] den flexibla eftersläpningen](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## Lägg till en uppgift eller ett problem som en smidig artikel

Du kan lägga till en befintlig uppgift eller ett befintligt problem som en artikel i en iteration. Mer information finns i [Lägga till artiklar i en befintlig upprepning](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md) eller [Lägg till artiklar och utgåvor från [!UICONTROL Scrum] board](../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Skapa underaktiviteter till en smidig artikel

Du kan skapa en underuppgift till en flexibel artikel på något av följande sätt:

* Genom att använda **[!UICONTROL Subtasks]** enligt beskrivning i [Skapa underaktiviteter](../../manage-work/tasks/create-tasks/create-subtasks.md#creating-subtasks) in [Skapa underaktiviteter](../../manage-work/tasks/create-tasks/create-subtasks.md).

* Direkt från artikelpanelen, enligt beskrivningen i [Skapa en iteration](../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

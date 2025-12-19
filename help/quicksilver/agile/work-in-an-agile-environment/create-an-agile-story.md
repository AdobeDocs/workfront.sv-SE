---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Skapa en Agile Story
description: Du kan skapa en flexibel artikel om en iteration på olika sätt. När du har skapat en flexibel artikel kan du lägga till underuppgifter i artikeln.
author: Jenny
feature: Agile
exl-id: d16ee940-3551-44da-8fe6-093f4fcac070
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# Skapa en Agile-artikel

Du kan skapa en Agile-artikel på en iteration på olika sätt. När du har skapat en Agile-artikel kan du lägga till underuppgifter i artikeln.

När du lägger till en artikel eller underaktivitet i en iteration anges varaktighetstypen till [!UICONTROL Simple] och aktivitetsbegränsningen anges till fasta datum, med datumen låsta i iteration. Du kan inte ändra varaktighetstypen eller aktivitetsbegränsningen i en iteration. Aktivitetens varaktighet måste också vara längre än 0 minuter.

Mer information om hur du hanterar artikeln när den har lagts till i iterationen finns i [Iterations](../../agile/use-scrum-in-an-agile-team/iterations/iterations.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Standard</p> 
   <p>Arbeta eller högre</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>Hantera åtkomst till det projekt som artikeln är på </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa en Agile-artikel i en iteration

1. Gå till den Agile-iteration där du vill skapa artikeln:

   {{step1-to-team}}

   1. (Valfritt) Klicka på ikonen **[!UICONTROL Switch team]** ![Byt team-ikon](assets/switch-team-icon.png) och välj sedan ett nytt Scrum-team i listrutan eller sök efter ett team i sökfältet.

   1. I den vänstra panelen väljer du **[!UICONTROL Iterations]** om du vill välja en viss iteration eller **[!UICONTROL Current Iteration]**.
   1. Klicka på namnet på den specifika upprepning där du vill skapa en artikel.

   ![Lägg till ny artikel i iteration](assets/iteration-stories-list.png)

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
      <td>Välj det här alternativet om artikeln är klar att läggas till i en iteration. När det här alternativet är markerat visar det för användarna vilka artiklar i efterloggen som är klara att läggas till i en iteration.<br>En artikel kan läggas till i en iteration oavsett om den är markerad som <strong>[!UICONTROL Ready] eller inte.</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimate] (punkter)</strong></td>
      <td>Ange uppskattningen för artikeln. Om ditt Agile-team är konfigurerat att uppskatta artiklar i poäng är standardvärdet 1 poäng 8 timmar. Uppskattningar läggs till som [!UICONTROL Planned Hours] i artikeln.<br>Om du till exempel uppskattar en artikel som 3 punkter är standardbeteendet att lägga till 24 [!UICONTROL Planned Hours] i artikeln.<br>Om en artikel innehåller underaktiviteter måste du komma ihåg att de kombinerade uppskattningarna för alla underaktiviteter avgör uppskattningen av den överordnade artikeln. Mer information finns i <a href="../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md" class="MCXref xref">Lägga till artiklar i en befintlig iteration</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Project]</strong></td>
      <td>Börja skriva namnet på det projekt som den här artikeln ska kopplas till.<br>Som standard visas artikelfärgen som samma färg som andra artiklar i det här projektet.<br>Projektets status måste anges till [!UICONTROL Current]. Om projektets status är något annat än [!UICONTROL Current] visas den inte i listrutan.</td>
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

## Skapa en Agile-artikel i eftersläpningen

Du kan skapa en Agile-artikel utifrån Agile-eftersläpningen, vilket beskrivs i avsnittet [Skapa nya artiklar på eftersläpningen](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#creating-new-stories) i artikeln [[!UICONTROL Manage] på Agile-eftersläpningen](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## Lägga till en aktivitet eller ett problem som en Agile-artikel

Du kan lägga till en befintlig uppgift eller ett befintligt problem som en artikel i en iteration. Mer information finns i [Lägga till artiklar i en befintlig iteration](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md) eller [Lägga till artiklar och utgåvor från [!UICONTROL Scrum] board](../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Skapa underaktiviteter till en Agile-artikel

Du kan skapa en underuppgift till en Agile-artikel på något av följande sätt:

* Genom att använda fliken **[!UICONTROL Subtasks]**, vilket beskrivs i [Skapa underaktiviteter](../../manage-work/tasks/create-tasks/create-subtasks.md#creating-subtasks) i [Skapa underaktiviteter](../../manage-work/tasks/create-tasks/create-subtasks.md).

* Direkt från artikelpanelen, enligt beskrivningen i [Skapa en iteration](../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

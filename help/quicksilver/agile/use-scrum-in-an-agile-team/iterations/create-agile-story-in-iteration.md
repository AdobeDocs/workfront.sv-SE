---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Skapa en flexibel artikel i en iteration
description: I den här artikeln beskrivs hur du skapar en ny, flexibel artikel när du redan är i iteration.
author: Lisa
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# Skapa en flexibel artikel i en iteration

I den här artikeln beskrivs hur du skapar en ny, flexibel artikel när du redan är i iteration. Mer information om hur du skapar en flexibel artikel från en aktivitet, ett problem eller något annat område i [!DNL Adobe Workfront] finns i [Lägga till artiklar i en befintlig iteration](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

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
   <td> <p>[!UICONTROL Worker] eller högre</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>[!UICONTROL Manage] åtkomst till det projekt som artikeln är på</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Skapa en flexibel artikel i en iteration

1. Gå till den smidiga upprepningen där du vill skapa artikeln:

   1. Klicka på ikonen **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe] Workfront och klicka sedan på **[!UICONTROL Teams]**.

   1. (Valfritt) Klicka på ikonen **[!UICONTROL Switch team]** ![Byt team-ikon](assets/switch-team-icon.png) och välj sedan ett nytt Scrum-team i listrutan eller sök efter ett team i sökfältet.

   1. Välj **[!UICONTROL Iterations]** i den vänstra panelen.
   1. Klicka på namnet på den specifika upprepning där du vill skapa en artikel.
   1. Välj **[!UICONTROL Stories]** i den vänstra panelen.

1.  Klicka på **[!UICONTROL New Story].**
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
      <td>Ange uppskattningen för artikeln. Om ditt flexibla team är konfigurerat att uppskatta artiklar i poäng är standardvärdet 1 poäng 8 timmar. Uppskattningar läggs till som [!UICONTROL Planned Hours] i artikeln.<br>Om du till exempel uppskattar en artikel som 3 punkter är standardbeteendet att lägga till 24 planerade timmar i artikeln.<br>Om en artikel innehåller underaktiviteter måste du komma ihåg att de kombinerade uppskattningarna för alla underaktiviteter avgör uppskattningen av den överordnade artikeln. Mer information finns i <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/add-a-subtask-to-an-existing-story-scrum.md" class="MCXref xref">Lägga till en underaktivitet i en befintlig artikel på [!UICONTROL Scrum] board</a>.</td>
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

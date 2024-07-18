---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Lägga till en underuppgift i en befintlig artikel på Urvalsritytan
description: När du skapar underaktiviteter för befintliga artiklar bör du tänka på inställningen för Slutförandeläge för projektet, eftersom detta påverkar hur artiklarna uppdateras.
author: Lisa
feature: Agile
exl-id: 264e66e9-94c7-4904-baad-f733d39b4791
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---

# Lägg till en underaktivitet i en befintlig artikel på [!UICONTROL Scrum]-panelen

Tänk på följande när du skapar underuppgifter för befintliga artiklar:

**När inställningen [!UICONTROL Completion Mode] för projektet är inställd på [!UICONTROL Manual]:**

* Om du flyttar en överordnad artikel med underaktiviteter till [!UICONTROL Complete] uppdateras den överordnade artikeln till 100 % och [!UICONTROL Status] till [!UICONTROL Complete]. Underaktiviteter uppdateras inte.
* Om du vill uppdatera [!UICONTROL Percent Complete] för artikeln måste du uppdatera den från fliken [!UICONTROL Stories] eller från sidan [!UICONTROL Details] för objektet.

**När inställningen [!UICONTROL Completion Mode] för projektet är inställd på[!UICONTROL Automatic]**:

* Om du flyttar en överordnad artikel med underaktiviteter till [!UICONTROL Complete] uppdateras den överordnade artikeln till 100 % och [!UICONTROL Status] till [!UICONTROL Complete]. Underaktiviteter uppdateras också till 100 % och [!UICONTROL Status] uppdateras till [!UICONTROL Complete].
* Om du vill uppdatera [!UICONTROL Percent Complete] för artikeln måste du uppdatera [!UICONTROL Percent Complete] för alla underaktiviteter. [!UICONTROL Percent Complete] för artikeln beräknas baserat på [!UICONTROL Percent Complete] för alla underaktiviteter.

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
   <td> <p>[!UICONTROL Contribute] eller [!UICONTROL Manage] åtkomst till aktiviteten som underaktiviteten är på</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Lägga till en underuppgift i en befintlig artikel på Urvalsritytan

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront] och klicka sedan på **[!UICONTROL Teams]**.

1. (Valfritt) Klicka på ikonen **[!UICONTROL Switch team]** ![Byt team-ikon](assets/switch-team-icon.png) och välj sedan ett nytt Scrum-team i listrutan eller sök efter ett team i sökfältet.

1. Gå till den smidiga upprepningen eller projektet som innehåller artikeln där du vill lägga till en underuppgift. Mer information om hur du navigerar till en iteration finns i [Visa en iteration](../../../agile/use-scrum-in-an-agile-team/iterations/view-iteration.md).
1. Gå till artikelrutan på artikelpanelen där du vill lägga till en underuppgift.
1. Klicka på **[!UICONTROL Add Subtask]** på artikelns huvudkort för att skapa en underuppgift till artikeln.

   ![Lägg till underaktivitet](assets/agile-story-addsubtask-NWE.png)

   eller

   Klicka på **[!UICONTROL Add Subtask]** på en underaktivitetspanel för att skapa en underaktivitet till underaktiviteten.

   [!DNL Workfront] har stöd för oändliga nivåer av underaktiviteter, men bara två nivåer (underaktiviteter för underaktiviteter) visas på den flexibla artikelpanelen.

   ![Lägg till underaktivitet](assets/agile-story-addsubtask2-NWE.png)

   När du lägger till en underaktivitet i en artikel som för närvarande inte har någon simbana, befordras den överordnade aktiviteten till kolumnen [!UICONTROL Parent Story] och underaktiviteten flyttas inuti simrutan.

1. Ange följande information:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Subtask Name]</strong></td>
      <td> Ange ett namn för underaktiviteten.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td>
      <td>Ange en beskrivning för underaktiviteten.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimate]</strong></td>
      <td>Ange uppskattningen för underaktiviteten.<br><p>Tänk på följande när du skapar uppskattningar:</p>
       <ul>
        <li>Om ditt flexibla team är konfigurerat att uppskatta artiklar i poäng är standardvärdet 1 poäng 8 timmar. Uppskattningar läggs till som [!UICONTROL Planned Hours] i artikeln.</li>
        <li>De kombinerade uppskattningarna för alla underaktiviteter avgör uppskattningen av den överordnade artikeln. Mer information finns i <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/update-status-of-stories-and-subtasks.md" class="MCXref xref">Uppdatera status för artiklar och underaktiviteter på kontrollpanelen</a>.</li>
        <li>När du skapar en ny underaktivitet är fältet [!UICONTROL Estimate] redan inställt. Om du återställer uppskattningen för underaktiviteten återställer du uppskattningen för den överordnade artikeln (eftersom den överordnade artikeln är summan av alla dess underaktiviteter).</li>
       </ul><br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Planned Hours]</strong></td>
      <td> (Endast tillgängligt i projekt) Ange antalet planerade timmar för aktiviteten.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Assignment]</strong></td>
      <td>Börja skriva namnet på teamet där du vill tilldela underuppgiften och klicka sedan på den när den visas i listrutan.</td>
     </tr>
    </tbody>
   </table>

1. Klicka på **[!UICONTROL Create]**.

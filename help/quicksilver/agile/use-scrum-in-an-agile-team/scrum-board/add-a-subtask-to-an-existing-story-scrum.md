---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Lägga till en underuppgift i en befintlig artikel på Urvalsritytan
description: När du skapar underaktiviteter för befintliga artiklar bör du tänka på inställningen Slutförandeläge för projektet, eftersom det påverkar hur artiklarna uppdateras.
author: Lisa
feature: Agile
exl-id: 264e66e9-94c7-4904-baad-f733d39b4791
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# Lägga till en underaktivitet i en befintlig artikel på [!UICONTROL Scrum] board

Tänk på följande när du skapar underuppgifter för befintliga artiklar:

**När [!UICONTROL Completion Mode] inställningen för projektet är inställd på [!UICONTROL Manual]:**

* Flytta en överordnad artikel med underuppgifter till [!UICONTROL Complete] uppdaterar den överordnade artikeln till 100 % och [!UICONTROL Status] till [!UICONTROL Complete]. Underaktiviteter uppdateras inte.
* Så här uppdaterar du [!UICONTROL Percent Complete] för artikeln måste du uppdatera den från [!UICONTROL Stories] eller från [!UICONTROL Details] objektets sida.

**När [!UICONTROL Completion Mode] inställningen för projektet är inställd på[!UICONTROL Automatic]**:

* Flytta en överordnad artikel med underuppgifter till [!UICONTROL Complete] uppdaterar den överordnade artikeln till 100 % och [!UICONTROL Status] till [!UICONTROL Complete]. Underaktiviteter uppdateras också till 100 % och [!UICONTROL Status] uppdateras till [!UICONTROL Complete].
* Så här uppdaterar du [!UICONTROL Percent Complete] för artikeln måste du uppdatera [!UICONTROL Percent Complete] för alla underaktiviteter. The [!UICONTROL Percent Complete] för artikeln beräknas utifrån [!UICONTROL Percent Complete] av alla underaktiviteter.

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
   <td> <p>[!UICONTROL Worker] eller högre</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>[!UICONTROL Contribute] eller [!UICONTROL Manage] behörighet till uppgiften som underaktiviteten är på</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Lägga till en underuppgift i en befintlig artikel på Urvalsritytan

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Teams]**.

1. (Valfritt) Klicka på **[!UICONTROL Switch team]** icon ![Byt ikon för team](assets/switch-team-icon.png)väljer du sedan ett nytt Scrum-team i listrutan eller söker efter ett team i sökfältet.

1. Gå till den smidiga upprepningen eller projektet som innehåller artikeln där du vill lägga till en underuppgift. Mer information om hur du navigerar till en iteration finns i [Visa en upprepning](../../../agile/use-scrum-in-an-agile-team/iterations/view-iteration.md).
1. Gå till artikelrutan på artikelpanelen där du vill lägga till en underuppgift.
1. Klicka **[!UICONTROL Add Subtask]** på artikelns huvudkort för att skapa en underuppgift till artikeln.

   ![Lägg till underaktivitet](assets/agile-story-addsubtask-NWE.png)

   eller

   Klicka **[!UICONTROL Add Subtask]** på en underaktivitetspanel för att skapa en underaktivitet till underaktiviteten.

   [!DNL Workfront] har stöd för oändliga nivåer av underaktiviteter, men bara två nivåer (underaktiviteter för underaktiviteter) visas på den flexibla artikelpanelen.

   ![Lägg till underaktivitet](assets/agile-story-addsubtask2-NWE.png)

   När du lägger till en underuppgift i en artikel som för närvarande inte har någon simbana, kommer den överordnade uppgiften att befordras till [!UICONTROL Parent Story] -kolumnen och underaktiviteten flyttas inuti simbanan.

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
        <li>Om ditt flexibla team är konfigurerat att uppskatta artiklar i poäng är standardvärdet 1 poäng 8 timmar. Beräkningar läggs till som [!UICONTROL Planned Hours] på storyn.</li>
        <li>De kombinerade uppskattningarna för alla underaktiviteter avgör uppskattningen av den överordnade artikeln. Mer information finns i <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/update-status-of-stories-and-subtasks.md" class="MCXref xref">Uppdatera status för artiklar och underaktiviteter på Scrum board</a>.</li>
        <li>När du skapar en ny underuppgift visas [!UICONTROL Estimate] fältet har redan angetts. Om du återställer uppskattningen för underaktiviteten återställer du uppskattningen för den överordnade artikeln (eftersom den överordnade artikeln är summan av alla dess underaktiviteter).</li>
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

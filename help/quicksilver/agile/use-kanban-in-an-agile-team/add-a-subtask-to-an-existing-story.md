---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Lägg till en underaktivitet i en befintlig artikel på Kanban-tavlan
description: Läs den här artikeln om du vill veta mer om hur du skapar underaktiviteter för befintliga artiklar på Kanban-tavlan.
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---

# Lägg till en underaktivitet i en befintlig artikel på Kanban-tavlan

Tänk på följande när du skapar underuppgifter för befintliga artiklar:

**När [!UICONTROL Summary Completion Mode] inställningen för projektet är inställd på [!UICONTROL Manual]:**

* Du kan flytta en överordnad artikel med underaktiviteter till [!UICONTROL Complete], som uppdaterar den överordnade artikeln till 100 % och [!UICONTROL Status] till [!UICONTROL Complete]. Underaktiviteter uppdateras inte.
* Så här uppdaterar du [!UICONTROL Percent Complete] för artikeln måste du uppdatera den från [!UICONTROL Stories] eller från [!UICONTROL Details] objektets sida.

**När [!UICONTROL Summary Completion Mode] inställningen för projektet är inställd på [!UICONTROL Automatic]:**

* Det går inte att flytta den överordnade artikeln över anslagstavlan. Så här uppdaterar du [!UICONTROL Percent Complete] för artikeln måste du uppdatera [!UICONTROL Percent Complete] för alla underaktiviteter. The [!UICONTROL Percent Complete] för artikeln beräknas utifrån [!UICONTROL Percent Complete] av alla underaktiviteter.
* Flytta en överordnad artikel med underuppgifter till [!UICONTROL Complete] uppdaterar den överordnade artikeln till 100 % och [!UICONTROL Status] till [!UICONTROL Complete]. Underaktiviteter uppdateras också till 100 % och [!UICONTROL Status] uppdateras till [!UICONTROL Complete].

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
   <td> <p>[!UICONTROL Worker] eller högre</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] administratören kan ändra din åtkomstnivå, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>[!UICONTROL Contribute] eller [!UICONTROL Manage] behörighet till uppgiften som underaktiviteten är på</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Lägga till en underaktivitet i en befintlig artikel på [!UICONTROL Kanban] board

1. Gå till [!UICONTROL Kanban] en anslagstavla som innehåller artikeln där du vill lägga till en underuppgift.
1. Klicka på uppgiftens namn i artikelrutan på sidan [!UICONTROL Kanban] bräda.
1. Lägg till en underaktivitet till uppgiften på samma sätt som du gör i andra uppgiftslistor i [!DNL Workfront], enligt beskrivningen i [Skapa underaktiviteter](../../manage-work/tasks/create-tasks/create-subtasks.md).

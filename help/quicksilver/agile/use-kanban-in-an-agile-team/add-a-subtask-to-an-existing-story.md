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
source-wordcount: '327'
ht-degree: 0%

---

# Lägg till en underaktivitet i en befintlig artikel på Kanban-tavlan

Tänk på följande när du skapar underuppgifter för befintliga artiklar:

**När inställningen [!UICONTROL Summary Completion Mode] för projektet är inställd på [!UICONTROL Manual]:**

* Du kan flytta en överordnad artikel med underaktiviteter till [!UICONTROL Complete], vilket uppdaterar den överordnade artikeln till 100 % och [!UICONTROL Status] till [!UICONTROL Complete]. Underaktiviteter uppdateras inte.
* Om du vill uppdatera [!UICONTROL Percent Complete] för artikeln måste du uppdatera den från fliken [!UICONTROL Stories] eller från sidan [!UICONTROL Details] för objektet.

**När inställningen [!UICONTROL Summary Completion Mode] för projektet är inställd på [!UICONTROL Automatic]:**

* Det går inte att flytta den överordnade artikeln över anslagstavlan. Om du vill uppdatera [!UICONTROL Percent Complete] för artikeln måste du uppdatera [!UICONTROL Percent Complete] för alla underaktiviteter. [!UICONTROL Percent Complete] för artikeln beräknas baserat på [!UICONTROL Percent Complete] för alla underaktiviteter.
* Om du flyttar en överordnad artikel med underaktiviteter till [!UICONTROL Complete] uppdateras den överordnade artikeln till 100 % och [!UICONTROL Status] till [!UICONTROL Complete]. Underaktiviteter uppdateras också till 100 % och [!UICONTROL Status] uppdateras till [!UICONTROL Complete].

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
   <td> <p>[!UICONTROL Worker] eller högre</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>[!UICONTROL Contribute] eller [!UICONTROL Manage] åtkomst till aktiviteten som underaktiviteten är på</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Lägg till en underaktivitet i en befintlig artikel på [!UICONTROL Kanban]-panelen

1. Gå till den [!UICONTROL Kanban]-panel som innehåller artikeln där du vill lägga till en underuppgift.
1. Klicka på aktivitetens namn i artikelrutan på [!UICONTROL Kanban]-panelen.
1. Lägg till en underaktivitet i aktiviteten på samma sätt som du gör i andra uppgiftslistor i [!DNL Workfront], enligt beskrivningen i [Skapa underaktiviteter](../../manage-work/tasks/create-tasks/create-subtasks.md).

---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Lägg till en underuppgift i en befintlig artikel i Kanban-styrelsen
description: Läs den här artikeln om du vill veta mer om hur du skapar underaktiviteter för befintliga artiklar på Kanban-tavlan.
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 452f8ddc5268a0d67e32090d166199f2fad7dbc7
workflow-type: tm+mt
source-wordcount: '289'
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

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td> <p>Nytt: [!UICONTROL Standard]</p> 
   eller
   <p>Aktuell: [!UICONTROL Work] eller högre</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>[!UICONTROL Contribute] eller [!UICONTROL Manage] åtkomst till aktiviteten som underaktiviteten är på</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lägg till en underaktivitet i en befintlig artikel på [!UICONTROL Kanban]-panelen

1. Gå till den [!UICONTROL Kanban]-panel som innehåller artikeln där du vill lägga till en underuppgift.
1. Klicka på aktivitetens namn i artikelrutan på [!UICONTROL Kanban]-panelen.
1. Lägg till en underaktivitet i aktiviteten på samma sätt som du gör i andra uppgiftslistor i [!DNL Workfront], enligt beskrivningen i [Skapa underaktiviteter](../../manage-work/tasks/create-tasks/create-subtasks.md).

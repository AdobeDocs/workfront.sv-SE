---
title: Åtkomst till listan över status för systemaktivitet
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Du kan använda status för en uppgift för att visa användare i vilket utvecklingsstadium en uppgift befinner sig vid en viss tidpunkt.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2cdedc67-b7b0-4e83-a446-d71e3afe255c
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# Åtkomst till listan över status för systemaktivitet

Du kan använda status för en uppgift för att visa användare i vilket utvecklingsstadium en uppgift befinner sig vid en viss tidpunkt.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planera</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Åtkomst till uppgiftsstatus

Mer information om hur du redigerar systemstatus eller skapar nya anpassade statusvärden finns i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

{{step-1-to-setup}}

1. Klicka på **Projektinställningar** > **Status**.

1. Klicka på fliken **Åtgärder**.

   De uppgiftsstatusvärden som är tillgängliga i Workfront visas på den här fliken.

   ![](assets/task-status.png)

   Mer information om de inbyggda aktivitetsstatusarna finns i [Systemuppgiftsstatus](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-task-statuses.md).

## Om att skapa anpassade aktivitetsstatusar

Som Workfront-administratör kan du lägga till anpassad systemuppgiftsstatus i Workfront.

Som gruppägare kan du lägga till anpassade uppgiftsstatusvärden för gruppen.

När du skapar en anpassad aktivitetsstatus måste du alltid matcha den nya statusen med en befintlig systemstatus. Du måste förstå hur systemstatusarna fungerar för att veta vilken status som är lämplig för att motsvara din anpassade status. När du har valt din likvärdiga status kan du inte ändra den här markeringen.

Mer information om hur du skapar anpassade statusvärden, redigerar systemlägen eller väljer nya standardstatusvärden för dina aktiviteter finns i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

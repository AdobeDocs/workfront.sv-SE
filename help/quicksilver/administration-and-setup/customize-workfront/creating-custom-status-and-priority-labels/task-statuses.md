---
title: Åtkomst till listan över status för systemaktivitet
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Du kan använda status för en uppgift för att visa användare i vilket utvecklingsstadium en uppgift befinner sig vid en viss tidpunkt.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2cdedc67-b7b0-4e83-a446-d71e3afe255c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Åtkomst till listan över status för systemaktivitet

Du kan använda status för en uppgift för att visa användare i vilket utvecklingsstadium en uppgift befinner sig vid en viss tidpunkt.

## Åtkomstkrav

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
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Åtkomst till uppgiftsstatus

Mer information om hur du redigerar systemstatus eller skapar nya anpassade statusvärden finns i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Konfigurera** ![](assets/gear-icon-settings.png) .

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

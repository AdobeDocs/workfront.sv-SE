---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-groups
title: Flytta en grupp
description: Du kan flytta en grupp under en annan grupp som du hanterar.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f5227454-457d-40d3-865c-c2551471d83e
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---

# Flytta en grupp

Du kan flytta en grupp under en annan grupp som du hanterar.

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
   <td>Du måste vara gruppadministratör för gruppen eller systemadministratör.</td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Flytta en grupp under en annan grupp

>[!NOTE]
>
>Om statusvärdena för den flyttade gruppen är låsta ärver den statusvärdena för den nya överordnade gruppen.
>
>Om statusvärdena för den flyttade gruppen är olåsta ärver den inte statusvärdena för den nya överordnade gruppen, och den nya överordnade gruppen får inte heller statusvärdena.
>
>Mer information om gruppstatus finns i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) och [Skapa eller redigera en gruppstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

{{step-1-to-setup}}

1. Klicka på **Grupper** ![](assets/groups-icon.png) i den vänstra panelen.

1. Markera målgruppen där du vill flytta gruppen och klicka sedan på redigeringsikonen ![](assets/edit-icon.png).
1. I rutan **Redigera grupp** som visas, under **Gruppmedlemmar och gruppadministratörer**, börjar du skriva namnet på gruppen som du vill flytta och klickar sedan på den när den visas.
1. Klicka på **Spara**.

>[!TIP]
>
>Du kan också göra en undergrupp till en grupp på den översta nivån. Anvisningar finns i avsnittet [Ta bort en undergrupp från den överordnade gruppen och gör den till en grupp på den översta nivån](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) i artikeln [Hantera en undergrupp](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).

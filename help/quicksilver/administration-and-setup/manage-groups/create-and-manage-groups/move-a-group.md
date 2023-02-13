---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-groups
title: Flytta en grupp
description: Du kan flytta en grupp under en annan grupp som du hanterar.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f5227454-457d-40d3-865c-c2551471d83e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# Flytta en grupp

Du kan flytta en grupp under en annan grupp som du hanterar.

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-plan*</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> <p>Du måste vara gruppadministratör för gruppen eller Workfront-administratör. Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppadministratörer</a> och <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du behöver ta reda på vilken plan eller licenstyp du har.

## Flytta en grupp under en annan grupp

>[!NOTE]
>
>Om statusvärdena för den flyttade gruppen är låsta ärver den statusvärdena för den nya överordnade gruppen.
>
>Om statusvärdena för den flyttade gruppen är olåsta ärver den inte statusvärdena för den nya överordnade gruppen, och den nya överordnade gruppen får inte heller statusvärdena.
>
>Mer information om gruppstatus finns i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) och [Skapa eller redigera en gruppstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **Grupper** ![](assets/groups-icon.png).

1. Markera målgruppen där du vill flytta gruppen och klicka sedan på ikonen Redigera ![](assets/edit-icon.png).
1. I **Redigera grupp** ruta som visas, under **Gruppmedlemmar och gruppadministratörer** börjar du skriva namnet på gruppen som du vill flytta och klickar sedan på den när den visas.
1. Klicka **Spara**.

>[!TIP]
>
>Du kan också göra en undergrupp till en grupp på den översta nivån. Instruktioner finns i avsnittet [Ta bort en undergrupp från den överordnade gruppen och gör den till en grupp på den översta nivån](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) i artikeln [Hantera en undergrupp](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).

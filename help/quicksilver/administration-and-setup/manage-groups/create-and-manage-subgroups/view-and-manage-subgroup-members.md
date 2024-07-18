---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Visa och hantera undergruppsmedlemmar
description: När du visar en grupp som du hanterar kan du visa och hantera alla användare i gruppens undergrupper.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8f7b0183-6035-4dd4-8e42-fd65485449bf
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# Visa och hantera undergruppsmedlemmar

När du visar en grupp som du hanterar kan du visa och hantera alla användare i gruppens undergrupper.

Om det finns grupper ovanför gruppen som du hanterar kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

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
   <td> <p>Plan </p> <p>Du måste vara gruppadministratör för gruppen eller Workfront-administratör. Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppadministratörer</a> och <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till användare med alternativet Användaradministratör (alla användare) markerat</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller vilka åtkomstnivåkonfigurationer du har.

## Visa och hantera medlemmar i undergrupperna under en grupp

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Konfigurera** ![](assets/gear-icon-settings.png) .

1. Klicka på **Grupper**.

   I listan som visas kan du se de grupper som du hanterar, tillsammans med eventuella undergrupper som de har. Adobe Workfront-administratörer kan se alla grupper.

1. Klicka på namnet på gruppen som du vill visa eller hantera undergruppsmedlemmar för.
1. Klicka på **Undergruppsmedlemmar** i den vänstra panelen.

   Det vänstra panelobjektet är bara tillgängligt om gruppen har undergrupper.

1. Gör något av följande:

   * Välj en medlem i listan och klicka sedan på Redigera ![](assets/edit-icon.png) för att ändra den personens användarprofil.

     Mer information finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) eller [Redigera användarprofiler gruppvis](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).

   * Markera ett valfritt antal medlemmar i listan och klicka sedan på Uppdatera ![](assets/comment-icon.png) för att lägga till en kommentar i deras användarprofiler.

     Användaren eller användarna får ett meddelande i appen samt ett e-postmeddelande med din kommentar. Kommentaren visas i området Uppdateringar i användarens profil.

   * Välj ett valfritt antal medlemmar i listan och klicka sedan på Inaktivera ![](assets/deactivate-user.png) eller Aktivera ![](assets/activate-user.png).

     Mer information finns i [Inaktivera eller återaktivera en användare](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

   * Exportera ![](assets/export.png) till listan med medlemmar.

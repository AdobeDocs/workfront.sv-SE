---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Visa och hantera undergruppsmedlemmar
description: När du visar en grupp som du hanterar kan du visa och hantera alla användare i gruppens undergrupper.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8f7b0183-6035-4dd4-8e42-fd65485449bf
source-git-commit: a42a167447d2f11b5502e4a0953b5e7eec2e67b1
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# Visa och hantera undergruppsmedlemmar

När du visar en grupp som du hanterar kan du visa och hantera alla användare i gruppens undergrupper.

Om det finns grupper ovanför gruppen som du hanterar kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Alla</p></td>
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td><p>Standard</p>
       <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste ha något av följande:</p> 
    <ul> 
     <li> <p>Åtkomstnivån Systemadministratör. </li> 
     <li> <p><b>Användare</b> i din åtkomstnivå har konfigurerats till <b>Redigera</b> åtkomst, med <b>Skapa</b> och minst ett av de två <b>användaradministratörsalternativen</b> som har aktiverats under <b>Finjustera inställningarna</b> <img src="assets/gear-icon-settings.png">. </p> <p>Om <b>Användaradministratör (gruppanvändare)</b> är aktiverat måste du vara gruppadministratör för en grupp där användaren är medlem.</p> </li> 
    </ul> </td> 
  </tr>  
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visa och hantera medlemmar i undergrupperna under en grupp

{{step-1-to-setup}}

1. Klicka på **Grupper**.

   I listan som visas kan du se de grupper som du hanterar, tillsammans med eventuella undergrupper som de har. Adobe Workfront-administratörer kan se alla grupper.

1. Klicka på namnet på gruppen som du vill visa eller hantera undergruppsmedlemmar för.
1. Klicka på **Undergruppsmedlemmar** i den vänstra panelen.

   Det vänstra panelobjektet är bara tillgängligt om gruppen har undergrupper.

1. Gör något av följande:

   * Markera en medlem i listan och klicka sedan på Redigera ![redigeringsikon](assets/edit-icon.png) för att ändra den personens användarprofil.

     Mer information finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) eller [Redigera användarprofiler gruppvis](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).

   * Markera ett valfritt antal undergruppsmedlemmar i listan och klicka sedan på **Skicka uppdatering till användare** för att lägga till en kommentar i användarprofilerna.

     Användaren eller användarna får ett meddelande i appen samt ett e-postmeddelande med din kommentar. Kommentaren visas i området Uppdateringar i användarens profil.

     Mer information finns i [Skicka direktmeddelanden till andra användare](/help/quicksilver/people-teams-and-groups/work-directly-with-others/send-direct-messages-to-other-users.md).

   * Markera ett valfritt antal medlemmar i listan och klicka sedan på Inaktivera ![användare](assets/deactivate-user.png) eller Aktivera ![användare](assets/activate-user.png).

     Mer information finns i [Inaktivera eller återaktivera en användare](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

   * Exportera ![Exportera](assets/export.png) listan med medlemmar.

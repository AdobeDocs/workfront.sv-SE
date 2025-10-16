---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: Hantera projektgruppen
description: Projektgruppen består av användare som är kopplade till projektet. Medlemmarna i projektgruppen visas i avsnittet Personer i projektet eller i avsnittet Personer i mallen som kan användas för att skapa ett projekt.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: 00e693fc8b35a59f6ed212bc30da7f85cc78c845
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---

# Hantera projektgruppen

<!--take preview and production references out at production - August 7-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>

-->

Projektgruppen består av användare som är kopplade till projektet. Mer information finns i [Översikt över projektgruppen](/help/quicksilver/manage-work/projects/planning-a-project/project-team-overview.md).

Medlemmarna i projektgruppen visas i avsnittet Personer i projektet.

De användare som visas i avsnittet Personer i en projektmall blir projektteam när projektet har skapats från mallen.

Följande användare läggs till automatiskt i projektteamet, både för projekt och mallar:

* Ägare
* Sponsorn
* Användare som tilldelats uppgifter
* Användare som har tilldelats till ärenden (endast för ett projekt)

Användare i projektteamet får meddelanden om projektet. Mer information finns i [Händelsemeddelandetyper](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Du kan hantera användarna i projektet och mallens team genom att lägga till dem (endast för projektet), ta bort dem eller skicka en uppdatering till dem.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Standard</p>
    <p>Plan</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt och mallar</p> <p>Visa eller ge användare högre åtkomst</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller ge högre behörighet till ett projekt eller till en mall</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old access: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Standard </p>
    <p>Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects and Templates</p> <p>View or higher access to Users</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project or to a template</p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).



## Add users to a Project Team

When you add users to the project team, they gain View permissions on the project and the tasks, issues, and documents of the project. For more information, see the article [Project Team overview](../../../manage-work/projects/planning-a-project/project-team-overview.md).

>[!TIP]
>
>Users on the Project Team are not automatically added to the resource management tools for the project.

You can add users to the project team in the following ways:

* [Automatically add users to a Project Team](#automatically-add-users-to-a-project-team) 
* [Manually add users to a Project Team](#manually-add-users-to-a-project-team)

### Automatically add users to a Project Team {#automatically-add-users-to-a-project-team}

The users that fulfill the following roles on the project are automatically added to the project team and appear  in the People section when the project is created:

* The creator of the project
* The project owner
* The project sponsor

Users are also automatically added to the project team when they are assigned to the following:

* Tasks
* Issues

### Manually add users to a Project Team {#manually-add-users-to-a-project-team}

If users that don't fulfill any role on the project want to be notified about certain updates or changes during the life of the project, you can manually add them to the project team. 

 For more information about what notifications can be enabled for users on the project team, see [Event notification types](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md). 

 <!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 



## Manage people on a project

1. Go to the project you want to manage the project team for.

   >[!TIP]
   >
   >You must have users assigned to tasks, issues or as stakeholders on the project to have them display in the People section.

1. Click **People** in the left panel. 

1. Click **Add users**. 

   The **Add users to Project Team** box displays.

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. In the **Add users** box, begin typing the name of an active Workfront user that you want to add to the project team, then click the name when it appears in the list.

   Repeat this step to add multiple users to the project team. The users must belong to the group associated with the project. 

   >[!TIP]
   >
   >* You cannot add users by adding their teams, groups, companies, or job roles.
   >* As you add the users, notice the avatar, the user's Primary Role, and their email address to distinguish between users with identical names. Users must be associated with at least one job role to view it as you add them.
   >
   >  You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

1. Click **Add**.

   The users gain View permissions to the project and receive notifications about the project as part of the project team.

1. (Optional) If you want a user to receive a  notification when their job role is added to a task, issue, or project approval, click inside the **Job Role** column for the user, and select a job role that will be associated with the approval. 

   The users will receive notifications related to the approvals assigned to the selected job role. 

   For more information see the "Role-based approvals" section in the article [Project Team overview](/help/quicksilver/manage-work/projects/planning-a-project/project-team-overview.md).

1. Select one or several users in the list, then click the **Remove** icon ![Remove icon](assets/remove-icon.png) to remove them from the team. 
 
1. Click **Yes, Remove Selected Users** to confirm and remove the users.

   Users are removed and unassigned from incomplete work items.

   For more information, see the [Considerations for removing users from a project team](#considerations-for-removing-users-from-a-project-team) section in this article.
1. (Optional) To send an update for this project to users, click **Update All** to send the update to everyone on the team

   Or 

   Select one or multiple users in the list, then click **Send Update to User**.

   <!--update screen shot when they fix the bug - the text above the box needs to match the OLD box, below-->

![Skicka uppdatering till användarrutan i projektet](assets/send-update-to-user-on-project-box-2025.png)

<!--Old UI for projects but the text above the comment box is right and matches the functionality):
   ![OLD Send update to user on a project](assets/send-update-to-user-on-project-box.png)-->

Rutan **Skicka uppdatering till användare** öppnas.

1. Gör något av följande:

   * Lägg till en uppdatering för de valda användarna.
   * Klicka på låsikonen för att göra uppdateringen privat för användarna i ditt företag.
   * Tagga ytterligare användare för att få samma uppdatering.
   * Klicka på **Skicka**.

   Uppdateringen läggs till i avsnittet **Uppdateringar** i projektet och alla markerade användare visas som taggade användare.

   Användarna kan få ett e-postmeddelande om de är aktiverade för dem och de får ett meddelande i appen om den nya uppdateringen.

1. (Valfritt) Klicka på ikonen **Exportera** ![Exportera ](assets/export-icon.png) för att exportera listan med användare till en fil

   eller

   Markera användare och klicka sedan på ikonen **Exportera** om du bara vill exportera vissa användare.

## Hantera personer i en mall

1. Gå till mallen som du vill hantera projektteamet för.

   >[!TIP]
   >
   >Du måste ha användare tilldelade till uppgifter eller som intressenter i mallen för att de ska kunna visas i avsnittet Personer.

1. Klicka på **Personer** i den vänstra panelen.

1. Markera en eller flera användare i listan och klicka sedan på ikonen **Ta bort** för att ta bort dem från gruppen.

1. Klicka på **Ja, ta bort markerade användare** för att bekräfta och ta bort användarna.

   Användare tas bort och tas bort från malluppgifterna.

   Mer information finns i avsnittet [Att tänka på när du tar bort användare från ett projektteam](#considerations-for-removing-users-from-a-project-team) i den här artikeln.

1. (Valfritt) Om du vill skicka en uppdatering till användare klickar du på **Uppdatera alla** för att skicka uppdateringen till alla användare i listan

   eller

   Markera en eller flera användare i listan och klicka sedan på **Skicka uppdatering till användare**.

   <!--update screen shot for unshim production, notice the text above the box - it needs to say "Post an update to each person's profile"-->

   ![Skicka uppdatering till användarrutan i mallen](assets/send-update-to-user-on-template-box.png)

   Rutan **Skicka uppdatering till användare** öppnas.

1. Gör följande:

   * Lägg till en uppdatering för de valda användarna.
   * Klicka på **Tagga personer** om du vill tagga fler användare för att få samma uppdatering.
   * Välj alternativet **Privat till mitt företag** för att göra uppdateringen privat för användarna i ditt företag.
   * Klicka på **Skicka**.

     >[!TIP]
     >
     >Inställningen **Privat till mitt företag** är bara tillgänglig när din Workfront-profil är associerad med ett företag.

   Uppdateringen läggs till i avsnittet **Uppdateringar** i varje taggad användares profil.

   Användarna kan få ett e-postmeddelande om de är aktiverade för dem och de får ett meddelande i appen om den nya uppdateringen.

1. Klicka på ikonen **Exportera** ![Exportera ](assets/export-icon.png) om du vill exportera listan med användare till en fil

   eller

   Markera användare och klicka sedan på ikonen **Exportera** om du bara vill exportera vissa användare.

## Att tänka på när du tar bort användare från ett projektteam

När du tar bort användare från deras roller i projektet blir de kvar i projektteamet.

Du måste ta bort dem från projektteamet, från avsnittet Personer i projektet, för att de ska kunna sluta ta emot meddelanden som skickas till projektteamet.

Om du tar bort en användare från projektteamet och användaren är tilldelad aktiviteter eller ärenden i projektet, tas användaren bort från de uppgifter och utgåvor som inte har slutförts. I det här fallet återgår uppgifterna och problemen till Ej tilldelat arbetsområde i Utjämning av arbetsbelastning.

Användare som är tilldelade till slutförda uppgifter och utgåvor förblir tilldelade till uppgifter och utgåvor, även när du har tagit bort dem från projektteamet.

Följande användare tas bort från sina roller i projektet när du tar bort dem från avsnittet Personer i ett projekt eller en mall:

* Användare som är tilldelade till ofullständiga uppgifter
* Användare som är tilldelade till ofullständiga utgåvor

Följande användare tas inte bort från sina roller i projektet när du tar bort dem från området Personer i ett projekt eller en mall:

* Ägare
* Sponsorn

Mer information om hur du tar bort användare från projektteamet finns i [Ta bort användare från projekt](../../../manage-work/projects/manage-projects/remove-users-from-projects.md).


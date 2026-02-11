---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Ändra flera användartilldelningar i en uppgiftslista
description: När du hanterar uppgiftstilldelningar kan du ändra dem samtidigt för flera uppgifter samtidigt genom att använda gruppredigeringsfunktionen i en lista med uppgifter.
author: Lisa
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 21c98e443a6d6ca79045e2f4aba5f792340833cd
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 0%

---

# Ändra flera användartilldelningar i en uppgiftslista

<!--Audited: 11/2025-->

<!--remove the old/new experience references when the toggles are removed-->

<!--
this article is similar and updates on this one might need to be repeated here: help/quicksilver/manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md</p>
-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Second Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-release-overview.md).  

</div>-->

När du hanterar uppgiftstilldelningar kan du ändra dem samtidigt för flera uppgifter samtidigt genom att använda gruppredigeringsfunktionen i en lista med uppgifter.

Den här artikeln handlar om att ändra flera användartilldelningar för flera uppgifter i en uppgiftslista. Se även följande artiklar för att ändra uppdrag för flera uppgifter i andra områden:

* Mer information om hur du tilldelar uppgifter med hjälp av belastningsutjämnaren finns i [Översikt över hur du tilldelar arbete i belastningsutjämnaren](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Mer information om hur du tilldelar en aktivitet till en resurs i en lista finns i [Tilldela uppgifter](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td> <p>Standard</p>
   <p>Arbeta eller högre</p>
   </td> 
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt och uppgifter</p> <p>Visa eller ge användare högre åtkomst</p> </td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td>
   <td>Contribute eller högre behörigheter för åtgärderna</td>
  </tr>
 </tbody>
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on tasks</h2>
<p>(NOTE: moved to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>You might want to modify the user assignments for multiple tasks for a variety of reasons, including the following:</p>
<ul>
<li>Users join or leave your team</li>
<li> <p>A user takes a vacation that extends beyond task due dates</p> <note type="note">
When assigning users to work, their availability according to their schedules affects the Planned and Projected Dates of tasks. For information about schedules, see
<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.
</note> </li>
<li>A specific role or user is set as the assignee for multiple tasks and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
<p><strong>How removing assignees affects task hours and allocation percentages</strong></p>
<p>(NOTE: move to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration Types:</p>
<ul>
<li> <p><strong>Simple:</strong> The planned hours assigned to that user are subtracted from the task's total planned hours.</p> <note type="important">
<span class="s1">This could negatively affect your project plan because it changes the total planned hours for the task and the project.</span>
</note> </li>
<li><span class="s1"><strong>Effort Driven:</strong> The allocation percentage does not change for other users.</span> </li>
<li><span class="s1"><strong>Calculated Assignment:</strong> The allocation percentages of other users are adjusted so that the total equals 100%.</span> </li>
<li><span class="s1"><strong>Calculated Work:</strong> The allocation percentage does not change for other users.</span> </li>
</ul>
</div>
-->

## Ändra tilldelningar för flera uppgifter

1. Gå till listan som innehåller de uppgifter där du vill ändra tilldelningar.
1. (Valfritt) Skapa ett filter som endast visar uppgifter som tilldelats den tilldelade personen och som du vill ändra.

   Om ditt projekt till exempel innehåller en viss roll som standardtilldelare för flera uppgifter kan du skapa ett filter som bara visar uppgifter med den rollen som tilldelad. Sedan kan du ersätta rollen med en viss användare.

   Mer information om hur du skapar ett filter finns i [Skapa eller redigera filter](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).


1. Om du vill filtrera efter en roll väljer du **Tilldelningsroller** och klickar sedan på **ID**.

   >[!TIP]
   >
   >Använd inte fältet **Tilldelad till**. Detta söker bara efter den primära ägaren för uppgiften i stället för någon av rollerna som kan tilldelas dem.

   eller

   Om du vill filtrera efter en användare väljer du **Tilldelningsanvändare** och klickar sedan på **ID.**

   >[!TIP]
   >
   >Använd inte fältet **Tilldelad till**. Detta söker bara efter den primära ägaren för uppgiften i stället för de användare som kan tilldelas till dem.

1. Markera de uppgifter som du vill ändra uppdrag för och klicka sedan på ikonen **Redigera** ![Redigera](assets/edit-icon.png) .

   1. Gör något av följande om du vill lägga till eller ta bort tilldelningar:

      * Om du vill lägga till tilldelningar börjar du skriva namnet på en tilldelad i fältet **Sök efter personer, roller eller team** och markerar dem sedan när de visas i listan.

        Den nya tilldelaren läggs till i de befintliga för de valda uppgifterna.
      * Om du vill ta bort tilldelningar klickar du på namnet på en tilldelad i rutan **Ta bort tilldelad**

        eller

        Klicka på **Ta bort alla befintliga tilldelningar**.

        Tilldelningar tas bort från alla markerade uppgifter.

        Om du tar bort användare från uppgifter kan detta påverka aktivitetstimmar och allokeringsprocentsatser.

        Mer information finns i [Översikt över att ändra aktivitetstilldelningar](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).


        >[!TIP]
        >
        >* Du kan tilldela flera användare, jobbroller eller team. Du kan bara tilldela aktiva användare, jobbroller och team.
        >   
        >* När du lägger till en användartilldelning bör du lägga märke till avataren, användarens primära roll eller användarens e-postadress för att skilja mellan användare med identiska namn. Användarna måste vara associerade med minst en jobbroll för att kunna visa den när du lägger till dem. Du måste ha inställningen Visa kontaktinformation aktiverad på din åtkomstnivå för att användare ska kunna visa användarnas e-postmeddelanden. Mer information finns i [Bevilja åtkomst för användare](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
        > 
        >   Om en användare, jobbroll eller ett team tilldelades innan de inaktiverades, förblir de tilldelade till arbetsuppgiften. I det här fallet rekommenderar vi följande:
        >   
        >* Tilldela om arbetsuppgiften till aktiva resurser.
        >* Associera användarna i ett inaktiverat team med ett aktivt team och omfördela arbetsposten till det aktiva teamet.


   1. (Valfritt) Ändra något av följande alternativ för tilldelningar:

      * (Villkorligt) **Allokering % eller Timmar**: Ange en ny allokeringsprocent eller timmar.

      >[!NOTE]
      >
      >Det här alternativet kan bara ändras om varaktighetstypen är densamma för alla åtgärder som redigeras. När varaktighetstypen är Beräknad arbets- eller insatsstyrd kan du uppdatera allokeringen %. När varaktighetstypen är Enkel kan du uppdatera timarna. Mer information om varaktighetstyp finns i [Översikt över aktivitetsvaraktighet och varaktighetstyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
      >
      >
      >Om fältet är tomt innebär det att värdet är olika för olika åtgärder, men du kan fortfarande ändra det.

      * **Gör primär**: Håll markören över de markerade aktiviteterna och välj det här alternativet om du vill att den som tilldelats ska vara ägare till uppgiften för alla aktiviteter som redigeras.
      * **Tilldelningens roll**: Välj en roll i listrutan. Om alternativet inte är markerat väljs automatiskt användarens primära roll.
      * **Varaktighetstyp**
      * **Varaktighet**
      * **Planerade timmar**

   1. Klicka på **Spara**.

<!-- temporary content - for Assignments redesign:

Editing assignments on tasks differs depending on which environment you choose. 

1. (Conditional) If you are using the Production environment to assign tasks, the **Edit Tasks** box opens in the new experience. Do the following in the Production environment: 

   1. To add or remove assignees, do one of the following:

      * To add assignees, start typing the name of an assignee in the **Search people, roles, or teams** field, then select them when they display in the list. 
      * To remove assignees, click the **x** icon to the right of their name. Only assignees that are common to all tasks display in the list. 
      * Click Assign to me to assign the selected tasks to yourself.

   1. (Conditional) When using the new experience, click **Save**.

   1. (Optional) Click **Switch to old experience** at the bottom of the **Edit Tasks** box.
      
      The **Edit Tasks** box opens in the old experience.

   1. (Conditional) In the old experience, do the following to modify the assignees:

      1. Go to the **Assignments** section.

         >[!IMPORTANT]
         >
         >Removing assignees can affect the task hours and allocation percentages. For more information, see the section [How removing assignees affects task hours and allocation percentages](#how-removing-assignees-affects-task-hours-and-allocation-percentages) in this article.

      1. Do one of the following to add or remove assignees:

         * To add a new assignee:

            1. In the **Assignments** section, select **Assignee**.

               Information that is common across all tasks selected displays. For example, if the same user is assigned to all tasks, that user displays in the **Assignee** column. If information is not common across the tasks selected, no information displays.
            
            1. Start typing the name of a user, role, or team, then select it when it displays in the list. The assignment is added and does not replace the current assignments on the selected tasks.

            >[!TIP]
            >
            > * You can assign multiple users, job roles, or teams. You can assign only active users, job roles, and teams.
            >   
            > * When adding a user assignment, notice the avatar, the user's Primary Role, or their email address to distinguish between users with identical names. Users must be associated with at least one job role to view it as you add them. You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
            > 
            >   If a user, job role, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:
            >   
            >     * Reassign the work item to active resources.
            >     * Associate the users in a deactivated team with an active team and reassign the work item to the active team.


         * To remove individual assignees:

            1. Click the **X icon** next to the name of the assignee that you want to remove if the assignee displays in the Assignments list.

               Or

               (Conditional) If the assignee that you want to remove does not display in the Assignments section because the assignee is assigned to only some of the tasks that you have selected, click **Remove Assignee** and start typing the name of the assignee that you want to remove, then click the name when it appears in the drop-down list.

         * To remove all existing assignees:

            1. Click **Remove All Existing Assignees**, then click **Yes, Delete All Assignees**.

               This removes not only common assignees (assignees that are displayed in the edit dialog box), but also all assignees on all the selected tasks.

            Removing users from tasks can affect task hours and allocation percentages.
            
            For more information, see [Overview of modifying task assignments](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

      1. (Optional) Modify any of the following options for assignees:

         * (Conditional) **Allocation % or Hours**: Specify a new allocation percentage or hours.

         >[!NOTE]
         >
         >This option can be modified only if the Duration Type is the same across all tasks that are being edited. When the Duration Type is Calculated Work or Effort Driven you can update the Allocation %. When the Duration Type is Simple you can update the Hours. For information about Duration Type, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
         >
         >
         >If the field is blank, this means that the value is different across tasks; however, you are still able to modify it.

         * **Task Owner**: Select this option to make the assignee the owner of the task for all tasks being edited.
         * **Assignee's Role**: Select a role from the drop-down list. If left unselected, Adobe Workfront automatically selects the Primary Role of the user. 

      1. Click **Save Changes.**
        

1. <span class="preview">(Conditional) If you are using the Preview environment to assign tasks, the **Edit Tasks** box opens. Do the following in the Preview environment: </span>

   <div class="preview">-->






---
product-area: projects
navigation-topic: manage-issues
title: Ändra användartilldelningar för flera utgåvor i en lista
description: Ändra användartilldelningar för flera utgåvor i en lista
author: Lisa
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: 8f7249e08268a8cb784d4c0ecc8c534542fa80cf
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 0%

---

# Ändra användartilldelningar för flera utgåvor i en lista

<!--Audited: 07/2024-->
<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

Du kan ändra användartilldelningar samtidigt till flera utgåvor. Mer information om hur du redigerar problem eller tilldelar dem en åt gången finns i följande artiklar:

* [Redigera problem](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Tilldela ärenden](../../../manage-work/issues/manage-issues/assign-issues.md)

Allmän information om hur du tilldelar problem finns i [Översikt över hur du ändrar problemtilldelningar](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>Du måste ha minst Contribute-behörighet för ett problem för att kunna göra tilldelningar av det.

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
   <td> <p>Medarbetare eller högre</p>
   <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till problem</p> <p>Visa eller högre åtkomst till projekt och uppgifter för att tilldela ett problem</p> </td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för problemet</p> <p>Contribute-behörigheter eller högre till det projekt eller den uppgift där problemet finns, när du tilldelar flera utgåvor.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:  drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of  reasons, including the following:</p>
<ul>
<li>Users join or leave  your team</li>
<li>A user takes a vacation that extends beyond the issue  due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## Ändra tilldelningar för flera utgåvor

1. Gå till listan med ärenden som innehåller de ärenden vars uppdrag du vill ändra.
1. (Valfritt) Skapa ett filter som endast visar ärenden som tilldelats den tilldelade personen som du vill ändra.

   Du kan t.ex. skapa ett filter som bara visar problem med en viss roll som tilldelad.  Sedan kan du ersätta rollen med en viss användare. Gör följande:

   1. Klicka på listrutan **Filter** och sedan på **Nytt filter**.

   1. I det första fältet börjar du skriva **Tilldelningsroller** och väljer **Tilldelningsroller: Namn** i listan.
   1. Välj **Är något av** i listrutan för modifierare och börja sedan skriva namnet på en roll och markera den när den visas i listan. Du kan skriva flera roller.

      >[!TIP]
      >
      >Använd inte **Tilldelad till** eftersom det här fältet endast refererar till utfärdaren och inte till alla tilldelningar.

      Listan över problem filtrerar automatiskt efter filtervillkoren.
   1. (Valfritt) Klicka på **Spara som ny** och sedan på **Spara**.

1. Markera de ärenden som du vill ändra uppdrag för och klicka sedan på ikonen **Redigera** ![Redigera ](assets/qs-edit-icon.png) .

   **Redigera problem** visas. Antalet markerade objekt visas i det övre vänstra hörnet på sidan.

1. Klicka på **Uppdrag** i den vänstra panelen och klicka sedan på ikonen **x** bredvid den tilldelade person som du vill ta bort.

   >[!TIP]
   >
   >Endast tilldelningar som har tilldelats alla markerade utgåvor visas i området **Uppdrag**.

   ![Området uppdrag i gruppredigeringsfrågor](assets/assignments-area-on-bulk-edit-issues.png)

1. Börja skriva namnet på en användare, roll eller team som ska lägga till tilldelningar till alla valda utgåvor.

   >[!TIP]
   >
   >Du kan tilldela flera användare, jobbroller eller team. Du kan bara tilldela aktiva användare, jobbroller och team.
   >
   >Om en användare, jobbroll eller ett team tilldelades innan de inaktiverades, förblir de tilldelade till arbetsuppgiften. I det här fallet rekommenderar vi följande:
   >
   >* Tilldela om arbetsuppgiften till aktiva resurser.
   >* Associera användarna i ett inaktiverat team med ett aktivt team och omfördela arbetsposten till det aktiva teamet.

   De tillagda tilldelningarna läggs till i de befintliga. De ersätter inte de befintliga för varje vald utgåva.

1. (Valfritt) Klicka på **Tilldela mig** om du vill tilldela dig själv alla utgåvor.
1. Klicka på **Spara**.


   <!--Old functionality for assignments for issues - before November 2025:
   1. (Conditional) In the Production environment, do the following: 
   1. Go to the **Assignments** section, then select **Assignee**.
      ![Assignments area](assets/classic-assignmens-area-on-edit-box-350x119.png)
   1. Do one of the following:
      1. To add a new assignee:
         1. Start typing the name of a user, role, or team, then select it when it displays in the list. The assignment is added and does not replace the current assignments on the selected issues.
         >[!TIP]
         >
         >You can assign multiple users, job roles, or teams. You can assign only active users, job roles, and teams.
         >
         >If a user, job role, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:
         >
         >* Reassign the work item to active resources.
         >* Associate the users in a deactivated team with an active team and reassign the work item to the active team.
          Information that is common across all issues selected displays. For example, if the same user is assigned to all issues, that user displays in the **Assignee**  column. If information is not common across the issues selected, no information displays.
      1. To remove individual assignees:
         1. Click the **X icon** next to the name of the assignee that you want to remove if the assignee displays in the Assignments list.
            Or
            If the assignee that you want to remove does not display in the Assignments section because the assignee is assigned to only some of the issues that you have selected, click **Remove Assignee** and start typing the name of the assignee that you want to remove, then click the name when it appears in the drop-down list.
         1. Click  **Remove Assignee** again to add another assignee to remove.
      1. To remove all existing assignees:
         1. Click **Remove All Existing Assignees**, then click **Yes, Delete All Assignees**.
            This removes not only common assignees (assignees that are displayed in the edit  dialog box), but also all assignees on all the selected issues.
         1. (Optional) Modify any of the following options for the assignees you selected to associate with the issues:
          * **Issue Owner:**  Select the radio button to indicate which assignee is designated as the Issues Owner. If left unselected, Adobe Workfront designates the first assignee as the Issue Owner. This is not available for team assignments. 
            * **Assignee's Role**: Select a role from the drop-down list. If left unselected, Workfront automatically selects the Primary Role of the user.
      1. Click **Save Changes**.-->





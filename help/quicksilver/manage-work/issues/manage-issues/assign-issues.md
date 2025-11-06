---
product-area: projects
navigation-topic: manage-issues
title: Tilldela ärenden
description: Du kan tilldela utgåvor till användare, roller och team för att ange vem som ansvarar för att slutföra utgåvorna. Allmän information om hur du tilldelar problem finns i Ändra problemtilldelningar - översikt.
author: Lisa
feature: Work Management
role: User
exl-id: e2dce29e-7370-4580-8326-99c4437998bf
source-git-commit: 0358e79bd606d0035959bba2a47256456b529b18
workflow-type: tm+mt
source-wordcount: '1366'
ht-degree: 0%

---

# Tilldela ärenden

<!--Audited: 10/2024-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

Du kan tilldela utgåvor till användare, roller och team för att ange vem som ansvarar för att slutföra utgåvorna. Allmän information om hur du tilldelar problem finns i [Översikt över hur du ändrar problemtilldelningar](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!TIP]
>
>Du kan tilldela flera användare, jobbroller eller team. Du kan bara tilldela aktiva användare, jobbroller och team.
>
>Om en användare, en jobbroll eller ett team tilldelades innan de inaktiverades, förblir de tilldelade till arbetsuppgiften. I det här fallet rekommenderar vi följande:
>
>* Tilldela om arbetsuppgiften till aktiva resurser.
>* Associera användarna i ett inaktiverat team med ett aktivt team och omfördela arbetsposten till det aktiva teamet.

Utöver den här artikeln rekommenderar vi att du läser följande artiklar för mer information om hur du tilldelar problem:

* [Översikt över att ändra problemtilldelningar](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md)
* [Redigera problem](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Ändra användartilldelningar för flera utgåvor i en lista](../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md)
* [Skapa avancerade tilldelningar](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [Gör smarta tilldelningar](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [Översikt över smarta tilldelningar](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [Översikt över tilldelning av arbete i belastningsutjämnaren](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

Du kan tilldela en utgåva till en eller flera resurser på en enskild utgåva eller tilldela flera resurser till flera utgåvor samtidigt.

Att tilldela ärenden och uppgifter är detsamma som i Adobe Workfront. Allmän information om hur du tilldelar uppgifter finns i [Översikt över hur du ändrar aktivitetstilldelningar](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
 <col> 
 </col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td> <p>Medarbetare eller högre</p>
   <p>Granska eller högre</p> </td> 
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till problem</p> <p>Visa eller högre åtkomst till projekt och uppgifter för att tilldela ett problem</p> </td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för problemet</p> <p> Visa behörigheter eller högre för det projekt eller den uppgift där problemet finns, när du tilldelar ett problem</p><p>Contribute-behörigheter eller högre till det projekt eller den uppgift där problemet finns, när du tilldelar flera utgåvor.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Överväganden för flera tilldelningar till jobbroller, team och användare

Tänk på följande när du tilldelar flera resurser till en arbetsuppgift:

* Användare kan ha mer än en jobbroll kopplad till sin profil. Mer information om hur du associerar användare med jobbroller finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Uppgifter eller ärenden tilldelas vanligtvis först till en eller flera jobbroller eller team. När projekten är klara att starta kan de behöva tilldelas användare.

  Om en uppgift eller ett ärende tilldelas till en eller flera roller och du sedan även tilldelar en användare, bestämmer Adobe Workfront vilken jobbroll som ska associeras med den andra användaren (om någon) enligt följande regler:

   * Om det bara finns en tilldelad jobbroll och den matchar användarens primära roll, tilldelas uppgiften eller utgåvan endast den användare som fyller sin primära roll.
   * Om det finns flera roller tilldelade och minst en av rollerna matchar användarens sekundära roller, tilldelas uppgiften eller utgåvan till användaren som uppfyller en av deras övriga roller - som Workfront väljer slumpmässigt om det finns flera matchningar - samt eventuella ytterligare roller som tilldelas.
   * Om det finns en eller flera jobbroller tilldelade och det inte finns några matchningar mot användarens roller, tilldelas uppgiften eller utgåvan till både rollen eller rollerna och till användaren.

* Om en uppgift eller ett problem har tilldelats ett team och du även tilldelar en användare, förblir uppgiften eller utgåvan tilldelad till både teamet och användaren.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2> </h2>
<h2>Considerations about removing assignments from issues</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and moved to Modify issue assignments overview article)</p>
<p>You can remove assignments from one issue at a time, or you can remove assignments from multiple issues in bulk.</p>
<p>For more information about removing assignments from issues in bulk, see <a href="../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md" class="MCXref xref">Modify user assignments for multiple issues in a list</a>. </p>
<p>Consider the following when removing assignments from issues: </p>
<ul>
<li>When you unassign a user from an issue, the issue remains assigned to the job role that the user fulfilled on the issue.</li>
<li>When you unassign a job role or a team from an issue, the issue remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->

## Tilldela en utgåva i utgåvans huvud

1. Gå till ett ärende som du vill tilldela.
1. Klicka på **Tilldela till** i det övre högra hörnet av ärendehuvudet i området **Uppdrag**

   eller

   Klicka på namnet på de aktuella tilldelningarna, om utgåvan redan har tilldelats.

   ![Tilldela till knapp](assets/assign-to-button-in-header.png)

1. Gör något av följande:

   * Börja skriva namnet på en användare, roll eller team som du vill tilldela och klicka sedan på den när den visas i listan.

     ![Uppdragssökning](assets/smart-assignments-issue-header.png)

   * (Villkorligt) Klicka på ett av namnen, rollerna eller teamen i de tillgängliga listorna
   * Klicka på **Tilldela mig** för att tilldela den till dig själv
   * Klicka på **Avancerat**.

     Att skapa avancerade uppdrag fungerar ungefär på samma sätt för uppgifter och ärenden. Mer information om hur du gör avancerade tilldelningar finns i [Skapa avancerade tilldelningar](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

     >[!TIP]
     >
     >När du lägger till en användartilldelning bör du lägga märke till avataren, användarens primära roll eller användarens e-postadress för att skilja mellan användare med identiska namn.
     >
     >Användarna måste vara associerade med minst en jobbroll för att kunna visa den när du lägger till dem.
     >
     >Du måste ha inställningen Visa kontaktinformation aktiverad på din åtkomstnivå för att användare ska kunna visa användarnas e-postmeddelanden. Mer information finns i [Bevilja åtkomst för användare](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
     >

     <!-- this doesn't apply to issues; if it does, add this to the TIP above: 
      ><span class="preview">When adding a job role assignment, you can search for the job role or location. Select a role from the Job roles list to use the default billing rate for the assignment, or select a Rate card job role to use the billing rate from the rate card. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>-->


1. Klicka på **Spara** för att slutföra tilldelningen av problemet.
1. (Valfritt) Klicka på ikonen **X** bredvid namnet på tilldelningarna i området Uppdrag i huvudet på utgåvan för att ta bort en tilldelning.

## Tilldela ett problem genom att redigera det i en lista

Du kan tilldela utgåvor i en lista eller en rapport när något av uppdragsfälten visas i listvyn. Det här är ett snabbare sätt att tilldela ärenden.

Beroende på vilket fält som visas i vyn kan du tilldela följande enheter till utgåvan:

| Alternativ | Enheter tilldelade |
|---|---|
| **Tilldela till** | Tilldela en användare |
| **Tilldelad** | Tilldela en användare |
| **Uppdrag** | Tilldela användare, jobbroller eller team. |

Så här tilldelar du utgåvor i en lista:

1. Gå till en lista med problem som har fälten Tilldelad, Tilldelad eller Uppdrag i vyn.
1. Gör något av följande om du vill tilldela problem:

   * Klicka i fälten **Tilldelad till** eller **Tilldelad** och börja skriva namnet på en aktiv användare som du vill tilldela utgåvan och klicka sedan på den när den visas i listan.

     ![Tilldelad till fält](assets/assigned-to-field-task-list-nwe.png)

   * Klicka i fältet **Uppdrag** och börja skriva namnet på en aktiv användare, jobbroll eller aktivt team som du vill tilldela utgåvan. Klicka sedan på den när den visas i listan.

     ![Uppdragsfält](assets/assignments-field-0825.png)

   >[!TIP]
   >
   >När du lägger till en användartilldelning bör du lägga märke till avataren, användarens primära roll eller användarens e-postadress för att skilja mellan användare med identiska namn.
   >
   >Användarna måste vara associerade med minst en jobbroll för att kunna visa den när du lägger till dem.
   >
   >Du måste ha inställningen Visa kontaktinformation aktiverad på din åtkomstnivå för att användare ska kunna visa användarnas e-postmeddelanden. Mer information finns i [Bevilja åtkomst för användare](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

1. (Villkorligt) I fältet Uppdrag klickar du på **Avancerat** längst ned i listan eller på ikonen **Personer** ![Ikonen Personer](assets/teams.png) i det övre högra hörnet av uppdragsrutan, öppnar rutan Avancerade uppdrag och skapar avancerade uppdrag. Mer information finns i [Skapa avancerade uppdrag](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >Du kan inte göra avancerade uppdrag från fälten Tilldelad till eller Tilldelad.

1. När du har lagt till dina tilldelningar till problemet trycker du på Enter eller klickar någonstans på sidan för att spara ändringarna.

## Tilldela ett problem i rutan Redigera problem

Du kan tilldela ett problem när du redigerar det i rutan Redigera problem.

Mer information finns i avsnittet Uppdrag i artikeln [Redigera problem](/help/quicksilver/manage-work/issues/manage-issues/edit-issues.md).

## Tilldela flera utgåvor samtidigt

<!--
Assigning issues in bulk is different depending on what environment you choose to do this. 

### Assign issues in bulk in the Production environment 

1. Go to a list of issues that you want to assign in bulk. 
1. Select several issues in the list. 
1. Click the **Edit icon** ![Edit icon](assets/qs-edit-icon.png).

   The **Edit Issues** dialog box opens.

1. In the **Assignments** area, select the **Assignee** box, then start typing the name of a user, job role, or team that you want to assign to all the issues.

   >[!IMPORTANT]
   >
   >If any of the issues is already assigned, the resources you indicate here are added to the issues instead of replacing the existing resources on the issues. 
   
1. (Optional) Select the radio button in the **Issue Owner** column to indicate which resource is the primary assignee or the Owner of the issue, when you assign more than one resource to the issue. This is not available for teams. 
1. (Optional) Select a role that the user should fulfill on the issue from the **Pick a role** drop-down menu in the **Assignee's Role** column when you assign users to issues. If you do not select a role, Workfront automatically selects the user's Primary Role. 

1. (Optional) If you want to remove existing assignees from all issues do one of the following:

   1. Start typing the name of a user, role, or team you want to remove from the issue, then select it when it appears on the list and click **Remove Assignee** to add additional assignees to remove. 
   1. Click **Remove All Existing Assignees** to remove all assignees from all selected issues.

1. Click **Save Changes**.
1. (Optional and conditional) When the Assigned to or the Assignments fields display in your list of issues, click inside one of these columns for an issue, then click the **X icon** next to the name of an assignee to remove it from the issue.

<div class="preview">

### Assign issues in bulk in the Preview environment

-->

1. Gå till en lista över problem som du vill tilldela gruppvis.
1. Markera flera problem i listan.
1. Klicka på ikonen **Redigera** ![Redigera](assets/qs-edit-icon.png).

   Dialogrutan **Redigera problem** öppnas.

1. Klicka på **Uppdrag** i den vänstra panelen och börja skriva namnet på en användare, roll eller team i fältet **Uppdrag** i fältet **Sök efter personer, roller eller team** och klicka sedan på det när det visas i listan

   eller

   Klicka på **Tilldela mig** om du vill tilldela utgåvorna till dig själv.

   >[!IMPORTANT]
   >
   >Om något av problemen redan har tilldelats läggs de resurser du anger här till i problemen i stället för att ersätta de befintliga resurserna i problemen.

1. (Valfritt) Om du vill ta bort befintliga tilldelningar från alla utgåvor klickar du på **x** bredvid deras namn.

1. (Valfritt) Uppdatera fältet **Antal planerade timmar**. Mer information finns i [Redigera problem](/help/quicksilver/manage-work/issues/manage-issues/edit-issues.md).

1. Klicka på **Spara**.
1. (Valfritt och villkorligt) När fälten **Tilldelad till** eller **Tilldelningar** visas i listan med utgåvor klickar du i en av dessa kolumner för ett problem och sedan på ikonen **X** bredvid namnet på en tilldelad för att ta bort den från utgåvan.



---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Tilldela uppgifter
description: Du kan tilldela uppgifter till användare, roller eller team för att ange vem som ansvarar för att slutföra uppgifterna. Du kan tilldela en uppgift till mer än en resurs åt gången.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 611b136e-2c3f-4eac-9d75-e8c12e06148d
source-git-commit: 070b0525f0cb2880d3c7daf88777ba48968ce759
workflow-type: tm+mt
source-wordcount: '1985'
ht-degree: 0%

---

# Tilldela uppgifter

<!--Audited: 07/2024-->

<!--remove the span class preview from everywhere but the Rate Card roles references must stay in yellow; replace the intro with preview and fast track only but not sure if with the link to third quarter release?!-->

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i förhandsvisningsmiljön för alla kunder, eller i produktionsmiljön för kunder som aktiverat snabba versioner.</span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Mer information om den aktuella versionen finns i [Översikt över utgåvan för tredje kvartalet 2024](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

Du kan tilldela uppgifter till användare, jobbroller eller team för att ange vem som ansvarar för att slutföra uppgifterna. Du kan tilldela en uppgift till mer än en resurs åt gången.

>[!TIP]
>
>Du kan tilldela flera användare, jobbroller eller team. Du kan bara tilldela aktiva användare, jobbroller och team.
>
>Om en användare, jobbroll eller ett team tilldelades innan de inaktiverades, förblir de tilldelade till arbetsuppgiften. I det här fallet rekommenderar vi följande:
>
>* Tilldela om arbetsuppgiften till aktiva resurser.
>* Associera användarna i ett inaktiverat team med ett aktivt team och omfördela arbetsposten till det aktiva teamet.
>

Antalet användare som tilldelats en aktivitet och schemat för aktivitetsägaren kan ändra de planerade datumen för en aktivitet, vilket resulterar i att tidslinjen för projektet ändras. Mer information om effekten av att tilldela flera användare till en uppgift finns i [Översikt över att ändra aktivitetstilldelningar](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

Utöver den här artikeln rekommenderar vi att du läser följande artiklar för mer information om hur du tilldelar uppgifter:

* [Översikt över ändring av aktivitetstilldelningar](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)
* [Översikt över smarta tilldelningar](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [Gör smarta tilldelningar](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [Skapa avancerade tilldelningar](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [Ändra flera användartilldelningar i en uppgiftslista](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)
* [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [Planera en projektöversikt](../../../manage-work/projects/planning-a-project/plan-project.md)
* [Översikt över aktiviteten Planerat slutförandedatum](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [Ange projektets planerade slutförandedatum](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)
* [Översikt över tilldelning av arbete i belastningsutjämnaren](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Nytt: Standard</p>
   <p>Aktuell: Arbete eller högre</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt och uppgifter</p> <p>Visa eller ge användare högre åtkomst</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>


*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Överväganden för flera tilldelningar till jobbroller, team och användare

Tänk på följande när du tilldelar flera resurser till en arbetsuppgift:

* Användare kan ha mer än en jobbroll kopplad till sin profil. Mer information om hur du associerar användare med jobbroller finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Om du tilldelar mer än en användare till en uppgift eller ett problem, kommer den första användaren som du väljer automatiskt att bli ägare till uppgiften eller problemet.
Instruktioner om hur du ändrar detta finns i informationen om alternativet Gör primär i artikeln [Skapa avancerade tilldelningar](create-advanced-assignments.md).

* Ett team kan inte vara primär tilldelad för en uppgift eller ett problem. Endast en användare eller en jobbroll kan definieras som primär för en uppgift eller ett problem.

<!-- If a task is assigned to multiple teams, the primary team sees the Work On It button. waiting on team to verify if this is true. (Courtney)
You cannot make a team be a Primary on a task/ issue. (Alina) -->

* Uppgifter och ärenden i ett projekt kan tilldelas först till ett eller flera team eller jobbroller. När projektet är klart att starta kan användarna behöva göra det:

  <table>
  <col> 
  <col> 
  <tbody>
  <tr>
   <td>Team</td>
   <td>Om du tilldelar en uppgift till ett team och även tilldelar en användare, förblir uppgiften tilldelad teamet och användaren, även om användaren inte är medlem i teamet.</td>
  </tr>
  <tr>
   <td>Jobbroller</td>
   <td><p>Om du tilldelar en uppgift eller ett ärende till en eller flera roller och sedan även tilldelar en användare, bestämmer dig för vilken jobbroll du vill associera med den andra användaren (om någon) enligt följande regler:</p>
     <ul>
      <li>Om det bara finns en tilldelad jobbroll och den matchar användarens primära roll (konfigurerad i deras profil), tilldelas uppgiften eller utgåvan endast den användaren.</li>
      <li>Om flera roller har tilldelats och minst en av dem matchar en av användarens andra roller, tilldelas uppgiften eller utgåvan till användaren (rollen väljs slumpmässigt om det finns flera matchningar), tillsammans med eventuella ytterligare roller som har tilldelats</li>
      <li>Om minst en jobbroll har tilldelats och det inte finns några matchningar mot användarens jobbroller, tilldelas uppgiften eller utgåvan till både rollen eller rollerna och till användaren.</li>
     </ul>
   <p>Mer information om en användares primära roll och andra roller finns i <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Redigera en användares profil</a>.</p>
   </td> 
     </tr>
  </tbody>
  </table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations for multiple user assignments and using schedules</h2>
<p>(NOTE: moved to the Modify task assignments overview standalone article)</p>
<p>You can assign multiple resources to a task. When you assign a user to a task, Workfront uses the user's schedule to calculate the planned dates for the task which ultimately determine the timeline of the project. Using the schedule of the user takes into account their time off, holidays, and weekend days which are considered non-working days when task activity cannot occur. </p>
<p>When you assign multiple users to a task, your Workfront administrator <span>or a group administrator</span> determines which one of the following schedules Workfront uses to determine the planned dates of the tasks, based on schedules: </p>
<ul>
<li> <p><strong>The Primary Assignee's schedule</strong>: this is the schedule associated with the user designated as the task Owner.</p> <p>For information about associating users with schedules, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li>
<li><strong>The Project's schedule</strong>: this is the schedule associated with the project. For adding a schedule to a project, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
</ul>
<p>For information about setting up which schedule a project uses in the case of multiple assignments, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p>
</div>
-->

## Tilldela en enskild uppgift

1. Gå till en uppgift som du vill tilldela.
1. Klicka på **Tilldela till** i fältet **Tilldelningar** i uppgiftens huvud

   eller

   Klicka på uppdragsnamnet om uppgiften redan är tilldelad.

   ![Uppdrag](assets/assignments-box-in-task-header.png)

1. Gör något av följande:

   * Börja skriva namnet på en användare, roll eller team som du vill tilldela och klicka sedan på den när den visas i listan.


     >[!TIP]
     >
     >När du lägger till en användartilldelning bör du lägga märke till avataren, användarens primära roll eller användarens e-postadress för att skilja mellan användare med identiska namn. Användarna måste vara associerade med minst en jobbroll för att kunna visa den när du lägger till dem.
     >
     >Du måste ha inställningen Visa kontaktinformation aktiverad på din åtkomstnivå för att användare ska kunna visa användarnas e-postmeddelanden. Mer information finns i [Bevilja åtkomst för användare](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
     >
     ><span class="preview">När du lägger till en jobbrolltilldelning kan du söka efter jobbrollen eller platsen. Välj en roll i listan Jobbroller om du vill använda standardfaktureringsnivån för tilldelningen, eller välj en jobbroll för tariffkort om du vill använda faktureringssatsen från tariffkortet. Mer information om tariffkort finns i [Hantera tariffkort](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>


   * (Villkorligt) Klicka på ett av namnen i listorna **Föreslagna tilldelningar**, **Användare och team**, **Jobbroller** eller <span class="preview">**Klassificera kortroller**</span> när de visas. Mer information finns i [Översikt över smarta uppdrag](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

     Du kan börja skriva namnet på en användare, ett team eller en jobbroll som ska tilldelas uppgiften och sedan markera den när den visas i listan.

   * Klicka på **Avancerat**

     Mer information om hur du gör avancerade tilldelningar finns i [Skapa avancerade tilldelningar](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. Klicka på **Spara**.
1. (Valfritt och villkorligt) Klicka på ikonen **X** bredvid namnet på uppdraget på den högra panelen för uppgiften för att ta bort ett uppdrag, om du klickade på **Avancerat**.

## Tilldela en uppgift i en lista

Du kan tilldela uppgifter i en lista eller en rapport när något av tilldelningsfälten visas i listvyn. Det här är ett snabbare sätt att tilldela uppgifter. I den här artikeln beskrivs hur du ändrar tilldelningar för en uppgift i en lista. Mer information om hur du ändrar flera uppdrag för flera uppgifter i en lista finns i [Ändra flera användartilldelningar i en uppgiftslista](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Beroende på vilket fält som visas i vyn kan du tilldela följande enheter till uppgiften:

| Fält | Enheter tilldelade |
|---|---|
| **Tilldela till** | Tilldela en användare |
| **Tilldelad** | Tilldela en användare |
| **Uppdrag** | Tilldela användare, jobbroller eller team |

Så här tilldelar du uppgifter i en lista:

1. Gå till en lista med uppgifter som har fälten Tilldelad, Tilldelad eller Uppdrag i vyn.
1. (Valfritt) Klicka på listrutan **Spara automatiskt** och välj bland följande alternativ:

   | Alternativ | Alternativbeskrivning |
   |---|---| 
   | Spara automatiskt | Ändringar som du gör i uppgifterna sparas automatiskt och du kan inte återställa dem |
   | Spara manuellt | Du måste spara ändringarna manuellt. Du kan återställa ändringarna innan du sparar dem. |
   | Planering av tidslinje | Du måste spara ändringarna manuellt. Du kan återställa ändringarna innan du sparar dem. Det går snabbare att spara ändringarna och alla projektberoenden än när du väljer Spara manuellt. |

   Mer information om hur du sparar uppgifter när du redigerar dem i en lista finns i [Redigera uppgifter i en lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. Så här tilldelar du uppgifter:

   * Klicka i fälten **Tilldelad till** eller **Tilldelad** och börja skriva namnet på en aktiv användare som du vill tilldela uppgiften och klicka sedan på den när den visas i listan.
   * Klicka i fältet **Uppdrag** och börja skriva namnet på en aktiv användare, jobbroll eller team som du vill tilldela uppgiften. Klicka sedan på den när den visas i listan.

     >[!TIP]
     >
     >När du lägger till en användartilldelning bör du lägga märke till avataren, användarens primära roll eller användarens e-postadress för att skilja mellan användare med identiska namn. Användarna måste vara associerade med minst en jobbroll för att kunna visa den när du lägger till dem.
     >
     >Du måste ha inställningen Visa kontaktinformation aktiverad på din åtkomstnivå för att användare ska kunna visa användarnas e-postmeddelanden. Mer information finns i [Bevilja åtkomst för användare](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
     >
     ><span class="preview">När du lägger till en jobbrolltilldelning kan du söka efter jobbrollen eller platsen. Välj en jobbroll om du vill använda standardfaktureringssatsen för tilldelningen, eller välj en jobbroll för tariffkort om du vill använda faktureringssatsen från tariffkortet. Mer information om tariffkort finns i [Hantera tariffkort](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>


1. (Villkorligt) När den visas i fältet **Tilldelningar** klickar du på ikonen **Personer** i det övre högra hörnet av uppdragsrutan för att öppna rutan **Avancerade tilldelningar** och skapa avancerade tilldelningar.

   <!--
   there is a People icon in NWE but it's hard to see - you need to assign the task to at least 2 users, not roles, or teams, before it shows up</p>
   -->

   Mer information finns i [Skapa avancerade uppdrag](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >Du kan inte göra avancerade uppdrag från fälten Tilldelad till eller Tilldelad.

1. När du har lagt till dina tilldelningar till uppgiften trycker du på Enter eller klickar någonstans på sidan för att spara ändringarna om du väljer Spara automatiskt. Annars klickar du på **Spara**.

## Tilldela flera uppgifter till en användare

1. Gå till en lista med uppgifter som du vill tilldela gruppvis.
1. (Villkorligt) Se till att alternativet **Spara automatiskt** är markerat om du finns med i en lista över aktiviteter under ett projekt.

   >[!IMPORTANT]
   >
   >Du kan inte redigera flera uppgifter samtidigt när du sparar uppgifter manuellt i ett projekt.

1. Markera flera uppgifter i uppgiftslistan.
1. Klicka på **Redigera**.

   Dialogrutan **Redigera uppgifter** öppnas.

1. I området **Tilldelningar** markerar du rutan **Tilldelad** och börjar sedan skriva namnet på en användare, en jobbroll eller ett team som du vill tilldela alla uppgifter.

   >[!IMPORTANT]
   >
   >Om någon av uppgifterna redan har tilldelats läggs de resurser som du anger här till i aktiviteterna i stället för att ersätta de befintliga resurserna för aktiviteterna.

1. (Valfritt) Markera alternativknappen i kolumnen **Aktivitetsägare** för att ange vilken resurs som är den primära tilldelaren eller aktivitetens ägare när du tilldelar mer än en resurs till aktiviteten. Detta är inte tillgängligt för team.
1. (Villkorligt) Ange **allokeringen %** för varje resurs som tilldelats till aktiviteten om alla aktiviteter som du har valt har varaktighetstypen ansträngningsstyrd eller beräknad tilldelning. Detta anger hur mycket av deras tid som dessa resurser ska lägga på att slutföra uppgiften. Detta är endast tillgängligt för användare och jobbroller.

   eller

   Ange **Timmar** för varje resurs som tilldelats aktiviteten om alla aktiviteter du har valt har varaktighetstypen Enkel. Det totala antalet timmar för alla resurser ska vara lika med antalet planerade timmar för uppgiften.

   >[!IMPORTANT]
   >
   >Det går inte att ange allokeringsprocenten eller antalet timmar per resurs om de markerade aktiviteterna har olika varaktighetstyper eller om de markerade aktiviteterna har olika varaktighetstyper.

   Mer information om varaktighetstyp för uppgifter finns i [Översikt över aktivitetsvaraktighet och varaktighetstyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Valfritt) Välj en roll som användaren ska utföra på uppgiften i listrutan **Välj en roll** i kolumnen **Tilldelningens roll** när du tilldelar användare till uppgifter. Om du inte väljer någon roll väljs automatiskt användarens primära roll.

1. (Valfritt) Om du vill ta bort befintliga tilldelningar från alla åtgärder gör du något av följande:

   1. Börja skriva namnet på en användare, roll eller team som du vill ta bort från uppgiften, markera den när den visas i listan och klicka på **Ta bort tilldelningar** för att ta bort fler tilldelningar.
   1. Klicka på **Ta bort alla befintliga tilldelningar** om du vill ta bort alla tilldelningar från alla markerade aktiviteter.

1. Klicka på **Spara ändringar**.
1. (Valfritt och villkorligt) När fälten Tilldelad till eller Uppdrag visas i listan med uppgifter klickar du i en av dessa kolumner för en uppgift och sedan på ikonen **X** bredvid namnet på en tilldelad för att ta bort den från uppgiften.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations about unassigning tasks</h2>
<p>(NOTE: moved this to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm)</p>
<p>You can remove assignments from one task at a time, or you can remove assignments from multiple tasks in bulk.</p>
<p>For more information about removing assignments from tasks in bulk, see <a href="../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md" class="MCXref xref">Modify multiple user assignments in a task list</a>. </p>
<p>Consider the following when removing assignments from tasks: </p>
<ul>
<li>When you unassign a user from a task, the task remains assigned to the job role that the user fulfilled on the task.</li>
<li>When you unassign a job role or a team from a task, the task remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->



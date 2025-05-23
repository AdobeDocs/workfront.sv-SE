---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Ange projektplanerat slutförandedatum
description: Planerat slutförandedatum för ett projekt är det datum då projektet är inställt på att slutföras.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 996398c5-de92-445e-8e86-36b2efdcf6b5
source-git-commit: fedb0328450896d212081715df4cde7644b169bc
workflow-type: tm+mt
source-wordcount: '591'
ht-degree: 0%

---

# Ange projektplanerat slutförandedatum

<!-- Audited: 4/2025 -->

Planerat slutförandedatum för ett projekt är det datum då projektet är inställt på att slutföras.

Planerade startdatum och planerade slutförandedatum för ett projekt är beroende av datumen för aktiviteterna i projektet. I den här artikeln beskrivs hur du manuellt eller automatiskt kan ange planerat slutförandedatum för ett projekt. Mer information om det planerade slutförandedatumet för en aktivitet finns i [Översikt över aktivitetens planerade slutförandedatum](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

Det planerade slutförandedatumet för ett projekt kan anges manuellt eller automatiskt, beroende på om du schemalägger projektet från Start eller från Slutförandedatumet.

## Åtkomstkrav

<!--drafted for P&P:

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
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>
   Nytt: Standard

eller

Aktuell: Planera </p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ange manuellt planerat slutförandedatum för ett projekt

Du måste manuellt ange planerat slutförandedatum för ett projekt när du schemalägger projektet från slutförandedatum.

>[!NOTE]
>
>När du ställer in det planerade slutförandedatumet för ett projekt manuellt beräknar Workfront automatiskt det planerade startdatumet för projektet baserat på varaktigheten för alla uppgifter.


Så här schemalägger du ett projekt från Slutförandedatum:

{{step1-to-projects}}

1. Klicka på **Nytt projekt** och välj sedan **Nytt projekt** i listrutan som visas.

   Mer information om hur du skapar projekt finns i artikeln [Skapa ett projekt](../../../manage-work/projects/create-projects/create-project.md).

1. Välj **Projektinformation** i den vänstra panelen.

1. Klicka på ikonen **Redigera projekt** ![Redigera ](/help/quicksilver/manage-work/projects/planning-a-project/assets/qs-edit-icon.png) i det övre högra hörnet och välj sedan **Översikt** i listrutan som visas.

1. Klicka på fältet **Schemaläge** i avsnittet **Projektdatum** och välj sedan **Slutförandedatum**.

1. Ange **Planerat slutförandedatum** för projektet.
1. Klicka på **Spara ändringar**.

   När du börjar lägga till aktiviteter i projektet beräknas projektets **planerade startdatum** baserat på den totala varaktigheten för alla aktiviteter. 

## Ange automatiskt planerat slutförandedatum för ett projekt

Det planerade slutförandedatumet för ett projekt beräknas automatiskt av Workfront när du schemalägger projektet från startdatumet. 

Så här schemalägger du ett projekt från startdatum:

{{step1-to-projects}}

1. Klicka på **Nytt projekt** och välj sedan **Nytt projekt** i listrutan som visas.

   Mer information om hur du skapar projekt finns i artikeln [Skapa ett projekt](../../../manage-work/projects/create-projects/create-project.md).

1. Välj **Projektinformation** i den vänstra panelen.

1. Klicka på ikonen **Redigera projekt** ![Redigera ](/help/quicksilver/manage-work/projects/planning-a-project/assets/qs-edit-icon.png) i det övre högra hörnet och välj sedan **Översikt** i listrutan som visas.

1. Klicka på fältet **Schemaläge** i avsnittet **Projektdatum** och välj sedan **Startdatum**.

1. Ange projektets **planerade startdatum**.
1. Klicka på **Spara ändringar**.

   När du börjar lägga till aktiviteter i projektet beräknas projektets **Planerade slutförandedatum** baserat på den totala varaktigheten för alla aktiviteter. 

   Mer information om aktivitetsvaraktighet finns i artikeln [Översikt över aktivitetsvaraktighet och varaktighetstyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   Det planerade slutförandedatumet för projektet sammanfaller i detta fall med det planerade slutförandedatumet för den sista aktiviteten i projektet.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>The Planned Completion Date of a task</h2>
<p>(NOTE: drafted because I created a new article, here: /Content/Manage work/Tasks/Task information/task-planned-completion-date.htm)</p>
<p>You can either specify the Planned Completion Date of a task, or you can leave it up to Workfront to calculate it depending on certain criteria.&nbsp;</p>
<ul>
<li><a href="#manually-set-the-planned-completion-date-of-a-task" class="MCXref xref">Manually set the Planned Completion Date of a task</a> </li>
<li><a href="#how-the-planned-completion-date-is-calculated-for-a-task" class="MCXref xref">How the Planned Completion Date is calculated for a task</a> </li>
</ul>
<p><strong>Manually set the Planned Completion Date of a task</strong></p>
<p>Setting the Planned Completion Date of a task depends on the type of Task Constraint you assign to the task.&nbsp;</p>
<p>You can manually set the Planned Completion Date&nbsp;when creating a task, as described in&nbsp;the article <a href="../../../manage-work/tasks/create-tasks/create-tasks-in-project.md" class="MCXref xref">Create tasks in a project</a>.</p>
<p>You can manually specify the Planned Completion Date when you select any of the following Task Constraints:&nbsp;</p>
<table border="1" cellspacing="15" cellpadding="1">
<col>
<col>
<thead>
<tr>
<th> <p><strong>Task Constraint Type</strong> </p> </th>
<th> <p><strong>Effect of Manually Changing the Planned Completion Date</strong> </p> </th>
</tr>
</thead>
<tbody>
<tr>
<td> <p>Must Finish On</p> <p>Finish No Later Than</p> <p>Finish No Earlier Than</p> </td>
<td> <p><span class="s1">The Planned Start Date is adjusted in order to keep the Duration the same.</span> </p> </td>
</tr>
<tr>
<td> <p>Fixed Dates</p> </td>
<td> <p>The Duration is adjusted in order to keep the Planned Start Date the same.</p> </td>
</tr>
</tbody>
</table>
<p><strong>How the Planned Completion Date is calculated for a task</strong></p>
<p>When it is calculated automatically by the system, the following can influence the Planned Completion Date of a Task:</p>
<ul>
<li> <p>Task Constraint</p> <p>For more information about Task Constraints, see the article <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a>.</p> </li>
<li> <p>Task predecessor relationship</p> <p>For more information about task predecessors, see the article <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p> </li>
<li>Project Completion Date, when the project is scheduled from Completion Date.</li>
<li> <p>The time off schedule of the Primary&nbsp;Assignee of the task. </p> <p>When the Primary Assignee has time off scheduled during the duration of the task, the planned dates of the task adjust accordingly when the <strong>Consider user time off in task durations</strong> setting is selected for the <strong>User Time Off</strong> field. New projects inherit this setting from the Project&nbsp;Preferences area, but you can edit the setting at the project level. </p> <p>For example, if a task with a Constraint of As Soon As Possible is scheduled to start on June 1 and complete on June 3, and the Primary Assignee has June 2 marked for Time-off, the task Planned Completion Date becomes June 4. </p> <p>For information about the <strong>User Time Off</strong> preference, see the articles <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a> or <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p> </li>
</ul>
<p>When set automatically, the Planned Completion Date&nbsp;is determined based on the following calculation:&nbsp;</p>
<p><code>Planned Completion Date = Planned Start Date + Duration</code> </p>
<p>For example, if your task has a start date of September 16 and a duration of 10 days, the Planned Completion Date is September 26.</p> <note type="note">
&nbsp;The Update Type for the project must also be&nbsp;set to Automatic and On Change or Automatically in order for the Planned Hours and Duration to be automatically&nbsp;adjusted.
<br>For more information about the Update Type, see the article
<a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.
</note>
</div>
-->

---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Översikt över smarta uppdrag
description: När du hanterar uppgifter och ärenden kan du använda smarta uppdrag för att identifiera vem som är bäst på att slutföra arbetet. Smarta tilldelningar är förslag som Adobe Workfront ger dig när du tilldelar resurser arbetsobjekt baserat på en algoritm som avgör vilken resurs som passar bäst för jobbet.
author: Alina
feature: Work Management
exl-id: 8d17eff6-5ff0-4985-b575-4934a3bb7c0b
source-git-commit: 7e220e496aff2675910416bd86e3ddf7b9231afa
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# Översikt över smarta uppdrag

När du hanterar uppgifter och ärenden kan du använda smarta uppdrag för att identifiera vem som är bäst på att slutföra arbetet. Smarta tilldelningar är förslag som Adobe Workfront ger dig när du tilldelar resurser arbetsobjekt baserat på en algoritm som avgör vilken resurs som passar bäst för jobbet.

>[!NOTE]
>
>Smarta tilldelningar tar inte hänsyn till användarens tillgänglighet. Men deras tillgänglighet enligt scheman påverkar planerade och planerade datum för uppgifter och ärenden när de tilldelas. Mer information om scheman finns i artikeln [Skapa ett schema](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Den här artikeln innehåller allmän information om smarta tilldelningar. Mer information om hur du använder smarta tilldelningar för att tilldela uppgifter och utgåvor till användare finns i [Gör smarta uppdrag](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md).

## Översikt över smarta uppdrag

Tänk på följande när du arbetar med smarta uppdrag:

* Algoritmen fungerar oberoende för uppgifter och problem. Det innebär att listan med föreslagna användare för problem kan skilja sig från listan med föreslagna användare för en uppgift eftersom Workfront skapar listorna enligt kriterier som gäller problem och uppgifter separat.
* Smarta uppdrag rekommenderar inte jobbroller eller team. De är i stället förslag från användare som är bäst lämpade att slutföra en uppgift eller ett problem.
* De föreslagna uppdragen är alltid aktiva användare.
* Användaren som visas först bör vara den bästa matchningen för uppgiften.

## Hitta förslag på smarta uppdrag

Du kan visa smarta uppdrag i följande områden där du kan tilldela uppgifter eller ärenden:

* En uppgiftslista eller utgivningslista eller rapport

   ![](assets/smart-assignments-task-list-nwe-350x280.png)

* En aktivitets- eller utgivningsrubrik

   ![](assets/smart-assignments-task-header-nwe-350x302.png)

* Åtgärds- eller ärendesammanfattningspanelen

   ![](assets/smart-assignments-summary-panel-nwe-350x332.png)

* Uppdragsfältet för ett objekt som visas i hemområdet

   ![](assets/smart-assignments-in-home-nwe-350x216.png)


<!--removed for scheduling deprecation: 

* Resource Scheduling

  ![](assets/smart-assignments-scheduling-350x219.png)

  >[!CAUTION]
  >
  >Resource Scheduling is a deprecated feature. For more information, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

-->
* Utjämning av arbetsbelastning

   ![](assets/smart-assignments-workload-balancer-bulk-assignments.png)


## Kriterier för smarta tilldelningar

Smarta tilldelningar visar de 50 främsta rekommendationerna baserat på en egen algoritm.

Användare rekommenderas i listrutan Smarta tilldelningar baserat på en kombination av följande kriterier (listas i ordning från viktigaste till minst viktiga):

* Användare som har tilldelats andra arbetsobjekt de senaste 30 dagarna av användaren som har gjort uppdraget. De första 50 användarna som matchar det här villkoret visas. Den användare som oftast tilldelas visas först.

   Om arbetsuppgiften tilldelas ett team eller en roll filtreras listan med föreslagna användare med hänsyn till de befintliga tilldelningarna nedan. I det här fallet visas endast följande användare i listan med förslag:

   * Användare vars hemteam är det team som tilldelats arbetsuppgiften.
   * Användare vars primära roll är den roll som tilldelats arbetsuppgiften.

      >[!TIP]
      >
      >* If <!--you're not part of any team and --> ingen roll eller team har tilldelats för uppgiften eller utgåvan. Workfront visar alla användare som tilldelats de senaste 30 dagarna, upp till 50 användare.
      >* Om du inte har gjort några uppdrag under de senaste 30 dagarna visas endast användare som tillhör det tilldelade teamet eller har rollen tilldelad till arbetsposten i listan med smarta uppdrag.


<!--the commented out piece in the tip above was live before but I am not totally sure that smart assignments look at your team. I think they look JUST at the team/ role assigned to the work item; see this help site request for more info: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/62fd222200037eb87572c5b6ad6bf53e/overview -->
<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h3>Smart assignments criteria for the Production environment</h3>
<p>(NOTE: drafted,this was the case BEFORE we updated the logic in the WB - with the 21.4 release)</p>
</div>
<p>Smart assignments display on tasks and issues when the following conditions are met:</p>
<ul>
<li>The task or issue is subordinate to a parent task or issue that has a user, team, or job role currently assigned. </li>
</ul>
<p>Smart assignments display the top twenty recommendations based on a proprietary algorithm that uses your own team information.</p>
<p>Users are recommended in the smart assignments drop-down list based on a combination of the following criteria (listed in order from most important to least important):</p>
<ul>
<li>The user has the team assigned to the task or issue designated as their Home Team</li>
<li>The user is also assigned to the parent task</li>
<li>The user has the same primary job role as is currently assigned to the task or issue</li>
<li>The user has the team assigned to the parent task or issue designated as their Home Team</li>
<li>The user is associated with the same primary job role currently assigned to the parent task</li>
<li>The user is a member of the same team as the user who assigned the task or issue and the team is designated as their Home Team</li>
<li>The user is a member of the same Home Group as the user who is assigning the task or issue</li>
<li>The user has the same primary job role as the user who is assigning the task or issue.</li>
</ul>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Make smart assignments</h2>
<p>(NOTE:&nbsp;this was moved to its own article: make-smart-assignments.) </p>
<p>Smart assignments are available in most locations where you can make assignments in Workfront.</p>
<p>You can use smart assignments on tasks and issues that have previously been assigned to a job role or a team.</p> <note type="note">
You must have a Plan or a Work license and have at least Contribute permissions to a task or an issue to be able to make assignments to the task or the issue. You must have the Make Assignments option enabled in your permission level to make assignments.
</note>
<p>To use smart assignments:</p>
<ol>
<li value="1">Navigate to an issue or a task and click one of the following fields to edit them: <br>
<ul>
<li><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">The <strong>Assignments</strong> field in the task or issue header</p></li>
<li>The <strong>Assignments</strong> field of a task or issue list using in-line editing in a task or issue list. </li>
<li>The <strong>Assignee</strong> field after you have clicked <strong>Advanced</strong> from a task or an issue. </li>
</ul></li>
<li value="2"> <p>Place your cursor in the assignment field, and wait for two seconds, then the <strong>Suggestions</strong> list is displayed.</p> <p>Users displayed in this list are the smart assignment suggestions for the task or the issue.<br></p> <p> <img src="assets/nwe-smart-assignment-suggestions-350x160.png" style="width: 350;height: 160;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3"> <p>Select the user in the recommendations list by clicking their name. </p> <p>If there are no suggestions, the suggestion list does not open.</p> </li>
<li value="4">(Optional) If you do not want to use one of the recommended users from the smart assignments list, start typing the name of the desired user and select the name when it appears in the list.</li>
<li value="5">Click <strong>Enter</strong> to make the assignment. </li>
</ol>
</div>
-->

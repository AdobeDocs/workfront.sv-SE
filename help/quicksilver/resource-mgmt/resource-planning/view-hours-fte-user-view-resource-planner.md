---
content-type: reference
product-area: resource-management;user-management
navigation-topic: resource-planning
title: Visa tillgängliga, planerade och faktiska timmar eller FTE i resursplaneraren när användarvyn används
description: Visa Tillgängliga, Planerade och Faktiska timmar eller Faktiska timmar i resursplaneraren när du använder användarvyn i Planering i den högra panelen, t.ex."Budgeteringsresurser i den högra panelen" eller"Hantera resurser i den högra panelen". eller behöver återanvändas från ett annat POV?!"
author: LIsa
feature: Resource Management
exl-id: 6b532aa2-435f-4fda-b7ce-abe0a785638f
source-git-commit: 3c3175c347431b10aed1a6034df6c756056399b3
workflow-type: tm+mt
source-wordcount: '1739'
ht-degree: 0%

---

# Visa tillgängliga, planerade och faktiska timmar eller FTE i resursplaneraren när du använder användarvyn

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Consider renaming this article (probably split already) to something other than "Planning" in the RP" - maybe "budgeting resources in the RP" or "Managing Resources in the RP." etc... - or might need to be repurposed from another POV?!)</p>
-->

Förutom budgeteringsresurser i projekt- och rollvyerna kan du använda användarvyn i Adobe Workfront Resource Planner för att visa information om värdena Planerad, Tillgänglig och Faktisk timme eller FTE för projekt och resurser.

## Översikt över användarvyn i resursplaneraren

Tänk på följande när du visar information om timmar eller FTE i resursplaneraren:

* Du kan visa tillgängliga och planerade timmar eller FTE-information för användare, jobbroller och projekt i alla vyer av resursplaneraren.
* Du kan bara visa följande information i användarvyn:

   * Skillnaden mellan antalet planerade timmar eller heltidsanställda och antalet tillgängliga timmar eller heltidsanställda. Du kan sedan budgetera allokeringen av dina användare enligt den här skillnaden i projekt- och rollvyerna.
   * Faktiska timmar eller heltidsanställda.

* Du kan visa skillnaden mellan Tillgänglig användare och mängden Planerade timmar eller FTE som ett tal eller som ett procentvärde i användarvyn.
* Du kan inte visa informationen i användarvyn efter Kostnad.
* Adobe Workfront fyller i Tillgängliga timmar eller FTE enligt den arbetstid som är associerad med användarna i deras scheman.\
  Användare som inte är associerade med ett schema visar tillgänglighet enligt standardschemat.\
  Mer information om standardschemat finns i [Skapa ett schema](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Workfront fyller i information om planerade timmar eller heltidsanställda från Planerade timmar om uppgifter och problem i projekten.
* Workfront fyller i Faktiska timmar med den faktiska tid som loggats för uppgifter och utgåvor av de användare som tilldelats dem. Detta inkluderar tid inloggad på ett projekt.
* I användarvyn kan du göra följande:

   * Expandera varje användare för att visa en lista över projekt där användaren är tilldelad.

     >[!NOTE]
     >
     >Endast användare som är kopplade till projekt som ingår i filtren kan expanderas.

   * Expandera varje projekt för att visa en lista över jobbroller som användare kan utföra i dessa projekt.
   * Expandera varje roll för att visa en lista över uppgifter som användaren i den rollen är tilldelad till.

  Om användare inte har några jobbroller kopplade till sig visas deras tillgängliga, planerade och faktiska timmar eller FTE i avsnittet **Ingen roll**.\
  Mer information om vilka fält och objekt som visas när användarvyn används i resursplaneraren finns i avsnittet Projekt/Roll/Val av användarvy i [Resursplaneringsnavigeringsöversikt](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Översikt över fält som visas i användarvyn i resursplaneraren

Se följande tabeller för att förstå informationen som visas i vyn Användare i Resursplaneraren. Informationen visas i timmar eller FTE-värden.

* [AVL (tillgänglig) kolumn](#the-avl-available-column)
* [PLN-kolumnen (planerad)](#the-pln-planned-column)
* [ACT-kolumnen (faktisk)](#The%C2%A0ACT)
* [DIF-kolumnen (Differens)](#the-dif-difference-column)
* [Kolumnen % (procentandel för planerad timfördelning)](#the-planned-hours-allocation-percentage-column)

### Kolumnen AVL (tillgänglig) {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Visas av</strong> </td> 
   <td> <p><strong>Beskrivning</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Användare</td> 
   <td>Det totala antalet tillgängliga timmar eller heltidsanställda för användaren enligt deras schema. </td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td>Den här informationen är inte tillgänglig för projektet när användarvyn används i resursplaneraren. </td> 
  </tr> 
  <tr> 
   <td>Roll</td> 
   <td> <p>Totalt antal tillgängliga timmar eller heltidsanställda för rollen enligt användarens schema och rollens <strong>procentuella FTE-tillgänglighet</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td>Uppgift eller ärende</td> 
   <td>Den här informationen är inte tillgänglig för uppgiften eller utgåvan. </td> 
  </tr> 
 </tbody> 
</table>

Mer information om hur tillgängligheten för användare och roller beräknas baserat på användarens schema och procentandelen FTE-tillgänglighet för rollen finns i [Översikt över beräkning av timmar och FTE för användare och roller i resursplaneraren](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

### Kolumnen PLN (planerad) {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Visas av</strong> </td> 
   <td> <p><strong>Beskrivning</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Användare</td> 
   <td> Totalt antal planerade timmar eller heltidsanställda av alla uppgifter eller ärenden som tilldelats användaren i alla projekt.<br><p>Detta inkluderar uppgifter och ärenden som tilldelats användaren men inte är kopplade till någon jobbroll och uppgifter eller problem som inte finns i projekt som du har åtkomst till Hantera.</p><p>När användarallokeringen för timmar har ändrats med hjälp av belastningsutjämnaren för arbetsbelastning kan data i resursplaneraren påverkas om de valda datumen bara innehåller en del av en aktivitet eller ett problem. Mer information om hur du ändrar allokeringar för användare finns i <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Hantera användarallokeringar i Arbetsbelastningsutjämnaren</a> . </p></td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td> Totalt antal planerade timmar eller heltidsekvivalenter för alla uppgifter och ärenden som tilldelats en viss användare i projektet.<br><p>Obs! Detta inkluderar inte Planerade timmar eller FTE från uppgifter eller ärenden som inte tilldelats några användare. </p></td> 
  </tr> 
  <tr> 
   <td>Roll</td> 
   <td> <p>Totalt antal planerade timmar eller heltidsekvivalenter för alla uppgifter och ärenden som tilldelats användaren i den här rollen i projektet.</p> <p> <p>Obs! Detta inkluderar inte Planerade timmar eller FTE från uppgifter eller ärenden som tilldelats den här rollen, men inte till den här användaren i den här rollen. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Uppgift eller ärende</td> 
   <td>Planerade timmar eller heltidsanställda som är associerade med aktiviteten eller problemet i projektet.</td> 
  </tr> 
 </tbody> 
</table>

Tänk på följande när du visar Planerade timmar:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view)</p>
-->

* Planerade timmar fördelas jämnt till varje dag inom varaktigheten för uppgifter och utgåvor, för varje resurs som tilldelats dem. Aktivitetens eller utgivarens varaktighet baseras på planerad start- och slutförandetid och omfattar varje kalenderdag inom den tidsperioden.\
  Workfront tar hänsyn till schemat för användare eller projekt när Planerade timmar distribueras till användare eller projekt. I det här fallet fördelas planerade timmar jämnt till varje dag under varaktigheten för uppgifter eller ärenden exklusive helger, lediga dagar och schemaläggningsundantag.

  Om du till exempel visar resursplaneraren efter vecka och du har uppgifter som sträcker sig över flera veckor i projekt, beror antalet planerade timmar per vecka på hur många dagar inom den veckan som ingår i aktivitetens varaktighet. Detta fungerar på liknande sätt när resursplaneraren visas efter månad eller kvartal och när uppgifterna sträcker sig över flera månader eller kvartal.\
  Veckoslutsdagar, schemaundantag och lediga dagar exkluderas från denna distribution.

* Följande kategorier av uppgifter ingår i beräkningen av planerade timmar för varje resurs:

   * uppgifter som tilldelats användare i Resurspooler, jobbroller eller team i projektet.

     >[!TIP]
     >
     >Om uppgifter tilldelas team visas deras allokering under avsnitten **Ingen roll** och **Ingen användare**. Du kan se de planerade timmar som är kopplade till team, men du kan inte budgetera timmarna eftersom inga roller eller användare är kopplade till uppgifterna.

* Planerade timmar i resursplaneraren inkluderar inte Planerade timmar som är associerade med följande:

   * överordnade uppgifter
   * ej tilldelade uppgifter
   * problem när inställningen **Inkludera timmar från problem** är inaktiverad.

* Planerade timmar visas inte i resursplaneraren om aktivitetens eller ärendets varaktighet är noll.
* Planerade timmar som är associerade med inaktiverade användare visas inte.

Mer information om Planerade timmar och heltidsekvivalenter i resursplaneraren finns i [Översikt över timmar, heltidsekvivalenter och kostnadsinformation i projekt- och rollvyerna i resursplaneraren](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

### Kolumnen ACT (faktisk)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Visas av</strong> </td> 
   <td> <p><strong>Beskrivning</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Användare </td> 
   <td> <p>Den tid som användaren loggade in på alla uppgifter eller ärenden som tilldelats dem.</p> <p>Detta inkluderar följande:</p> 
    <ul> 
     <li>Uppgifter och ärenden som tilldelats användaren men inte är associerade med någon jobbroll.</li> 
     <li>Uppgifter och ärenden som inte finns i projekt som du har tillgång till Hantera. </li> 
    </ul> <p>Detta inkluderar endast den tid som är inloggad på projektet när användaren är tilldelad aktiviteter eller ärenden i det projektet.  </p> </td> 
  </tr> 
  <tr> 
   <td>Projekt </td> 
   <td> <p>Den tid som användaren loggade in på alla uppgifter och ärenden som tilldelats dem i projektet.</p> <p>Detta gäller även när de loggat direkt i projektet.</p> <p>Detta omfattar inte följande:</p> 
    <ul> 
     <li> <p>Tidsloggade uppgifter och ärenden som inte tilldelats några användare. </p> </li> 
     <li> <p>Tid för inloggning på överordnade uppgifter. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Roll</td> 
   <td> <p>Den tid som har loggats in på alla uppgifter eller ärenden som tilldelats användaren i den här rollen. </p> <p>Detta omfattar inte följande:</p> 
    <ul> 
     <li>Tidsloggade uppgifter och ärenden som tilldelats den här rollen men inte den här användaren i den här rollen.</li> 
     <li>Tid som loggats direkt i projektet eller de överordnade aktiviteterna. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Uppgift eller ärende </td> 
   <td> <p>Den tid som användaren loggade in på uppgifter och problem, som även är tilldelade till dem. </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>Den loggade tiden visas i den tidsram som motsvarar anmälningsdatumet för timposten, oavsett tidsramen för den uppgift, utgåva eller det projekt där timarna loggas.

Mer information om faktiska timmar finns i [Visa faktiska timmar](../../manage-work/tasks/task-information/actual-hours.md).

### DIF-kolumnen (Differens) {#the-dif-difference-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Visas av</strong> </td> 
   <td> <p><strong>Beskrivning</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Användare</td> 
   <td> <p>Skillnaden mellan användarens tillgängliga och planerade timmar eller FTE. </p> <p>Skillnaden i timma eller heltidsekvivalent beräknas med följande formel:</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <p>Obs! Om värdet visas i negativa röda tal, överfördelas användaren. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td>Den här informationen är inte tillgänglig för projektet. </td> 
  </tr> 
  <tr> 
   <td>Roll</td> 
   <td> <p>Skillnaden mellan tillgängliga och planerade timmar eller heltidsanställda för jobbrollen. </p> <p>Skillnaden i timma eller heltidsekvivalent beräknas med följande formel:</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <p>Obs! Om värdet visas i negativa röda tal överfördelas rollen. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Uppgift eller ärende</td> 
   <td>Den här informationen är inte tillgänglig för aktiviteten, utgåvan eller projektet. </td> 
  </tr> 
 </tbody> 
</table>

### Kolumnen % (procentandel för planerad timfördelning) {#the-planned-hours-allocation-percentage-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Visas av</strong> </td> 
   <td> <p><strong>Beskrivning</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Användare</td> 
   <td> <p>Fördelningen av planerade timmar eller heltidsekvivalenter som en procentandel av tillgängliga timmar. Procentandelen för allokering av planerade timmar beräknas med följande formel:</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>Samma beräkning används för FTE-värden. </p> </td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td>Den här informationen är inte tillgänglig för projektet när vyn <strong>Visa efter användare</strong> tillämpas på resursplaneraren.</td> 
  </tr> 
  <tr> 
   <td>Roll</td> 
   <td> Fördelningen av planerade timmar eller heltidsekvivalenter som en procentandel av tillgängliga timmar. <p>Procentandelen för allokering av planerade timmar beräknas med följande formel:</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>Samma beräkning används för FTE-värden.</p></td> 
  </tr> 
  <tr> 
   <td>Uppgift eller ärende</td> 
   <td>Den här informationen är inte tillgänglig för aktiviteten, utgåvan eller projektet. </td> 
  </tr> 
 </tbody> 
</table>

Om värdet för Planerade timmar eller FTE är noll är procentallokeringen 0 %. Om värdet för Tillgängliga timmar eller FTE är noll kan procentallokeringen inte beräknas.

Mer information om planerade timmar och heltidsekvivalenter och hur de visas i resursplaneraren finns i [Budgetresurser i resursplaneraren med projekt- och rollvyerna](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this table is ideal but it does not render in Markdown) </p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Column Name (Hours or FTE)</strong> </td>
<td><strong>Displayed By</strong> </td>
<td> <p><strong>Description</strong> </p> </td>
</tr>
<tr>
<td rowspan="5">AVL <br>(Available Hours or FTE)</td>
<td>User</td>
<td>The total of Available Hours or FTE for the user according to their schedule. </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project when applying the User view to the Resource Planner. </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Available Hours or FTE for the role according to the schedule of the user and the <strong>Percentage of FTE Availability</strong> of the role.</p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project.</td>
</tr>
<tr>
<td colspan="2"> <p colspan="2">For more information about how user and role availability is calculated based on the schedule of the user and the Percentage of FTE Availability of the role, see <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td rowspan="5">PLN <br>(Planned Hours or FTE)</td>
<td>User</td>
<td> The total of Planned Hours or FTE from all the tasks or issues assigned to the user on all the projects.<br><p>This includes tasks and issues that are assigned to the user but not associated with any job role and tasks or issues that are not on projects that you have access to Manage.</p><p>When the user allocation for hours has been modified using the Workload Balancer, the data in the Resource Planner can be affected if the dates selected contain only a portion of a task or issue. For information about modifying allocations for users, see <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a> . </p></td>
</tr>
<tr>
<td>Project</td>
<td> The total of Planned Hours or FTE from all the tasks and issues assigned to a specific user on the project.<br><note type="note">
This does not include the Planned Hours or FTE from tasks or issues that are not assigned to any users.
</note></td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Planned Hours or FTE from all the tasks and issues assigned to the user in this role on the project.</p> <p> <note type="note">
This does not include the Planned Hours or FTE from tasks or issues that are assigned to this role but not to this user in this role.
</note> </p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>The Planned Hours or FTE associated with the task or the issue on the project.</td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when viewing Planned Hours:</p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view))</p>
<ul>
<li> <p>Planned Hours are equally distributed to each day within the Duration of tasks and issues , for each resource assigned to them. The task or issue Duration is based on their Planned Start and Completion Dates and includes every calendar day within that period of time.<br>Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks or issues excluding weekends, time-off days, and schedule exceptions.</p> <p>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li>
<li> <p>The following categories of tasks are included in calculating the Planned Hours for each resource: </p>
<ul>
<li> <p> tasks assigned to users in Resource Pools, job roles, or teams on the project.</p> <note type="tip">
If tasks are assigned to teams, their allocation will appear under
<strong>No Role</strong> and
<strong>No User</strong> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks.
</note> </li>
</ul> </li>
</ul>
<ul>
<li> Planned Hours in the Resource Planner do not include Planned Hours associated with the following:
<ul>
<li>parent tasks</li>
<li>unassigned tasks</li>
<li>issues, when the <strong>Include hours from Issues</strong> setting is disabled.</li>
</ul></li>
<li>Planned Hours do not display in the Resource Planner if the task or issue Duration is zero.</li>
<li>Planned Hours associated with deactivated users do not display. </li>
</ul> <p>For more information about Planned Hours and FTE in the Resource Planner, see <a href="../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md" class="MCXref xref">Overview of hours, FTE, and cost information in the Project and&nbsp;Role views of the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td rowspan="5">ACT<br>(Actual Hours or FTE) </td>
<td>User </td>
<td> <p>The time logged by the user on all the tasks or issues assigned to them.</p> <p>This includes the following:</p>
<ul>
<li>Tasks and issues that are assigned to the user but not associated with any job role.</li>
<li>Tasks and issues that are not on projects for which you have access to Manage.. </li>
</ul> <p>This does not include time logged directly on the project or on parent tasks. </p> </td>
</tr>
<tr>
<td>Project </td>
<td> <p>The time logged by the user on all the tasks and issues assigned to them on the project.</p> <p>This includes any time that they logged directly on the project.</p> <p>This does not include the following:</p>
<ul>
<li> <p>Time logged on tasks and issues that are not assigned to any users. </p> </li>
<li> <p>Time logged on parent tasks. </p> </li>
</ul> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The time logged on all the tasks or issues assigned to the user in this role. </p> <p>This does not include the following:</p>
<ul>
<li>Time logged on tasks and issues assigned to this role but not to this user in this role.<em> </em></li>
<li>Time logged directly on the project or parent tasks. </li>
</ul> </td>
</tr>
<tr>
<td>Task or Issue </td>
<td> <p>The time logged on tasks and issues by the user who is also assigned to them. </p> </td>
</tr>
<tr>
<td colspan="2"> <p> <note type="important">
The time logged is displayed in the timeframe corresponding to the Entry Date of the hour entry, regardless of the timeframe of the task, issue, or project where the hours are logged.
</note> </p> <p>For more information about Actual Hours, see <a href="../../manage-work/tasks/task-information/actual-hours.md" class="MCXref xref">View Actual Hours</a></p> </td>
</tr>
<tr>
<td rowspan="4">DIF <br>(Hour or FTE Difference) <br><br></td>
<td>User</td>
<td> <p>The difference between the Available and Planned Hours or FTE of the user. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <note type="note">
If the value displays in negative red numbers, the user is overallocated.
</note> </p> </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project. </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The difference between the Available and Planned Hours or FTE of the job role. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <note type="note">
If the value is displayed in negative red numbers, the role is overallocated.
</note> </p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project. </td>
</tr>
<tr>
<td rowspan="5">Planned Hours or FTE Allocation Percentage (%)</td>
<td>User</td>
<td> <p>The allocation of the Planned Hours or FTE as a percentage of the Available Hours. The percentage of the Planned Hours Allocation is calculated using the following formula:</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>The same calculation is used for FTE values. </p> </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project when applying the <strong>View by User</strong> view to the Resource Planner.</td>
</tr>
<tr>
<td>Role</td>
<td> The allocation of the Planned Hours or FTE as a percentage of the Available Hours. <p>The percentage of the Planned Hours Allocation is calculated using the following formula:</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>The same calculation is used for FTE values.</p></td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project. </td>
</tr>
<tr>
<td colspan="2"> <p> If the value of the Planned Hours or FTE is zero, the Percentage Allocation is 0%. If the value of the Available Hours or FTE is zero, the Percentage Allocation cannot be calculated. </p> <p>For more information about Planned Hours and FTE and how they are displayed in the Resource Planner, see <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a>. </p> </td>
</tr>
</tbody>
</table>
-->

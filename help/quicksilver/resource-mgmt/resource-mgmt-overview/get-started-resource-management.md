---
content-type: overview
product-area: resource-management
navigation-topic: resource-management-overview
title: Kom igång med resurshantering
description: Med Resurshantering kan du konfigurera ditt system så att användningen av dina resurser beräknas utifrån tillgängligheten, så att det arbete som måste utföras i tid och budget slutförs korrekt.
author: Alina
feature: Resource Management
exl-id: b10ef503-60ea-4450-b63e-b2918e9bcc11
source-git-commit: c80d9b0b7eb2a638af9e0a11ca3038ed99ecf1ee
workflow-type: tm+mt
source-wordcount: '1167'
ht-degree: 0%

---

# Kom igång med resurshantering

<!-- Audited: 12/2023 -->

<!--
<p>(NOTE: DO NOT DELETE THIS ARTICLE. MANY ARTICLES MENTIONING RES MANAGEMENT ARE AND STILL SHOULD / WILL BE LINKED TO IT.) </p>
<p>(NOTE: Alina: ***As functionality is removed from Legacy and added to Res Planning - this will be continually updated: remove the Legacy Res Planning when that functionality is removed from the system.) </p>
</div>
-->

Med Resurshantering kan du konfigurera ditt system så att användningen av dina resurser beräknas utifrån tillgängligheten, så att det arbete som måste utföras i tid och budget slutförs korrekt.

## Översikt över resurshantering i Adobe Workfront

Resurshantering avser alla aktiviteter som utförs av Adobe Workfront-administratören, resurshanteraren och projektägaren för att planera (resurs- eller scenarioplanering) och schemalägga (arbetsbelastningsutjämning) en organisations resurser och tilldela dem till det arbete som behöver utföras, med hänsyn till deras tillgänglighet. Dessutom hänvisar resurshanteringen också till att visa information om den planerade och faktiska resursallokeringen i en rapportvy (utnyttjanderapport).

Workfront har flera verktyg som används för att hantera resurser. Varje verktyg har ett enskilt omfång. För närvarande kan du använda följande resurshanteringsverktyg i Workfront, beroende på vilket stadium av resurshanteringen du befinner dig i:

* Använd följande verktyg för att planera hur resurser fördelas på en högre nivå innan det verkliga arbetet i projekt börjar:

   * **Resursplaneraren**: Du kan använda resursplaneraren i det första steget i resurshanteringen för att budgetera projekttid för dina resurser enligt deras schemalagda tillgänglighet. Under planeringen av resursfasen kan du ordna användare i resurspooler och tilldela flera resurspooler till ett projekt.

     Mer information om resursplanering finns i [Resursplanering: artikelindex](../../resource-mgmt/resource-planning/resource-planning-overview.md).

   * **Scenarioplanering**: Det här är en planering på högre nivå av resurser som gör att du kan hantera dem över flera initiativ som kan omfatta en, tre eller fem års plan och innehålla flera projekt. Du kan använda det bästa scenariot för att få ut så mycket som möjligt av deras tillgänglighet och budget.

     Scenario Planner kräver en separat licens utöver Workfront-licensen. Mer information om Workfront Scenarioplan finns i [Översikt över scenarioplanen](../../scenario-planner/scenario-planner-overview.md).

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when more functionality is added, maybe we add that we recommend to start here if this is available for them?!) </p>   
     -->

* Använd följande verktyg om du vill schemalägga eller tilldela resurser till det verkliga arbetet (uppgifter och ärenden):

   * **Utjämning av arbetsbelastning**: Detta hör till en resurshanteringsfas på lägre nivå, där du kan tilldela resurser till det arbete (uppgifter och ärenden) som de måste utföra, baserat på hur många timmar som behövs för att slutföra dem och deras tillgänglighet. Med Utjämning av arbetsbelastning kan du tilldela användare till verkligt arbete som för närvarande inte är tilldelat eller tilldelat till jobbroller.

     Mer information om Workfront Balancer finns i [Arbetsbelastningsutjämning: artikelindex](../../resource-mgmt/workload-balancer/workload-balancer.md).

<!--

  * **Scheduling** (deprecated <span class="preview">and removed from the Preview environment</span>): Refers to assigning actual work to users by matching the job roles assigned to the tasks and issues with the job roles they can fulfill, or assigning actual work to users on tasks and issues which are currently unassigned. This happens at a lower-level in the process of managing resources, where you can assign your resources to the actual work (tasks and issues) that they must fulfill, according to the hours needed in the project plan to fulfill them.  

     For more information about resource scheduling, see the section [Resource Scheduling](../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md).

    >[!CAUTION]
    >
    >
    >We are no longer supporting the Resource Scheduling tools and they will be removed from Workfront in **January 2023**. We recommend that you use the Workload Balancer for scheduling your resources. 
    >
    >
    >* For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).
    >
    >
    >* For more information about the timeline for removing the Resource Scheduling tools and replacing them with the Workload Balancer, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

-->
* Använd följande verktyg för att analysera budgeterade, planerade och faktiska tilldelningar i flera projekt:

   * **Användningsrapport**: Använd den här rapporten om du vill visa användningen av resurser för projekt. Du kan jämföra budgeterade, planerade och faktiska tilldelningar för dina projekt och hur de påverkar projektens kostnader och intäkter.

     Mer information om användningsrapporten finns i [Visa information om resursutnyttjande](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Komponenterna i resurshanteringsprocessen

>[!NOTE]
>
>Resurshantering är aldrig en central process i Workfront. När schemana för projekten, tillgängligheten för användarna eller deras roller ändras måste du kontinuerligt justera informationen om resurser, deras tilldelningar och deras tilldelningar till projekt, uppgifter och ärenden.

Processen för att hantera resurser i Workfront omfattar följande steg:

* **Konfiguration**: Som systemadministratör, resurshanterare eller projektägare måste du konfigurera vissa fält och objekt i din Workfront-instans innan du hanterar dina resurser. Mer information om vilka krav som krävs för att börja hantera resurser i Workfront finns i avsnittet [Krav för korrekt resurshantering](#prerequisites-for-accurate-resource-management) i den här artikeln.\
  Förutom att ha projekt med arbetsobjekt måste du konfigurera följande objekt i Workfront:

   * Användare\
     Mer information om hur du skapar användare finns i artikeln [Lägg till användare](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   * Jobbroller\
     Mer information om hur du skapar jobbroller finns i artikeln [Skapa och hantera jobbroller](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

   * Scheman\
     Mer information om hur du skapar scheman finns i artikeln [Skapa ett schema](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   * Projektinställningar

     >[!TIP]
     >
     >Det är bara en system- eller gruppadministratör som kan ändra projektinställningarna för systemet eller gruppen.

     Mer information om hur du definierar projektinställningar finns i artikeln [Konfigurera systemomfattande projektinställningar](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * Resursgrupper

     Mer information om hur du skapar resurspooler finns i [Skapa resurspooler](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

   * Resurshanteringsinställningar

     Som system måste du bestämma hur Workfront ska beräkna användarnas tillgänglighet på systemnivå, oavsett om det sker med användarens schema eller systemets standardschema.

     Mer information finns i [Konfigurera inställningar för resurshantering](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **Resursallokering**: Som resurshanterare eller projektägare kan du definiera resursallokering för dina projekt samt tilldela arbete. I det här steget kan du hantera uppskattningen av resursallokeringen med hjälp av Resursplaneraren eller Scenarioplaneraren och tilldela faktiska arbeten till användare i Utjämning av arbetsbelastning.

  Mer information om resursplanering och tilldelning av arbete finns i följande avsnitt:

   * [Resursplanering: artikelindex](../../resource-mgmt/resource-planning/resource-planning-overview.md)
   * [Adobe Workfront Scenario Planner](../../scenario-planner/scenario-planning.md)
   * [Utjämning av arbetsbelastning: artikelindex](../../resource-mgmt/workload-balancer/workload-balancer.md)

<!--
* **Resource scheduling**: After generally planning for resources to use on your projects at a high level, you can start assigning work items (tasks and issues) to users based on their job roles using the Workload Balancer.

  For more information, see [Workload Balancer overview](../workload-balancer/overview-workload-balancer.md). 
-->

* **Analys**: Som resurshanterare, projektägare eller personansvarig granskar du användningsrapporten för att få en förståelse för hur budgeterade och planerade allokeringar av dina resurser jämfört med de faktiska. Granska informationen per timmar, kostnad eller intäkt. Mer information om användningsrapporten finns i [Visa information om resursutnyttjande](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Åtkomst som behövs för att visa och hantera resurser med verktygen för resurshantering i Workfront

Följande användare har tillgång till verktygen för resurshantering i Workfront:

Du måste vara en av följande användare och ha följande åtkomst och behörigheter för att komma åt resurshanteringsverktygen:

* Systemadministratören.
* En användare med en planlicens.

  En användare med en arbetslicens kan använda belastningsutjämnaren för ett projekt och hantera tilldelningar och tilldelningar.

  Förutom att du har en Work-licens eller en senare licens måste du ha följande för att kunna använda specifika resurshanteringsverktyg:

   * Redigera åtkomst till resurshantering (behövs inte för att göra tilldelningar i arbetsbelastningsutjämnaren)
   * Redigera åtkomst till finansiella data för att visa kostnadsinformation i resursplaneraren
   * Visa åtkomst till ekonomiska data för att visa kostnads- och intäktsinformation i användningsrapporten (endast användare med en planlicens)

* Contribute eller högre behörigheter som innehåller Skapa uppdrag för de projekt du vill hantera resurser för.

<!--
* Designated as a Resource Manager for projects to use the Scheduling tool (the Scheduling tool is deprecated).

  >[!TIP]
  >
  >You do not have to be a Resource Manager to use the Resource Planner, Scenario Planner, or the Workload Balancer. 
-->

Mer information om den åtkomst som krävs för att budgetera resurser finns i artikeln [Åtkomst krävs för att budgetera resurser](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

Mer information om åtkomsten som behövs för att hantera resurser i arbetsbelastningsutjämnaren finns i [Åtkomst som behövs för att hantera resurser i arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

## Krav för korrekt resurshantering  {#prerequisites-for-accurate-resource-management}

Du måste uppfylla en uppsättning krav innan du kan använda resurshanteringsverktygen i Workfront på ett effektivt sätt.

Mer information om kraven för varje resurshanteringsverktyg i Workfront finns i:

* Avsnittet [Krav för att arbeta i resursplaneraren](../../resource-mgmt/resource-planning/get-started-resource-planner.md#prerequisites-for-working-in-the-resource-planner) i artikeln [Resursplaneringsöversikt](../../resource-mgmt/resource-planning/get-started-resource-planner.md).
  <!--remove this at production: * The section "Prerequisites" in the article [Get started with Resource Scheduling](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).-->
* Avsnittet [Bästa tillvägagångssätt för att använda arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/overview-workload-balancer.md#best-practices-for-using-the-workload-balancer) i artikeln [Översikt över belastningsutjämnaren](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
* [Åtkomst krävs för att budgetera resurser i Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).
* [Åtkomst krävs för att hantera resurser i arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted and replaced with the links to each prerequisites instead) </p>
<p> We recommend that the following settings exist before starting to manage resources for your organization: </p>
<ul>
<li> You must have users in the system who have active accounts. </li>
<li> You must assign a Plan or a Worker license to the users whose work allocation you want to manage. <note type="note">
Although you can assign work to a Reviewer or a Requestor, they cannot complete it.
<br>We recommend against assigning work to Reviewers or Requestors. For information about access levels in Workfront, see
<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref" xrefformat="{para}">Access levels overview</a>.
</note></li>
<li> You must have job roles configured in the system.<br>For information about adding job roles to Workfront, see the article <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" xrefformat="{para}">Create and manage job roles</a>.</li>
<li> (Optional) If you want to budget cost for your work, your job roles and your users must also have rates associated with them.<br></li>
<li> You must associate at least one job role with your users. </li>
<li> You must specify a valid value for the FTE field of all users when you use the User's Schedule instead of The Default Schedule in your Resource Management system preferences. <br>For information about editing users to ensure they have a job role, FTE, or cost associated with them, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" xrefformat="{para}">Edit a user's profile</a>. For information about editing the Resource Management preferences in your system, see <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref" xrefformat="{para}">Configure Resource Management preferences</a>.</li>
<li>You must associate accurate schedules with your users and they should include schedule exceptions.<br>For information about creating and editing schedules, see the article <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" xrefformat="{para}">Create a schedule</a>.</li>
<li>The Time Off calendar of the users must be up to date. </li>
<li> <p>The following is recommended for the Resource Planner when applying the Project and Role views: </p>
<ul>
<li> <p>You must associate projects with Resource Pools.<br>For information about associating projects with Resource Pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md" class="MCXref xref" xrefformat="{para}">Associate resource pools with projects and templates</a>.</p> </li>
</ul> </li>
<li> <p>Your must designate a Resource Manager on your projects and they must have the correct access to budget resources when using the Scheduling tools. </p> <p>For information about the access needed to budget resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref" xrefformat="{para}">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p> </li>
<li> <p>You must assign the tasks and issues in your system to job roles, teams, or users.</p> </li>
<li>You must specify a valid value for Planned Hours and Duration for all tasks in your system.<br>For information about Planned Hours, see the article <a href="../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref" xrefformat="{para}">Planned Hours overview</a>.<br>For information about Duration, see the article <a href="../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref" xrefformat="{para}">Overview of Task Duration and Duration Type</a>.</li>
</ul>
</div>
-->

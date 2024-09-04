---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: Resursplanering - översikt
description: Du kan beräkna och budgetera allokeringen av dina resurser till de projekt som de är tilldelade och prognostisera deras tillgänglighet för framtida arbete med hjälp av Resursplanering.
author: Lisa
feature: Resource Management
exl-id: 06cd2226-f94d-4b6a-8692-6d35210782f2
source-git-commit: a5317e3126939d4c648977635af2dbc6add02780
workflow-type: tm+mt
source-wordcount: '2075'
ht-degree: 0%

---

# Översikt över resursplanering

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: this used to be the beginning of Planning in the Resource Planner - consider restructuring it further? Merging some of this information with information about Understanding Navigation in the RP?!)</p>
-->

Du kan beräkna och budgetera allokeringen av dina resurser till de projekt som de är tilldelade och prognostisera deras tillgänglighet för framtida arbete med hjälp av Resursplanering.

En allmän översikt över resursplanering i Adobe Workfront finns i artikeln [Kom igång med resursplanering](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Översikt över resursplanering

Du kan använda resursplaneraren för att enkelt förstå tillgängligheten för användare och jobbroller samt den tid som krävs för att slutföra arbetet med projekt. Du kan sedan bestämma hur du ska tilldela användare och deras jobbroller till de projekt de tilldelas baserat på deras tillgängliga tid.

>[!IMPORTANT]
>
>Du kan inte använda resursplaneraren för att tilldela användare verkligt arbete (uppgifter och ärenden). Du kan bara beräkna hur lång tid det tar för användare eller jobbroller att slutföra ett projekt, oavsett vilka uppgifter och ärenden de har tilldelats.\
>Om du vill tilldela användare verkligt arbete måste du använda Utjämning av arbetsbelastning. Mer information om belastningsutjämnaren finns i [Översikt över belastningsutjämnaren](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Du kan visa information i resursplaneraren i tre olika vyer. Du kan använda varje vy för att uppfylla något av följande syften:

* Om du vill budgetera tiden eller kostnaden för dina resurser för det arbete som behöver utföras med projekt- och rollvyerna. Detta är huvudsyftet med resursplaneraren.\
  Mer information om budgetering i resursplaneraren finns i artikeln [Budgetresurser i resursplaneraren med projekt- och rollvyerna](../resource-planning/budget-resources-project-role-views-resource-planner.md).

* Så här visar du följande information i användarvyn:

   * Tillgängligheten för dina användare enligt deras schema
   * Den planerade tid som krävs för att slutföra arbetet enligt projektplanen
   * Den tid som användare redan har loggat in på faktiska arbetsobjekt

  Mer information om hur du visar Tillgängliga, Planerade och Faktiska timmar eller FTE för användare i resursplaneraren finns i artikeln [Visa tillgängliga, Planerade och Faktiska timmar eller FTE i resursplaneraren när du använder användarvyn](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md#using).

## Resursplaneringsfrågor

* Du kan prioritera de projekt som du arbetar med och budgetera resurstilldelningen utifrån deras prioritet, så att du ser till att du har resurser tilldelade till de viktigaste projekten först.

  Mer information om hur du prioriterar projekt i resursplaneraren finns i [Prioritera projekt i resursplaneraren](../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).

* Du kan visa timtals-, FTE- och kostnadsinformation från uppgifter och utgåvor av projekt.

  >[!NOTE]
  >
  >Uppgifter och ärenden visas inte i resursplaneraren. Timmar, heltidsekvivalenter och kostnadsinformation från resursallokeringarna för aktiviteterna visas i resursplaneraren som ett totalt antal för projektet.

* Timme-, FTE- och kostnadsinformation från överordnade uppgifter är exkluderad från de projekt som visas i resursplaneraren. Vi rekommenderar att du endast tilldelar resurser till underordnade uppgifter om du vill hantera resursernas tid eller kostnad i resursplaneraren.

  Mer information om överordnade uppgifter finns i följande artiklar:

   * [Aktivitetsöversikt](../../manage-work/tasks/task-information/tasks-overview.md)
   * [Skapa underaktiviteter](../../manage-work/tasks/create-tasks/create-subtasks.md)

  >[!TIP]
  >
  >Överordnade uppgifter visar det totala antalet timmar och kostnader för de underordnade uppgifterna. På grund av detta räknas dessa belopp två gånger när du räknar timmar, heltidsekvivalenter och kostnader för de underordnade aktiviteterna och de överordnade aktiviteterna. Det är därför den överordnade uppgiftsinformationen inte ingår i resursplaneraren.

* Du kan inte hantera allokeringen av team i de projekt där de har uppgifter eller problem i resursplaneraren.
* Du kan budgetera resurser för flera projekt samtidigt med hjälp av Resursplanering eller för ett enskilt projekt med hjälp av resursbudgeteringsområdet i affärsärendet. Den information du budgeterar för ett projekt visas också i Resursplanering.

  Mer information om hur du kan budgetera resurser för ett enskilt projekt finns i artikeln [Budgetresurser i affärsärendet](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

  Mer information om hur du kan budgetera resurser i resursplaneraren för flera projekt samtidigt finns i avsnittet Budgetresurser i resursplaneraren i artikeln [Budgetresurser i resursplaneraren med hjälp av projekt- och rollvyerna](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

## Krav för att arbeta i resursplaneraren {#prerequisites-for-working-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(<b>THIS SECTION IS LINKED TO ALL RES PLANNING ARTICLES. DO NOT RENAME OF DELETE THIS!</b> - do NOT ADD the variable here, because it might break this link!)</p>
-->

Om du vill använda resursplaneraren för att budgetera dina resurser måste du först se till att du, dina projekt och dina aktiviteter uppfyller en uppsättning krav. Dessa krav är obligatoriska för att visa korrekt information i resursplaneraren och för att hantera dina resurser på ett korrekt sätt.

>[!IMPORTANT]
>
>Om något av följande villkor saknas kanske en del av informationen om allokeringen eller tillgängligheten för resurserna saknas eller har ett nollvärde.\
>Om du vill ha mer information om varför fält saknar data eller har noll värden håller du pekaren över fälten.

![](assets/no-users-with-this-role-in-the-res-pool-350x57.png)

>[!NOTE]
>
>Följande krav är bara obligatoriska när du visar resursplaneraren efter projekt eller jobbroll eller vid budgetering av resurser i ett projekts affärsfall.

Följande typer av krav krävs för att resursplaneraren ska fungera korrekt när den visas efter projekt eller roll:

* [Förutsättningar för användare](#user-prerequisites)
* [Projektkrav](#project-prerequisites)
* [Förutsättningar för aktiviteter och ärenden](#tasks-and-issues-prerequisites)
* [Krav på systemnivå](#system-level-prerequisites)

### Krav för användare {#user-prerequisites}

Kontrollera att följande användarinställningar finns innan du börjar använda resursplaneraren:

* Du har rätt åtkomst till budgetresurser.

  Mer information om den åtkomst som krävs för att budgetera resurser finns i artikeln [Åtkomst krävs för att budgetera resurser i Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* Användare som är tilldelade aktiviteter läggs till i de resurspooler som är associerade med projektet.

  Mer information om hur du lägger till användare i resurspooler finns i [Associera resurspooler med användare](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md).

  >[!NOTE]
  >
  >När användare inte läggs till i resurspooler kan följande scenarier finnas:
  >
  >   
  >   
  >   * Användarna visas inte i resursplaneraren även om de kan tilldelas aktiviteter i projekten.
  >   * Om de uppgifter de är kopplade till har Planerade timmar visas dessa timmar inte för projektet i resursplaneraren, såvida inte användaren också är associerad med en jobbroll för dessa uppgifter.
  >   * Om användarna är associerade med en jobbroll för en aktivitet i projektet visas Planerade timmar i resursplaneraren för jobbrollen, men jobbrollen kan inte budgeteras.
  >   
  >

* Användare som är tilldelade till arbets- och resurspooler måste ha scheman och jobbroller kopplade till sin profil.

  Mer information om hur du associerar scheman och jobbroller med användare finns i [Redigera en användares profil](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

  >[!NOTE]
  >
  >Användare som inte är associerade med ett schema men som finns i projektets resurspool kan inte budgeteras i resursplaneraren.

* För korrekt information om tillgängliga timmar bör du se till att scheman som är kopplade till dina användare har schemaundantagen och tidsgränsen för uppdateringar.

  >[!NOTE]
  >
  >Om en användare inte är associerad med ett schema, är standardschemat i ditt Workfront-system associerat med användaren som standard i Resursplaneraren.

  Mer information om hur du skapar scheman finns i artikeln [Skapa ett schema](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Om du vill budgetera dina resurser efter kostnad måste du associera jobbroller med Kostnad/tim. räntenivåer. Kostnaden som är associerad med jobbroller som tilldelats användare i dina resurspooler används för att beräkna budgeterad arbetskostnad och budgeterad kostnad för projektet.\
  Mer information om hur du associerar jobbroller med frekvenser finns i artikeln [Skapa och hantera jobbroller](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
  Mer information om beräkning av budgeterad arbetskostnad finns i artikeln [Förstå budgeterad arbetskostnad och budgeterade timmar för projekt](../../manage-work/projects/project-finances/budgeted-labor-cost.md).\
  Mer information om hur du beräknar budgeterad kostnad finns i artikeln [Beräkna budgeterad kostnad](../../manage-work/projects/project-finances/budgeted-cost.md).

### Projektkrav {#project-prerequisites}

Kontrollera att följande projektinställningar finns innan du börjar använda resursplaneraren:

* Dina projekt är kopplade till resurspooler.\
  Mer information om hur du lägger till resurspooler i projekt finns i [Associera resurspooler med projekt och mallar](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md).

  >[!IMPORTANT]
  >
  >Projekt utan resurspooler visar inte information om planerad timme eller tilldelningar i resursplaneraren.

### Krav för uppgifter och problem {#tasks-and-issues-prerequisites}

Även om du inte kan visa uppgifter och problem i resursplaneraren överförs deras information till de projekt som visas i resursplaneraren.

Se till att följande installations- och utgivningsinställningar finns innan du startar budgeteringsresurserna i resursplaneraren:

* Aktiviteter eller problem i projekt som du budgeterar resurser för tilldelas en av dessa enheter:

   * Användare i projektets resurspooler som också är associerade med jobbroller
   * Jobbroller

  >[!NOTE]
  >
  >De planerade timmarna med uppgifter och ärenden som tilldelats till jobbroller visas i resursplaneraren, men dessa timmar kan inte budgeteras om inte en användare som är associerad med jobbrollen listas i en resurspool som är associerad med projektet.

* Du bör inte tilldela överordnade uppgifter till användare eller roller.

  Om du vill visa timinformation i resursplaneraren för användare eller roller som är kopplade till överordnade uppgifter måste du även tilldela dem till de underordnade uppgifterna. Resursplaneraren visar inte information från överordnade aktiviteter.

* Aktiviteter och ärenden har ett värde för Planerade timmar som är större än noll.
* Aktiviteter och ärenden har ett värde för Varaktighet som är större än noll.
* Planerade datum för problemen ligger inom tidslinjen för projektet.

### Krav på systemnivå {#system-level-prerequisites}

Du måste förstå hur din instans av Workfront beräknar användartillgänglighet enligt inställningarna för resurshantering i ditt system. Workfront kan beräkna användartillgängligheten med hjälp av användarens schema så som det definieras på sidan Användarprofil eller med datorns standardschema.

![](assets/resource-management-preferences-section-in-setup-350x89.png)

Din Workfront-administratör konfigurerar inställningarna för resurshantering.

Mer information finns i [Konfigurera inställningar för resurshantering](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Leta reda på resursplaneraren

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This became another standalone article; drfat this section here when article is live.)</p>
-->

Du kan hitta resursplaneraren i två områden i Workfront, beroende på om du vill budgetera dina resurser för flera projekt eller bara för ett projekt.

Mer information om hur du hittar resursplaneraren finns i [Hitta resursplaneraren](../../resource-mgmt/resource-planning/locate-resource-planner.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(this is drafted and moved to its own article: locate-resource-planner) </p>
<p>Ensure that all prerequisites are met before starting to use the Resource Planner. This way, you ensure that the Resource Planner displays the correct information before you start budgeting your resources.<br>For information about the prerequisites that must be met before you can start using the Resource Planner, see the <a href="#prerequisites-for-working-in-the-resource-planner" class="MCXref xref">Prerequisites for working in the Resource Planner</a> section in this article. </p>
<p>You can locate the Resource Planner in two areas of Workfront, depending on whether you want to budget your resources for multiple projects, or for just one project.</p>
<ul>
<li><a href="#use-the-resource-planner-for-multiple-projects" class="MCXref xref">Use the Resource Planner for multiple projects</a> </li>
<li> <p><a href="#use-the-resource-planner-for-one-project" class="MCXref xref">Use the Resource Planner for one project</a> </p> </li>
</ul>
<p><strong>Use the Resource Planner for multiple projects</strong></p>
<p>When using the Resource Planner for multiple projects, the allocation numbers for your resources represent numbers across multiple projects. </p>
<p>To access the  Planner section  in the  Resourcing area: </p>
<ol>
<li value="1">  Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.  </li>
<li value="2"> <p>  Click <strong>Resourcing</strong>. The Resource Planner displays by default.  For information about budgeting resources in the Resource Planner, see the article <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a>. </p> <p> <img src="assets/qs-resource-management-area-with-planner-as-default-350x152.png" style="width: 350;height: 152;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">  Hover over the left panel, and click <strong>Resource Pools</strong>. <br>For information about creating new resource pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md" class="MCXref xref">Create resource pools</a>.</li>
</ol>
<p><strong>Use the Resource Planner for one project</strong></p>
<p>When using the Resource Planner for one project, the allocation numbers for your resources represent numbers for the selected project. </p>
<ol>
<li value="1"> <p>Go to a project you want to budget resources for.</p> </li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Business Case</strong> in the left panel.</p> </li>
<li value="3"> <p>Scroll to the <strong>Resource Budgeting</strong> section of the Business Case.</p> </li>
<li value="4"> <p>Click <strong>Edit Resource Budgeting</strong> to add resource pools to your project and start budgeting your resources. </p> <note type="tip">
You can only add a resource pool in the Resource Budgeting area of the Business Case when the project has no resource pools associated with it. When the project already has a resource pool, the users in the pool and their job roles display in the Resource Budgeting area by default.
</note> <p> <img src="assets/resource-budgeting-area-on-project-350x70.png" style="width: 350;height: 70;"> </p> <p>For information about budgeting resources for one project, see the article <a href="../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md" class="MCXref xref">Budget resources in the Business Case</a>.</p> </li>
</ol>
</div>
-->

## Resursplaneringens områden

Du kan visa följande information eller utföra följande åtgärder i resursplaneraren:

* Information om de resurser som har tilldelats dina projekt i resursplaneraren på en allmän tidslinje.
* Överbeläggning eller underutnyttjande av resurser i Resursplanering.
* Budgetera dina resurser för arbete manuellt eller automatiskt.

Mer information om vilka områden som visas i resursplaneraren och hur du konfigurerar vilken information som visas i de här områdena finns i artikeln [Resursplaneringsnavigeringsöversikt](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Begränsningar i visning av information i resursplaneraren

För att förbättra prestanda begränsar Workfront mängden objekt som du kan visa i resursplaneraren.

Mer information om de här begränsningarna finns i artikeln [Resursplanering, visningsbegränsningar](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md) .

## Beräkna heltidsanställd i resursplaneraren

Du kan visa värden för tillgänglighet, allokering och planerad i resursplaneraren i Timmar, FTE eller Kostnad.

Mer information om hur du ändrar den information du visar i resursplaneraren finns i avsnittet [Visa information per timme, heltid eller kostnad](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#display-by-hour-or-fte-menu) i artikeln [Granska resurstillgänglighet och allokering med Adobe Workfront resursplanerare](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

Mer information om hur timmar och heltidsanställda för användare och roller beräknas i Workfront finns i artikeln [Översikt över beräkning av timmar och heltidsanställda för användare och roller i resursplaneraren](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

## Beräkna kostnader i resursplaneraren

Du måste ha behörigheterna Visa åtkomst till finansiella data och Visa ekonomiska behörigheter för projekten för att kunna se informationen efter kostnad i resursplaneraren.

Förutom att visa tillgänglighets-, allokerings- och planvärden i resursplaneraren i timmar och heltidsekvivalenter kan du även visa dem som Kostnad.

>[!TIP]
>
>Du måste associera dina användare och dina jobbroller med kostnad per timme för att kunna visa information efter kostnad i resursplaneraren.

Mer information om hur du associerar kostnadsnivåer per timme med jobbroller finns i artikeln [Skapa och hantera jobbroller](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
Mer information om hur du associerar kostnad per timme med användare finns i artikeln [Redigera en användares profil](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Tänk på följande när du visar information per kostnad i resursplaneraren:

* Kostnaden för varje typ av timmar (Planerat, Tillgängligt, Budgeterat, Faktiskt för användare, Roller eller Projekt) beräknas med en annan kostnadsnivå.
* Den planerade kostnaden påverkas av kostnadstypen för aktiviteterna i projekten.
* När du använder användarvyn i resursplaneraren kan du inte visa information om allokering och tillgänglighet per kostnad.

Mer information om hur kostnader beräknas i resursplaneraren för användare och roller finns i artikeln [Beräkna kostnader i resursplaneraren](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the User View to view Available, Planned, and Actual Hours or FTE </h2>
<p>(this information is repeated from above where it exists in shorter form. Drafted to simplify the amount of info of this article.) </p>
<p>You can use the User View of the Resource Planner to display information about the Planned, Available, and Actual Hours or FTE values for projects and resources. </p>
<p>For information about using the Resource Planner to review the Available, Planned, and Actual Hours and FTE for resources, see the article <a href="../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md" class="MCXref xref">View Available, Planned, and Actual Hours or FTE in the Resource Planner when using the User view</a>.</p>
<p><strong>Use the Project and Role Views to budget resources </strong></p>
<p> The main function of the Resource Planner is to budget your resources for the work that needs to be completed on the projects that you can manage. </p>
<p> You can budget your resources only if you apply the <strong>View by Project</strong> or <strong>View by Role</strong> views to the Resource Planner.</p>
<p>For information about budgeting resources using the Project and Role views in the Resource Planner, see the article <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md"><a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a></a>.</p>
</div>
-->

## Filtrera information i resursplaneraren

Du kan minska antalet projekt, roller eller användare som visas i resursplaneraren genom att skapa ett filter.\
Mer information finns i artikeln [Filterinformation i resursplaneraren](../../resource-mgmt/resource-planning/filter-resource-planner.md).

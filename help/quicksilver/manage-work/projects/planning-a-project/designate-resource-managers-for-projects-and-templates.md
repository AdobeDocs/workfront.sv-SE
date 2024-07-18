---
product-area: projects;templates
navigation-topic: plan-a-project
title: Ange resurshanterare för ett projekt eller en mall
description: Du kan utse resurshanterare för ett projekt för att ange vem som ansvarar för att hantera resurser i projektet.
author: Alina
feature: Work Management
exl-id: ae2a89e7-8049-4ee6-9b28-ce247d3f2a6f
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 0%

---

# Ange resurshanterare för ett projekt eller en mall

<!--
<p This article might have to be deleted when the Resource Manager field/ requirement will be forever removed from the system; right now it's still a requirement for Scheduler - January 2023/p>
-->

<!-- remove Prod and Prev references with Prod release - Jan 2023-->

Du kan utse resurshanterare för ett projekt för att ange vem som ansvarar för att hantera resurser i projektet. Det här är ett informationsfält och det är inte anslutet till några resurshanteringsverktyg.

<!-- drafted for res scheduling deprecation blurb for preview release
Designating Resource Managers for a project is a prerequisite for using the Scheduling tools in Adobe Workfront, in the Production environment.
  
>[!CAUTION]  
>  
>  
> <span class="preview">Some of the information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span>  
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span>  
>  
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../../resource-mgmt/workload-balancer/workload-balancer.md).</span>  
>  
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

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
   <td> <p>Edit access to Projects and Templates</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project or template</p> 
   
   <p><b>NOTE</b>
   
   Users who are added as Resource Managers to a project or a template immediately gain Manage permissions on the project or the template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till projekt och mallar</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för projektet eller mallen</p>

<p><b>ANMÄRKNING</b>

Användare som läggs till som resurshanterare i ett projekt eller en mall får omedelbart behörigheten Hantera i projektet eller mallen</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td>
</tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Överväganden om resurshanterare

>[!NOTE]
>
>Resurshanteraren är inte en jobbroll. Det är ett fält som är tillgängligt i ett projekt eller en mall som du kan uppdatera manuellt.

* Du kan utse upp till 30 användare till resurshanterare för ett enskilt projekt eller en enskild mall.

<!--
* In the Production environment,designating Resource Managers on projects is a prerequisite to allowing users to schedule resources for work on the project when using the Scheduling tools.

  For information about resource scheduling, see [Resource Scheduling](../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md). 

  <span class="preview">Scheduling tools have been removed from the Preview environment.</span>

* Designating Resource Managers on projects is not a prerequisite to allowing users to schedule resources for work using the Workload Balancer.

  For information about the Workload Balancer, see [Workload Balancer overview](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md). 

 -->

* Du kan inte ange team eller grupper som resurshanterare. Du kan bara utse användare som resurshanterare.

* De användare som du anger som resurshanterare för ett projekt eller en mall blir inte automatiskt en del av projektgruppen.

  Mer information om projektteam finns i [Hantera projektteamet](../../../manage-work/projects/planning-a-project/manage-project-team.md).

* Du kan utse resurshanterare för projekt eller för projektmallar. När du anger Resurshanterare för en projektmall blir alla användare som du anger som resurshanterare för mallen automatiskt Resurshanterare för alla projekt som skapas med den mallen.
* Du kan visa fältet Resurshanterare i följande områden:

   * När du redigerar ett projekt, enligt beskrivningen i den här artikeln.
   * När du redigerar en mall, enligt beskrivningen i den här artikeln.
   * När projekt- eller mallrapporter skapas. Mer information om hur du skapar rapporter finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
   * När du skapar eller anpassar ett projekt eller en mallvy för en lista. Mer information finns i [Vyöversikt i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* Du kan snabbt lägga till eller ta bort resurshanterare för flera projekt eller mallar genom att lägga till resurshanterarfältet i en vy av en lista eller ett projekt och redigera det här fältet med hjälp av redigering i rad.

## Ange resurshanterare för ett projekt

1. Gör något av följande:

   * Om du vill lägga till resurshanterare i ett enskilt projekt går du till det projekt där du vill utse en eller flera resurshanterare, klickar på **Mer-menyn** bredvid projektnamnet och sedan på **Redigera.**

   * Om du vill lägga till resurshanterare i flera projekt samtidigt går du till en lista med projekt, markerar de projekt där du vill utse en eller flera resurshanterare och klickar sedan på **Redigera**.

     Befintliga resurshanterare tas inte bort från projekt som du redigerar. Alla användare som du lägger till på det här sättet läggs till som resurshanterare i projektet utöver befintliga resurshanterare.

   * Börja skapa ett nytt projekt om du vill lägga till resurshanterare i ett nytt projekt.

     Mer information om hur du skapar ett projekt finns i [Skapa ett projekt](../../../manage-work/projects/create-projects/create-project.md).

1. Klicka i fältet **Resurshanteraren** i avsnittet **Översikt** i dialogrutan Redigera projekt.
1. Börja skriva namnet på den användare som du vill lägga till som resurshanterare för projektet och klicka sedan på namnet när det visas i listan.

   Upprepa det här steget om du vill lägga till flera resurshanterare för projektet.

1. Klicka på **Spara ändringar**.

## Ange resurshanterare för en mall

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.

1. Klicka på **Mallar**.

1. Gör något av följande:

   * Om du vill lägga till resurshanterare i en enskild mall går du till mallen där du vill utse en eller flera resurshanterare, klickar på menyn **Mer** bredvid mallnamnet och sedan på **Redigera.**

   * Om du vill lägga till resurshanterare i flera mallar samtidigt går du till en lista med mallar och väljer de mallar där du vill utse en eller flera resurshanterare. Klicka sedan på **Redigera**.

     Befintliga resurshanterare tas inte bort från mallarna som du redigerar. Alla användare som du lägger till på det här sättet läggs till som resurshanterare i mallen förutom befintliga resurshanterare.

   * Om du vill lägga till resurshanterare i en ny mall klickar du på **Ny mall** och sedan på **Mer-menyn** bredvid mallnamnet och sedan på **Redigera.**

1. Klicka i fältet **Resurshanteraren** i avsnittet **Översikt**.
1. Börja skriva namnet på den användare som du vill lägga till som resurshanterare för mallen och klicka sedan på namnet när det visas i listan.

   Upprepa det här steget om du vill lägga till flera resurshanterare i mallen.

1. Klicka på **Spara ändringar**.

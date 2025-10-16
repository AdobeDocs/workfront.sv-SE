---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Åtkomst krävs för att hantera resurser i arbetsbelastningsutjämnaren
description: Utan rätt åtkomst eller behörigheter kanske du inte kan visa eller hantera dina arbetstilldelningar i Utjämning av arbetsbelastning.
author: Lisa
feature: Resource Management
exl-id: b3da9a62-481e-4503-8f27-136d6513262e
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---

# Åtkomst krävs för att hantera resurser i arbetsbelastningsutjämnaren

{{preview-fast-release-general}}

Utan rätt åtkomst eller behörigheter kanske du inte kan visa eller hantera dina arbetstilldelningar i Utjämning av arbetsbelastning.

Du måste ha tillgång till de användare vars arbetsbelastning du vill visa eller hantera i Utjämning av arbetsbelastning. Utöver detta måste du ha rätt åtkomstnivå och rätt behörigheter för de projekt som arbetet är kopplat till.

<!--## Adobe Workfront package needed to use the Workload Balancer for different areas

The following table illustrates the connection between the Workfront plan your company has and where in the system you can use the Workload Balancer:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><p><b>Workfront Plan (Current)</b></p></td> 
   <td> <p><b>Areas where you can access the Workload Balancer</b></p> </td> 
  </tr> 
  <tr> 
   <td>Team or higher </td> 
   <td>Workload Balancer for a team or a project</td> 
  </tr> 
  <tr> 
   <td>Pro or higher</td> 
   <td>Workload Balancer for multiple projects, at the system level</td> 
  </tr> 
  <tr> 
   <td><p><b>Workfront Plan (New)</b></p></td> 
   <td> <p><b>Areas where you can access the Workload Balancer</b></p> </td> 
  </tr>
  <tr> 
   <td>Any </td> 
   <td>Access the Workload Balancer anywhere in Workfront</td> 
  </tr> 
 </tbody> 
</table>

For information about the Workfront plans, see [Our Plans](https://business.adobe.com/se/products/workfront/pricing.html).

For information about where you can locate the Workload Balancer in Workfront, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).-->

## Åtkomst krävs för att visa arbetsbelastningsutjämnaren

Du måste ha följande åtkomst för att kunna visa arbetsbelastningsutjämnaren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Alla</p></td>
  </tr>
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td><p>Standard</p>
       <p>Planera, för att visa belastningsutjämnaren i resursområdet, Arbete, för att visa belastningsutjämnaren för ett team eller projekt</p></td>
  </tr>  
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa eller högre åtkomst till resurshantering</p> <p>Mer information om åtkomstnivån för resurshantering finns i artikeln <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md">Bevilja åtkomst till resurshantering</a>.</p></td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td> 
   <td> <p>Du måste ha behörigheten Visa för det projekt vars uppdrag du vill visa. </p> <p>Mer information om projektbehörigheter finns i artikeln <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md">Dela ett projekt i Adobe Workfront</a>.</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<span class="preview">Alla användare har tillgång till arbetsbelastningsutjämnaren för sina egna profiler. Detta begränsas inte av licens- eller åtkomstnivå. Observera att belastningsutjämnaren för arbetsbelastning i en användarprofil är skrivskyddad och att tilldelningar och allokeringar inte kan ändras.</span>

## Åtkomst krävs för att hantera tilldelningar i arbetsbelastningsutjämnaren

Du måste ha följande åtkomst för att kunna hantera belastningsutjämnaren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Alla</p></td>
  </tr>
  <tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td><p>Standard</p>
       <p>Planera, för att hantera tilldelningar i Utjämning av arbetsbelastning i resursområdet, Arbeta, för att hantera tilldelningar i Utjämning av arbetsbelastning för ett team eller projekt</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td>
   <td> <p>Redigera åtkomst till resurshantering</p>
     <p>Mer information om åtkomstnivån för resurshantering finns i artikeln <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" >Bevilja åtkomst till resurshantering</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td> 
   <td> <p> Contribute eller högre behörigheter för det projekt vars uppdrag du vill hantera, inklusive behörigheter för att utföra uppdrag. </p> <p>Mer information om projektbehörigheter finns i artikeln <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md">Dela ett projekt i Adobe Workfront</a>.</p></td>
  </tr> 
 </tbody>
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--these notes were inside the table: for the Edit access to Res Management
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">View or higher access to Financial Data, if you want to view information by cost (NOTE: this is not possible yet!)</p>    
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Financial Data access level, see the article<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. (NOTE: this is not possible yet!)</p>
    -->

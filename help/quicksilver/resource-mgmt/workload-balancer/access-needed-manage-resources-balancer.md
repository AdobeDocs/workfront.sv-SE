---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Åtkomst krävs för att hantera resurser i arbetsbelastningsutjämnaren
description: Utan rätt åtkomst eller behörigheter kanske du inte kan visa eller hantera dina arbetstilldelningar i Utjämning av arbetsbelastning.
author: Lisa
feature: Resource Management
exl-id: b3da9a62-481e-4503-8f27-136d6513262e
source-git-commit: 78d73d0d7bd0ffc00ae1afed0adb324501e0c310
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# Åtkomst krävs för att hantera resurser i arbetsbelastningsutjämnaren

{{preview-fast-release-general}}

Utan rätt åtkomst eller behörigheter kanske du inte kan visa eller hantera dina arbetstilldelningar i Utjämning av arbetsbelastning.

Du måste ha tillgång till de användare vars arbetsbelastning du vill visa eller hantera i Utjämning av arbetsbelastning. Utöver detta måste du ha rätt åtkomstnivå och rätt behörigheter för de projekt som arbetet är kopplat till.

## Adobe Workfront-planen behövs för att använda belastningsutjämnaren för olika områden

Följande tabell visar kopplingen mellan den Workfront-plan ditt företag har och var i systemet du kan använda belastningsutjämnaren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p><b>Workfront-plan (aktuell)</b></p></td> 
   <td> <p><b>Områden där du kan komma åt arbetsbelastningsutjämnaren</b></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Team eller högre </td> 
   <td>Utjämning av arbetsbelastning för ett team eller ett projekt</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pro eller högre</td> 
   <td>Utjämning av arbetsbelastning för flera projekt på systemnivå</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p><b>Workfront-plan (ny)</b></p></td> 
   <td> <p><b>Områden där du kan komma åt arbetsbelastningsutjämnaren</b></p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Alla </td> 
   <td>Få åtkomst till belastningsutjämnaren var som helst i Workfront</td> 
  </tr> 
 </tbody> 
</table>

Mer information om Workfront-planer finns i [Våra planer](https://business.adobe.com/products/workfront/pricing.html).

Mer information om var du kan hitta arbetsbelastningsutjämnaren i Workfront finns i [Leta reda på arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Åtkomst krävs för att visa arbetsbelastningsutjämnaren

Du måste ha följande åtkomst för att kunna visa arbetsbelastningsutjämnaren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planerar att visa arbetsbelastningsutjämnaren i resursområdet:</br>
       Arbeta, för att visa belastningsutjämnaren för ett team eller projekt</p></td>
  </tr>  
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa eller högre åtkomst till resurshantering</p> <p>Mer information om åtkomstnivån för resurshantering finns i artikeln <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">Bevilja åtkomst till resurshantering</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Du måste ha behörigheten Visa för det projekt vars uppdrag du vill visa. </p> <p>Mer information om projektbehörigheter finns i artikeln <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Dela ett projekt i Adobe Workfront</a>.</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<span class="preview">Alla användare har tillgång till arbetsbelastningsutjämnaren för sina egna profiler. Detta begränsas inte av licens- eller åtkomstnivå. Observera att belastningsutjämnaren för arbetsbelastning i en användarprofil är skrivskyddad och att tilldelningar och allokeringar inte kan ändras.</span>

## Åtkomst krävs för att hantera tilldelningar i arbetsbelastningsutjämnaren

Du måste ha följande åtkomst för att kunna hantera belastningsutjämnaren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planera, för att hantera tilldelningar i arbetsbelastningsutjämnaren i resursområdet:</br>
       Arbeta, för att hantera tilldelningar i belastningsutjämnaren för ett team eller projekt</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till resurshantering</p> 
     <p>Mer information om åtkomstnivån för resurshantering finns i artikeln <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">Bevilja åtkomst till resurshantering</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p> Contribute eller högre behörigheter för det projekt vars uppdrag du vill hantera, inklusive behörigheter för att utföra uppdrag. </p> <p>Mer information om projektbehörigheter finns i artikeln <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Dela ett projekt i Adobe Workfront</a>.</p></td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--these notes were inside the table: for the Edit access to Res Management
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">View or higher access to Financial Data, if you want to view information by cost (NOTE: this is not possible yet!)</p>    
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Financial Data access level, see the article<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. (NOTE: this is not possible yet!)</p>
    -->

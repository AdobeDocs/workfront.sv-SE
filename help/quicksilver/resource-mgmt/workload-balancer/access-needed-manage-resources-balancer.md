---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Åtkomst krävs för att hantera resurser i arbetsbelastningsutjämnaren
description: Om du inte har rätt behörighet eller behörighet kanske du inte kan visa eller hantera dina arbetstilldelningar i Arbetsbelastningsbalanseraren.
author: Alina
feature: Resource Management
exl-id: b3da9a62-481e-4503-8f27-136d6513262e
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 0%

---

# Åtkomst krävs för att hantera resurser i arbetsbelastningsutjämnaren

Om du inte har rätt behörighet eller behörighet kanske du inte kan visa eller hantera dina arbetstilldelningar i Arbetsbelastningsbalanseraren.

Du måste ha tillgång till de användare vars arbetsbelastning du vill visa eller hantera i Utjämning av arbetsbelastning. Utöver detta måste du ha rätt åtkomstnivå och rätt behörigheter för de projekt som arbetet är kopplat till.

## Adobe Workfront-planen behövs för att använda belastningsutjämnaren för olika områden

Följande tabell visar kopplingen mellan den Workfront-plan ditt företag har och var i systemet du kan använda belastningsutjämnaren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Workfront Plan</p></td> 
   <td> <p>Områden där du kan komma åt arbetsbelastningsutjämnaren</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Team eller högre </td> 
   <td>Utjämning av arbetsbelastning för ett team eller ett projekt</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pro eller högre</td> 
   <td>Utjämning av arbetsbelastning för flera projekt på systemnivå</td> 
  </tr> 
 </tbody> 
</table>

Mer information om Workfront planer finns i [Våra planer](https://www.workfront.com/plans).

Information om var du kan hitta belastningsutjämnaren i Workfront finns i [Leta reda på arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Åtkomst krävs för att visa arbetsbelastningsutjämnaren

Du måste ha följande åtkomst för att kunna visa arbetsbelastningsutjämnaren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Planera att visa arbetsbelastningsutjämnaren i resursområdet</p>
   <p>Arbeta för att visa belastningsutjämnaren för ett team eller projekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa eller högre åtkomst till resurshantering</p> <p>Mer information om åtkomstnivån Resurshantering finns i artikeln <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">Bevilja åtkomst till resurshantering</a>.</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Du har behörigheten Visa för det projekt vars uppdrag du vill visa. </p> <p>Mer information om projektbehörigheter finns i artikeln <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Dela ett projekt i Adobe Workfront</a>.</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Åtkomst krävs för att hantera tilldelningar i arbetsbelastningsutjämnaren

Du måste ha följande åtkomst för att kunna hantera belastningsutjämnaren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Planera att hantera tilldelningar i Utjämning av arbetsbelastning i resursområdet</p>
   <p>Arbeta för att hantera tilldelningar i belastningsutjämnaren för ett team eller projekt</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till resurshantering</p> 
     <p>Mer information om åtkomstnivån Resurshantering finns i artikeln <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">Bevilja åtkomst till resurshantering</a>.</p>
     <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p> Contribute eller högre behörigheter för det projekt vars uppdrag du vill hantera, inklusive behörigheter för att utföra uppdrag. </p> <p>Mer information om projektbehörigheter finns i artikeln <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Dela ett projekt i Adobe Workfront</a>.</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

<!--these notes were inside the table: for the Edit access to Res Management
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">View or higher access to Financial Data, if you want to view information by cost (NOTE: this is not possible yet!)</p>    
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Financial Data access level, see the article<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. (NOTE: this is not possible yet!)</p>
    -->
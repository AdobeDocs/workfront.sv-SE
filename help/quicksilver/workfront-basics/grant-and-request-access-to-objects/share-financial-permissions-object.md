---
title: Dela ekonomiska behörigheter för ett objekt
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Din Adobe Workfront-administratör kan ge dig åtkomst att visa eller redigera ekonomiska data när du tilldelar åtkomstnivån. Mer information finns i Bevilja åtkomst till finansiella data.
author: Courtney
feature: Get Started with Workfront
exl-id: 0d0e13d9-b234-48d3-a818-5b6fb36a4688
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

# Dela ekonomiska behörigheter för ett objekt

Din Adobe Workfront-administratör kan ge dig åtkomst att visa eller redigera ekonomiska data när du tilldelar åtkomstnivån. Mer information finns i [Bevilja åtkomst till ekonomiska data](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

Förutom den åtkomstnivå som användare har beviljats kan du även ge dem behörighet att visa eller hantera ekonomi för specifika projekt, uppgifter eller problem som du har tillgång till för delning.

Mer information om vad användare på varje åtkomstnivå kan göra med ekonomiska data finns i avsnittet [Finansiella data](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) i artikeln [Tillgängliga funktioner för varje objekttyp](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Åtkomstkrav

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects, Tasks, Issues, and Financial  Data</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to projects, tasks, and issues that include at least View Finance permissions</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Standard</p> 
   <p>Plan</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa eller öka åtkomst till projekt, uppgifter, ärenden och ekonomiska data</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter eller högre för projekt, uppgifter och utgåvor som innehåller minst Visa ekonomibehörigheter</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Dela ett objekt och bevilja ekonomiska behörigheter

Tänk på följande när du tilldelar ekonomiska behörigheter till objekt:

* Du kan bevilja ekonomiska behörigheter för projekt, uppgifter och ärenden.
* Behörigheter kan ärvas: om du har behörigheten Visa finansiering för ett projekt ärver du automatiskt behörigheten Visa ekonomi för aktiviteterna och problemen i projektet.

Så här tilldelar du ekonomiska behörigheter till ett objekt:

1. Gå till en uppgift, ett projekt eller ett problem som du vill dela med andra.
1. I närheten av objektets namn klickar du på Mer-menyn ![](assets/more-icon.png) och sedan på **Delning**.

1. I fältet **Ge `<Object name>` åtkomst till** börjar du skriva namnet på en användare, ett team, en roll, en grupp eller ett företag som du vill dela objektet med.

   >[!TIP]
   >
   >Du kan bara dela ett objekt med aktiva användare, team, roller eller företag.

1. Om en nedrullningsbar meny visas till höger om det namn du valde, klickar du på något av följande alternativ som är tillgängliga:

   * **Visa det**
   * **Bidra till det**
   * **Hantera det**

1. Klicka på **Avancerade inställningar** i samma nedrullningsbara meny och gör sedan något av följande:

   * Om du valde något av de tre alternativen i föregående steg kontrollerar du att **Visa finansiering** är markerat.
   * Om du valde **Hantera ekonomi** i föregående steg kontrollerar du att **Hantera ekonomi** är markerat.

1. Klicka på **Spara**.

## Ekonomisk behörighet för alla delningsnivåer

Följande tabell visar vilka ekonomiska behörigheter användare får när du ger dem behörigheterna Visa, Contribute eller Hantera för objekt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Åtgärder</strong> </th> 
   <th><strong>Hantera</strong> </th> 
   <th><strong>Contribute</strong> </th> 
   <th><strong>Visa</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Hantera faktureringsposter</td> 
   <td>✓</td> 
   <td> <p>  </p> </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Hantera/visa rollfakturering och kostnadstariffer</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Hantera/visa användarfakturering och kostnadstariffer</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Visa ekonomi</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr> 
  <tr> 
   <td>Visa information efter kostnad i Resursplaneringsverktygen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Budgetresurser i verktygen för resursplanering*</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Visa resurser i verktygen för resursplanering*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kräver ytterligare åtkomst till resurshanteringen.

Mer information om åtkomst till resurshantering finns i [Bevilja åtkomst till resurshantering](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

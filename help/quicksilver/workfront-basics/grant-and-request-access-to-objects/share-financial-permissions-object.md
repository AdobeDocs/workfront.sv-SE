---
title: Dela ekonomiska behörigheter för ett objekt
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Din Adobe Workfront-administratör kan ge dig åtkomst att visa eller redigera ekonomiska data när du tilldelar åtkomstnivån. Mer information finns i Bevilja åtkomst till finansiella data.
author: Courtney
feature: Get Started with Workfront
exl-id: 0d0e13d9-b234-48d3-a818-5b6fb36a4688
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: e974adc053a076a4370aa0c4ec41fea700d836be
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# Dela ekonomiska behörigheter för ett objekt

Din Adobe Workfront-administratör kan ge dig åtkomst att visa eller redigera ekonomiska data när du tilldelar åtkomstnivån. Mer information finns i [Bevilja åtkomst till ekonomiska data](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

Förutom den åtkomstnivå som användare har beviljats kan du även ge dem behörighet att visa eller hantera ekonomi för specifika projekt, uppgifter eller problem som du har tillgång till för delning.

Mer information om vad användare på varje åtkomstnivå kan göra med ekonomiska data finns i avsnittet [Finansiella data](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) i artikeln [Tillgängliga funktioner för varje objekttyp](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Åtkomstkrav

<!--
drafted for P&P:

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
   <td> Visa behörigheter eller högre för projekt, uppgifter och utgåvor som innehåller minst Visa faktureringstariffer, Visa kostnadstariffer och Visa allmänna behörigheter för ekonomi</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Dela ett objekt och bevilja ekonomiska behörigheter

Tänk på följande när du tilldelar ekonomiska behörigheter till objekt:

* Du kan bevilja ekonomiska behörigheter för projekt, uppgifter och ärenden.
* Behörigheter kan ärvas: om du har behörigheten Visa allmänna ekonomier för ett projekt ärver du automatiskt behörigheten Visa allmänna ekonomier för aktiviteterna och problemen i projektet.
* Genom att bevilja behörigheter för fakturering och kostnadstariffer kan användaren visa eller redigera taxorna för det objektet. Tillstånd till allmän finansiering gör det möjligt för användaren att visa eller redigera allmänna ekonomiska områden (som inte är relaterade till fakturering eller kostnadstariffer) för objektet.

Så här tilldelar du ekonomiska behörigheter till ett objekt:

1. Gå till en uppgift, ett projekt eller ett problem som du vill dela med andra.
1. Klicka på **Dela** nära objektets namn.

1. I fältet **Ge `<Object name>` åtkomst till** börjar du skriva namnet på en användare, ett team, en roll, en grupp eller ett företag som du vill dela objektet med.

   >[!TIP]
   >
   >Du kan bara dela ett objekt med aktiva användare, team, roller eller företag.

1. Klicka på listrutan till höger om användarens namn och välj något av följande alternativ:

   * **Visa**
   * **Contribute**
   * **Hantera**

1. I samma nedrullningsbara meny klickar du på ikonen för avancerade alternativ bredvid behörighetsnivån och gör sedan något av följande:

   * Välj **Visa faktureringstariffer**, **Visa kostnadstariffer** och **Visa allmänna ekonomi** efter behov, för alla behörighetsnivåer.
   * Välj **Redigera faktureringstariffer**, **Redigera kostnadstariffer** och **Redigera allmänna ekonomier** efter behov, endast för **Hantera**-behörigheter.

1. Klicka på **Spara**.

## Ekonomisk behörighet för alla delningsnivåer

Tabellen nedan visar vilka ekonomiska behörigheter användare får när du ger dem behörigheterna Visa, Contribute eller Hantera för objekt:

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
   <td>Redigera faktureringstariffer</td> 
   <td>✓</td> 
   <td></td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Redigera kostnadstariffer</td> 
   <td>✓</td> 
   <td></td> 
   <td>  </td> 
  </tr>  
  <tr> 
   <td>Redigera allmän finansiering</td> 
   <td>✓</td> 
   <td></td> 
   <td>  </td> 
  </tr>
  <tr> 
   <td>Visa faktureringstariffer</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr> 
  <tr> 
   <td>Visa kostnadstariffer</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr>  
  <tr> 
   <td>Visa allmän finansiering</td> 
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

<!--
These rows removed from last table.

  <tr> 
   <td>Manage/ View Role Billing and Cost Rates</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Manage/ View User Billing and Cost Rates</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 

-->

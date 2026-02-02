---
product-area: projects
navigation-topic: task-duration
title: Uppdatera de planerade timmarna och varaktigheten för en aktivitet med enkel varaktighetstyp
description: Som standard beräknar Adobe Workfront varaktigheten för en aktivitet med en enkel varaktighetstyp baserat på antalet planerade timmar. Du kan också manuellt redigera mängden Planerade timmar och Längd för en enkel varaktighet-uppgift i vissa delar av Workfront.
author: Alina
feature: Work Management
exl-id: 47a9b095-2b7d-4ed0-8cb6-e6bd5e37ce9c
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# Uppdatera planerade timmar och varaktighet för en aktivitet med enkel varaktighetstyp

Som standard beräknar Adobe Workfront varaktigheten för en aktivitet med en enkel varaktighetstyp baserat på antalet planerade timmar. Du kan också manuellt redigera mängden Planerade timmar och Längd för en enkel varaktighet-uppgift i vissa delar av Workfront.

Du kan antingen redigera Planerade timmar och Varaktighet för en uppgift med en enkel varaktighetstyp infogad eller på aktivitetsnivå i uppdragsområdet.

Mer information om redigering av information finns i [Redigera objekt i en lista i Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

I den här artikeln beskrivs hur du kan uppdatera Planerade timmar och Varaktighet för en uppgift med en enkel varaktighetstyp på aktivitetsnivån i uppdragsområdet.

## Åtkomstkrav

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
   <td><p>Standard eller högre</p> 
   <p>Arbeta eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa eller ge högre åtkomst till projekt</p> <p>Redigera åtkomst till uppgifter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera åtkomst till uppgiften </p></td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

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
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Uppdatera planerade timmar och varaktighet för en aktivitet med enkel varaktighetstyp

>[!IMPORTANT]
>
>När du har uppdaterat varaktigheten manuellt för en enkel varaktighetsåtgärd, slutar Workfront att beräkna den baserat på de planerade timmarna.

Så här redigerar du de planerade timmarna och varaktigheten för en aktivitet med en enkel varaktighetstyp i rutan Avancerade tilldelningar:

1. I en uppgiftslista klickar du på namnet på den uppgift som du vill ändra varaktighetstypen för.
1. Gör något av följande:

   * Klicka på ikonen **Mer** ![Mer på ett objekt](assets/qs-more-icon-on-an-object.png) bredvid namnet på aktiviteten, klicka på **Redigera** och sedan på **Uppdrag**.
   * Klicka på **Tilldelad till** eller namnet på tilldelningarna i uppdragsområdet i uppgiftshuvudet och klicka sedan på **Avancerat**.

1. Ange ett totalt värde för **Planerade timmar** för alla tilldelningar, till exempel 10 timmar. Det totala antalet planerade timmar fördelas jämnt mellan alla resurser som tilldelats aktiviteten.
1. (Valfritt) Justera manuellt de planerade timmarna för varje resurs som tilldelats till aktiviteten. Det totala antalet planerade timmar för aktivitetsuppdateringarna för att återspegla de nya timmarna som är individuellt tilldelade till dina resurser.
1. Ange ett värde för aktiviteten **Varaktighet**, till exempel 2 dagar.

   ![Avancerade tilldelningar, enkel varaktighet för flera resurser](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. Klicka på **Spara**.

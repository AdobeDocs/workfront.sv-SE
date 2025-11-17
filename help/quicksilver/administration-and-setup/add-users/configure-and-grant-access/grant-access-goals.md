---
title: Bevilja åtkomst till Adobe Workfront mål
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: Som Adobe Workfront-administratör kan du använda en åtkomstnivå för att definiera en användares åtkomst till Workfront-mål.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 8639da14-d545-4f9a-894b-12c29699b0db
source-git-commit: 6948f9462c59bad9e6db67d6169e5f9dec4157fe
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# Ge åtkomst till Adobe Workfront mål

Som Adobe Workfront-administratör kan du använda en åtkomstnivå för att definiera en användares åtkomst till Adobe Workfront-mål, vilket förklaras i [Översikt över åtkomstnivåer](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande för att ge användare åtkomst till Workfront-mål:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront package</td> 
   <td> <p>Workfront Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivåkonfiguration</td> 
   <td> <p>Du måste ha åtkomstnivån Systemadministratör.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Workfront Goals <p>Contact your Workfront account manager to learn about a Workfront Goals license. </p> <p>Workfront Goals is available only in the new Adobe Workfront experience.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configuration*</td> 
   <td> <p>You must have the System Administrator access level.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Ge användare åtkomst till Workfront-mål med en anpassad åtkomstnivå

1. Börja skapa eller redigera åtkomstnivån enligt beskrivningen i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klicka på alternativet till höger om **Mål** som du vill använda för den här åtkomstnivån.


   >[!NOTE]
   >
   >Den externa licenstypen tillåter inte Visa eller Redigera åtkomst till Workfront-mål.

1. (Valfritt) Om du vill konfigurera åtkomstinställningar för andra objekt och områden på den åtkomstnivå du arbetar med ska du fortsätta med en av artiklarna i [Konfigurera åtkomst till Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), till exempel [Bevilja åtkomst till aktiviteter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) och [Bevilja åtkomst till ekonomiska data](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. När du är klar klickar du på **Spara**.

## Tillgång till Workfront-mål per licenstyp

En Workfront-administratör kan använda en åtkomstnivå för att bevilja åtkomst till Workfront-mål för användare med följande licenser:

* Standard, Light, Contributor
* Planera, Arbeta, Begär eller Granska licens.

Mer information om åtkomst till Workfront-mål finns i [Krav för att använda Workfront-mål](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

---
product-area: projects
navigation-topic: convert-issues
title: Bryt länken till problem från deras lösta objekt
description: När du skapar ett projekt eller en uppgift genom att konvertera en utgåva till projektet eller uppgiften kan du välja att behålla den ursprungliga utgåvan. Din Adobe Workfront-administratör måste aktivera den här inställningen för att du ska kunna använda det här alternativet när du konverterar utgåvan. Mer information om hur du konverterar problem till projekt och uppgifter finns i Översikt över hur du konverterar problem i Adobe Workfront.
author: Alina
feature: Work Management
exl-id: c18160e5-9f95-4575-a1b3-b4f7e5334844
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# Bryt länken till problem från deras lösta objekt

<!--Audited: 08/2025-->

När du skapar ett projekt eller en uppgift genom att konvertera en utgåva till projektet eller uppgiften kan du välja att behålla den ursprungliga utgåvan. Din Adobe Workfront-administratör måste aktivera den här inställningen för att du ska kunna använda det här alternativet när du konverterar utgåvan.\
Mer information om hur du konverterar problem till projekt och uppgifter finns i [Översikt över hur du konverterar problem i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

När du bestämmer dig för att behålla det problem som konverterades till projektet eller uppgiften är problemlösningen knuten till projektet eller uppgiften. Problemet blir ett objekt som kan lösas i projektet eller uppgiften. Projektet eller aktiviteten är problemlösarens objekt.

Du kan också manuellt länka ett problem till ett annat problem. Den andra utgåvan blir det upplösta objektet för den första utgåvan, i det här fallet.\
Mer information om hur du löser objekt finns i [Översikt över objekt som kan lösas och lösas](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

>[!TIP]
>
>Det går inte att ändra utgivningsstatusen eftersom den ändras automatiskt med statusen för det upplösta objektet.

Du kan bryta länken mellan en problemlösning och en fråga i ett projekt, en uppgift eller ett ärende genom att ta bort projektet, uppgiften eller problemet.

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
   <td> <p>Medarbetare eller högre</p>
   <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivåkonfiguration</td> 
   <td> <p>Redigera åtkomst till problem</p> <p>Visa åtkomst till aktiviteter och projekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för problemet</p> <p>Visa behörigheter för aktiviteten eller projektet</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Issues</p> <p>View access to Tasks and&nbsp;Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the issue</p> <p>View permissions on the task or project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Bryta länken för ett problem från ett projekt, en uppgift eller ett ärende

1. Gå till problemet som är länkat till ett projekt, en uppgift eller ett problem.
1. Klicka på avsnittet **Ärendeinformation**.
1. Gå till området **Översikt** i avsnittet **Ärendeinformation**.
1. Ta bort den matchningsbara objekttypen i fältet **Löst av**.\
   Ett problem kan lösas av ett projekt, en uppgift eller ett problem.

   Detta tar bort det matchande objektet från problemet.

1. Klicka på **Spara** **Ändringar**.\
   Problemet är inte längre kopplat till ett projekt, en uppgift eller ett problem, och du kan nu lösa problemet separat.

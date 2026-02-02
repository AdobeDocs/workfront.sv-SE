---
product-area: projects
navigation-topic: task-information
title: Uppdatera aktivitetsnivåfördröjning
description: Ibland kan det finnas konflikter mellan aktivitetsscheman i ett projekt. Du kan fördela resurser eller hantera resurskonflikter genom att schemalägga om resurser och aktiviteter så att alla aktiviteter kan slutföras inom ett realistiskt schema. Mer information om att jämna ut uppgifter finns i Nivåresurser i Gantt-schemat.
author: Alina
feature: Work Management
exl-id: 6695448c-76ce-460c-aa59-63a3d5e2e18d
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Uppdatera nivåfördröjning för aktivitet

Ibland kan det finnas konflikter mellan aktivitetsscheman i ett projekt. Du kan fördela resurser eller hantera resurskonflikter genom att schemalägga om resurser och aktiviteter så att alla aktiviteter kan slutföras inom ett realistiskt schema. Mer information om att jämna ut aktiviteter finns i [Nivåresurser i Gantt-schemat](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

Som projektledare eller tilldelad uppgift kan du även lägga till en nivåfördröjning för enskilda uppgifter för att ta hänsyn till eventuella konflikter mellan resurser och schemaläggning. Med andra ord kan en aktivitet schemaläggas med en fördröjning för att säkerställa att en mer realistisk schemaläggning åsidosätter resurskonflikter när Adobe Workfront nivåer används.

Om du lägger till en nivåfördröjning för en aktivitet justeras aktivitetens beräknade slutförandedatum. Information om det planerade slutförandedatumet finns i [Översikt över det planerade slutförandedatumet för projekt, aktiviteter och problem](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

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
   <td> <p>Standard</p>
   <p>Arbeta eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till uppgifter och projekt</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för aktiviteter </p> <p>Contribute eller högre behörighet till projekt</p> </td> 
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
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to Tasks </p> <p>Contribute or higher permissions to Projects</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Lägga till en nivåfördröjning till en uppgift

1. Gå till en uppgift som du vill lägga till en nivåfördröjning för.
1. Klicka på ikonen **Mer** till höger om aktivitetsnamnet och klicka sedan på **Redigera**.

1. Klicka på **Inställningar**.

   ![Utjämningsfördröjning vid redigering av uppgift](assets/leveling-delay-edit-task-nwe-350x345.png)

1. Ange **Leveling Delay** i timmar och välj sedan en tidsenhet.\
   Det här är den tidpunkt då resursen kommer att fördröjas när aktiviteten startas på grund av resurskonflikter.

   Välj bland följande alternativ för tidsenheter:

   * Minuter
   * Timmar. Det här är standardinställningen.
   * Dagar
   * Veckor
   * Månader
   * Förflutna minuter
   * Förflutna timmar
   * Förflutna dagar
   * Förflutna veckor
   * Förflutna månader

   >[!TIP]
   >
   >Förfluten tid är en tidsenhet för en uppgifts varaktighet. Det är tiden mellan det planerade startdatumet och det planerade slutförandedatumet för en aktivitet som omfattar helger, helger och ledig tid. Med andra ord är förfluten tid en del av kalenderdagarna.

1. Klicka på **Spara**.



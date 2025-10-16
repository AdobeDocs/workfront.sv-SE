---
product-area: projects
navigation-topic: update-work-in-a-project
title: Använd status för arbete som är associerat med en grupp
description: Om ett projekt är associerat med en grupp kan du använda både systemnivåstatusvärden och en anpassad status som är associerad med den gruppen för projektet, uppgiften eller problemen i det projektet.
author: Alina
feature: Work Management
exl-id: 7564ab6a-8ddf-4e76-8e45-d59f9cf8d38b
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---

# Tillämpa statusvärden på arbete som är associerat med en grupp

<!--
Alina, I moved this out of an admin article about statuses (Create and customize statuses)
-->

Om ett projekt är associerat med en grupp kan du använda både systemnivåstatus och en anpassad status som är associerad med den gruppen för projektet, eller aktiviteter och ärenden i det projektet. Mer information om gruppstatus i Adobe Workfront finns i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

>[!TIP]
>
>Du kan bara associera projekt med grupper. Problem och uppgifter ärver gruppen från det projekt de tillhör.

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
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för projektet</p> </td> 
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
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Uppdatera projektgrupp och status

När du uppdaterar gruppen för ett projekt ändras alternativen som är tillgängliga för status för uppgifter, utgåvor eller projektet så att de matchar gruppen.

1. Gå till ett projekt eller skapa ett nytt projekt, enligt beskrivningen i [Skapa ett projekt](../../../manage-work/projects/create-projects/create-project.md).
1. Klicka på ikonen **Mer** ![Mer](assets/more-icon.png) och klicka sedan på **Redigera**.

1. Markera gruppen i listrutan **Grupp** i rutan **Redigera projekt** , som visas längst ned i avsnittet **Översikt** .

1. Välj anpassad status i listrutan **Status**.

   >[!NOTE]
   >
   >Om du väljer en annan grupp i den nedrullningsbara menyn **Grupp** ändras de anpassade statusarna på menyn **Status** automatiskt så att de korrelerar med den nya gruppen.
   >
   >
   >![Listrutan Status utökad med anpassade statusvärden för projektet](assets/status-drop-down-expanded-with-custom-statuses-for-project-nwe.png)
   >

1. Välj status för projektet. De anpassade statusvärden som du skapade och tillämpade på den gruppen visas i listan.

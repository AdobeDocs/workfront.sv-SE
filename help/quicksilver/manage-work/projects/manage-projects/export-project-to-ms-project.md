---
product-area: projects
navigation-topic: manage-projects
title: Exportera ett projekt till Microsoft Project
description: Du kan exportera Adobe Workfront-projekt till Microsoft Project.
author: Alina
feature: Work Management
exl-id: 3f0f3644-a763-4b72-a93a-85af8626b5b3
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---

# Exportera ett projekt till Microsoft Project

Du kan exportera Adobe Workfront-projekt till Microsoft Project. 

>[!IMPORTANT]
>
>* Alla Workfront-fält överförs inte i Microsoft Project-filen.\
>  Mer information om kompatibilitet för fält mellan Workfront och Microsoft Project finns i artikeln [Mappa Microsoft-projektfält till Adobe Workfront-projekt](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).
>* Vi rekommenderar att du begränsar antalet gånger du överför projekt från ett program till ett annat. 
>

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
   <td> <p>Ljus eller högre</p>
   <p>Granska eller högre</p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa eller ge högre åtkomst till projekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p> Visa eller högre behörigheter för projektet</p></td> 
  </tr> 
 </tbody> 
</table>

*Mer information om informationen i den här tabellen finns i [Åtkomstkraven i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> View or higher permissions to the project</p> <p>For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Exportera ett projekt från Workfront till Microsoft Project

Du kan exportera ett projekt från Workfront från projektsidan eller från en projektlista eller rapport.

1. Gå till projektet som du vill exportera och klicka på ikonen **Mer** ![Mer meny](assets/qs-more-menu.png) till höger om projektnamnet

   ![Fler listrutor](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   eller

   Gå till en projektlista eller rapport och välj ett projekt och klicka sedan på ikonen Mer ![Mer](assets/qs-more-menu.png) överst i listan.

   ![Mer meny utökad](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. Klicka på **Exportera MS-projekt**.

   Projektet laddas ned som en XML-fil till datorn och kan importeras till Microsoft Project. 

---
product-area: projects
navigation-topic: create-projects
title: Importera ett projekt från Microsoft Project
description: Du kan importera projekt från Microsoft Project till Adobe Workfront och hantera alla projekt i ett och samma program. Varje gång du importerar ett projekt från Microsoft Project skapas ett nytt projekt i Workfront.
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# Importera ett projekt från Microsoft Project

Du kan importera projekt från Microsoft Project till Adobe Workfront och hantera alla projekt i ett och samma program. Varje gång du importerar ett projekt från Microsoft Project skapas ett nytt projekt i Workfront.

>[!IMPORTANT]
>
>Alla Microsoft Project-fält överförs inte till Workfront.
>
>Mer information om kompatibilitet för fält mellan Workfront och Microsoft Project finns i [Mappa Microsoft Project-fält till Adobe Workfront-projekt](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Ny licens: Standard </p> 
   eller
   <p>Aktuell licens: Planera </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>När du skapar ett projekt får du automatiskt behörigheten Hantera i projektet </p> </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--old permissions model: 

You must have the following access to perform the steps in this article:

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
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

## Skapa ett projekt från ett MS-projekt

Du kan skapa ett projekt från området Projekt på huvudmenyn eller från området Projekt i en portfölj eller ett program.

1. Gå till Microsoft Project och öppna ett projekt som du vill importera från i Workfront.
1. Klicka på **Arkiv** och sedan på **Spara som** för att spara projektet som en XML-fil.

1. Logga in på Workfront.
1. Gör något av följande:

   * Klicka på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet av Workfront, eller klicka på **Huvudmeny** ![Huvudmenyrader](assets/lines-main-menu.png) i det övre vänstra hörnet, om det är tillgängligt, klicka på **Projekt** och expandera sedan **Nytt projekt**.
   * Gå till en portfölj och expandera sedan **Nytt projekt**.
   * Gå till ett program och expandera sedan **Nytt projekt**.
   * Om du är gruppadministratör kan du även skapa ett projekt i avsnittet Projekt i en grupp som du hanterar. Mer information finns i [Skapa och ändra en grupps projekt](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. Välj alternativet **Importera MS-projekt**.

   ![Listrutan Nytt projekt](assets/new-project-dropdown-nwe-350x358.png)

1. Klicka på **Välj fil** och bläddra sedan efter XML-filen på datorn som du exporterade från Microsoft Project.
1. Importera den markerade filen.

   Workfront påbörjar importprocessen och skapar ett nytt projekt baserat på den fil som exporteras från Microsoft Project.

   När importen är klar dirigeras du till den nya projektsidan som visar en bekräftelse på att importen har slutförts.

   >[!NOTE]
   >
   >Workfront har 15 minuters tidsbegränsning för filöverföringar. Om filöverföringen tar längre tid än så rekommenderar vi att du delar upp ditt projekt i mindre projekt och importerar dem separat. När du har importerat dem till Workfront flyttar du arbetsmomenten från ett projekt till ett annat. Mer information om hur du flyttar uppgifter finns i [Flytta uppgifter](../../../manage-work/tasks/manage-tasks/move-tasks.md).

1. (Valfritt) Fortsätt redigera projektet i Workfront. Mer information om hur du redigerar projekt finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

   Statusen för ett nytt projekt som skapats från en mall motsvarar den status som definieras av Workfront-administratören i området Projektinställningar eller av en gruppadministratör i området Gruppprojektinställningar. Mer information om hur du konfigurerar projektinställningar finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

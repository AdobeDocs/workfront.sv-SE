---
product-area: projects
navigation-topic: use-predecessors
title: Skapa föregående relationer efter kedjningsaktiviteter
description: Du kan skapa underordnade relationer på flera sätt i Adobe Workfront. En metod är att kedja uppgifter.
author: Alina
feature: Work Management
exl-id: 38ea13a5-ab95-4617-a47f-9dde5f752fb4
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---

# Skapa tidigare relationer genom att kedja uppgifter

Du kan skapa underordnade relationer på flera sätt i Adobe Workfront. En metod är att kedja uppgifter.

Mer information om föregående aktiviteter finns i [Översikt över föregående aktiviteter](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Genom att kedja uppgifter kan du låta systemet skapa föregående relationer automatiskt för valda uppgifter, i stället för att manuellt skapa en relation för varje uppgift själv. Olika typer av föregående relationer kan fortfarande användas mellan uppgifter.

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
   <td><p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till uppgifter och projekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för aktiviteterna och projektet</p></td> 
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
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Standard </p>
    <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Kedjuppgifter för att skapa föregående relationer

1. Gå till det projekt som innehåller de uppgifter som du vill kedja.
1. Klicka på **Åtgärder** i den vänstra panelen.
1. (Villkorligt) Välj **Spara automatiskt** i det övre högra hörnet av uppgiftslistan och välj sedan de uppgifter som du vill kedja.

   ![Ikonen Spara automatiskt på markerad](assets/nwe-autosave-icon-on-highlighted-350x295.png)

   >[!IMPORTANT]
   >
   >Det går inte att kedja uppgifter i en uppgiftslista när du manuellt sparar ändringar i uppgifter eller använder tidslinjens planeringsläge för att spara uppgifter.

1. Högerklicka på de markerade aktiviteterna och klicka sedan på **Kedja**.
1. Välj bland följande beroendetyper:

   * **Slutför-Start**
   * **Slutför**
   * **Start-Start**
   * **Start-slut**

   Mer information om beroendetyper för föregångare finns i [Översikt över typer av uppgiftsberoenden](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. (Valfritt) Klicka på **Ta bort kedja** om några av uppgifterna har kedjats tidigare.

   >[!CAUTION]
   >
   >Endast sekventiella föregångare tas bort med alternativet Dela upp när gruppredigeringsuppgifter används.

   Dina valda uppgifter är nu länkade av föregående relationer.

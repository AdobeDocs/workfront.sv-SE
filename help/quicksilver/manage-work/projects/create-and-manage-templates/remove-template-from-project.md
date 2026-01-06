---
product-area: templates
navigation-topic: templates-navigation-topic
title: Ta bort mallinformation från ett projekt
description: Du kan inte ta bort en mall från ett projekt. Du kan bara ta bort information som har lagts till i projektet manuellt efter att en mall har kopplats till projektet. Mer information om hur du bifogar mallar finns i Bifoga en mall till ett projekt.
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Ta bort mallinformation från ett projekt

Du kan inte ta bort en mall från ett projekt. Du kan bara ta bort information som har lagts till i projektet manuellt efter att en mall har kopplats till projektet. Mer information om hur du bifogar mallar finns i [Koppla en mall till ett projekt](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

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
   <td> <p>Redigera åtkomst till uppgifter</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera åtkomst till uppgifter </p> <p>Contribute eller senare åtkomst till projektet</p>  </td> 
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
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard</p>
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to tasks </p> <p>Contribute or higher access to the project </p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Alternativ för att ta bort mallinformation från ett projekt

Om du vill ta bort mallinformation som har lagts till i projektet kan du göra något av följande:

* Ta bort information från projektet manuellt när mallen har bifogats.

  Mer information finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

* Ta bort de uppgifter i projektet som lades till med mallen.

  Mer information finns i avsnittet [Ta bort uppgifter som har skapats från en mall](#delete-tasks-created-from-a-template) i den här artikeln.

* Ta bort mallen från Workfront. När du tar bort mallen från Workfront tas inte uppgifter som lagts till från mallen bort från projekt.

  Mer information finns i [Ta bort projektmallar](../../../manage-work/projects/create-and-manage-templates/delete-templates.md).

## Ta bort uppgifter som skapats från en mall {#delete-tasks-created-from-a-template}

1. Gå till avsnittet **Åtgärder** i projektet.
1. Gör något av följande:

   * Skapa ett filter för uppgiftslistan så att endast uppgifter som har skapats från en mall visas med följande programsats:

     ```
     Task >> Template Task ID >>Is Not Blank
     ```

     Mer information om hur du skapar ett filter finns i [Skapa eller redigera filter i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

     När du använder filtret visas endast uppgifter som är kopplade till ett malluppgifts-ID i listan.

   * Skapa en vy för uppgiftslistan om du vill visa fälten **Malluppgift-ID** eller **Malluppgiftsnamn** i en kolumn.

     När du använder vyn skapades de uppgifter som innehåller information i kolumnen Malluppgift-ID eller Malluppgiftsnamn med hjälp av en mall.

     Mer information om hur du skapar en vy finns i [Vyöversikt i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Markera alla uppgifter som identifieras i steg 2 som de har skapats från en mall och klicka sedan på **ikonen Ta bort****> Ja, Ta bort den**. Mer information finns i [Ta bort uppgifter](../../../manage-work/tasks/manage-tasks/delete-tasks.md).

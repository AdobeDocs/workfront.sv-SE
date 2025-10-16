---
product-area: projects
navigation-topic: manage-projects
title: Ändra status för ett projekt
description: Du kan uppdatera status för ett projekt manuellt till en annan status om det behövs. Du kan uppdatera ett projekts status manuellt till en status som motsvarar Fullständigt endast när projektets slutföringsläge är Manuellt.
author: Alina
feature: Work Management
exl-id: 80098514-fd44-436d-836b-bd9c1b52b3a9
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 0%

---

# Ändra status för ett projekt

<!--Audited: 02/2024-->

Du kan uppdatera status för ett projekt manuellt till en annan status om det behövs.

Du kan uppdatera ett projekts status manuellt till en status som motsvarar Fullständigt endast när projektets slutföringsläge är Manuellt.

I annat fall markeras projektet automatiskt som färdigt när alla uppgifter och utgåvor av projektet har slutförts och godkänts.

Mer information om projektets slutföringsläge finns i [Redigera projekt](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

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
   <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i projektet</p> </td> 
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
   <td> <p>New: Standard </p> 
   Or
   <p>Current: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Att tänka på när du uppdaterar till specifika statusar

* **När du uppdaterar ett projekt till Fullständigt:** Kontrollera att alla aktiviteter och ärenden har slutförts i projektet. Du kan inte välja statusen Fullständig för ett projekt eller någon annan status som motsvarar Fullständig när det finns uppgifter eller problem som inte har slutförts i projektet. Detta inkluderar godkännande av alla uppgifter eller problem som har statusen Slutför väntande godkännande.
* **När du uppdaterar ett projekt från Fullständigt till Aktuell:** Om alla aktiviteter och problem i projektet har slutförts kontrollerar du att projektets slutföringsläge är Manuellt. Om projektets slutföringsläge är Automatiskt, förblir projektets status Fullständigt.

## Ändra projektstatus

1. Gå till det projekt vars status du vill uppdatera.
1. Klicka på statusnamnet i fältet **Status** i projektrubriken och välj sedan en ny status.

   ![Ändra projektstatus](assets/change-project-status-in-header-drop-down-nwe-350x371.png)

   eller

   Klicka på menyn **Mer** ![Mer ](assets/qs-more-menu.png) bredvid namnet på projektet och klicka på **Redigera** och välj en ny status i fältet **Status**. Klicka sedan på **Spara**.

   Projektstatusen uppdateras till den valda statusen.

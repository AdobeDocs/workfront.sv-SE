---
product-area: projects
navigation-topic: manage-projects
title: Ändra status för ett projekt
description: Du kan uppdatera status för ett projekt manuellt till en annan status om det behövs. Du kan uppdatera ett projekts status manuellt till en status som motsvarar Fullständigt endast när projektets slutföringsläge är Manuellt.
author: Alina
feature: Work Management
exl-id: 80098514-fd44-436d-836b-bd9c1b52b3a9
source-git-commit: 7363e86f5c507e40955e16843c6776777c7ad823
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Ändra status för ett projekt

<!--Audited: 02/2024-->

Du kan uppdatera status för ett projekt manuellt till en annan status om det behövs.

Du kan uppdatera ett projekts status manuellt till en status som motsvarar Fullständigt endast när projektets slutföringsläge är Manuellt.

I annat fall markeras projektet automatiskt som färdigt när alla uppgifter och utgåvor av projektet har slutförts och godkänts.

Mer information om projektets slutföringsläge finns i [Redigera projekt](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

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
   <td> <p>Nytt: Standard </p> 
   eller
   <p>Aktuell: Planera </p>
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

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har. Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Att tänka på när du uppdaterar till specifika statusar

* **När du uppdaterar ett projekt till Fullständigt:** Kontrollera att alla aktiviteter och ärenden har slutförts i projektet. Du kan inte välja statusen Fullständig för ett projekt eller någon annan status som motsvarar Fullständig när det finns uppgifter eller problem som inte har slutförts i projektet. Detta inkluderar godkännande av alla uppgifter eller problem som har statusen Slutför väntande godkännande.
* **När du uppdaterar ett projekt från Fullständigt till Aktuell:** Om alla aktiviteter och problem i projektet har slutförts kontrollerar du att projektets slutföringsläge är Manuellt. Om projektets slutföringsläge är Automatiskt, förblir projektets status Fullständigt.

## Ändra projektstatus

1. Gå till det projekt vars status du vill uppdatera.
1. Klicka på statusnamnet i fältet **Status** i projektrubriken och välj sedan en ny status.

   ![](assets/change-project-status-in-header-drop-down-nwe-350x371.png)

   eller

   Klicka på **Mer**-menyn ![](assets/qs-more-menu.png) bredvid namnet på projektet och klicka på **Redigera** och välj en ny status i fältet **Status**. Klicka sedan på **Spara**.

   Projektstatusen uppdateras till den valda statusen.

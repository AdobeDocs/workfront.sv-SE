---
product-area: projects
navigation-topic: manage-projects
title: Ändra status för ett projekt
description: Du kan ändra status för ett projekt manuellt.
author: Alina
feature: Work Management
exl-id: 80098514-fd44-436d-836b-bd9c1b52b3a9
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 0%

---

# Ändra status för ett projekt

Du kan ändra status för ett projekt manuellt.

## Åtkomstkrav

<!--drafted for P&P:

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b> If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till projekt</p> <p><b>ANMÄRKNING</b> Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Att tänka på när du uppdaterar till specifika statusar

* **När du uppdaterar ett projekt till Fullständigt:** Se till att alla uppgifter och ärenden har slutförts i projektet. Du kan inte välja statusen Fullständig för ett projekt eller någon annan status som motsvarar Fullständig när det finns uppgifter eller problem som inte har slutförts i projektet. Detta inkluderar godkännande av alla uppgifter eller problem som har statusen Slutför väntande godkännande.
* **När du uppdaterar ett projekt från Fullständigt till Aktuellt:** Om alla uppgifter och problem i projektet är slutförda kontrollerar du att projektets slutförningsläge är inställt på Manuellt. Om projektets slutföringsläge är Automatiskt, förblir projektets status Fullständigt.

## Ändra projektstatus

1. Gå till det projekt vars status du vill uppdatera.
1. Klicka på statusens namn i projektrubriken i **Status** och välj sedan en ny status.

   ![](assets/change-project-status-in-header-drop-down-nwe-350x371.png)

   eller

   Klicka på **Mer** meny ![](assets/qs-more-menu.png) bredvid namnet på projektet och klicka på **Redigera** och välj en ny status i dialogrutan **Status** fält och klicka sedan på **Spara**.

   Projektstatusen uppdateras till den valda statusen.

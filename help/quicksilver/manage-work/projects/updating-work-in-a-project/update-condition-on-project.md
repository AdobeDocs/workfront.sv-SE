---
product-area: projects
navigation-topic: update-work-in-a-project
title: Uppdatera villkor för ett projekt
description: Villkoret för ett projekt är en flagga som placeras på det för att ange om arbetet som är kopplat till det går smidigt eller om du har stött på några hinder. Detta skiljer sig från projektets status, vilket anger om du arbetar aktivt med det eller inte.
author: Alina
feature: Work Management
exl-id: 1f46386e-e1ae-4845-8cc4-09dd7d39076f
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 0%

---

# Uppdatera villkor för ett projekt

Villkoret för ett projekt är en flagga som placeras på det för att ange om arbetet som är kopplat till det går smidigt eller om du har stött på några hinder. Detta skiljer sig från projektets status, vilket anger om du arbetar aktivt med det eller inte.

Du kan ange ett projekts villkor antingen automatiskt eller manuellt. Om du vill ändra villkoret för ett projekt manuellt måste du vara projektägare eller ha behörighet att hantera det.

Adobe Workfront-administratören kan skapa anpassade villkor för din miljö enligt beskrivningen i [Skapa eller redigera ett anpassat villkor](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Åtkomstkrav

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td><p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   
   For the current licenses:
  <p>Standard</p>
   
   For legacy licenses:
   <ul><li><p>Plan</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Manage permissions on tasks and issues to update the Condition</p>
    <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>Redigera åtkomst till projekt</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Ange villkoret automatiskt

Inställningen av villkor för ett projekt bestäms automatiskt av projektets villkorstyp. Villkorstypen måste anges till Förloppsstatus för Workfront för att automatiskt ställa in Projektets villkor.

Din Workfront- eller gruppadministratör bestämmer standardvärdet för fältet Villkorstyp för nya projekt i systemet när du anger projektinställningar under Konfigurera. Mer information finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

När du skapar ett projekt ställs villkoret automatiskt in så att det matchar projektets förloppsstatus vid den tidpunkten. Projektets förloppsstatus baseras på förloppet för aktiviteterna i projektet.

Mer information om projektvillkor och hur de beräknas baserat på förloppsstatus finns i [Översikt över status för projektförlopp](../../../manage-work/projects/planning-a-project/project-progress-status.md).

## Uppdatera villkoret för ett projekt manuellt

Om du ställer in projektets villkorstyp på Manuell i stället för Status kan du uppdatera ett projekts villkor manuellt.

1. Gå till det projekt som du vill uppdatera villkoret för.
1. Klicka på **Projektinformation** -avsnitt.

   ![](assets/project-details-overview-edit-enabled-with-condition-shot-nwe-350x251.png)

1. Se till att **Villkorstyp** fältet är inställt på **Manuell**.

1. I **Villkor** väljer du bland följande alternativ det som matchar din förståelse för om arbetet som är kopplat till det går smidigt eller om det blir några förseningar:

   * **På mål**
   * **Risk**
   * **I problem**

   Mer information om projektvillkor finns i [Översikt över projektvillkor och villkorstyp](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

   >[!NOTE]
   >
   >Villkoren kan anpassas efter din miljö, så du kan hitta fler än tre alternativ för Villkor i din miljö. Namnen på villkoren kan skilja sig från namnen ovan. Mer information om hur du anpassar villkor i Workfront finns i [Skapa eller redigera ett anpassat villkor](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

1. Klicka **Spara**.Klicka **Spara ändringar**.

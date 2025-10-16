---
product-area: projects;user-management
navigation-topic: manage-projects
title: Ta bort användare från projekt
description: Du kan ta bort användare från ett projekt när de inte längre deltar i arbetet med projektet.
author: Alina
feature: Work Management
exl-id: 3a75c78d-faed-41cd-a0a4-59504bb981af
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Ta bort användare från projekt

Du kan ta bort användare från ett projekt när de inte längre deltar i arbetet med projektet. Att ta bort användare från projekt påverkar uppgifter, ärenden och projektroller. Borttagna användare slutar ta emot meddelanden som är avsedda för projektgruppen. Mer information om meddelanden för projektteamen finns i [Händelsemeddelandetyper](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

De användare som är associerade med ett projekt visas i området Personer i ett projekt. De representerar projektteamet. Mer information om projektteamet finns i [Översikt över projektteamet](../../../manage-work/projects/planning-a-project/project-team-overview.md).

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
   <td> <p>Hantera behörigheter i projektet</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <td> <p>Manage permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Hur borttagning av en användare påverkar befintliga uppgifter, problem och projekt

När en användare tas bort från ett projekt kan uppgifter eller problem som tilldelats dem påverkas, beroende på om uppgiften eller problemet slutfördes när användaren togs bort:

* **Om objektet inte slutförs när användaren tas bort:** Objektet omtilldelas till en jobbroll om en jobbroll redan har tilldelats, eller om det har tilldelats till den jobbroll som användaren tog i objektet. Om artikeln eller användaren inte har tilldelats någon jobbroll måste du tilldela om posten manuellt.
* **Om objektet slutförs när användaren tas bort:** Namnet på den borttagna användaren finns kvar på objektet.
* **Om användaren som tagits bort även är skapare av ett projekt:** Projektet tas inte bort från deras **Projekt jag är på** i projektområdet. Projektet tas bort från listorna för alla andra användare som filtrerar projektet efter fältet Anges av.
* **Om användaren är projektägare eller sponsor:** Användaren behåller sin roll som sponsor eller projektägare.

## Ta bort användare från ett projekt och projektgrupp

Du kan ta bort användare från ett projekt genom att ta bort dem från projektgruppen.

När användare fyller roller i ett projekt blir de en del av projektgruppen.

När du tar bort användare från deras roller i projektet blir de kvar i projektteamet.

Mer information om användarnas roller i ett projekt finns i [Hantera projektteamet](../planning-a-project/manage-project-team.md).

Så här tar du bort användare från projektteamet:

1. Gå till det projekt där du vill ta bort användarna.

1. Klicka på **Personer** i den vänstra panelen och markera sedan de användare som du vill ta bort.

1. Klicka på ikonen **Ta bort** ![Ta bort objekt](assets/remove-icon---x-in-circle.png) högst upp i listan över användare.

1. Klicka på **Ja, ta bort markerade användare** för att bekräfta borttagningen.

   Användarna tas bort från projektteamet och från ofullständiga uppgifter eller problem som de kan tilldelas till. De får inte längre meddelanden som är avsedda för projektteamet.

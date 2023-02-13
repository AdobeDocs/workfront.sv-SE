---
title: Ta bort projekt
product-area: projects
navigation-topic: manage-projects
description: Du kan ta bort ett projekt om projektet och dess data inte längre behövs.
author: Alina
feature: Work Management
exl-id: a0e80c4d-29a8-4bf8-aa19-0c2d493236c6
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# Ta bort projekt

Du kan ta bort ett projekt om projektet och dess data inte längre behövs.

Som ett alternativ till att ta bort ett projekt rekommenderar vi att du redigerar projektet och ändrar statusen till Fullständigt eller Dölj. Detta tar bort alla aktuella uppgifter som är relaterade till projektet från en användares uppgiftslista, men sparar alla data som är kopplade till projektet.

## Åtkomstkrav

<!-- drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Delete</span> projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>Edit access to Projects, Tasks,&nbsp;Issues with ability to Delete projects, tasks, and issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till projekt, uppgifter, problem med möjlighet att ta bort projekt, uppgifter och problem</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för projektet, uppgifter och problem med projektet med möjlighet att ta bort projektet, uppgifterna och problemen. </p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.
Du kan ta bort ett projekt i en projektlista eller på projektnivå.

## Förstå processen med att ta bort projekt

* [Begränsningar för att ta bort projekt](#limitations-for-deleting-projects)
* [Effekten av att ta bort projekt](#the-impact-of-deleting-projects)

### Begränsningar för att ta bort projekt  {#limitations-for-deleting-projects}

* Borttagna objekt flyttas till papperskorgen i 30 dagar och kan endast återställas av Workfront-administratören.

   Mer information om hur du återställer objekt finns i artikeln [Återställ borttagna objekt](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* Om projektet innehåller uppgifter eller problem med loggade timmar måste Workfront- eller gruppadministratören tillåta att dessa uppgifter tas bort genom att konfigurera inställningarna för Aktivitet och Problem i din Workfront-instans så att du kan ta bort det projekt som innehåller uppgifterna.

   Mer information om hur du aktiverar borttagning av uppgifter, problem eller projekt där timmar är loggade finns i avsnittet Borttagning i [Konfigurera inställningar för uppgifter och problem i hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays in NWE only forever)</p>
  -->

### Effekten av att ta bort projekt {#the-impact-of-deleting-projects}

* När du tar bort ett projekt påverkas andra objekt som är länkade till projektet.

   Följande objekt som är kopplade till ett projekt tas också bort när du tar bort ett projekt:

   * Dokument

      Du kan inte ta bort ett projekt som har ett bifogat dokument som har checkats ut. Mer information om utcheckning av dokument finns i [Checka ut dokument](../../../documents/managing-documents/check-out-documents.md).

   * Uppgifter
   * Underaktiviteter
   * Problem
   * Anteckningar
   * Godkännanden
   * Utgifter

* Beroende på hur din Workfront-administratör konfigurerar inställningarna för projekt, uppgift eller borttagning av problem i tidrapport och timinställningar för din Workfront-instans, hanteras timmar som är loggade för uppgifter, problem eller projektet på något av följande sätt när du tar bort projektet:

   * Timmarna finns kvar på tidrapporten som allmän tid.
   * Timmarna tas bort och återställs om projektet återställs.

   Mer information om hur du konfigurerar raderingsinställningarna för timmar som är inloggade finns i [Konfigurera tidrapport och timinställningar](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Om det projekt du tar bort är länkat till ett projekt i Workfront Scenario Planner:

   * Initiativet ligger kvar i planen, men kopplingen till projektet har tagits bort.
   * Om projektet som du tar bort är länkat till det enda publicerade initiativet från en plan, tas även indikationen på att planen har publicerats bort.
   * Om du återställer ett borttaget projekt återställs projektet, men länken till projektet återställs inte och området för scenarioplanering visas inte längre i Projektinformation.

      Scenarioplaneraren finns endast i den nya Adobe Workfront-upplevelsen och kräver ytterligare en licens. Mer information om Workfront Scenario Planner finns i [Översikt över scenarioplanen](../../../scenario-planner/scenario-planner-overview.md).

      Mer information om projekt som är kopplade till initiativ i scenarioplanen finns i [Uppdatera eller skapa projekt genom att publicera initiativ i Scenarioplanen](../../../scenario-planner/publish-scenarios-update-projects.md).

* Om projektet även är en aktivitet för ett mål i Workfront-målen:

   * Projektet tas bort från målet. Det förlopp som anges för målet i projektet tas också bort.

   * Om du återställer det borttagna projektet återställs även projektet som målaktivitet.

      Detta kräver ytterligare en licens. Mer information om Workfront-mål finns på [Översikt över Adobe Workfront-mål](../../../workfront-goals/goal-management/wf-goals-overview.md).

      Mer information om hur du associerar projekt med mål finns i [Lägga till projekt i mål i Adobe Workfront-mål](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

## Ta bort ett projekt i en lista

Du kan ta bort projekt från en lista med projekt.

1. Gå till en lista med projekt eller en projektrapport.
1. Markera projektet som du vill ta bort och klicka sedan på **Ta bort** högst upp i listan.

1. Klicka **Ja, ta bort den** för att bekräfta borttagningen.

   Projektet tas bort och lagras i papperskorgen i 30 dagar. Din Workfront-administratör kan återställa den från papperskorgen under den här tiden.

## Ta bort ett projekt på projektnivå

1. Gå till det projekt som du vill ta bort.
1. Klicka på **Mer** icon ![](assets/qs-more-menu.png).

1. Klicka **Ta bort projekt**.

1. Klicka **Ja, ta bort den**.

   Projektet tas bort och lagras i papperskorgen i 30 dagar. Din Workfront-administratör kan återställa den från papperskorgen under den här tiden.

## Återställer borttagna projekt

En system- eller gruppadministratör kan återställa projekt inom 30 dagar efter att de har tagits bort, vilket beskrivs i artikeln [Återställ borttagna objekt](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

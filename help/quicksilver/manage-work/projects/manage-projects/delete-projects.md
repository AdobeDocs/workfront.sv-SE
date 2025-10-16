---
title: Ta bort projekt
product-area: projects
navigation-topic: manage-projects
description: Du kan ta bort ett projekt om projektet och dess data inte längre behövs. Som ett alternativ till att ta bort ett projekt rekommenderar vi att du redigerar projektet och ändrar statusen till Fullständigt eller Dölj. Detta tar bort alla aktuella uppgifter som är relaterade till projektet från en användares uppgiftslista, men sparar alla data som är kopplade till projektet.
author: Alina
feature: Work Management
exl-id: a0e80c4d-29a8-4bf8-aa19-0c2d493236c6
recommendations: noDisplay, noCatalog
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# Ta bort projekt

<!--Audited: 07/2024-->

Du kan ta bort ett projekt om projektet och dess data inte längre behövs.

Som ett alternativ till att ta bort ett projekt rekommenderar vi att du redigerar projektet och ändrar statusen till Fullständigt eller Dölj. Detta tar bort alla aktuella uppgifter som är relaterade till projektet från en användares uppgiftslista, men sparar alla data som är kopplade till projektet.

Du kan ta bort ett projekt i en projektlista eller på projektnivå.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront package</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-licens</p> </td> 
   <td> <p>Standard</p>
   <p>Plan</p> 
   </td> 
  </tr> 
    <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt med möjlighet att skapa och ta bort projekt</p> </td> 
  </tr> 
    <td> <p>Objektbehörigheter</p> </td> 
   <td> <p>Redigera åtkomst till projekt, uppgifter, problem med möjlighet att ta bort projekt, uppgifter och problem</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>New license: Standard </p>
   <p>Current license: Plan </p> 
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level configuration</td> 
   <td> <p>Edit access to Projects with ability to Create and Delete projects</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>Edit access to Projects, Tasks, Issues with ability to Delete projects, tasks, and issues</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Förstå processen med att ta bort projekt

* [Begränsningar för att ta bort projekt](#limitations-for-deleting-projects)
* [Effekten av att ta bort projekt](#the-impact-of-deleting-projects)

### Begränsningar för att ta bort projekt  {#limitations-for-deleting-projects}

* Borttagna objekt flyttas till papperskorgen i 30 dagar och kan endast återställas av Workfront-administratören.

  Mer information om hur du återställer objekt finns i artikeln [Återställa borttagna objekt](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* Om projektet innehåller uppgifter eller problem med loggade timmar måste Workfront- eller gruppadministratören tillåta att dessa uppgifter tas bort genom att konfigurera inställningarna för Aktivitet och Problem i din Workfront-instans så att du kan ta bort det projekt som innehåller uppgifterna.

  Mer information om hur du aktiverar borttagning av uppgifter, problem eller projekt där timmar har loggats finns i avsnittet Borttagning i [Konfigurera systemomfattande uppgifter och inställningar för problem](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

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
   * Uppdateringar
   * Godkännanden
   * Utgifter
   * Risker
   * Baslinjer
   * Affärsärendeinformation
   * Information om köinformation
   * Faktureringstaxor
   * Faktureringsposter

     Du kan inte ta bort ett projekt som har faktureringsposter med statusen Fakturerad. Mer information finns i [Skapa faktureringsposter](../../projects/project-finances/create-billing-records.md).

* Beroende på hur din Workfront-administratör konfigurerar inställningarna för projekt, uppgift eller borttagning av problem i tidrapportinställningarna för din Workfront-instans, hanteras timmar som är loggade för uppgifter, problem eller projektet på något av följande sätt när du tar bort projektet:

   * Timmarna finns kvar på tidrapporten som allmän tid.
   * Timmarna tas bort och återställs om projektet återställs.

  Mer information om hur du konfigurerar raderingsinställningarna för timmar som är inloggade finns i [Konfigurera tidrapport och timinställningar](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Om det projekt du tar bort är länkat till ett projekt i Workfront Scenario Planner:

   * Initiativet ligger kvar i planen, men kopplingen till projektet har tagits bort.
   * Om projektet som du tar bort är länkat till det enda publicerade initiativet från en plan, tas även indikationen på att planen har publicerats bort.
   * Om du återställer ett borttaget projekt återställs projektet, men länken till projektet återställs inte och området för scenarioplanering visas inte längre i Projektinformation.

     Scenario Planner kräver ytterligare licens. Mer information om Workfront Scenarioplan finns i [Översikt över scenarioplanen](../../../scenario-planner/scenario-planner-overview.md).

     Mer information om projekt som är länkade till initiativ i scenarioplaneraren finns i [Uppdatera eller skapa projekt genom att publicera initiativ i scenarioplaneraren](../../../scenario-planner/publish-scenarios-update-projects.md).

* Om projektet även är en aktivitet för ett mål i Workfront-målen:

   * Projektet tas bort från målet. Det förlopp som anges för målet i projektet tas också bort.

   * Om du återställer det borttagna projektet återställs även projektet som målaktivitet.

     Detta kräver ytterligare en licens. Mer information om Workfront-mål finns i [Översikt över Adobe Workfront-mål](../../../workfront-goals/goal-management/wf-goals-overview.md).

     Mer information om hur du associerar projekt med mål finns i [Lägga till projekt i mål i Adobe Workfront-mål](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

## Ta bort ett projekt i en lista

Du kan ta bort projekt från en lista med projekt.

1. Gå till en lista med projekt eller en projektrapport.
1. Markera det eller de projekt som du vill ta bort och klicka sedan på ikonen **Ta bort** ![Ta bort](assets/delete-icon.png) längst upp i listan.

1. Klicka på **Ja, ta bort** för att bekräfta borttagningen.

   Projekten tas bort och lagras i papperskorgen i 30 dagar. Din Workfront-administratör kan återställa borttagna projekt från papperskorgen under den här tiden.

## Ta bort ett projekt på projektnivå

1. Gå till det projekt som du vill ta bort.
1. Klicka på ikonen **Mer** ![Mer meny](assets/qs-more-menu.png) till höger om projektnamnet och klicka sedan på **Ta bort projekt**.

   ![Mer meny utökad](assets/more-icon-expanded-delete-project-highlighted.png)

1. Klicka på **Ja, ta bort den**.

   Projektet tas bort och lagras i papperskorgen i 30 dagar. Din Workfront-administratör kan återställa den från papperskorgen under den här tiden.

## Återställer borttagna projekt

En system- eller gruppadministratör kan återställa projekt inom 30 dagar efter att de har tagits bort, vilket beskrivs i artikeln [Återställ borttagna objekt](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

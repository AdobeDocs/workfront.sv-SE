---
product-area: projects
navigation-topic: manage-tasks
title: Ta bort uppgifter
description: Du kan ta bort uppgifter som kan vara dubbletter eller som har skapats av fel.
author: Alina
feature: Work Management
exl-id: aee5c293-e5fa-413e-9d9b-c62528941be7
source-git-commit: 463fc65db6adb5cae6ecffb2e165155c89a63d6d
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 0%

---

# Ta bort uppgifter

Du kan ta bort uppgifter som kan vara dubbletter eller som har skapats av fel.

För uppgifter som har historisk information (uppdateringar, schemaändringar, statusändringar eller andra fält) rekommenderar vi att du stänger dem eller markerar dem som döda i stället för att ta bort dem. På så sätt kan du spara den historiska informationen för dina projekt.

## Åtkomstkrav

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
   <td> <p>Arbeta eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till aktiviteter och projekt med åtkomst till Ta bort</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om åtkomst till aktiviteter finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Bevilja åtkomst till aktiviteter</a>. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Contribute-behörigheter till projektet med möjlighet att lägga till uppgifter eller högre</p> <p>När du skapar en uppgift får du automatiskt behörigheten Hantera för uppgiften</p> <p> Mer information om aktivitetsbehörigheter finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Dela en uppgift </a>. </p> <p>Mer information om hur du begär ytterligare behörigheter finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förstå processen med att ta bort uppgifter

* [Begränsningar för att ta bort aktiviteter](#limitations-for-deleting-tasks)
* [Effekten av att ta bort uppgifter](#the-impact-of-deleting-tasks)

### Begränsningar för att ta bort uppgifter  {#limitations-for-deleting-tasks}

* När ett projekt har statusen Slutfört kan du bara ta bort uppgifter om Workfront-administratören eller en gruppadministratör har tillåtit detta i området Projektinställningar. Mer information om hur du ställer in projektinställningar finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Om aktiviteten har loggat timmar måste Workfront- eller gruppadministratören tillåta att dessa uppgifter tas bort genom att konfigurera inställningarna för Aktivitet och problem i din Workfront-instans. Detta gäller också när du försöker ta bort projekt som har uppgifter som har loggats in i timmar.

  <!--
  (NOTE: the last statement is NWE&nbsp;only; not possible in classic)
  -->

  Mer information om hur du aktiverar borttagning av uppgifter där timmar har loggats finns i avsnittet Borttagning i [Konfigurera systemomfattande aktivitet och inställningar för problem](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### Effekten av att ta bort uppgifter {#the-impact-of-deleting-tasks}

När du tar bort en uppgift påverkas andra objekt som är länkade till uppgiften.

Följande objekt som är kopplade till en uppgift tas också bort när du tar bort en uppgift:

* Dokument

  Du kan inte ta bort en uppgift som har ett dokument som har checkats ut bifogat. Mer information om utcheckning av dokument finns i [Checka ut dokument](../../../documents/managing-documents/check-out-documents.md).

* Problem
* Underaktiviteter
* Anteckningar
* Godkännanden

Beroende på hur din Workfront-administratör konfigurerar inställningarna för projekt, uppgift eller borttagning av problem i tidrapport och timinställningar för din Workfront-instans, hanteras timmar som loggas för uppgifterna på något av följande sätt när du tar bort en uppgift:

* Flytta till projektet och återställ inte aktiviteten om den återställs senare.
* tas bort och återställs om uppgiften återställs senare.

  Detta gäller också när du försöker ta bort projekt som har uppgifter som har loggats in i timmar.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this stays NWE; not possible in classic;)
  </MadCap:conditionalText>
  -->

  Mer information om hur du konfigurerar raderingsinställningarna för timmar som är inloggade finns i [Konfigurera tidrapport och timinställningar](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Utgifter för aktiviteten flyttas till projektet.

* De användare som är tilldelade till uppgiften eller aktivitetsgodkännandet blir kvar i projektteamet.

  Mer information om projektteam finns i [Översikt över projektteamet](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Ta bort uppgifter

* [Ta bort flera uppgifter i ett projekt samtidigt](#delete-multiple-tasks-in-a-project-simultaneously)
* [Ta bort en enstaka uppgift](#delete-a-single-task)

### Ta bort flera uppgifter i ett projekt samtidigt  {#delete-multiple-tasks-in-a-project-simultaneously}

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.

1. Klicka på **Projekt**.
1. Klicka på projektnamnet som innehåller de uppgifter du vill ta bort.
1. Klicka på **Åtgärder** i den vänstra panelen.
1. Gör något av följande:

   1. (Villkorligt) När växeln **Spara automatiskt** är aktiverad:

      1. Markera de uppgifter du vill ta bort och klicka sedan på **Mer**
      1. Klicka på **Ta bort** och sedan på **Ta bort** för att bekräfta borttagningen.

         Uppgifterna tas bort.

   1. (Villkorligt) Klicka på ikonen **Planeringsläge** och välj **Spara manuellt** om du vill ångra ändringarna som du gör i uppgiftslistan.

      ![Välj Spara manuellt](assets/manual-save-option.png)

      Gör följande:

      1. Markera de uppgifter som du vill ta bort.
      1. Klicka på **Ta bort**.
      1. (Valfritt) Klicka på **Ångra** om du vill ångra ändringen och inte ta bort uppgifterna.
      1. Klicka på **Gör om** om du vill behålla ändringen och ta bort uppgiften.
      1. Klicka på **Spara** för att ta bort uppgifterna.

         Aktiviteter tas bort först när du har sparat ändringarna.

### Ta bort en enstaka uppgift {#delete-a-single-task}

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.

1. Klicka på **Projekt**.
1. Klicka på projektnamnet som innehåller uppgiften som du vill ta bort.
1. Klicka på **Åtgärder** i den vänstra panelen.
1. Klicka på namnet på den uppgift som du vill ta bort.
1. Klicka på ikonen **Mer** ![](assets/qs-more-menu.png) i det övre högra hörnet.

   ![](assets/delete-tasks-task-level-nwe-350x225.png)

1. Klicka på **Ta bort uppgift**.
1. Om borttagningen tillåts klickar du på **Ta bort**.

   Din Workfront-administratör eller gruppadministratör kanske inte tillåter att uppgifter tas bort där timmar har loggats.

   Mer information om åtkomst och behörigheter som krävs för att ta bort en aktivitet finns i avsnittet [Begränsningar för att ta bort aktiviteter](#limitations-for-deleting-tasks) i den här artikeln.

## Återställ borttagna uppgifter

En Workfront- eller gruppadministratör kan återställa uppgifter inom 30 dagar efter att de har tagits bort, vilket beskrivs i [Återställ borttagna objekt](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

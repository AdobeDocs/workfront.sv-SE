---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Översikt över aktivitetens planerade startdatum
description: Det planerade startdatumet för en uppgift är det datum då du, som skapare av uppgiften, bestämmer att arbetet med uppgiften ska starta. Planerade aktivitetsdatum påverkar datum och tidslinjen i projektet. Information om projektets planerade startdatum finns i Översikt över projektets planerade startdatum.
author: Alina
feature: Work Management
exl-id: 2ac6327f-4a13-4fb8-ad8e-03d032221483
source-git-commit: 0ff02569d3c7fb532a2faafc46fe4235ce77acd4
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---

# Översikt över aktivitetens planerade startdatum

<!-- Audited: 6/2025 -->

Det planerade startdatumet för en uppgift är det datum då du, som skapare av uppgiften, bestämmer att arbetet med uppgiften ska starta. Planerade aktivitetsdatum påverkar datum och tidslinjen i projektet. Information om projektets planerade startdatum finns i [Översikt över projektets planerade startdatum](../../../manage-work/projects/planning-a-project/project-planned-start-date.md).

## Det planerade startdatumet för en uppgift

Du kan antingen ange aktivitetens planerade startdatum eller låta Adobe Workfront beräkna det utifrån vissa kriterier. 

* [Ange det planerade startdatumet för en aktivitet manuellt](#manually-set-the-planned-start-date-of-a-task)
* [Så här beräknas det planerade startdatumet för en aktivitet](#how-the-planned-start-date-is-calculated-for-a-task)

### Ange manuellt planerat startdatum för en uppgift {#manually-set-the-planned-start-date-of-a-task}

Inställningen av en uppgifts planerade startdatum beror på vilken typ av aktivitetsbegränsning du tilldelar uppgiften. 

Du kan ställa in det planerade startdatumet manuellt när du skapar en uppgift. Mer information finns i [Skapa uppgifter i ett projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

Du kan ange det planerade startdatumet manuellt när du väljer något av följande åtgärdsbegränsningar: 

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Typ av aktivitetsbegränsning</strong> </p> </th> 
   <th> <p><strong>Effekt av att ändra det planerade slutförandedatumet manuellt</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Måste börja på</p> <p>Starta tidigast</p> <p>Starta senast</p> </td> 
   <td> <p><span class="s1">Planerat slutförandedatum justeras så att varaktigheten är densamma.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Fasta datum</p> </td> 
   <td> <p>Varaktigheten justeras för att det planerade slutförandedatumet ska vara samma.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Så här beräknas det planerade startdatumet för en aktivitet {#how-the-planned-start-date-is-calculated-for-a-task}

När det beräknas automatiskt av systemet kan följande påverka det planerade startdatumet för en uppgift:

* Inställningen Startdatum i området Åtgärder och problem i installationsprogrammet

  Din Workfront- eller gruppadministratör kan avgöra om en ny uppgift ska starta samma datum som projektets planerade startdatum eller samma dag som du skapar uppgiften.

  Mer information om inställningar för aktiviteter och problem finns i [Konfigurera uppgifter och utgåvor för hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Aktivitetsbegränsning

  Mer information om uppgiftsbegränsningar finns i [Översikt över uppgiftsbegränsningar](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Relation till aktivitetsföregångare

  Mer information om föregående aktiviteter finns i [Översikt över föregående aktiviteter](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Projektets startdatum, när projektet är schemalagt från startdatum.
* Tidsperioden för schemat för aktivitetens primära tilldelare.

  När den primära tilldelaren har en tid som inte är schemalagd under aktivitetens varaktighet, justeras de planerade datumen för aktiviteten därefter när inställningen Överväg användarens tid för aktivitetens varaktighet är markerad för fältet Användartid inte. Nya projekt ärver den här inställningen från området Projektinställningar, men du kan redigera inställningen på projektnivå.

  Om en aktivitet med ett villkor som är inställt på Så snart som möjligt är schemalagd att starta den 1 juni och slutföras den 3 juni, och den primära tilldelaren har markerat 1 juni som ledig tid, blir den planerade startdatumet den 2 juni.

  Mer information om inställningen för Tid av för användaren finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) eller [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

När det anges automatiskt bestäms det planerade startdatumet utifrån följande beräkning: 

```
Planned Start Date = Planned Completion Date - Task Duration
```

Om aktiviteten till exempel har ett slutförandedatum som är 16 september och en varaktighet på 10 dagar, är det planerade startdatumet 6 september.

>[!NOTE]
>
> Uppdateringstypen för projektet måste också ställas in på Automatisk och Vid ändring eller Automatiskt för att de planerade timmarna och varaktigheten ska kunna justeras automatiskt.\
>Mer information om uppdateringstypen finns i [Välj projekttyp](../../../manage-work/projects/manage-projects/select-project-update-type.md).

---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Översikt över aktivitetens planerade slutförandedatum
description: Det planerade slutförandedatumet för en aktivitet är det datum då aktiviteten är inställd på att slutföras.
author: Alina
feature: Work Management
exl-id: b0522db5-9c68-4b1a-82c8-5a9e613eb2ff
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 0%

---

# Översikt över aktivitetens planerade slutförandedatum

Det planerade slutförandedatumet för en aktivitet är det datum då aktiviteten är inställd på att slutföras.

Du kan antingen ange planerat slutförandedatum för en aktivitet eller låta Adobe Workfront beräkna det utifrån vissa kriterier. 

Planerade slutförandedatum för aktiviteter i ett projekt bestämmer det planerade slutförandedatumet för ett projekt när projektet schemaläggs från startdatumet. Mer information om projektets planerade slutförandedatum finns i [Ange projektplanerat slutförandedatum](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>Det planerade slutförandedatumet för en aktivitet skiljer sig från implementeringsdatumet för aktiviteten eller det planerade slutförandedatumet för aktiviteten på följande sätt:
>
>* Bekräftelsedatum är det datum då den person som tilldelats uppgiften manuellt beräknar att de har slutfört uppgiften. Mer information finns i följande artiklar:
   * [Genomför datumöversikt](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
   * [Interaktion mellan implementeringsdatumet och det planerade slutförandedatumet](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
* Planerat slutförandedatum är ett datum som beräknas av Workfront och som tar hänsyn till förseningar, tidslinjer för aktiviteten eller deras föregångare samt andra faktorer för att fastställa ett realtidsdatum för när uppgiften kan slutföras på ett realistiskt sätt. Mer information finns i [Översikt över planerat slutförandedatum för projekt, uppgifter och ärenden](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>


## Ange manuellt planerat slutförandedatum för en uppgift

Du måste ha behörigheterna Redigera och Hantera för aktiviteten för att kunna uppdatera aktivitetens planerade slutförandedatum.

Inställningen för planerat slutförandedatum för en uppgift beror på vilken typ av uppgiftsbegränsning du tilldelar uppgiften. 

Du kan ställa in det planerade slutförandedatumet manuellt i följande områden i Workfront:

* I rutan Redigera uppgift när du skapar eller redigerar en uppgift. Mer information finns i [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* I området Uppgiftsinformation. Mer information finns i [Hantera aktivitetsinformation i området Översikt över aktivitetsinformation](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md).
* I området Hem om Planerat slutförandedatum visas när du visar en uppgift. Mer information finns i [Uppdatera eller redigera en arbetsuppgift i hemområdet](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* I uppgiftshuvudet. Mer information finns i [Nya objektrubriker](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* I en uppgiftslista eller rapport när fältet Planerat slutförandedatum visas i vyn.

   Mer information finns i [Redigera uppgifter i en lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

Du kan ange planerat slutförandedatum manuellt när du väljer något av följande åtgärdsbegränsningar: 

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Typ av aktivitetsbegränsning</strong> </p> </th> 
   <th> <p><strong>Effekt av Manuell ändring av planerat slutförandedatum</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Måste avslutas</p> <p>Avsluta senast</p> <p>Avsluta tidigast</p> </td> 
   <td> <p><span class="s1">Det planerade startdatumet justeras så att varaktigheten är densamma.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Fasta datum</p> </td> 
   <td> <p>Varaktigheten justeras för att det planerade startdatumet ska vara samma.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Hur Workfront automatiskt beräknar planerat slutförandedatum för en uppgift

När det beräknas automatiskt av systemet kan följande påverka det planerade slutförandedatumet för en uppgift:

* Aktivitetsbegränsning

   Mer information om uppgiftsbegränsningar finns i artikeln [Översikt över uppgiftsbegränsning](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Relation till aktivitetsföregångare

   Mer information om föregående aktiviteter finns i artikeln [Översikt över föregående aktiviteter](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Projektets slutförandedatum, när projektet är schemalagt från slutförandedatum.
* Tidsperioden för schemat för aktivitetens primära uppdragsgivare.

   När den primära tilldelade har en tid som inte är schemalagd under aktivitetens varaktighet justeras aktivitetens planerade datum i enlighet med detta när den **Överväg användarens ledig tid i aktivitetsvaraktigheter** inställningen är markerad för **Användningstid av** fält. Nya projekt ärver den här inställningen från området Projektinställningar, men du kan redigera inställningen på projektnivå.

   Om en uppgift med ett villkor som är så snart som möjligt är schemalagd att påbörjas den 1 juni och slutföras den 3 juni och den primära uppdragen har markerats med 2 juni, blir uppgiften Planerat slutförandedatum 4 juni.

   Mer information om **Användningstid av** inställningar, se artiklarna [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) eller [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

* Den tid som är associerad med godkännandeinställningar om aktiviteten är associerad med ett godkännande. Mer information finns i [Konfigurera globala inställningar för godkännande](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

När detta anges automatiskt bestäms det planerade slutförandedatumet utifrån följande beräkning: 

```
Planned Completion Date = Planned Start Date + Duration
```

Om aktiviteten till exempel har startdatumet 16 september och varaktigheten 10 dagar är det planerade slutförandedatumet 26 september.

>[!NOTE]
 Uppdateringstypen för projektet måste ställas in på Automatisk och Vid ändring eller Automatiskt för att de planerade timmarna och varaktigheten ska kunna justeras automatiskt.\
Mer information om uppdateringstypen finns i artikeln [Välj typ av projektuppdatering](../../../manage-work/projects/manage-projects/select-project-update-type.md).

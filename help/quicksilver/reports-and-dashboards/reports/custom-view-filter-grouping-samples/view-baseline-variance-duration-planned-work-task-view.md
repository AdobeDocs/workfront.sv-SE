---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: Baslinjeavvikelse för Varaktighet och Planerat arbete i en aktivitetsvy'
description: Visa baslinjeavvikelsen för Varaktighet och Planerat arbete.
author: Nolan
feature: Reports and Dashboards
exl-id: 2a1eef9c-016c-4a04-acda-6070fcb0e23d
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---

# Visa: baslinjeavvikelse för Varaktighet och Planerat arbete i en uppgiftsvy

<!--Audited: 11/2024-->

I den här vyn visas följande i en uppgiftsvy:

* Uppgiftsinformation med baslinjeaktivitetsinformation.
* Skillnaden mellan Varaktighet och Standardvaraktighet för baslinje.
* Skillnaden mellan det planerade arbetet och standardoriginalarbetet.

>[!NOTE]
>
>De data som visas i följande vy jämför de faktiska aktivitetsvärdena med de värden som är associerade med standardschemauppgifterna.

![baseline_variance_in_a_task_view.png](assets/baseline-variance-in-a-task-view-350x38.png)

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
   <td> 
    <p>Nytt:</p>
   <ul><li><p>Medarbetare som ändrar ett filter </p></li>
   <li><p>Standard för att ändra en rapport</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Begäran om att ändra ett filter </p></li>
   <li><p>Planera att ändra en rapport</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra ett filter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visa baslinjeavvikelse för Varaktighet och Planerat arbete i en uppgiftsvy

1. Gå till en lista med uppgifter.
1. I listrutan **Visa** väljer du **Ny vy** eller redigerar en befintlig vy.
1. Ta bort alla kolumner i vyn, förutom den första.
1. När den första kolumnen är markerad klickar du på **Växla till textläge** och sedan på **Redigera textvy**.
1. Kopiera texten nedan och klistra in den i vyns första kolumn:

   ```
   column.0.descriptionkey=name
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat=int
   column.0.link.lookup=link.view
   column.0.link.valuefield=objCode
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.0.displayname=Task Name
   column.1.descriptionkey=duration
   column.1.linkedname=direct
   column.1.listsort=intAsInt(durationMinutes)
   column.1.namekey=duration.abbr
   column.1.querysort=durationMinutes
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=durationFieldLong
   column.1.valueformat=compound
   column.1.viewalias=duration
   column.1.width=100
   column.1.displayname=Task Duration
   column.2.descriptionkey=view.relatedcolumn
   column.2.descriptionkeyargkey.0=defaultbaselinetask
   column.2.descriptionkeyargkey.1=duration
   column.2.linkedname=defaultBaselineTask
   column.2.listsort=intAsInt(durationMinutes)
   column.2.namekey=duration
   column.2.namekeyargkey.0=defaultbaselinetask.abbr
   column.2.namekeyargkey.1=duration.abbr
   column.2.querysort=defaultBaselineTask:durationMinutes
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=defaultBaselineTask:durationFieldLong
   column.2.valueformat=compound
   column.2.viewalias=defaultBaselineTask:duration
   column.2.width=100
   column.2.displayname=Dflt Baseline Tsk: Dur
   column.2.durationunitfield=durationUnit.value
   column.3.description=Duration Variance"column.3.linkedname=direct
   column.3.listsort=intAsInt(durationMinutes)
   column.3.name=Duration Variance
   column.3.querysort=durationMinutes
   column.3.shortview=false
   column.3.stretch=0
   column.3.valueexpression=CONCAT(SUB({duration},{defaultBaselineTask}.{duration})/480," Days")
   column.3.valueformat=HTML
   column.3.viewalias=duration
   column.3.width=100
   column.3.displayname=Duration Variance
   column.4.descriptionkey=workrequired
   column.4.linkedname=direct
   column.4.listsort=doubleAsDouble(workRequired)
   column.4.namekey=workrequired.abbr
   column.4.querysort=workRequired
   column.4.shortview=false
   column.4.stretch=0
   column.4.valuefield=workFieldLong
   column.4.valueformat=compound
   column.4.viewalias=workrequired
   column.4.width=100
   column.4.displayname=Wrk Req
   column.5.descriptionkey=view.relatedcolumn
   column.5.descriptionkeyargkey.0=defaultbaselinetask
   column.5.descriptionkeyargkey.1=workrequired
   column.5.linkedname=defaultBaselineTask
   column.5.listsort=doubleAsDouble(workRequired)
   column.5.namekey=view.relatedcolumn
   column.5.namekeyargkey.0=defaultbaselinetask.abbr
   column.5.namekeyargkey.1=workrequired.abbr
   column.5.querysort=defaultBaselineTask:workRequired
   column.5.shortview=false
   column.5.stretch=0
   column.5.valuefield=defaultBaselineTask:workFieldLong
   column.5.valueformat=compound
   column.5.viewalias=defaultBaselineTask:workrequired
   column.5.width=100
   column.5.displayname=Dflt Baseline Tsk: Wrk Req
   column.6.descriptionkey=workrequired
   column.6.linkedname=direct
   column.6.listsort=doubleAsDouble(workRequired)
   column.6.name=Effort Variance
   column.6.querysort=workRequired
   column.6.shortview=false
   column.6.stretch=0
   column.6.valueexpression=CONCAT(SUB({workRequired},{defaultBaselineTask}.{workRequired})/60," Hours")
   column.6.valueformat=HTML
   column.6.viewalias=workrequired
   column.6.width=100
   column.6.displayname=Effort Variance
   ```

1. Klicka på **Spara vy**.

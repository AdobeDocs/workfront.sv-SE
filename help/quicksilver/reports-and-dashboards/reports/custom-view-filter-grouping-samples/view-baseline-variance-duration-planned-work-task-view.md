---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: baslinjeavvikelse för Varaktighet och Planerat arbete i en uppgiftsvy'
description: Visa baslinjeavvikelsen för Varaktighet och Planerat arbete.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2a1eef9c-016c-4a04-acda-6070fcb0e23d
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 0%

---

# Visa: baslinjeavvikelse för Varaktighet och Planerat arbete i en uppgiftsvy

I den här vyn visas följande i en uppgiftsvy:

* Uppgiftsinformation med baslinjeaktivitetsinformation.
* Skillnaden mellan Varaktighet och Standardvaraktighet för baslinje.
* Skillnaden mellan det planerade arbetet och standardoriginalarbetet.

>[!NOTE]
>
> De data som visas i följande vy jämför de faktiska aktivitetsvärdena med de värden som är associerade med standardschemauppgifterna.

 

![baseline_variance_in_a_task_view.png](assets/baseline-variance-in-a-task-view-350x38.png)

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
   <td> <p>Begäran om att ändra en vy </p>
   <p>Planera att ändra en rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra en vy</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Visa baslinjeavvikelse för Varaktighet och Planerat arbete i en uppgiftsvy

1. Gå till en lista med uppgifter.
1. Välj **Ny vy** i listrutan **Visa**.

1. Ta bort alla kolumner i vyn, förutom den första.
1. När den första kolumnen är markerad klickar du på **Växla till textläge**.
1. Kopiera texten nedan och klistra in den i vyns första kolumn:
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.link.property.0.valuefield=ID<br>column.0.link.link.property.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>5}column.0.link.valueFormat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.0.displayname=Task Name<br>column.1.descriptionkey=duration<br>column.1.linkedname=direct<br>column.1.listsort=intAs Int(durationMinutes)<br>column.1.namekey=duration.abbr<br>column.1.querysort=durationMinutes<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=durationFieldLong<br>column.1.valueformat=compound{compound 25}column.1.viewAlias=duration<br>column.1.width=100<br>column.1.displayname=Task Duration<br>column.2.descriptionkey=view.relatedcolumn<br>column.2.descriptionkeykey.0=defaultbaselinetask<br>column.2.descripdescrip tionkeykey.1=duration<br>column.2.linkedname=defaultBaselineTask<br>column.2.listsort=intAsInt(durationMinutes)<br> column.2.namekey=duration<br>column.2.namekeyargkey.0=defaultbaselinetask.abbr<br>column.2.namekeyargkey.1=duration.abbr<br>column.2.querysort=defaultBaselineTask:durationMinutes<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=defaultBaselineTask:durationFieldLong<br>column.2.valueformat=compound<br> column.2.viewAlias=defaultBaselineTask:duration<br>column.2.width=100<br>column.2.displayname=Dflt Baseline Tsk: Dur<br>column.2.durationunitfield=durationUnit.value<br>column.3.description=Duration Variance"column.3 .linkedname=direct<br>column.3.listsort=intAsInt(durationMinutes)<br>column.3.name=Duration Variance<br>column.3.querysort=durationMinutes<br>column.3.shortview=false<br>column.3.stretch=0<br>column.3.valueexpression=true CONCAT(SUB({duration},{defaultBaselineTask}).<br>{duration})/480," Days")<br>column.3.valueformat=HTML<br>column.3.viewalias=duration<br>column.3.width=100<br>column.3.displayname=Duration Variance<br>column.4.descriptionkey=workrequired<br>column.4.linkedname=direct<br>column.column 4.listsort=doubleAsDouble(workRequired)<br>column.4.namekey=workrequired.abbr<br>column.4.querysort=workRequired<br>column.4.shortview=false<br>column.4.stretch=0<br>column.4.valuefield=workFieldLong<br>column.4 .valueformat=compound<br>column.4.viewalias=workrequired<br>column.4.width=100<br>column.4.displayname=Work Req<br>column.5.descriptionkey=view.relatedcolumn<br>column.5.descriptionkeykey.0=defaultbaselinetask<br> 9}column.5.descriptionkeykey.1=workrequired<br>column.5.linkedname=defaultBaselineTask<br>column.5.listsort=doubleAsDouble(workRequired)<br>column.5.namekey=view.relatedcolumn<br>column.5.namekeykey.0=defaultbaselell inetask.abbr<br>column.5.namekeyargkey.1=workrequired.abbr<br>column.5.querysort=defaultBaselineTask:workRequired<br>column.5.shortview=false<br>column.5.stretch=0<br>column.5.valuefield=defaultBaselineTask:work FieldLong<br>column.5.valueformat=compound<br>column.5.viewalias=defaultBaselineTask:workrequired<br>column.5.width=100<br>column.5.displayname=Dflt Baseline Task: Wrk Req<br>column.6.descriptionkey=workrequired<br>column.6.linkedname=direct<br>column.6.listsort=doubleAsDouble(workRequired)<br>column.6.name=Effort Variance<br>column.6.querysort=workRequired<br>column.6.shortview=false<br>column.6.stretch=0<br>column.6 .valueexpression=CONCAT(SUB({workRequired},{defaultBaselineTask}).{workRequired})/60," Timmar")<br>column.6.valueformat=HTML<br>column.6.view=workrequired<br>column.6.width=100<br>column.6.displayName=Effort Variance</pre>

1. Klicka på **Spara vy**.
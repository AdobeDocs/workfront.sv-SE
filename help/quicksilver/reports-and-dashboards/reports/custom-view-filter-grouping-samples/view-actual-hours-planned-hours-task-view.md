---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Vy: Faktiska timmar över planerade timmar i samma kolumn i en uppgiftsvy"
description: I den här uppgiftsvyn visas det faktiska antalet timmar som registrerats för en uppgift över de timmar som planerats för varje uppgift.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1179283-dc2e-40d3-b8e0-4b1b79f83ad3
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# Visa: Faktiska timmar över planerade timmar i samma kolumn i en uppgiftsvy

I den här uppgiftsvyn visas det faktiska antalet timmar som registrerats för en aktivitet över de timmar som planerats för varje aktivitet.

![actual_vs_planning_in_task_report.png](assets/actual-vs-planned-in-task-report-350x58.png)

## Krav för åtkomst

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Någon</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licens för Adobe Workfront*</td> 
   <td> <p>Begära att ändra en vy </p>
   <p>Planera att ändra en rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra en vy</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst kan du fråga Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra din åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Behörigheter för objekt</td> 
   <td> <p>Hantera behörigheter till en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Om du vill ta reda på vilket abonnemang, vilken licenstyp eller vilken åtkomst du har kontaktar du Workfront-administratören.

## Visa faktiska timmar över planerade timmar i en uppgiftsvy

Så här använder du den här vyn:

1. Gå till en lista med uppgifter.
1. Välj **Ny vy** i listrutan **Visa**.

1. Ta bort alla kolumner utom en i området **Förhandsvisa kolumn**.
1. Klicka på rubriken för den återstående kolumnen och klicka sedan på **Växla till textläge**.
1. Håll muspekaren över textlägesområdet och klicka på **Klicka för att redigera text**.
1. Ta bort texten som du hittar i **rutan Textläge** och ersätt den med följande kod:
   <pre>column.0.descriptionkey=namn<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val column.0.linkedname=direkt<br><br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=namn<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.viewalias=tilldelningar<br>column.1.displayname=<br>column.1.linkedname=direkt<br>column.1.namekey=uppdrag<br>column.1.valuefield=assignmentsListString<br>column.1.valueformat=HTML<br>column.1.tile.name=komponent.assignmentslist<br>column.2.displayname=faktiska/ planerade timmar<br>column.2.linkedname=direkt<br>column.2.namekey=actualworkrequired<br>column.2.querysort=actualWork<br>column.2.textmode=true<br>column.2.valueexpression=CONCAT({actualWorkRequired}/60,' / ',{workRequired}/60)<br>column.2.valuefield=actualWorkRequired<br>column.2.valueformat=compound<br>column.2.viewalias=actualworkrequired<br>column.3.aggregator.function=SUM column.3.aggregator.valueexpression=SUB<br>({actualWork}, {workRequired})<br>column.3.aggregator.valueformat=compound<br>column.3.displayname=Timmar varians<br>column.3.linkedname=direkt<br>column.3.textmode=true<br>column.3.valueexpression=SUB({actualWork}, {workRequired})/60<br>column.3.valueformat=customNumberAsString</pre>

1. Klicka på **Spara vy**.

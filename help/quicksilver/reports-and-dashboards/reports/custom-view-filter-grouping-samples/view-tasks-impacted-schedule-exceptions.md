---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: aktiviteter som påverkas av schemaundantag'
description: I den här aktivitetsvyn identifieras aktiviteter som måste slutföras sent på grund av helger, personlig tid av eller andra schemaundantag.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7d7c77fa-d9a7-4e91-8dae-ad3aaca6f1da
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 0%

---

# Visa: aktiviteter som påverkas av schemaundantag

I den här aktivitetsvyn identifieras aktiviteter som måste slutföras sent på grund av helger, personlig tid av eller andra schemaundantag.

I den här vyn visas följande:

* Aktiviteternas längd
* De planerade start- och slutförandedatumen för aktiviteterna
* Aktiviteternas längd enligt antalet dagar mellan aktiviteternas planerade startdatum och planerade slutförandedatum (kalendervaraktighet)
* Antalet dagar i projektets schema när aktiviteten startar (kalenderns startdatum)
* Veckodagslängd för uppgifterna enligt antalet veckodagar mellan planerat start- och slutförandedatum för aktiviteterna (Veckodagslängd)
* Om Veckodagslängd är längre än aktiviteternas längd, vilket betyder att det finns undantagsdagar i aktiviteternas längd, markeras aktiviteterna som ett undantag.\
  ![tasks_with_calendar_Exceptions.png](assets/tasks-with-calendar-exceptions-350x51.png)

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

## Visa aktiviteter som påverkas av schemaundantag

1. Gå till en lista med uppgifter.
1. Välj **Ny vy** i listrutan **Visa**.

1. Ta bort alla kolumner utom en i området **Förhandsvisa kolumn**.
1. Klicka på rubriken för den återstående kolumnen och klicka sedan på **Växla till textläge**.
1. För musen över textlägesområdet och klicka **Klicka för att redigera text**.
1. Ta bort texten som du söker i rutan **Textläge** och ersätt den med följande kod:
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.link.property.0.valuefield=ID<br>column.0.link.link.property.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>5}column.0.link.valueFormat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=duration<br>column.1.linkedname=direct<br>column.1.listsort=intAsInt(durationMinutes)<br>column.1.namekey=duration.abbr<br>column.1.querysort=durationMinutes<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=durationFieldLong<br>column.1.valueformat=compound<br>column.1.viewalias=duration{22 5}column.1.width=80<br>column.2.descriptionkey=plannedstartdate<br>column.2.linkedname=direct<br>column.2.listsort=atDateAsAtDate(planningStartDate)<br>column.2.namekey=plannedstartdate.abbr<br>column.2.2 querysort=planningStartDate<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=planningStartDate<br>column.2.valueformat=atDate<br>column.2.width=80<br>column.3.descriptionKey=plan completeDate<br>column.3.linkedname=direct<br>column.3.listsort=atDateAsAtDate(planningCompletionDate)<br>column.3.namekey=plannedcomplitiondate.abbr<br>column.3.querysort=planningCompletionDate<br>column.3.shortview=false <br>column.3.stretch=0<br>column.3.valuefield=planningCompletionDate<br> column.3.valueformat=atDate<br>column.3.width=80<br>column.4.aggregator.displayformat=int<br>column.4.aggregator.function=SUM<br>48} column.4.aggregator.namekey=id<br>column.4.aggregator.valueexpression=DATEDIFF({plannedCompletionDate},<br>{plannedStartDate})+1<br>column.4.aggregator.valueformat=intAsInt<br>column.4.descriptionkey=id<br>column.4.linkedst name=direct<br>column.4.listsort=intAsInt(ID)<br>column.4.name=Calendar Duration<br>column.4.querysort=ID<br>column.4.shortview=false<br>column.4.stretch=0<br>column.4.valueexpression=DATEDIFF({6 <br>,{plannedStartDate})+1<br>column.4.valueformat=int<br>column.4.width=80<br>column.5.aggregator.displayformat=int<br>column.5.aggregator.function=SUM<br>column.5.aggregator.namekey=id<br>column.5.5.aggreg. ator.valueexpression=DATEDIFF({plannedStartDate},{project}).{plannedCompletionDate}<br>{plannedStartDate})+0<br>column.5.aggregator.valueformat=intAsInt<br>column.5.descriptionkey=id<br>column.5.linkedname=direct<br>column.5.listsort=intAsInt(ID)<br>column.5.name=Calendar Start Date<br>column.5.querysort=ID{plannedStartDate} 8}column.5.shortview=false<br>column.5.stretch=0<br>column.5.valueexpression=DATEDIFF(<br>,{project}).{plannedStartDate})+0<br>column.5.valueformat=int<br>column.5.width=80<br>column.6.aggregator.displayformat=int<br>column.6.aggregator.function=SUM<br>column.6.aggregator.namekey=id<br>column.6.aggregator.valueexpression=WEEKDADIFF({plannedStartDate}, <br>{plannedCompletionDate})+0<br>column.6.aggregator.valueformat=HTML<br> column.6.descriptionkey=id<br>column.6.linkedname=direct<br>column.6.listsort=intAsInt(ID)<br>column.6.name=Week Day Duration<br>column.column 6.querysort=ID<br>column.6.shortview=false<br>column.6.stretch=0<br>column.6.valueexpression=WEEKDAYDIFF({plannedStartDate},{plannedCompletionDate})+0<br>column.6.valueformat=int<br>column.6.width=80{22 3}column.7.aggregator.displayformat=int<br>column.7.aggregator.expression=IF((WEEKDAYDIFF(<br>,{plannedCompletionDate}))&gt;({duration}/480),"Exception",")<br>column.7.aggregator.function=SUM<br>column.7.7 aggregator.namekey=id<br>column.7.aggregator.valueformat=HTML<br>column.7.linkedname=direct<br>column.7.listsort=intAsInt(ID){plannedStartDate} column.7.name=Schedule<br>column.7.querysort=ID<br>column.7.shortview=view false<br>column.7.stretch=0<br>column.7.valueexpression=IF((WEEKDAYDIFF(<br>,{plannedCompletionDate}))&gt;({duration}/480),"Exception",")<br>column.7.valueFormat=HTML<br>column.7.width=0 80{plannedStartDate}</pre>

1. Klicka på **Spara vy**.

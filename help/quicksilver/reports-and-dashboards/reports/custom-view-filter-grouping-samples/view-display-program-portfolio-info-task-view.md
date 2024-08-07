---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: visa information om Program och Portfolio i en uppgiftsvy'
description: I den här uppgiftsvyn visas programmet och Portfolio som är associerade med aktivitetens projekt. Den här informationen är inte tillgänglig i Report Builder när en uppgiftsvy skapas. Den här informationen är bara tillgänglig i textläge.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cdd5a1e9-3cbf-4951-b803-fca544b2519a
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Visa: visa Program- och Portfolio-information i en uppgiftsvy

I den här uppgiftsvyn visas programmet och Portfolio som är associerade med aktivitetens projekt. Den här informationen är inte tillgänglig i Report Builder när en uppgiftsvy skapas. Den här informationen är bara tillgänglig i textläge.

Vyn innehåller även länkar till projekt, program och Portfolio från en uppgiftslista.

![](assets/view--program-and-portfolio-350x116.png)

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

## Visa program- och Portfolio-information i en uppgiftsvy

Så här använder du den här vyn på en uppgiftslista:

1. Gå till en lista med uppgifter.
1. Välj **Ny vy** i listrutan **Visa**.

1. Ta bort alla kolumner utom en i området **Förhandsvisa kolumn**.
1. Klicka på rubriken för den återstående kolumnen och klicka sedan på **Växla till textläge**.
1. För musen över textlägesområdet och klicka på **Klicka för att redigera text**.
1. Ta bort texten som du söker i rutan **Textläge** och ersätt den med följande kod:
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.link.property.0.valuefield=ID<br>column.0.link.link.property.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>5}column.0.link.valueFormat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=project<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.link.0.valuefield=project:ID{11 8}column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.valuefield=project:objCode<br>column.1.link.valueformat=val<br>column.1.linkedname=project<br>column.1.listsort=nested (project).string(name)<br>column.1.namekey=project<br>column.1.querysort=project:name<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=project:name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.descriptionkey=program<br>column.2.displayName=Program<br>, column.2.link.link.property.0.name=ID<br>column.2.link.link.property.0.valuefield=project:program:ID<br>column.2.link.link.link.property.property .0.valueFormat=int<br>column.2.link.lookup=link.view<br>column.2.link.valueField=project:program:objCode<br>column.2.link.valueFormat=val<br>column.2.linkedname=project<br>column.2.listsort=nested(project:program).project string(name)<br>column.2.namekey=project<br> column.2.querysort=project:program:name<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=project:program:name<br>column.2.valueformat=HTML <br>column.2.width=150<br>column.3.descriptionkey=portfolio<br>column.3.displayname=Portfolio<br>column.3.link.linkproperty.0.name=ID<br>column.3.link.linkproperty.0.valuefield=project:portfolio:ID<br>column.3.link.linkproperty.0.valueformat=int<br>column.3.link.lookup=link.view<br>column.3.link.valuefield=project:portfolio:objCode<br>column.3.link.valueformat=val<br>column.3.linkedname=project<br>column.3.listsort=nested(nested project:portfolio).string(name)<br>column.3.namekey=project<br>column.3.querysort=project:portfolio:name<br>column.3.shortview=false<br>column.3.stretch=0<br>column.3.valuefield=project:portfolio:name<br>column.3.value eformat=HTML<br>column.3.width=150 <br></pre>

1. Klicka på **Spara vy**.

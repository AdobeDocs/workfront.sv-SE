---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: visa överordnade aktiviteter på upp till fyra nivåer'
description: I den här uppgiftsvyn visas aktivitetsnamnet i den första kolumnen och (om det finns) upp till 4 överordnade uppgifter i separata kolumner i samma lista.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 66b45d64-794d-4adc-b208-2ded0dc9c5dc
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 0%

---

# Visa: visa överordnade uppgifter på upp till 4 nivåer

I den här uppgiftsvyn visas aktivitetsnamnet i den första kolumnen och (om det finns) upp till 4 överordnade uppgifter i separata kolumner i samma lista.

![parent_tasks_4_levels_deep.png](assets/parent-tasks-4-levels-deep-350x29.png)

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

## Visa överordnade aktiviteter på upp till 4 nivåer

1. Gå till en lista med uppgifter.
1. Välj **Ny vy** i listrutan **Visa**.

1. Ta bort alla kolumner utom en i området **Förhandsvisa kolumn**.
1. Klicka på rubriken för den återstående kolumnen och klicka sedan på **Växla till textläge**.
1. För musen över textlägesområdet och klicka på **Klicka för att redigera text**.
1. Ta bort texten som du söker i rutan **Textläge** och ersätt den med följande kod:

   ```
   column.0.descriptionkey=name
   ```

   <pre>column.0.link.linkproperty.0.name=ID<br>column.0.link.property.0.valuefield=ID<br>column.0.link.property.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=parent<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.link.property.0.valuefield=parent:ID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.lookup=up link.view<br>column.1.link.valuefield=parent:objCode<br>column.1.link.valueformat=val<br>column.1.linkedname=parent<br>column.1.listsort=nested(parent).string(name)<br>column.1.namekey=parent<br>column.1.querysort=parent:name<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=parent:name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.description=parent<br>0 column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=parent:parent:ID<br>column.2.link.property.0.valueformat=int<br>column.2.link.lookup=link.view<br>column.2.link.valuefield=parent:parent:objCode<br>column.2.link.valueformat=val<br>column.2.linkedname=parent<br>column.2.listsort=nested(parent:parent).string(name)<br>column.2.name=Parent Parent<br>column.2.querysort=parent:parent:name<br>column.2.shortview=false<br> column.2.stretch=0<br>column.2.valuefield=parent:parent:name<br>column.2.valueformat=HTML<br>column.2.width=150<br>column.3.description=Parent Parent Parent<br>column.3.link.link.link property.0.name=ID<br>column.3.link.linkproperty.0.valuefield=parent:parent:parent:ID<br>column.3.link.property.0.valueformat=int<br>column.3.link.lookup=link.view<br>column.3.link.valuefield=parent:parent:parent:obj Code<br>column.3.link.valueformat=val<br>column.3.linkedname=parent<br>column.3.listsort=nested(parent:parent:parent).string(name)<br>column.3.name=Parent Parent Parent<br>column.3.querysort=parent:parent:parent:name{name 64}column.3.shortview=false<br>column.3.stretch=0<br>column.3.valuefield=parent:parent:parent:name<br>column.3.valueformat=HTML<br>column.3.width=150<br>column.4.description=parent{77 1}column.4.link.linkproperty.0.name=ID<br>column.4.link.link.property.0.valuefield=parent:parent:parent:parent:ID<br>column.4.link.linkproperty.0.valueformat=int<br>column.4.link.lookup=link.view<br>column.4.link.value.value field=parent:parent:parent:parent:objCode<br>column.4.link.valueformat=val<br>column.4.linkedname=parent<br>column.4.listsort=nested(parent:parent:parent:parent).string(name)<br>column.4.name=Parent Parent Parent{8 5}column.4.querysort=parent:parent:parent:parent:name<br>column.4.shortview=false<br>column.4.stretch=100<br>column.4.valuefield=parent:parent:parent:parent:name<br>column.4.valueformat=HTML<br>4 column.4.width=150<br><br><br></pre>

1. Klicka på **Spara vy**.

   Uppgiftens namn visas i den första kolumnen, och om uppgiften har överordnade visas upp till 4 överordnade i de återstående kolumnerna.

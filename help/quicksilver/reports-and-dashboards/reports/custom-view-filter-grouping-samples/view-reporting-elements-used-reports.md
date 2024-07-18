---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: rapportelement som används i rapporter'
description: I den här vyn visas den vy, det filter och den gruppering som används för att skapa respektive rapport i Adobe Workfront när du använder den i en lista med rapporter.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 67f86523-e136-4768-af93-586a107b106f
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# Visa: rapportelement som används i rapporter

I den här vyn visas den vy, det filter och den gruppering som används för att skapa respektive rapport i Adobe Workfront när du använder den i en lista med rapporter.

Du kan se

```
valuefields
```

eller

```
valueexpressions
```

används i alla element i rapporten.

![report_with_elements_definitions.png](assets/report-with-elements-definitions-350x130.png)

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

## Visa rapportelement som används i rapporter

1. Gå till en lista med rapporter.
1. Välj **Ny vy** i listrutan **Visa**.

1. Ta bort alla kolumner utom en i området **Förhandsvisa kolumn**.
1. Klicka på rubriken för den återstående kolumnen och klicka sedan på **Växla till textläge**.
1. För musen över textlägesområdet och klicka på **Klicka för att redigera text**.
1. Ta bort texten som du söker i rutan **Textläge** och ersätt den med följande kod:
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.link.property.0.valuefield=ID<br>column.0.link.property.0.valueformat=string<br>column.0.link.lookup=link.run<br>column.0.link.value=val(objCode)<br>}column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=200<br>column.1.descriptionkey=objectType{1 <br> column.1.listsort=nested(view).string(uiObjCode)<br>column.1.namekey=objectype.abbr<br>column.1.querysort=uiObjCode<br>column.1.valuefield=uiObjCode<br>column.1.valueformat=obint jCodeMessage<br>column.1.width=80<br>column.2.descriptionkey=enter<br>column.2.listsort=nested(enteredBy).string(lastName)<br>column.2.namekey=enteredby.abbr<br>column.2.querysort=enteredBy Namn<br>column.2.valuefield=enteredBy:name<br>column.2.valueformat=HTML<br>column.2.width=130<br>column.3.displayname=Filterdefinition<br>column.3.textmode=true<br>column.3.valuefield=filter:definition<br> column.3.valueformat=HTML<br>column.4.displayname=View definition<br>column.4.textmode=true<br>column.4.valuefield=view:definition<br>column.4.valueformat=HTML<br>column.5.displayname=Grouping definition<br>column.5.textmode=true{3 5}column.5.valuefield=groupBy:definition<br>column.5.valueformat=HTML<br><br></pre>

1. Klicka på **Spara vy**.

---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visa: tilldelad användares företag och hemgrupp"
description: Den här uppgiftsvyn visar företag och hemgrupp för uppgiftens primära ägare. Dessa är värden som inte är tillgängliga i standardgränssnittet, men som är tillgängliga via textläge.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 818c1f3a-4e82-4dc3-af86-4f9dcf5c11a4
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# Visa: tilldelad användares företag och hemgrupp

Den här uppgiftsvyn visar företag och hemgrupp för uppgiftens primära ägare. Dessa är värden som inte är tillgängliga i standardgränssnittet, men som är tillgängliga via textläge.

![](assets/view--assigned-user-s-company-and-home-group-350x80.png)

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

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Visa den tilldelade användarens företag och hemgrupp

1. Gå till en lista med uppgifter.
1. Från **Visa** nedrullningsbar meny, välja **Ny vy**.

1. I **Förhandsgranska kolumn** -område, ta bort alla kolumner utom en.
1. Klicka på rubriken för den återstående kolumnen och klicka sedan på **Växla till textläge**.
1. För musen över textlägesområdet och klicka **Klicka för att redigera text**.
1. Ta bort den text du hittar i **Textläge** och ersätt den med följande kod:
   <pre>column.0.descriptionkey=name<br> column.0.link.linkproperty.0.name=ID<br> column.0.link.linkproperty.0.valuefield=ID<br> column.0.link.linkproperty.0.valueformat=int<br> column.0.link.lookup=link.view<br> column.0.link.valuefield=objCode<br> column.0.link.valueFormat=val<br> column.0.linkedname=direct<br> column.0.listsort=string(name)<br> column.0.namekey=name.abbr<br> column.0.querysort=name<br> column.0.shortview=false<br> column.0.stretch=100<br> column.0.valuefield=name<br> column.0.valueformat=HTML<br> column.0.width=150<br> column.1.descriptionkey=tilldelad till<br> column.1.link.linkproperty.0.name=ID<br> column.1.link.linkproperty.0.valuefield=assignTo:ID<br> column.1.link.linkproperty.0.valueformat=int<br> column.1.link.lookup=link.view<br> column.1.link.valueField=assignTo:objCode<br> column.1.link.valueFormat=val<br> column.1.linkedname=assignTo<br> column.1.listsort=nested(assignTo).string(name)<br> column.1.namekey=tilldelad till<br> column.1.querysort=assignTo:name<br> column.1.shortview=false<br> column.1.stretch=0<br> column.1.valuefield=assignTo:name<br> column.1.valueformat=HTML<br> column.1.width=150<br> column.2.description=Tilldelad till företag<br> column.2.displayName=Assignated To Company<br> column.2.linkedname=assignTo:company<br> column.2.listsort=nested(assignTo:company).string(name)<br> column.2.namekey=tilldelad till<br> column.2.querysort=assignTo:company:name<br> column.2.shortview=false<br> column.2.stretch=0<br> column.2.valuefield=assignTo:company:name<br> column.2.valueformat=HTML<br> column.2.width=150<br> column.3.description=Tilldelad till hemgrupp<br> column.3.displayName=Tilldelad till hemgrupp<br> column.3.linkedname=assignTo:homeGroup<br> column.3.listsort=nested(assignTo:homeGroup).string(name)<br> column.3.namekey=tilldelad till<br> column.3.querysort=assignTo:homeGroup:name<br> column.3.shortview=false<br> column.3.stretch=0<br> column.3.valuefield=assignTo:homeGroup:name<br> column.3.valueformat=HTML<br> column.3.width=150</pre>

1. Klicka **Spara ändringar**.

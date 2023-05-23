---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: problem med företagsnamnet för upphovsmannen'
description: I den här problemvyn visas det företagsnamn som är associerat med den användare som skickade problemet.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e628f7cf-4a7b-4125-bea6-348c72477bd7
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Visa: problem med företagsnamnet för upphovsmannen

I den här problemvyn visas det företagsnamn som är associerat med den användare som skickade problemet.

![custom_view_for_issues_with_originator_company_name.png](assets/custom-view-for-issues-350x33.png)

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

## Visa problem med företagsnamnet för upphovspersonen

Så här använder du den här vyn:

1. Gå till en lista med problem.
1. Från **Visa** nedrullningsbar meny, välja **Ny vy**.

1. I **Förhandsgranska kolumn** -område, ta bort alla kolumner utom en.
1. Klicka på rubriken för den återstående kolumnen och klicka sedan på **Växla till textläge**.
1. För musen över textlägesområdet och klicka **Klicka för att redigera text**.
1. Ta bort den text du hittar i **Textläge** och ersätt den med följande kod:
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=val<br>column.0.link.lookup=link.view<br>column.0.link.value=val(objCode)<br>column.0.listsort=string(name)<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=140<br>column.1.descriptionkey=originator<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=ownerID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.valuefield=owner:objCode<br>column.1.link.valueFormat=val<br>column.1.listsort=nested(owner).string(name)<br>column.1.namekey=originator.abbr<br>column.1.querysort=owner:name<br>column.1.valuefield=owner:name<br>column.1.valueformat=HTML<br>column.1.width=151<br>column.2.descriptionkey=entrydate<br>column.2.listsort=atDateAsAtDate(entryDate)<br>column.2.namekey=entrydate.abbr<br>column.2.querysort=entryDate<br>column.2.valuefield=entryDate<br>column.2.valueformat=atDate<br>column.2.width=75<br>column.3.descriptionkey=age<br>column.3.listsort=doubleAsDouble(age)<br>column.3.namekey=age<br>column.3.querysort=age<br>column.3.valuefield=howOld<br>column.3.valueformat=val<br>column.3.width=80<br>column.4.viewalias=statusicons<br>column.4.displayName=Flags<br>column.4.linkedname=direct<br>column.4.namekey=statusicons<br>column.4.valuefield=<br>column.4.valueformat=HTML<br>column.4.querysort=<br>column.4.tile.name=component.issues.statusicons<br>column.4.tile.pdfcomponent=issueStatusIcons<br>column.4.delimiter=<br>column.4.tile.template=/WEB-INF/jsp/lists/components/issueStatusIcons.jsp<br>column.5.description=Originators företagsnamn<br>column.5.link.linkproperty.0.name=ID<br>column.5.link.linkproperty.0.valuefield=owner:companyID<br>column.5.link.linkproperty.0.valueformat=int<br>column.5.link.lookup=link.view<br>column.5.link.valueField=owner:company:objCode<br>column.5.link.valueFormat=val<br>column.5.listsort=nested(owner:company).string(name)<br>column.5.name=Originator Company<br>column.5.querysort=owner:company:name<br>column.5.valuefield=owner:company:name<br>column.5.valueformat=HTML<br>column.5.width=151</pre>

1. Klicka **Spara vy**.

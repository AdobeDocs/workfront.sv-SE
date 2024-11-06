---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: Problem med att lösa objektinformation'
description: I den här problemvyn visas namnet och procentandelen som är slutförd för problemlösningsobjektet, vilket gör att den som skapade problemet kan få insikt i hur problemet fortskrider, även utan åtkomst till lösningsaktiviteten eller -projektet.
author: Nolan
feature: Reports and Dashboards
exl-id: 7f4c923a-01e4-4896-9f54-1f0c66d64bb5
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Visa: problem med att lösa objektinformation

<!--Audited: 11/2024-->

I den här problemvyn visas namnet och procentandelen som är slutförd för problemlösningsobjektet, vilket gör att den som skapade problemet kan få insikt i hur problemet fortskrider, även utan åtkomst till lösningsaktiviteten eller -projektet.

I den här vyn används taggen `sharecol=true` för att kombinera flera fält under samma kolumnrubrik. Mer information om taggen `sharecol` finns i [Visa: sammanfoga information från flera kolumner i en delad kolumn](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

![issue_custom_view_with_resolving_object_name_and_percent_complete.png](assets/issue-custom-view-350x77.png)

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
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Nytt:<ul><li>Medarbetare som ändrar en vy</li><li>Standard för att ändra en rapport</li></ul></p><p>eller</p>Aktuell:<ul><li>Begäran om att ändra en vy</li><li>Planera att ändra en rapport</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra en vy</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visa problem med att lösa objektinformation

1. Gå till en lista med problem.
1. Välj **Ny vy** i listrutan **Visa**.

1. Ta bort alla kolumner utom en i området **Förhandsvisa kolumn**.
1. Klicka på rubriken för den återstående kolumnen, klicka på **Växla till textläge** och klicka sedan på **Redigera textläge**.
1. Ta bort den text du söker i rutan **Redigera textläge** och ersätt den med följande kod:

   ```
   column.0.querysort=name
   column.0.stretch=0
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.descriptionkey=sourceobject
   column.1.linkedname=direct
   column.1.listsort=nested(referenceObject).HTML(name)
   column.1.namekey=sourceobject.abbr
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=referenceObject:name
   column.1.valueformat=HTML
   column.1.viewalias=source
   column.1.width=100
   column.2.descriptionkey=assignedto
   column.2.link.linkproperty.0.name=ID
   column.2.link.linkproperty.0.valuefield=assignedTo:ID
   column.2.link.linkproperty.0.valueformat=int
   column.2.link.lookup=link.view
   column.2.link.valuefield=assignedTo:objCode
   column.2.link.valueformat=val
   column.2.linkedname=assignedTo
   column.2.listsort=nested(assignedTo).string(name)
   column.2.namekey=assignedto
   column.2.querysort=assignedTo:name
   column.2.shortview=false
   column.2.stretch=25
   column.2.valuefield=assignedTo:name
   column.2.valueformat=HTML
   column.2.width=150
   column.3.descriptionkey=entrydate
   column.3.linkedname=direct
   column.3.listsort=atDateAsAtDate(entryDate)
   column.3.namekey=entrydate.abbr
   column.3.querysort=entryDate
   column.3.shortview=false
   column.3.stretch=0
   column.3.valuefield=entryDate
   column.3.valueformat=atDate
   column.3.width=150
   column.4.descriptionkey=description
   column.4.linkedname=direct
   column.4.listsort=string(description)
   column.4.namekey=description.abbr
   column.4.querysort=description
   column.4.shortview=false
   column.4.stretch=75
   column.4.valuefield=description
   column.4.valueformat=HTML
   column.4.width=150
   column.5.descriptionkey=status
   column.5.enumclass=com.attask.common.constants.OpTaskStatusEnum
   column.5.linkedname=direct
   column.5.listsort=string(status)
   column.5.namekey=status.abbr
   column.5.querysort=status
   column.5.shortview=false
   column.5.stretch=0
   column.5.type=enum
   column.5.valuefield=status
   column.5.valueformat=val
   column.5.width=150
   column.6.displayname=Resolving Object Name
   column.6.linkedname=resolveTask
   column.6.namekey=view.relatedcolumn
   column.6.namekeyargkey.0=resolveTask
   column.6.namekeyargkey.1=name
   column.6.querysort=resolveTask:name
   column.6.sharecol=true
   column.6.textmode=true
   column.6.valuefield=resolveTask:name
   column.6.valueformat=HTML
   column.7.displayname=
   column.7.linkedname=resolveOpTask
   column.7.namekey=view.relatedcolumn
   column.7.namekeyargkey.0=resolveOpTask
   column.7.namekeyargkey.1=name
   column.7.querysort=resolveOpTask:name
   column.7.sharecol=true
   column.7.textmode=true
   column.7.valuefield=resolveOpTask:name
   column.7.valueformat=HTML
   column.8.displayname=
   column.8.linkedname=resolveProject
   column.8.namekey=view.relatedcolumn
   column.8.namekeyargkey.0=resolveProject
   column.8.namekeyargkey.1=name
   column.8.querysort=resolveProject:name
   column.8.textmode=true
   column.8.valuefield=resolveProject:name
   column.8.valueformat=HTML
   column.9.displayname=Resolving Object Percent Complete
   column.9.textmode=true
   column.9.valueexpression=IF(ISBLANK({resolveTask}.{ID}),{resolveProject}.{percentComplete},IF(ISBLANK({resolveProject}.{ID}),{resolveTask}.{percentComplete},''))
   column.9.valueformat=doubleAsPercentRounded
   ```

1. Klicka på **Klar** > **Spara vy**.
1. (Valfritt) Uppdatera vynamnet och klicka sedan på **Spara vy**.

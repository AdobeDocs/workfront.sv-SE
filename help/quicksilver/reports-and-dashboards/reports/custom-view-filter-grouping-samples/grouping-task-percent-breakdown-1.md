---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppering: Uppgiftsprocentuell uppdelning 1'
description: '''I den här anpassade projektgrupperingen kan du visa projekt grupperade efter ett intervall av deras procentvärden för slutförande. Uppdelningarna visar ett procentvärde på 25 procents ökning av poängen: 0-25 %, 25-50 % osv.'
author: Nolan
feature: Reports and Dashboards
exl-id: ddb9496c-9347-4dc9-a4ce-b9017abd0bb2
source-git-commit: a6874c3a2dfda02b8a25f78056767d8c59c888e9
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# Gruppering: aktivitetsprocentuell uppdelning 1

<!--Audited: 10/2024-->

I den här anpassade projektgrupperingen kan du visa projekt grupperade efter ett intervall av deras procentvärden för slutförande. Uppdelningarna visar ett procentvärde på 25 procentenheter i steg om 0-25 %, 25-50 % osv.

I följande gruppering ordnas uppgifter enligt värdet för Procent färdigt i sex olika grupperingar:

* 0 %
* 1-25 %
* 26-50 %
* 51-75 %
* 76-99 %
* 100 %

![task_25_break_grouping.png](assets/task-25--breakdown-grouping-350x412.png)

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

## Gruppera efter procentindelning för uppgift

Så här använder du den här grupperingen:

1. Gå till en lista med uppgifter.
1. Välj **Ny gruppering** i listrutan **Gruppering**.
1. Klicka på **Lägg till gruppering**.

1. Klicka på **Växla till textläge**.
1. Ta bort texten i området **Gruppera efter**.
1. Ersätt texten med följande kod:

   ```
   group.0.linkedname=direct
   group.0.name=Percent Breakdown
   group.0.notime=false
   group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}<=26,"0-25 %",IF({percentComplete}<=51,"26-50 %",IF({percentComplete}<=76,"51-75 %",IF({percentComplete}<100,"76-99 %","100 %")))))
   group.0.valueformat=string
   ```

1. Klicka på **Klar** > **Spara gruppering**.
1. (Valfritt) Uppdatera grupperingsnamnet och klicka sedan på **Spara gruppering**.

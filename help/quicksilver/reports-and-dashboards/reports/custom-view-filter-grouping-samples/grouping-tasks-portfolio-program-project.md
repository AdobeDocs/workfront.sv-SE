---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppering: Uppgifter efter Portfolio, Program och Projekt'
description: Använd den här uppgiftsgrupperingen för att gruppera uppgifter efter portföljen, efter program och sedan efter det projekt de är kopplade till.
author: Nolan
feature: Reports and Dashboards
exl-id: 8fdad6a1-54b3-4d3e-8f21-4f2efc2dc27a
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# Gruppering: uppgifter efter portfölj, program och projekt

<!--Audited: 10/2024-->

Använd den här uppgiftsgrupperingen för att gruppera uppgifter efter portföljen, efter program och sedan efter det projekt de är kopplade till.

![Projektgruppering för Portfolio](assets/portfolio-program-project-grouping-for-tasks-350x120.png)

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

## Gruppera uppgifter efter portfölj, program och projekt

Så här använder du den här grupperingen:

1. Gå till en lista med uppgifter.
1. Välj **Ny gruppering** i listrutan **Gruppering**.
1. Klicka på **Lägg till gruppering**.

1. Klicka på **Växla till textläge**.
1. Ta bort texten i området **Gruppera efter**.
1. Ersätt texten med följande kod:

   ```
   group.0.linkedname=project
   group.0.namekey=portfolio
   group.0.notime=false
   group.0.valuefield=project:portfolio:name
   group.0.valueformat=string
   group.1.linkedname=project
   group.1.namekey=program
   group.1.notime=false
   group.1.valuefield=project:program:name
   group.1.valueformat=string
   group.2.name=Project
   group.2.valuefield=project:name
   group.2.valueformat=HTML
   textmode=true
   ```

1. Klicka på **Klar** > **Spara gruppering**.
1. (Valfritt) Uppdatera grupperingsnamnet och klicka sedan på **Spara gruppering**.


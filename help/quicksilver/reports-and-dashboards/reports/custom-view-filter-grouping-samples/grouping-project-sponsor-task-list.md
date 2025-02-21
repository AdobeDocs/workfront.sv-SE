---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppering: Projektsponsor för en uppgiftslista'
description: Med den här uppgiftsgrupperingen kan du gruppera uppgifter efter projektsponsorn.
author: Nolan
feature: Reports and Dashboards
exl-id: 2d8f85ea-492e-4b08-82f5-726170acc7d5
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---

# Gruppering: Projektsponsor för en uppgiftslista

<!--Audited: 11/2024-->

Med den här uppgiftsgrupperingen kan du gruppera uppgifter efter projektsponsorn.

![Gruppera efter projektsponsor](assets/grouping--project-sponsor-for-a-task-350x189.png)

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

## Gruppera efter projektsponsorer för en uppgiftslista


Så här använder du den här grupperingen:

1. Gå till en lista med uppgifter.
1. Välj **Ny gruppering** i listrutan **Gruppering**.

1. Klicka på **Växla till textläge**.
1. Ta bort texten i området som visas och ersätt den med följande kod:

   ```
   group.0.name=Project Sponsor
   group.0.valuefield=project:sponsor:name
   group.0.valueformat=string
   ```

1. Klicka på **Klar**.
1. Uppdatera grupperingsnamnet och klicka sedan på **Spara gruppering**.


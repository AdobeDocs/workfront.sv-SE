---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppering: Projektsponsor för en uppgiftslista'
description: Med den här uppgiftsgrupperingen kan du gruppera uppgifter efter projektsponsorn.
author: Courtney
feature: Reports and Dashboards
exl-id: 2d8f85ea-492e-4b08-82f5-726170acc7d5
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---

# Gruppering: Projektsponsor för en uppgiftslista

<!--Audited: 11/2024-->

Med den här uppgiftsgrupperingen kan du gruppera uppgifter efter projektsponsorn.

![Gruppera efter projektsponsor](assets/grouping--project-sponsor-for-a-task-350x189.png)

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> 
   <p>Medarbetare eller begäran om att ändra ett filter </p>
   <p>Standard eller Plan för att ändra en rapport</p>
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

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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


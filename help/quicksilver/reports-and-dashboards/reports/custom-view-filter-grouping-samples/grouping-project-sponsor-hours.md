---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppering: Projektsponsorer för timmar'
description: Den här timgrupperingen organiserar timmar av sponsorn för projektet där timmarna är loggade. Standardgränssnittet för Report Builder för timgrupperingar innehåller ingen mappning till fältet Project Sponsor. Du måste använda gränssnittet Textläge för att komma åt det här fältet.
author: Nolan
feature: Reports and Dashboards
exl-id: 6b35b0ef-18b7-4121-ae39-d7957d76c04b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Gruppering: Projektsponsorer i timmar

<!--Audited: 10/2024-->

Den här timgrupperingen organiserar timmar av sponsorn för projektet där timmarna är loggade. Standardgränssnittet för Report Builder för timgrupperingar innehåller ingen mappning till fältet Project Sponsor. Du måste använda gränssnittet Textläge för att komma åt det här fältet.

![hour_report_grouped_by_sponor.png](assets/hour-report-grouped-by-sponsor-350x39.png)

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

## Gruppera efter projektsponsorer i timmar

Så här använder du den här grupperingen:

1. Gå till en lista med timmar.
1. Välj **Ny gruppering** i listrutan **Gruppering**.

1. Klicka på **Växla till textläge**.
1. Ta bort texten i området som visas och ersätt den med följande kod:

```
   group.0.linkedname=project:sponsor:name
   group.0.name=
   group.0.valuefield=project:sponsor:name
   group.0.valueformat=HTML
   textmode=true
```

1. Klicka på **Klar**.
1. Uppdatera grupperingsnamnet och klicka sedan på **Spara gruppering**.

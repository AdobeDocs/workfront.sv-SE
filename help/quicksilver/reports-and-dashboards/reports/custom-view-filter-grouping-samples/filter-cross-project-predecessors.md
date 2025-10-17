---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: visa ofullständiga föregångare mellan projekt'
description: Aktivitetsfiltret returnerar ofullständiga föregångare mellan projekt.
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: 7ee2432c-1d82-454e-a73a-f1f6b6a5c10d
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---

# Filter: visa ofullständiga föregångare mellan projekt

<!--Audited: 10/2024-->

Aktivitetsfiltret returnerar ofullständiga föregångare mellan projekt.

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

## Filtrera föregångare mellan projekt

Så här använder du det här filtret:

1. Gå till en lista med uppgifter eller en uppgiftsrapport.
1. Välj **Nytt filter** i listrutan **Filter**.

1. (Villkorligt) Klicka på **Textläge** om du använde filtret från en lista eller på **Växla till textläge** om du använde filtret från en rapport.
1. Klistra in följande kod i det nya området:
   <pre>predecessorsMM:projectID=FIELD:projectID<br>predecessorsMM:projectID_Mod=ne<br>percentComplete=100<br>percentComplete_Mod=ne</pre>

1. (Villkorligt) Klicka på **Spara filter** om du har öppnat filtret från en rapport eller **Använd** och sedan **Spara som nytt** om du har öppnat filtret från en uppgiftslista.

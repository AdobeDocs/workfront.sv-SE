---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: visa ofullständiga projektövergripande efterföljande'
description: Aktivitetsfiltret returnerar ofullständiga projektövergripande efterföljande.
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: aea955b1-581a-4ce0-8634-863ba1083c05
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '151'
ht-degree: 0%

---

# Filter: visa ofullständiga projektövergripande efterföljande

Aktivitetsfiltret returnerar ofullständiga projektövergripande efterföljande.

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

## Filtrera efterföljande projekt

Så här använder du det här filtret:

1. Gå till en lista med uppgifter.
1. Välj **Nytt filter** i listrutan **Filter**.

1. Klicka på **Textläge**.
1. Klistra in följande kod i det område som visas:
   <pre>percentComplete=100<br>percentComplete_Mod=ne<br>efterföljandeMM:projectID=FIELD:projectID<br>efterföljandeMM:projectID_Mod=ne</pre>

1. Klicka på **Använd** > **Spara som ny**.

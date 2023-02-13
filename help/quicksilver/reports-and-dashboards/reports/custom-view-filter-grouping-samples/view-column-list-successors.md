---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: lägg till en lista med efterföljande aktiviteter i en kolumn'
description: Du kan lägga till en kolumn i en uppgiftsvy för att visa en lista över de efterföljande uppgifterna. Kolumnen Uppgiftens efterföljare innehåller både numret på efterträdaren och namnet.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Visa: lägga till en lista med efterföljande aktiviteter i en kolumn

Du kan lägga till en kolumn i en uppgiftsvy för att visa en lista över de efterföljande uppgifterna. The **Uppgiftsefterföljande aktiviteter** -kolumnen innehåller både numret på den efterföljande parten och namnet.

![task_view_with_a_list_of_Succors_.png](assets/task-view-with-a-list-of-successors--350x118.png)

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Lägga till en lista med efterföljande aktiviteter i en kolumn

Så här lägger du till den här kolumnen i en uppgiftsvy:

1. Gå till en befintlig uppgiftsvy.
1. Expandera listrutan Visa och välj **Anpassa vy**.
1. Klicka **Lägg till kolumn**.
1. Klicka **Växla till textläge**.
1. För musen över **Visa i den här kolumnen** och klicka **Klicka för att redigera text**.

1. Ta bort all text i rutan Textläge och ersätt den med följande kod:

   <pre>displayName=Uppgiftsövare<br>listdelimiter=<br><br>listmethod=nested(Succors).lists<br>textmode=true<br>type=iterate<br>valueExpression=CONCAT({Succor}).{taskNumber}, -,{Succor}.{name})<br>valueFormat=HTML</pre>

1. Klicka **Spara vy**.

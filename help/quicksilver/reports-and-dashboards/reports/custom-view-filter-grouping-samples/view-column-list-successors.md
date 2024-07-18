---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: lägg till en lista med efterföljande aktiviteter i en kolumn'
description: Du kan lägga till en kolumn i en uppgiftsvy för att visa en lista över de efterföljande uppgifterna. Kolumnen Uppgiftens efterföljare innehåller både numret på efterträdaren och namnet.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Visa: lägg till en lista med efterföljande aktiviteter i en kolumn

Du kan lägga till en kolumn i en uppgiftsvy för att visa en lista över de efterföljande uppgifterna. Kolumnen **Uppgiftens efterföljare** innehåller både antalet efterföljare och namnet.

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
   <td> <p>Begäran om att ändra en vy </p>
   <p>Planera att ändra en rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra en vy</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
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
1. Klicka på **Lägg till kolumn**.
1. Klicka på **Växla till textläge**.
1. För musen över **Visa i den här kolumnen** och klicka på **Klicka för att redigera text**.

1. Ta bort all text i rutan Textläge och ersätt den med följande kod:
   <pre>displayname=Task Successors<br>listdelimiter=<br><br>listmethod=nested(Successors).lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({successor}).{taskNumber}, - {successor}.{name})<br>värdeformat=HTML</pre>

1. Klicka på **Spara vy**.

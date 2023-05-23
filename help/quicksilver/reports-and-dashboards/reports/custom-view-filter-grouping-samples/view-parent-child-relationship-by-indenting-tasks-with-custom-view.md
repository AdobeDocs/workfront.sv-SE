---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: visa relationen överordnad-underordnad i en uppgift genom att dra in aktivitetens'
description: Du kan behålla skillnaden mellan överordnade och underordnade relationer i en exporterad uppgiftslista genom att lägga till en anpassad vy i uppgiftslistan och se till att den här vyn är markerad innan du exporterar listan.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# Visa: visa relationen överordnad-underordnad i en uppgift genom att dra in uppgifterna

Du kan behålla skillnaden mellan överordnade och underordnade relationer i en exporterad uppgiftslista genom att lägga till en anpassad vy i uppgiftslistan och se till att den här vyn är markerad innan du exporterar listan.

![](assets/parent-child-indented-custom-view-350x94.png)

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

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Visa relationen överordnad-underordnad i en uppgift genom att dra in uppgifterna

1. Gå till projektet med uppgiftslistan som du vill exportera.
1. Klicka på **Visa** nedrullningsbar meny och välj **Ny vy**.

1. Namnge filtret i skärmens övre vänstra hörn.
1. Klicka på **Aktivitetsnamn** kolumnrubrik.

1. Välj **Växla till textläge** i det övre högra hörnet.
1. Klicka någonstans i textrutan för att redigera text och ta bort all befintlig text.
1. Klistra in följande text:

   ```
   displayname=<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br>valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))<br>valueformat=HTML
   ```

1. Klicka **Spara**.
1. Klicka **Spara vy**.

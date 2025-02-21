---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: Visa den överordnade-underordnade relationen i en uppgift genom att dra in uppgifterna'
description: Du kan behålla skillnaden mellan överordnade och underordnade relationer i en exporterad uppgiftslista genom att lägga till en anpassad vy i uppgiftslistan och se till att den här vyn är markerad innan du exporterar listan.
author: Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Visa: visa relationen överordnad-underordnad i en uppgift genom att dra in uppgifterna

<!--Audited: 11/2024-->

Du kan behålla skillnaden mellan överordnade och underordnade relationer i en exporterad uppgiftslista genom att lägga till en anpassad vy i uppgiftslistan och se till att den här vyn är markerad innan du exporterar listan.

![Indrag för överordnad underordnad](assets/parent-child-indented-custom-view-350x94.png)

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
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p> Aktuell: 
   <ul>
   <li>Begäran om att ändra en vy</li> 
   <li>Planera att ändra en rapport</li>
   </ul>
     </p>
     <p> Nytt: 
   <ul>
   <li>Medarbetare som ändrar en vy</li> 
   <li>Standard för att ändra en rapport</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra en vy</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visa relationen överordnad-underordnad i en uppgift genom att dra in uppgifterna

1. Gå till projektet med uppgiftslistan som du vill exportera.
1. Klicka på listrutan **Visa** och välj **Ny vy**.
1. Klicka i kolumnrubriken **Aktivitetsnamn**.
1. Välj **Växla till textläge** i det övre högra hörnet.
1. Klicka på **Redigera textläge** och ta bort all befintlig text.
1. Klistra in följande text:


   ```
   displayname=
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))
   valueformat=HTML
   ```

1. Klicka på **Klar** > **Spara vy**.

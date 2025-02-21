---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: Visa aktivitetsindrag i en uppgiftslista'
description: I den här uppgiftsvyn kan du lägga till kod i kolumnen Uppgiftsnamn om du vill visa uppgifter som är indragna enligt projektets arbetsgruppsstruktur.
author: Nolan
feature: Reports and Dashboards
exl-id: f7f43e1e-db32-48b8-9a23-ff9fa6195386
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# Visa: visa indrag för uppgifter i en uppgiftslista

<!--Audited: 11/2024-->

I den här uppgiftsvyn kan du lägga till kod i kolumnen Uppgiftsnamn om du vill visa uppgifter som är indragna enligt projektets arbetsgruppsstruktur.

![Visa aktivitetsindrag](assets/view-text-mode-indentation-task-list-350x171.png)

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

## Visa indrag för aktiviteter i en kolumn i en uppgiftslista

1. Gå till en lista med uppgifter.
1. Klicka på **Ny vy** i listrutan **Visa**.

1. Klicka på **Lägg till kolumn** och börja skriva &quot;Aktivitetsnamn&quot; i fältet **Visa i den här kolumnen** och markera den när den visas i listan.

1. Klicka på **Växla till textläge** > **Redigera textläge** i den nya kolumnen.
1. Ta bort texten som du hittar på raden `valuefield=` och ersätt den med följande kod:

   ```
   displayname=Task hierarchy
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(' - ',{name}),IF({indent}<3,CONCAT(' - - ',{name}),IF({indent}<4,CONCAT(' - - - ',{name}),CONCAT(' - - - - ',{name})))))
   ```

1. Klicka på **Klar** och sedan på **Spara vy**.
1. (Valfritt) Uppdatera vynamnet och klicka sedan på **Spara vy**.

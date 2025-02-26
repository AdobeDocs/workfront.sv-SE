---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: Dölj innehållet i en kolumn'
description: Du kanske vill dölja information i kolumnen för en vy. Du kan göra detta genom att ändra kolumnens textläge.
author: Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: e8acdf8f7b3859385237e788dfda34ee62ee11d1
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# Visa: dölj innehållet i en kolumn

<!--Audited: 11/2024-->

Du kanske vill dölja information i kolumnen för en vy. Du kan göra detta genom att ändra kolumnens textläge.

>[!NOTE]
>
>* Du kan använda dolda kolumner för att sortera efter ett visst objekt som du inte vill visa i vyn.\
>  Du kan till exempel sortera efter Uppgiftsnummer i en uppgiftsvy och dölja informationen om Uppgiftsnummer i vyn. I det här fallet kan objektet som refereras i kolumnen sortera vyn, men informationen om objektet visas inte i vyn.
>* När du döljer en kolumn bör du tänka på att informationen i kolumnen är dold, men kolumnen finns fortfarande i vyn.

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
   <td> <p>Nytt:<ul><li>Medarbetare som ändrar en vy</li><li>Standard för att ändra en rapport</li></ul></p><p>Aktuell:<ul><li>Begäran om att ändra en vy</li><li>Planera att ändra en rapport</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
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

## Exempel: Sortera och dölja kolumnen Aktivitetsnummer i en uppgiftsvy:

1. Gå till en lista med uppgifter.
1. Klicka på **Ny vy** i listrutan **Visa**.

1. Klicka på **Lägg till kolumn** och börja skriva &quot;Aktivitetsnummer&quot; i fältet **Visa i den här kolumnen** och markera den när den visas i listan.

1. Klicka på **Växla till textläge** och sedan på **Redigera textläge**.
1. Ta bort den text du söker i rutan **Redigera textläge** och ersätt den med följande kod:

   ```
   displayname=
   linkedname=direct
   querysort=taskNumber
   sortOrder=1
   sortType=asc
   textmode=true
   value=
   valueformat=int
   width=0
   ```

   De viktiga ändringarna i koden som gör kolumnen dold är:

   * `displayname=`: Den här raden måste vara tom.
   * `valuefield=`: Den här raden måste ersättas med `value=`, som måste vara tom.
   * `width=`: Beroende på fältet måste värdet vara **0** eller **1**.

1. Klicka på **Klar** och sedan på **Spara vy**.

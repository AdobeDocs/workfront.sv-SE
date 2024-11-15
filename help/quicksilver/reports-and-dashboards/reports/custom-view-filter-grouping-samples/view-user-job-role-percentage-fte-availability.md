---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: Procent av användarjobbroll för FTE-tillgänglighet'
description: Du kan lägga till en kolumn i vyn över en användarlista för att visa en lista över de jobbroller användaren är kopplad till samt procentandelen FTE-tillgänglighet för varje jobbroll, enligt definitionen i användarprofilen.
author: Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 66de6c952272f52876f8e912c96d1526575b6f0b
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# Visa: användarroll i procent av FTE-tillgänglighet

<!--Audited: 11/2024-->

Du kan lägga till en kolumn i vyn över en användarlista för att visa en lista över de jobbroller användaren är kopplad till samt procentandelen FTE-tillgänglighet för varje jobbroll, enligt definitionen i användarprofilen.

Mer information om hur du definierar procentandelen FTE-tillgänglighet för användare finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

![user_with_percent_avialbility_per_role.png](assets/user-with-percent-avialbility-per-role-350x138.png)

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

## Visa användarjobbrollens procentandel av FTE-tillgänglighet

1. Gå till en lista med användare.
1. Välj **Ny vy** i listrutan **Visa**.

1. Klicka på **Lägg till kolumn** i området **Förhandsvisa kolumn**.

1. Klicka på den nya kolumnens rubrik och klicka sedan på **Växla till textläge** > **Redigera textläge**.
1. Ta bort den text du söker i rutan **Redigera textläge** och ersätt den med följande kod:

   ```
   displayname=Roles Time Percentage
   listdelimiter=
   listmethod=nested(userRoles).lists
   textmode=true
   type=iterate
   valueexpression=CONCAT({role},'-',{timePercentage},'%')
   valueformat=HTML
   ```

1. Klicka på **Klar** och sedan på **Spara vy**.

1. (Valfritt) Uppdatera vynamnet och klicka sedan på **Spara vy**.

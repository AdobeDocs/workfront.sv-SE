---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: Ta bort länk till ett objekt i en kolumn'
description: Vissa objekt som du visar i en vy länkar till objektets detaljsida som standard. Kolumnen som visar namnet på ett projekt är till exempel en länk till projektet. Kolumnen som visar namnet på en användare är en länk till användarens profilsida.
author: Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 17a277a5a63a521ec7285e3f5051bfd42fc204bf
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Visa: ta bort länk till ett objekt i en kolumn

<!--Audited: 11/2024-->

Vissa objekt som du visar i en vy länkar till objektets detaljsida som standard. Kolumnen som visar namnet på ett projekt är till exempel en länk till projektet. Kolumnen som visar namnet på en användare är en länk till användarens profilsida.

Du kan ta bort den här länken i textläge i kolumner som visas i alla vyer.

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


## Exempel: Ta bort länken till en aktivitet från kolumnen Uppgiftsnamn i en uppgiftsvy:

1. Gå till en lista med uppgifter.
1. Klicka på **Ny vy** i listrutan **Visa** för att skapa en ny vy.

   eller

   Klicka på ikonen **Redigera** ![](assets/edit-icon.png)

   Om du vill redigera en befintlig vy markerar du vyn.

1. Klicka på **Lägg till kolumn** för att lägga till en ny kolumn.

   eller

   Klicka på en befintlig kolumn med en länk till ett objekt.

1. Klicka på **Växla till textläge** > **Redigera textläge**.
1. Ta bort den text du söker i rutan **Redigera textläge** och ersätt den med följande kod:

   ```
   displayname=Task Name
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression={name}
   valueformat=Compound
   ```

   >[!TIP]
   >
   >Du kan använda liknande kod för andra objekt genom att justera följande:
   >
   >* Ersätt `valuefield`-raden i koden med `valueexpression` och behåll samma namn inom klammerparenteser efter likhetstecknet.
   >* Ta bort alla rader som börjar med `link.` från den ursprungliga texten i kolumnen. Ta till exempel bort alla följande rader:
   >
   >  ```
   >  link.linkproperty.0.name=ID
   >  link.linkproperty.0.valuefield=ID
   >  link.linkproperty.0.valueformat=string
   >  link.lookup=link.view
   >  link.value=val(objCode)
   >  ```
   >

1. Klicka på **Klar** och sedan på **Spara vy**.


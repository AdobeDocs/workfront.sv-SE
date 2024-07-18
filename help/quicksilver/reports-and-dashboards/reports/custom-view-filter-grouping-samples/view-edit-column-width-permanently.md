---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: redigera bredden på en kolumn permanent'
description: Du kan tillfälligt ändra kolumnbredden genom att dra och släppa marginalerna så att de matchar den önskade bredden. Mer information finns i Ändra kolumnbredd och -ordning.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# Visa: redigera bredden på en kolumn permanent

<!-- Audited: 1/2024 -->

Du kan tillfälligt ändra kolumnbredden genom att dra och släppa marginalerna så att de matchar den önskade bredden. Mer information finns i [Ändra kolumnbredd och ordning](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Om du vill ändra bredden på en kolumn i en vy permanent måste du använda textläget i kolumnen när du redigerar vyn.

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
   <td> <p>Nytt:<ul><li>Medarbetare som ändrar en vy</li><li>Standard för att ändra en rapport</li></ul></p><p>eller</p>Aktuell:<ul><li>Begäran om att ändra en vy</li><li>Planera att ändra en rapport</li></ul></p> </td> 
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

## Redigera bredden på en kolumn permanent

>[!IMPORTANT]
>
>Om du ändrar bredden på en kolumn manuellt enligt beskrivningen i avsnittet [Ändra bredden och ordningen på kolumner tillfälligt](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md#modify-width-and-order-of-columns-temporarily) i artikeln [Ändra kolumnbredden och ordningen](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) när du har ändrat bredden på kolumnen permanent, bevaras bredden på kolumnen enligt den manuella storleksändringen. I det här fallet skrivs bredden på kolumnen som uppdateras enligt följande steg över. Du kan visa kolumnen enligt den bredd som definieras i följande steg när du har rensat cachen eller loggat in från en annan webbläsare.
>
>Mer information om hur du anpassar bredden på kolumner när du använder gränssnittet för textläge finns i definitionerna för bredd och sträckning i [ordlistan för Adobe Workfront-terminologi](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. Gå till en lista med objekt.
1. Klicka på **Ny vy** i listrutan **Visa**.

1. Klicka på **Lägg till kolumn** för att lägga till en ny kolumn.

   eller

   Klicka på kolumnrubriken för en befintlig kolumn.

1. Klicka på **Växla till textläge**.
1. Hovra över textlägesområdet och klicka på **Klicka för att redigera text**.
1. Lägg till följande kod i textläget för kolumnen:

   ```
   width=200
   usewidths=true
   ```

   För raden **width** anger du ett tal (i pixlar) som representerar hur bred du vill att kolumnen ska visas i vyn.

1. Klicka på **Spara** och sedan på **Spara vy**.



---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: visa resultatet av en beräkning mellan två fält i en kolumn'
description: Du kan använda textläge i en kolumn för att visa en beräkning mellan två fält.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Visa: visa resultatet av en beräkning mellan två fält i en kolumn

<!--Audited: 11/2024-->

Du kan använda textläge i en kolumn för att visa en beräkning mellan två fält.

Om du t.ex. vill ta reda på antalet veckodagar som förflutit mellan två datum kan du använda textlägessyntax och datauttryck för att beräkna skillnaden.\
Du kan till exempel beräkna skillnaden mellan det planerade slutförandedatumet och det faktiska slutförandedatumet för en aktivitet och visa resultatet i en kolumn.

Du kan använda två andra datum i den här beräkningen (Faktisk start, Faktisk slutförning, Projicerad start, Projicerad slutförning osv.).\
Mer information om beräknade datauttryck finns i [Översikt över beräknade datauttryck](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

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


## Visa resultatet av en beräkning mellan två fält i en kolumn

Så här lägger du till den här kolumnen i en uppgiftsvy:

1. Gå till en lista med uppgifter.
1. Klicka på **Ny vy** i listrutan **Visa**.

1. Klicka på **Lägg till kolumn** och sedan på **Växla till textläge** > **Redigera textläge**.
1. Ta bort texten som du söker i rutan **Textläge** och ersätt den med följande kod:

   ```
   displayname=Week Day Difference
   textmode=true
   valueexpression=WEEKDAYDIFF({plannedCompletionDate},{actualCompletionDate})
   valueformat=HTML
   ```

1. (Valfritt) Om du vill samla de värden som visas i vyn i en gruppering följer du stegen som beskrivs i [Gruppera: visa resultatet av att samla flera beräknade värden i en gruppering](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. Klicka på **Klar** och sedan på **Spara vy**.

---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: visa resultatet av en beräkning mellan två fält i en kolumn'
description: Du kan använda textläge i en kolumn för att visa en beräkning mellan två fält.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# Visa: visa resultatet av en beräkning mellan två fält i en kolumn

Du kan använda textläge i en kolumn för att visa en beräkning mellan två fält.

Om du t.ex. vill ta reda på antalet veckodagar som förflutit mellan två datum kan du använda textlägessyntax och datauttryck för att beräkna skillnaden.\
Du kan till exempel beräkna skillnaden mellan det planerade slutförandedatumet och det faktiska slutförandedatumet för en aktivitet och visa resultatet i en kolumn.

Du kan använda två andra datum i den här beräkningen (Faktisk start, Faktisk slutförning, Projicerad start, Projicerad slutförning osv.).\
Mer information om beräknade datauttryck finns i [Beräknade datauttryck](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

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

## Visa resultatet av en beräkning mellan två fält i en kolumn

Så här lägger du till den här kolumnen i en uppgiftsvy:

1. Gå till en lista med uppgifter.
1. Från **Visa** nedrullningsbar meny, klicka **Ny vy**.

1. Klicka **Lägg till kolumn** sedan **Växla till textläge**.

1. Håll muspekaren över textlägesområdet och klicka **Klicka för att redigera text**.
1. Ta bort den text du hittar i **Textläge** och ersätt den med följande kod:
   <pre>displayName=Week Day Difference<br>textmode=true<br>valueExpression=WEEKDAYDIFF({planningCompletionDate},{actualCompletionDate})<br>valueFormat=HTML</pre>

1. (Valfritt) Följ stegen som beskrivs i [Gruppering: visa resultatet av att aggregera flera beräknade värden i en gruppering](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. Klicka **Spara** sedan **Spara vy**.

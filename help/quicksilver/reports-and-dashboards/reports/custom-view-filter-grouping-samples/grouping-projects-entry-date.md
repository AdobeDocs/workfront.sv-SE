---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Gruppering: projekt efter anmälningsdatum'
description: I den här anpassade projektgrupperingen kan du visa projekt grupperade efter deras värden för anmälningsdatum.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 511faad5-b5bd-4e2d-8daa-3fcde49a502c
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 0%

---

# Gruppering: projekt efter anmälningsdatum

I den här anpassade projektgrupperingen kan du visa projekt grupperade efter deras värden för anmälningsdatum.

Varje gruppering visar projekt med ett anmälningsdatum inom:

* De senaste 30 dagarna
* 30-60 dagar
* 60 dagar eller äldre

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

## Gruppera projekt efter anmälningsdatum

Så här använder du den här grupperingen:

1. Gå till en befintlig projektrapport eller skapa en ny projektrapport.\
   Mer information om hur du skapar en rapport finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Från **Gruppering** flik, klicka **Lägg till gruppering**.

1. Klicka **Växla till textläge**.
1. Ta bort texten i **Gruppera din rapport** område.
1. Ersätt texten med följande kod:

   ```
   group.0.linkedname=direct<br>
   ```

   ```
   group.0.name=Project Entry<br>
   ```

   ```
   group.0.valueexpression=IF(ABS(DATEDIFF({entryDate},$$TODAY))<=30,"Last 30 Days",IF(ABS(DATEDIFF({entryDate},$$TODAY))>30&&ABS(DATEDIFF({entryDate},$$TODAY))<=60,"30-60 Days","Older than 60 days"))<br>
   ```

   ```
   group.0.valueformat=atDateAsMonthString<br>
   ```

   ```
   textmode=true
   ```

1. Klicka **Spara + Stäng**.

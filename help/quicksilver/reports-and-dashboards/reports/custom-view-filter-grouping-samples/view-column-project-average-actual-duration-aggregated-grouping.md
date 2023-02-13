---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa och gruppera: visa projektets faktiska varaktighet aggregerat med genomsnittet i en gruppering'
description: Du kan lägga till följande kolumn i en projektrapport om du vill visa den faktiska varaktigheten som ett genomsnitt i en gruppering.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Visa och gruppera: visa projekt, faktisk varaktighet aggregerat med medelvärdet i en gruppering

Du kan lägga till följande kolumn i en projektrapport om du vill visa den faktiska varaktigheten som ett genomsnitt i en gruppering.

![project_with_aggregate_actual_duration_in_grouping_view.png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

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

## Visa projektets faktiska varaktighet aggregerad av medelvärdet i en gruppering

Så här lägger du till den här kolumnen i en projektvy:

1. (Rekommenderas) För bästa resultat och för att se det aggregerade genomsnittliga värdet för Faktisk varaktighet måste du lägga till en gruppering i projektlistan eller -rapporten.\
   Mer information om hur du skapar grupperingar finns i artikeln [Översikt över grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Gå till en befintlig projektvy.
1. Expandera listrutan Visa och välj **Anpassa vy**.
1. Klicka **Lägg till kolumn**.
1. Klicka **Växla till textläge**.
1. För musen över **Visa i den här kolumnen** och klicka **Klicka för att redigera text**.

1. Ta bort all text i rutan Textläge och ersätt den med följande kod:

   <pre>aggregator.displayformat=compound <br>aggregator.function=AVG <br>aggregator.namekey=view.relatedcolumn <br>aggregator.namekeyargkey=actualDuration <br>aggregator.valueField=actualDurationMinutes <br>aggregator.valueFormat=val <br>displayName=Project Actual Duration <br>durationunitfield=durationUnit.value <br>linkedname=project <br>namekey=actualDuration <br>namekeyargkey=actualDuration <br>querysort=actualDurationMinutes <br>textmode=true <br>valueField=actualDurationMinutes <br>valueFormat=compound#M:D <br>viewalias=actualDuration</pre>

1. Klicka **Spara vy**.

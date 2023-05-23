---
content-type: reference
product-area: reporting;projects
keywords: beräknad,aggregat,avancerad,vyer
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Gruppering: visa resultatet av sammanställningen av flera beräknade värden i en gruppering'
description: Du kan använda textläge i en kolumn för att visa en beräkning mellan två fält i vyn för en rapport eller lista. Varje rad visar beräkningen för varje objekt i rapporten eller listan.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# Gruppering: visa resultatet av att aggregera flera beräknade värden i en gruppering

Du kan använda textläge i en kolumn för att visa en beräkning mellan två fält i vyn för en rapport eller lista. Varje rad visar beräkningen för varje objekt i rapporten eller listan.

Du kan till exempel visa skillnaden mellan faktiska timmar och Planerade timmar i en tredje kolumn som heter Arbetsbalans för varje uppgift i en uppgiftsrapport. Mer information om beräknade datauttryck finns i [Beräknade datauttryck](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Du kan visa det aggregerade värdet för flera objekt i den beräknade vyn i samma kolumn i en grupp genom att lägga till en beräkning i `aggregator` rad i kolumnen som innehåller det beräknade värdet. Du kan t.ex. aggregera (visa summan av) antalet timmar i Arbetsbalans för alla uppgifter i grupperingen av rapporten eller listan för kolumnen Arbetsbalans. I den här artikeln beskrivs hur du gör detta.

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
   <td> <p>Begäran om att ändra en gruppering </p>
   <p>Planera att ändra en rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra en gruppering</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Visa resultatet av sammanställning av flera beräknade värden i en gruppering

1. Gå till en uppgiftsrapport, klicka på **Rapportåtgärder** > **Redigera**.
1. I **Grupperingar** flik, klicka **Lägg till gruppering** och börja skriva **Projektnamn** i **Gruppera din rapport** > **Först efter** markerar du det när det visas i listan.

1. I **Kolumner (vy)** flik, klicka **Lägg till kolumn** börjar sedan skriva **Planerade timmar** i **Visa i den här kolumnen** markerar du det när det visas i listan.

   >[!TIP]
   >
   >Börja alltid lägga till så mycket information som du vill i standardgränssnittet innan du redigerar information i textläge. Lägg till fält som är närmast eller innehåller så mycket information som möjligt för beräkningen som du försöker göra.

1. I **Sammanfatta den här kolumnen med** fält, markera **Summa** och sedan klicka **Klar**.
1. Klicka **Växla till textläge** i den kolumn som du lade till.
1. Håll muspekaren över textlägesområdet och klicka **Klicka för att redigera text**.
1. Ersätt `valuefield ` och `aggregator.valuefield` rader med linjerna markerade i följande exempel på textläge:

   ```
   valueformat=compound
   aggregator.displayformat=minutesAsHoursString
   aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2)
   aggregator.function=SUM
   aggregator.valueformat=val
   aggregator.namekey=workrequired
   linkedname=direct
   textmode=true
   valuefield=workRequired
   namekey=workrequired
   valueexpression=CONCAT(ROUND(({workRequired}-{actualWorkRequired})/60,2)," Hours") 
   viewalias=workrequired 
   displayname=Work Balance
   ```

   >[!TIP]
   >
   >För att få det aggregerade värdet i grupperingen för att visa den aggregerade skillnaden mellan fälten Planerade timmar och Faktiska timmar anger du samma ekvation i `aggregator.valuefield` linje. The `aggregator.displayformat` som används för kolumnen Planerade timmar konverterar minuter till timmar. Eftersom fältet Planerade timmar användes som platshållare behöver den här raden inte justeras.
   >
   >
   >The `minutesAsHoursString` definition av `aggregator.displayformat` betyder att du inte behöver dela upp varje fält med 60 som på `valueexpression` för resultaten. I den här `aggregator.valuefield=workRequired` blir: `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`.

1. Klicka **Spara+stäng**.

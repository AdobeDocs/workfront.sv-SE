---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: visningsobjekt som inte ingår i standardgränssnittet'
description: Du kan visa objekt som inte ingår i standardlägesgränssnittet i en vy. Du kan bara göra detta genom att referera till dem via textläge. Du kan bestämma vilka fält som kan inkluderas i en vy på något av följande sätt - REDIGERA ME.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# Visa: visningsobjekt som inte ingår i standardgränssnittet

Du kan visa objekt som inte ingår i standardlägesgränssnittet i en vy. Du kan bara göra detta genom att referera till dem via textläge.\
Du kan bestämma vilka fält som kan inkluderas i en vy på något av följande sätt:

* Använd [API Explorer](../../../wf-api/general/api-explorer.md) för att identifiera andra objekt som kan refereras via textläge.\
   Alla fält som finns dokumenterade i API Explorer är inte giltiga för textläge. Vissa fält kan bara rapporteras via API:t.

* Hitta objektets ID-fält i en kolumn. De flesta objekt som har ett fält-ID har också ett motsvarande kolumn- eller fältnamn som kanske inte är tillgängligt via standardlägesgränssnittet.

   Du kan använda textläge för att inkludera kolumn- eller fältnamnet i en vy i stället för ID:t genom att ersätta `fieldnameID` med `fieldname:name`.

   I standardlägesgränssnittet **Ägar-ID för Portfolio** -fältet är tillgängligt för en projektvy, men **Portfolio ägarnamn** fältet är inte. Du kan använda textläge för att visa **Portfolio ägarnamn** i kolumnen för en vy.

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

## Exempel: lägg till kolumnen Portfolio ägarnamn i en projektvy

1. Gå till en lista med projekt.
1. Från **Visa** nedrullningsbar meny, klicka **Ny vy**.

1. Klicka **Lägg till kolumn** börjar du skriva &quot;Portfolio Owner ID&quot; i dialogrutan **Visa i den här kolumnen** markerar du det när det visas i listan.

1. Klicka **Växla till textläge**.
1. Håll muspekaren över textlägesområdet och klicka **Klicka för att redigera text**.
1. Ersätt `valuefield` line (`valuefield=portfolio:ownerID`) med följande rad:

   ```
   valuefield=portfolio:owner:name
   ```

   eller

   Ta bort den text du hittar i **Textläge** och ersätt den med följande kod:

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   I det här exemplet sorterar rapporten efter Portfolio-ägar-ID:t, vilket anges i `querysort` linje.

   >[!TIP]
   >
   >Ersätta ett fält `ID` med fältet `name` använda textläge, ersätt alltid `ID` med `:name` i `valuefield` linje.

1. Klicka **Spara** sedan **Spara vy**.

---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: visningsobjekt som inte ingår i standardgränssnittet'
description: Du kan visa objekt som inte ingår i standardlägesgränssnittet i en vy. Du kan bara göra detta genom att referera till dem via textläge.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# Visa: visningsobjekt som inte ingår i standardgränssnittet

Du kan visa objekt som inte ingår i standardlägesgränssnittet i en vy. Du kan bara göra detta genom att referera till dem via textläge.\
Du kan bestämma vilka fält som kan inkluderas i en vy på något av följande sätt:

* Använd [API Explorer](../../../wf-api/general/api-explorer.md) för att identifiera andra objekt som kan refereras via textläge.\
  Alla fält som finns dokumenterade i API Explorer är inte giltiga för textläge. Vissa fält kan bara rapporteras via API:t.

* Hitta objektets ID-fält i en kolumn. De flesta objekt som har ett fält-ID har också ett motsvarande kolumn- eller fältnamn som kanske inte är tillgängligt via standardlägesgränssnittet.

  Du kan använda textläge för att i en vy inkludera kolumn- eller fältnamnet i stället för ID:t genom att ersätta `fieldnameID` med `fieldname:name`.

  I standardlägesgränssnittet är t.ex. fältet **Portfolio Ägar-ID** tillgängligt för en projektvy, men fältet **Portfolio Ägarnamn** är inte tillgängligt. Du kan använda textläge för att visa **Portfolio ägarnamn** i en vykolumn.

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
   <td> <p>Begäran om att ändra en vy </p>
   <p>Planera att ändra en rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra en vy</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
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
1. Klicka på **Ny vy** i listrutan **Visa**.

1. Klicka på **Lägg till kolumn** och börja sedan skriva &quot;Portfolio Owner ID&quot; i fältet **Show i den här kolumnen** och markera den när den visas i listan.

1. Klicka på **Växla till textläge**.
1. Hovra över textlägesområdet och klicka på **Klicka för att redigera text**.
1. Ersätt raden `valuefield` (`valuefield=portfolio:ownerID`) med följande rad:

   ```
   valuefield=portfolio:owner:name
   ```

   eller

   Ta bort texten som du söker i rutan **Textläge** och ersätt den med följande kod:

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   I det här exemplet sorterar rapporten efter Portfolio-ägar-ID:t, vilket anges av raden `querysort`.

   >[!TIP]
   >
   >Ersätt alltid `ID` med `:name` på raden `valuefield` om du vill ersätta ett fält `ID` med fältet `name` i textläge.

1. Klicka på **Spara** och sedan på **Spara vy**.

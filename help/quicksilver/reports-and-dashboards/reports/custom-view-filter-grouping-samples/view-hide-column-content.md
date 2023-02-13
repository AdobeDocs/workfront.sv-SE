---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: dölj innehållet i en kolumn'
description: Du kanske vill dölja information i kolumnen för en vy. Du kan göra detta genom att ändra kolumnens textläge.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Visa: dölja innehållet i en kolumn

Du kanske vill dölja information i kolumnen för en vy. Du kan göra detta genom att ändra kolumnens textläge.

>[!TIP]
>
>* Du kan använda dolda kolumner för att sortera efter ett visst objekt som du inte vill visa i vyn.\
   >  Du kan till exempel sortera efter Uppgiftsnummer i en uppgiftsvy och dölja informationen om Uppgiftsnummer i vyn. I det här fallet kan objektet som refereras i kolumnen sortera vyn, men informationen om objektet visas inte i vyn.
>* När du döljer en kolumn bör du tänka på att informationen i kolumnen är dold, men kolumnen finns fortfarande i vyn.
>


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

## Exempel: Sortera och dölja kolumnen Uppgiftsnummer i en uppgiftsvy:

1. Gå till en lista med uppgifter.
1. Från **Visa** nedrullningsbar meny, klicka **Ny vy**.

1. Klicka **Lägg till kolumn** och börja skriva &quot;Aktivitetsnummer&quot; i **Visa i den här kolumnen** markerar du det när det visas i listan.

1. Klicka **Växla till textläge**.
1. Håll muspekaren över textlägesområdet och klicka **Klicka för att redigera text**.
1. Ta bort den text du hittar i **Textläge** och ersätt den med följande kod:

   <pre><strong>displayname=</strong>linkedname=direct<br>querysort=taskNumber<br>sortOrder=1<br>sortType=asc<br>textmode=true<br><strong>value=</strong>valueFormat=int<br><strong>width=0</strong></pre>De viktiga ändringarna i koden som gör kolumnen dold är:

   ```
   displayname
   ```

   den här raden måste vara tom.

   ```
   valuefield
   ```

   Detta har ersatts med *value* och måste vara tom.

   ```
   width
   ```

   : Beroende på fältet måste värdet vara *0* eller *1*.

1. Klicka **Spara** sedan **Spara vy**.

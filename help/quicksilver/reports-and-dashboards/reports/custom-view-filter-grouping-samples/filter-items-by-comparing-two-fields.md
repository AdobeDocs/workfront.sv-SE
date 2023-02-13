---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: ta bort objekt i en lista genom att jämföra två fälts'
description: Du kan filtrera objekt från en lista genom att jämföra två av deras fält. Du kan till exempel bara visa uppgifter där aktivitetens verkliga slutförandedatum är större än det planerade slutförandedatumet.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Filter: ta bort objekt i en lista genom att jämföra två fält

Du kan filtrera objekt från en lista genom att jämföra två av deras fält. Du kan till exempel bara visa uppgifter där aktivitetens verkliga slutförandedatum är större än det planerade slutförandedatumet.

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

## Filtrera objekt genom att jämföra två fält

1. Gå till en lista med uppgifter.
1. Från **Filter** nedrullningsbar meny, välja **Nytt filter**.

1. Klicka **Lägg till filterregel** och lägga till **Faktiskt slutförandedatum** >**Större än** > **Välj ett datum**.

   >[!TIP]
   >
   >Välj den filtermodifierare som du vill använda för det markerade fältet, om den är tillgänglig.

1. Klicka **Växla till textläge**.
1. I **Ange filterregler för rapporten** lägger du till följande kod:

   ```
   actualCompletionDate=FIELD:plannedCompletionDate<br>actualCompletionDate_Mod=gt
   ```

1. Klicka **Klar** sedan **Spara filter**.

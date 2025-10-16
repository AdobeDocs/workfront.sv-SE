---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: ta bort objekt i en lista genom att jämföra två fält'
description: Du kan filtrera objekt från en lista genom att jämföra två av deras fält. Du kan till exempel bara visa uppgifter där aktivitetens verkliga slutförandedatum är större än det planerade slutförandedatumet.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# Filter: ta bort objekt i en lista genom att jämföra två fält

<!--Audited: 10/2024-->

Du kan filtrera objekt från en lista genom att jämföra två av deras fält. Du kan till exempel bara visa uppgifter där aktivitetens verkliga slutförandedatum är större än det planerade slutförandedatumet.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> 
   <p>Medarbetare eller begäran om att ändra ett filter </p>
   <p>Standard eller Plan för att ändra en rapport</p>
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

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrera objekt genom att jämföra två fält

1. Gå till en lista med uppgifter.
1. Välj **Nytt filter** i listrutan **Filter**.

1. Lägg till ett filter för **aktiviteten:Actual Slutförandedatum** > **Större än** > **Välj ett datum**.

   >[!TIP]
   >
   >Välj den filtermodifierare som du vill använda för det markerade fältet, om den är tillgänglig.

1. Klicka på **Textläge**.
1. Lägg till följande kod i det område som visas:

   ```
   actualCompletionDate=FIELD:plannedCompletionDate
   actualCompletionDate_Mod=gt
   ```

1. Klicka på **Använd** > **Spara som ny**.

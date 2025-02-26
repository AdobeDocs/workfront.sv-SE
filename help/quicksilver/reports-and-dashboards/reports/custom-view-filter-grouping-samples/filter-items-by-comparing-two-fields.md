---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: ta bort objekt i en lista genom att jämföra två fält'
description: Du kan filtrera objekt från en lista genom att jämföra två av deras fält. Du kan till exempel bara visa uppgifter där aktivitetens verkliga slutförandedatum är större än det planerade slutförandedatumet.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: e8acdf8f7b3859385237e788dfda34ee62ee11d1
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# Filter: ta bort objekt i en lista genom att jämföra två fält

<!--Audited: 10/2024-->

Du kan filtrera objekt från en lista genom att jämföra två av deras fält. Du kan till exempel bara visa uppgifter där aktivitetens verkliga slutförandedatum är större än det planerade slutförandedatumet.

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

## Filtrera objekt genom att jämföra två fält

1. Gå till en lista med uppgifter.
1. Välj **Nytt filter** i listrutan **Filter**.

1. Lägg till ett filter för **aktiviteten:Faktiskt slutförandedatum** > **Större än** > **Välj ett datum**.

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

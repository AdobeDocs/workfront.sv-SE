---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Visa rapporter som schemalagts för leverans'
description: Det här rapportfiltret visar alla rapporter som schemalagts att levereras automatiskt i Adobe Workfront. Den används bäst med standardvyn.
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: 7b937384-80c9-4bc7-94be-5573cf86b35b
source-git-commit: be102fd5f490b12837a231774253c030973c1c4f
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 0%

---

# Filter: visa rapporter som är schemalagda för leverans

<!--Audited: 10/2024-->

Det här rapportfiltret visar alla rapporter som schemalagts att levereras automatiskt i Adobe Workfront. Den används bäst med standardvyn.

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

## Rapportleveransfilter

Så här använder du det här filtret:

1. Gå till en lista med rapporter.

1. Välj **Nytt filter** i listrutan **Filter**.

1. Klicka på **Växla till textläge**.

1. Kopiera och klistra in följande kod i området **Ange filterregler för rapporten**:

   ```
    scheduledReportsOM:ID_Mod=notblank
   ```

1. Klicka på **Spara filter**.

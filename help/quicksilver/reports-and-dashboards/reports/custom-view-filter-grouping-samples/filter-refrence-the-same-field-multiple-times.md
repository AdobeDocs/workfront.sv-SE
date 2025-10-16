---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Skapa flera filterregler som refererar till samma fält (AND-satser)'
description: I standardlägesgränssnittet, när du försöker skapa flera filter som refererar till samma fält (med AND-kvalificeraren), tas ett av filtren bort när du sparar rapporten och avslutar rapportbyggaren.
author: Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---

# Filter: skapa flera filterregler som refererar till samma fält (&quot;AND&quot;-satser)

<!--Audited: 10/2024-->

I standardlägesgränssnittet, när du försöker skapa flera filter som refererar till samma fält (med AND-kvalificeraren), tas ett av filtren bort när du sparar rapporten och avslutar rapportbyggaren.

**Exempel:** Du kanske bara vill visa uppgifter som innehåller ordet &quot;green&quot; men som inte innehåller ordet &quot;red&quot; i namnet. Adobe Workfront tillåter inte att du sparar följande filterregler med standardlägesgränssnittet eftersom det refererar till samma fält (aktivitetsnamn), men använder olika modifierare och refererar till olika värden:

* Uppgiftsnamn > Innehåller > Grönt
* Uppgiftsnamn > Innehåller inte > Rött

Du kan dock skapa det här filtret i textläge.

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

## Skapa flera filterregler som refererar till samma fält

1. Gå till en lista med uppgifter.
1. Välj **Nytt filter** i listrutan **Filter**.
1. Klicka på **Textläge**.
1. Lägg till följande kod i den ruta som visas:

   ```
   name=green
   name_Mod=cicontains
   AND:1:name=red
   AND:1:name_Mod=cinotcontains
   ```

   >[!TIP]
   >
   >Om du vill skapa liknande filter måste du först skapa den första programsatsen. Exempel:
   >
   >```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >Kopiera och klistra in programsatsen så många gånger som behövs. Du kan sedan lägga till så många programsatser som du behöver referera till samma fält (i vårt fall &quot;name&quot;) och göra följande ändringar i de ytterligare programsatserna:
   >
   >1. Före de två kopierade raderna med &quot;AND:1:&quot;, &quot;AND:2:&quot;, &quot;AND:3:&quot; osv. för varje nytt fält finns ett möjligt värde.
   >1. Ersätt fältraden med det nya fältvärdet (efter &quot;=&quot;-tecknet).
   >1. Ersätt modifieringslinjen (_Mod) med den nya modifieraren.
   >   
   >Programsatserna är skiftlägeskänsliga.

1. Klicka på **Använd** och sedan på **Spara som ny**.

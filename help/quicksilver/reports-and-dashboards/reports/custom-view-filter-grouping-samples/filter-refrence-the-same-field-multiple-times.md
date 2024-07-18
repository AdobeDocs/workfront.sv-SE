---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filter: skapa flera filterregler som refererar till samma fält (AND-satser)"
description: I standardlägesgränssnittet, när du försöker skapa flera filter som refererar till samma fält (med AND-kvalificeraren), tas ett av filtren bort när du sparar rapporten och avslutar rapportbyggaren.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: d3525d9f286e08258d75d770d257b325b9ee8ca9
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---

# Filter: skapa flera filterregler som refererar till samma fält (&quot;AND&quot;-satser)

I standardlägesgränssnittet, när du försöker skapa flera filter som refererar till samma fält (med AND-kvalificeraren), tas ett av filtren bort när du sparar rapporten och avslutar rapportbyggaren.

**Exempel:** Du kanske bara vill visa uppgifter som innehåller ordet &quot;green&quot; men som inte innehåller ordet &quot;red&quot; i namnet. Adobe Workfront tillåter inte att du sparar följande filterregler med standardlägesgränssnittet eftersom det refererar till samma fält (aktivitetsnamn), men använder olika modifierare och refererar till olika värden:

* Uppgiftsnamn > Innehåller > Grönt
* Uppgiftsnamn > Innehåller inte > Rött

Du kan dock skapa det här filtret i textläge.

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
   <td> <p>Begäran om att ändra ett filter </p>
   <p>Planera att ändra en rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra ett filter</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Skapa flera filterregler som refererar till samma fält

1. Gå till en lista med uppgifter.
1. Välj **Nytt filter** i listrutan **Filter**.
1. Klicka på **Växla till textläge**.
1. Hovra över textlägesområdet och klicka på **Klicka för att redigera text**.
1. Lägg till följande kod i Ange filterregler för rapportområdet:

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

1. Klicka på **Klar** och sedan på **Spara filter**.

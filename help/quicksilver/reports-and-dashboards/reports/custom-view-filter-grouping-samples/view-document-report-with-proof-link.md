---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: Dokumentrapport med länk till ett korrektur'
description: 'Visa: dokumentrapport med länk till ett korrektur'
author: Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Visa: dokumentrapport med länk till ett korrektur

<!--Audited: 11/2024-->

I den här dokumentvyn kan du infoga en länk till ett korrektur av den aktuella versionen av dokumentet.

![Visa dokument med korrekturlänk](assets/view-document-with-proof-link-350x92.png)

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

## Visa en dokumentrapport med en länk till ett korrektur

Så här använder du den här vyn:

1. Gå till en lista med dokument.
1. Välj **Ny vy** i listrutan **Visa**.
1. Klicka på **Lägg till kolumn**.
1. Klicka på **Växla till textläge** och sedan på **Redigera textläge**.
1. Ta bort den text du söker i rutan **Redigera textläge** och ersätt den med följande kod:

   ```
   displayname=Proof Link
   shortview=true
   textmode=true
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   valueformat=HTML
   ```

   >[!TIP]
   >
   >Ersätt&quot;Din domän&quot; med din faktiska Workfront-domän. Om ditt företags Workfront-URL är *Company.my.workfront.com* är din domän&quot;Company&quot;.

1. Klicka på **Klar** och sedan på **Spara vy**.
1. (Valfritt) Uppdatera vynamnet och klicka sedan på **Spara vy**.
1. (Valfritt) Om du bara vill visa dokument med korrektur lägger du till ett filter genom att göra följande:

   1. Klicka på listrutan **Filter** och sedan på **Nytt filter**.
   1. Klicka på **Lägg till en filterregel** och börja skriva Korrekturägare och välj sedan **Korrekturägar-ID** när den visas i listan.
   1. Välj **Är inte tom** för filtermodifieraren.
   1. Klicka på **Spara filter**.
   1. (Valfritt) Uppdatera filternamnet och klicka sedan på **Spara filter**.

1. Klicka på länken i kolumnen Korrekturlänk för att komma åt korrekturet för den senaste versionen av dokumentet.

---
product-area: reporting
navigation-topic: text-mode-reporting
title: Jämför fält i villkorlig formatering
description: Du kan använda villkorsstyrd formatering för att jämföra två olika fält i en vy och markera dem när vissa villkor uppfylls mellan fälten.
author: Nolan
feature: Reports and Dashboards
exl-id: da4447ba-6e76-4701-88ee-87a30393bed9
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# Jämför fält i villkorlig formatering

<!-- Audited: 1/2025 -->

Du kan använda villkorsstyrd formatering för att jämföra två olika fält i en vy och markera dem när vissa villkor uppfylls mellan fälten.

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
     <p>Standard</p>
     <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att redigera vyn i en rapport</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter till en rapport för att redigera vyn i en rapport</p> <p>Hantera behörigheter till en vy</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exempel: Jämför faktiskt startdatum och planerat startdatum

Om t.ex. det faktiska startdatumet för en uppgift infaller efter det planerade startdatumet kan du markera kolumnen Planerat startdatum med villkorsstyrd formatering.

Så här jämför du det planerade startdatumet och det faktiska startdatumet för aktiviteten med villkorsstyrd formatering:

1. Gå till en uppgiftsvy eller en rapport.
1. (Villkorligt) Om du arbetar med en rapport går du till fliken **Kolumner (Visa)** i rapportredigeraren och klickar på rubriken för den kolumn som du vill formatera för att markera den.\
   Markera till exempel kolumnen **Faktiskt startdatum** om du vill lägga till den villkorliga formateringen genom att jämföra fälten Planerat startdatum och Faktiskt startdatum.

1. Klicka på **Avancerade alternativ** och sedan på Lägg till en **regel för den här kolumnen**.

1. Ange jämförelsevillkoren med hjälp av befintliga värden som finns i verktyget och ange villkorsstyrd formatering.\
   Vi vill t.ex. markera uppgifter där det faktiska startdatumet är senare än ( eller större än) det planerade startdatumet. Markera modifieringen Större än och välj ett faktiskt datum i datumfältet.

   ![Villkorsstyrd formatering för faktiskt startdatum](assets/cond-format-1-350x84.png)

1. (Valfritt) Välj **Använd på hela raden** om du vill använda formateringen på hela raden.
1. Klicka på **Spara**.

1. Markera kolumnen **Faktiskt startdatum** och klicka sedan på **Växla till textläge**.

1. Klicka på **Redigera textläge** och lägg sedan till följande textrad:

   ```
   styledef.case.0.comparison.rightmethod= <field to compare>
   ```

   I vårt exempel:

   ```
   styledef.case.0.comparison.rightmethod=plannedStartDate
   ```

   >[!NOTE]
   >
   >Om du jämför ett Workfront-fält använder du kamelversionssyntax för fältets namn. Om du jämför ett anpassat fält använder du **DE:Actual-namnet för fältet** för det namnfält som du jämför med det första fältet.\
   >Om du till exempel jämför **Faktiskt startdatum** med ett anpassat fält med namnet **Leveransdatum** lägger du till följande programsats i textlägeskoden:
   >
   >`styledef.case.0.comparison.rightmethod=DE:Delivery Date`

1. Kontrollera att kodraden `righttext` matchar satsen i kodraden `rightmethod`.

   ![Villkorsstyrd formatering](assets/cond-format-2-350x171.png)

1. Klicka på **Spara**.
1. Klicka på **Spara + Stäng**.

   Kolumnen markerar de fält som uppfyller villkoren.

---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppering: Ange om resultatet av en gruppering ska komprimeras eller utökas i textläge'
description: 'Gruppering: ange om resultatet av en gruppering ska komprimeras eller expanderas i textläge'
author: Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# Gruppering: ange om resultatet av en gruppering ska komprimeras eller expanderas i textläge

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

Du kan ange om resultatet i en gruppering ska visas komprimerat eller expanderat i en lista eller rapport med hjälp av standardrapportverktyget. Resultatet i en grupperingsvisning expanderat som standard. Mer information om hur du skapar en gruppering finns i [Skapa grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Understanding text mode, Edit groupings to organize reports, Create a Custom Report; create a snippet when convenient)</p>
-->

>[!TIP]
>
>* När du justerar grupperingar manuellt när du visar en lista kommer Adobe Workfront ihåg dina manuella inställningar tills du loggar ut. När du loggar in igen visas listan enligt den här inställningen.
>* Resultatet av en gruppering visas alltid expanderat när du har öppnat dem från ett diagramelement.
>

Du kan också ange om en gruppering ska visas expanderad eller komprimerad i textläge.

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

## Ange om resultatet av en gruppering ska komprimeras eller expanderas i textläge

1. Gå till en lista med objekt.
1. Välj **Ny gruppering** i listrutan **Gruppering**.

1. Lägg till en gruppering och klicka sedan på **Växla till textläge**.

   eller

   Om grupperingen redan är i textläge lägger du till följande kod till grupperingsnivån som du vill visa komprimerad:

   `group.0.iscollapsed=true`

1. (Valfritt) Om du vill att grupperingen ska visas expanderad lägger du till följande kod till rätt grupperingsnivå:

   `group.0.iscollapsed=false`

1. Klicka på **Klar** och sedan på **Spara gruppering**.
1. (valfritt) Uppdatera grupperingens namn och klicka sedan på **Spara gruppering**.

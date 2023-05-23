---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Gruppering: ange om resultatet av en gruppering ska komprimeras eller expanderas i textläge'
description: '''Gruppering: ange om resultatet av en gruppering ska komprimeras eller expanderas i textläge'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# Gruppering: ange om resultatet av en gruppering ska komprimeras eller expanderas i textläge

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
   <td> <p>Begäran om att ändra en gruppering </p>
   <p>Planera att ändra en rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra en gruppering</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Ange om resultatet av en gruppering ska komprimeras eller expanderas i textläge

1. Gå till en lista med objekt.
1. Från **Gruppering** nedrullningsbar meny, välja **Ny gruppering**.

1. Lägg till en gruppering och klicka på **Växla till textläge**.

   eller

   Om grupperingen redan är i textläge lägger du till följande kod till grupperingsnivån som du vill visa komprimerad:

   ```
   group.0.iscollapsed=true
   ```

1. (Valfritt) Om du vill att grupperingen ska visas expanderad lägger du till följande kod till rätt grupperingsnivå:

   ```
   group.0.iscollapsed=false
   ```

1. Klicka **Klar** sedan **Spara gruppering**.

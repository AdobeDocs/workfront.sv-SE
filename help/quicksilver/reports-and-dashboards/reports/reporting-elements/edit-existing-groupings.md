---
title: Redigera befintliga grupperingar
description: Redigera befintliga grupperingar
author: Nolan
feature: Reports and Dashboards
exl-id: bd9e6794-3196-4a73-a86a-9ba6048e613b
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---

# Redigera befintliga grupperingar

<!-- Audited: 11/2024 -->

<!--NOTE: This is the third part of a former article split in 3: two how-tos and one reference article about creating and customizing groupings)-->

Du kan anpassa en befintlig gruppering som du ursprungligen skapade eller som delades med dig. Sedan kan du spara den som en ny gruppering.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licens*</strong></td> 
   <td> 
      <p>Nytt:</p>
         <ul>
         <li><p>Medarbetare eller högre</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Begäran eller senare</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att redigera en gruppering i en rapport</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Hantera behörigheter till en rapport för att redigera en gruppering i en rapport</p> <p>Hantera behörigheter för en gruppering</p></td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Du måste skapa en gruppering innan du kan redigera den.

Mer information om hur du skapar en gruppering finns i [Skapa grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

## Instruktioner

1. Gå till en lista med objekt som innehåller den gruppering som du vill anpassa.
1. Klicka på ikonen **Gruppera**.
1. Markera den gruppering som du vill anpassa och klicka sedan på ikonen **Redigera** ![Redigera](assets/edit-icon.png) .

   ![Välj redigeringsikonen.](assets/customizegrouping-nwe-standard-350x291.png)

   Gränssnittsverktyget för att anpassa grupperingen öppnas.

1. I avsnittet **Förhandsgranska gruppering** klickar du på **Lägg till gruppering** för att definiera hur informationen i rapporten ska ordnas. En förhandsgranskning av hur grupperingen ser ut i rapporten visas nedan.

1. Börja skriva namnet på det fält som representerar hur du vill organisera informationen i rapporten och klicka sedan på det när det visas i listrutan.
1. (Valfritt och villkorligt) När du visar en uppdaterad lista väljer du **Komprimera den här grupperingen som standard** om du vill att resultaten i grupperingen ska visas komprimerade i stället för expanderade. Den här inställningen är inaktiverad som standard och resultatet av grupperingen visas alltid i den utökade listan.

   Mer information om uppdaterade och äldre listor finns i avsnittet&quot;Skillnaden mellan uppdaterade och äldre listor&quot; i artikeln [Kom igång med listor i Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create grouping article and Common uses of text mode)</p>
   -->

   >[!TIP]
   >
   >* När du justerar grupperingar manuellt när du visar en lista kommer Workfront ihåg dina manuella inställningar tills du loggar ut. När du loggar in igen visas listan enligt den här inställningen.
   >* Resultatet av en gruppering visas alltid utökat när du har öppnat dem från ett diagramelement eller i en äldre lista. I dessa fall ignoreras den här inställningen.

1. Upprepa steg 4, 5 och 6 för att definiera ytterligare grupperingar.\
   Du kan definiera upp till tre grupperingar för att ordna information. Du kan organisera informationen ytterligare med upp till fyra grupperingar genom att skapa en matrisrapport. Mer information om matrisrapporter finns i [Skapa en matrisrapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. Klicka på **Spara gruppering** om du vill ersätta den aktuella grupperingen med dina ändringar.

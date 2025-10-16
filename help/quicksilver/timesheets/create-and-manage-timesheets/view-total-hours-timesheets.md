---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Visa totalt antal timmar på tidrapporten
description: Du kan visa det totala antalet timmar på tidrapporten. Det totala antalet tidrapportstimmar inkluderar timmar som loggats för projekt, uppgifter, utleveranser och alla allmänna timmar.
author: Lisa
feature: Timesheets
exl-id: ff0823f2-61d0-453f-ae1c-68f0f1465d73
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# Visa totalt antal timmar på tidrapporten

<!--Audited: 8/2024-->

Du kan visa det totala antalet timmar på tidrapporten. Det totala antalet tidrapportstimmar inkluderar timmar som loggats för projekt, uppgifter, utleveranser och alla allmänna timmar.

Det totala antalet timmar motsvarar timmar som skickats in via tidrapporten, uppdateringsområdet eller timområdet för projekt, uppgifter eller utgåvor.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td> <p>Ljus eller högre </p>
   <p>Granska eller högre</p> </td> 
  </tr> 
  <tr> 
   <td>Åtkomstnivåkonfiguration</td> 
   <td> <p>Visa eller ge högre åtkomst till uppgifter och ärenden</p> </td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter för uppgifter och problem</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visa det totala antalet timmar för en tidrapport i tidrapporthuvudet

Du kan visa tidrapportets totala timmar i tidrapporthuvudet.

![](assets/timesheet-total-hours-in-header-highlighted-redesigned.png)

## Visa det totala antalet timmar på tidrapporten i en lista över tidrapporter

{{step1-to-timesheets}}

Området **Tidrapporter** öppnas.

![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Valfritt) Uppdatera filtret i listan över tidrapporter genom att göra något av följande:

   * Välj **Mina tidrapportgodkännanden** i det övre högra hörnet av sidan om du bara vill visa tidrapporter som du godkänner

     eller

     Välj **Mina tidrapporter** om du bara vill visa dina tidrapporter.

     Detta tillämpar filtren Mina tidrapportgodkännanden eller Min tidrapport på listan med tidrapporter.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Klicka på Filterikonen ![](assets/filter-nwepng.png) om du vill använda ett annat filter eller skapa ett nytt. Mer information om hur du skapar eller uppdaterar filter finns i [Skapa eller redigera filter i Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Alternativen Mina tidrapportgodkännanden och Mina tidrapporter visas inte högst upp i tidrapportlistan eller i filterlistan om Workfront-administratören eller en gruppadministratör har tagit bort filtren Mina tidrapportgodkännanden och Mina tidrapporter från antingen listkontrollerna i inställningsområdet eller från layoutmallen. Mer information finns i följande artiklar:
   >
   >   
   >   
   >   * [Anpassa filter, vyer och grupperingar med en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Valfritt) Klicka på ikonerna **Visa** ![](assets/view-icon.png) eller **Gruppera** ![](assets/grouping.png) om du vill använda en annan vy eller gruppering eller skapa en ny.

   Mer information om hur du skapar filter, vyer och grupperingar finns i följande artiklar:

   * [Skapa eller redigera filter i Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Skapa eller redigera vyer i Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Skapa grupperingar i Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Det totala antalet timmar för varje tidrapport som visas i kolumnen **Totalt antal timmar**.

   ![](assets/total-hours-column-highlighted-all-timesheets-list-nwe-350x120.png)

   >[!TIP]
   >
   >När du använder standardvyn för en lista med tidrapporter visas kolumnen Totalt antal timmar i rött om den tid som loggas för objekten på tidrapporten överstiger antalet timmar i tidrapporgens tidsram. Mer information finns i fältet&quot;Total Hours&quot; i [Ordlista för Adobe Workfront-terminologi](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

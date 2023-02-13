---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Visa totalt antal timmar på tidrapporten
description: Du kan visa det totala antalet timmar på tidrapporten. Det totala antalet tidrapportstimmar inkluderar timmar som loggats för projekt, uppgifter, utleveranser och alla allmänna timmar.
author: Alina
feature: Timesheets
exl-id: ff0823f2-61d0-453f-ae1c-68f0f1465d73
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 0%

---

# Visa totalt antal timmar på tidrapporten

Du kan visa det totala antalet timmar på tidrapporten. Det totala antalet tidrapportstimmar inkluderar timmar som loggats för projekt, uppgifter, utleveranser och alla allmänna timmar.

Det totala antalet timmar motsvarar timmar som skickats in via tidrapporten, uppdateringsområdet eller timområdet för projekt, uppgifter eller utgåvor.

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
   <td> <p>Granska </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa åtkomst eller senare till uppgifter och ärenden</p> <p>Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter för uppgifter och problem</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan eller licenstyp du har.

## Visa det totala antalet timmar för en tidrapport i tidrapporthuvudet

Du kan visa tidrapportets totala timmar i tidrapporthuvudet.

![](assets/timesheet-total-hours-in-header-highlighted-redesigned.png)

## Visa det totala antalet timmar på tidrapporten i en lista över tidrapporter

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Tidrapporter**. The **Alla** Filtret är markerat som standard och visar alla tidrapporter du har tillgång till.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Valfritt) Uppdatera filtret i listan över tidrapporter genom att göra något av följande:

   * Välj **Mina tidrapportgodkännanden** i det övre högra hörnet av sidan om du bara vill visa tidrapporter som du har godkänt

      eller

      Välj **Mina tidrapporter** om du bara vill visa dina tidrapporter.

      Detta tillämpar filtren Mina tidrapportgodkännanden eller Min tidrapport på listan med tidrapporter.

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Klicka på ikonen Filter ![](assets/filter-nwepng.png) om du vill använda ett annat filter eller skapa ett nytt. Mer information om hur du skapar eller uppdaterar filter finns i [Skapa eller redigera filter i Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >Alternativen Mina tidrapportgodkännanden och Mina tidrapporter visas inte högst upp i tidrapportlistan eller i filterlistan om Workfront-administratören eller en gruppadministratör har tagit bort filtren Mina tidrapportgodkännanden och Mina tidrapporter från antingen listkontrollerna i inställningsområdet eller från layoutmallen. Mer information finns i följande artiklar:
   * [Anpassa filter, vyer och grupperingar med en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Valfritt) Klicka på **Visa** ![](assets/view-icon.png) eller **Gruppering** ![](assets/grouping.png) ikoner för att använda en annan vy eller gruppering eller för att skapa en ny.

   Mer information om hur du skapar filter, vyer och grupperingar finns i följande artiklar:

   * [Skapa eller redigera filter i Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Skapa eller redigera vyer i Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Skapa grupperingar i Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Det totala antalet timmar för varje tidrapport som visas i **Totalt antal timmar** kolumn.

   ![](assets/total-hours-column-highlighted-all-timesheets-list-nwe-350x120.png)

   >[!TIP]
   När du använder standardvyn för en lista med tidrapporter visas kolumnen Totalt antal timmar i rött om den tid som loggas för objekten på tidrapporten överstiger antalet timmar i tidrapporgens tidsram. Mer information finns i fältet&quot;Totalt antal timmar&quot; i [Ordlista för Adobe Workfront-terminologi](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

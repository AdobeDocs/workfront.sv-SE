---
navigation-topic: use-the-gantt-chart
title: Exportera Gantt-schemat till PDF
description: Du kan exportera Gantt-schemat till en PDF. Efteråt kan du skriva ut eller bifoga den i ett e-postmeddelande för att dela den med andra användare.
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: 0792651822fd85cb3bfbb754aaf949c4fc4038a1
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 0%

---

# Exportera [!UICONTROL Gantt Chart] till PDF

<!--Audited: 5/2025-->

Du kan exportera [!UICONTROL Gantt chart] till en PDF. Efteråt kan du skriva ut eller bifoga den i ett e-postmeddelande för att dela den med andra användare.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] plan</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] licens</td> 
   <td> <p>Nytt:[!UICONTROL Light] eller senare</p>
   <p>Aktuell:[!UICONTROL Review] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>[!UICONTROL View] eller högre åtkomst till projekt och uppgifter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>[!UICONTROL View] eller bättre åtkomst till projektet</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exportera [!UICONTROL Gantt chart]

1. Få åtkomst till [!UICONTROL Gantt chart] som du vill exportera till PDF, enligt beskrivningen i [Kom igång med [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. Konfigurera [!UICONTROL Gantt chart] så att rätt information visas som du vill exportera.

   >[!NOTE]
   >
   >Om du exporterar [!UICONTROL Gantt chart] från en lista med projekt innehåller PDF-filen bara projekten i listan, inte aktiviteterna i varje projekt. Om du vill exportera en lista med uppgifter kan du göra det från det projekt som de är kopplade till, eller genom att skapa en aktivitetsrapport och visa resultaten av rapporten i [!UICONTROL Gantt View].

   Konfigurera någon av följande information:

   * Klicka på ikonerna **Filter**, **Visa** och **Gruppera** ovanför ikonerna [!UICONTROL Gantt chart] och lägg till eller redigera det befintliga filter, den befintliga vyn eller den befintliga grupperingen som används i listan med objekt i [!UICONTROL Gantt chart].

     Alla filter och grupperingar som är markerade i listvyn bevaras när [!UICONTROL Gantt chart] visas. Vyer visas bara i den exporterade [!UICONTROL Gantt chart] i listan som visas bredvid [!UICONTROL Gantt chart] på den första sidan. Vyer visas inte på själva [!UICONTROL Gantt chart].

     >[!TIP]
     >
     >Om du vill ha mer utrymme för [!UICONTROL Gantt chart] använder du en vy som innehåller så få kolumner som möjligt.

   * Välj alternativet **Växla till beräknade datum** om du vill visa Planerade datum i stället för Planerade datum. Som standard visas planerade datum.

   * Klicka på ikonen **Inställningar** ![Inställningar](assets/settings-icon.png) i det övre högra hörnet av Gantt-diagrammet och välj vilken information du vill visa. När du har valt det här alternativet inkluderas den här informationen i den exporterade Gantt PDF-filen.

     Välj bland följande alternativ:

      * Faktiska datum
      * Uppdrag
      * Baslinje
      * Bekräftelsedatum
      * % klart
      * Kritisk sökväg
      * Milstolpediamanter
      * Milstolpslinjer
      * Föregående
      * Status för förlopp
      * (Villkorligt) Planerade datum
      * (Villkorligt) Planerade datum

     Mer information finns i   [Konfigurera hur information visas på [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

     >[!NOTE]
     >
     > Uppdrag visas inte på [!UICONTROL Gantt chart] när [!UICONTROL Gantt chart] exporteras till PDF. När uppdragen har exporterats visas de bara i listvyn.

   * Den tidsperiod som visas på [!UICONTROL Gantt chart]. Hur detta visas i exportfilen beror på om du väljer **[!UICONTROL What I see]** eller **[!UICONTROL Multiple pages]** i ett senare steg.

     Mer information finns i [Visa information i [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).



1. (Valfritt) Om du bara vill ta med vissa uppgifter i den exporterade PDF-filen markerar du de uppgifter som du vill ta med. Om du inte markerar några uppgifter inkluderas alla uppgifter i den exporterade PDF-filen.

   Om du till exempel visar [!UICONTROL Gantt chart] för ett projekt som innehåller 50 uppgifter, men bara vill visa 10 uppgifter för den exporterade [!UICONTROL Gantt chart], markerar du de 10 uppgifter som du vill visa.

1. Klicka på skrivarikonen ![Skrivarikon](assets/printer-icon.png) i det övre högra hörnet av Gantt-diagrammet.
Dialogrutan **[!UICONTROL Export to PDF]** visas.

   ![Dialogrutan Exportera till PDF](assets/exported-gantt-ui-350x225.png)

1. I avsnittet **Exportera** väljer du bland följande alternativ för att ange om du bara vill exportera det du ser eller hela [!UICONTROL Gantt chart]:

   * **[!UICONTROL What I see]:** Exporterar alla aktiviteter (inklusive alla underaktiviteter) som visas på skärmen innan upp till 500 objekt exporteras. (Detta är inte vad som visas i avsnittet **[!UICONTROL Preview]**. Avsnittet **Förhandsgranska** innehåller bara exempeldata.)

     Underaktiviteter inkluderas i den exporterade PDF-filen även om den överordnade uppgiften är komprimerad och underaktiviteterna inte visas. Om du bara vill ta med överordnade uppgifter markerar du de överordnade uppgifter som du vill ta med och låter alla underaktiviteter vara omarkerade.

     >[!TIP]
     >
     >Du kan använda zoomnings- eller skjutreglaget för att endast visa en del av [!UICONTROL Gantt chart], vilket beskrivs i [Visningsinformation i [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md). Välj ett mer detaljerat alternativ om du vill visa fler sidor att exportera eller välj ett mindre detaljerat alternativ om du vill visa färre sidor att exportera.


   * **[!UICONTROL Multiple pages]:** Exporterar hela [!UICONTROL Gantt chart] (upp till 500 objekt), inklusive objekt som inte visas på den aktuella skärmen.

     >[!NOTE]
     >
     >* Om du behöver exportera en [!UICONTROL Gantt chart] som innehåller fler än 500 objekt ska du tillämpa ett filter på listan innan du visar [!UICONTROL Gantt chart] så att färre än 500 objekt eller 250 sidor visas. Mer information om hur du använder ett filter finns i [Översikt över filter](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
     >
     >
     >* Du kan inte exportera hela Gantt-schemat under följande omständigheter:
     >   
     >   * När den sträcker sig över mer än 250 sidor.
     >   * När den innehåller fler än 500 objekt.


1. Om PDF skrivs ut efter att det har exporterats till PDF väljer du den pappersstorlek som du vill skriva ut till i listrutan **[!UICONTROL Page Size]**.
Du kan välja mellan följande alternativ:

   * **[!UICONTROL Letter]**
   * **[!UICONTROL Legal]**
   * **[!UICONTROL Ledger]**
   * **[!UICONTROL A1]**
   * **[!UICONTROL A2]**
   * **[!UICONTROL A3]** (endast tillgängligt för vissa språk)
   * **[!UICONTROL A4]**
1. I avsnittet **[!UICONTROL Page Orientation]** väljer du om du vill att PDF ska exporteras i liggande eller stående orientering.
1. Välj **[!UICONTROL Show Legend]** om du vill inkludera förklaringen i din exporterade PDF.
1. Klicka på **[!UICONTROL Export]**. PDF-filen skapas och hämtas till din dator.

   Förklaringen längst ned i den exporterade filen förklarar endast de alternativ som du har aktiverat i [!UICONTROL Gantt chart] och som är tillgängliga i uppgiftslistan. Delmål visas t.ex. bara i förklaringen om du har minst en uppgift som är kopplad till en milstolpe.

   ![gantt_chart_with_updated_limited_förklard.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)

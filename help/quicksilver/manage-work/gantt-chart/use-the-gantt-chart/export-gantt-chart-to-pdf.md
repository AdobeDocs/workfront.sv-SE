---
navigation-topic: use-the-gantt-chart
title: Exportera Gantt-schemat till PDF
description: Du kan exportera Gantt-diagrammet till PDF.
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '853'
ht-degree: 0%

---

# Exportera [!UICONTROL Gantt Chart] till PDF

Du kan exportera [!UICONTROL Gantt chart] till PDF.

När du har exporterat [!UICONTROL Gantt chart] till PDF kan du skriva ut eller bifoga den i ett e-postmeddelande och dela den med andra användare.

## Åtkomstkrav

Du måste ha följande för att kunna följa stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] licens*</td> 
   <td> <p>[!UICONTROL Review] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>[!UICONTROL View] eller högre åtkomst till projekt och uppgifter</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>[!UICONTROL View] eller bättre åtkomst till projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Exportera [!UICONTROL Gantt chart]

1. Få åtkomst till [!UICONTROL Gantt chart] som du vill exportera till PDF, enligt beskrivningen i [Kom igång med [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. Kontrollera att du har konfigurerat [!UICONTROL Gantt chart] så att rätt information visas innan du exporterar den.

   >[!NOTE]
   >
   >Om du exporterar [!UICONTROL Gantt chart] från en lista med projekt innehåller PDF-filen bara projekten i listan, inte aktiviteterna i varje projekt. Om du vill exportera en lista med uppgifter kan du göra det från det projekt som de är kopplade till, eller genom att skapa en aktivitetsrapport och visa resultaten av rapporten i [!UICONTROL Gantt View].

   Du kan konfigurera följande information:

   * Filter, vyer och grupperingar efter behov i listan över uppgifter. Alla filter och grupperingar som är markerade i listvyn bevaras när [!UICONTROL Gantt chart] visas. Vyer visas bara i den exporterade [!UICONTROL Gantt chart] i listan som visas bredvid [!UICONTROL Gantt chart] på den första sidan. Vyer visas inte på själva [!UICONTROL Gantt chart].

     >[!TIP]
     >
     >Om du vill ha mer utrymme för själva [!UICONTROL Gantt chart] använder du en vy som innehåller så få kolumner som möjligt.

   * Konfigurationsalternativ på [!UICONTROL Gantt chart]. Du kan till exempel aktivera att milstolpar, datum, [!UICONTROL baselines] eller [!UICONTROL percent complete] visas på [!UICONTROL Gantt chart].

     Mer information finns i   [Konfigurera hur information visas på [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

     >[!NOTE]
     >
     > Uppdrag visas inte på [!UICONTROL Gantt chart] när [!UICONTROL Gantt chart] exporteras till PDF. När [!UICONTROL Gantt chart] exporteras till PDF visas uppdrag endast i listvyn.

   * Den tidsperiod som visas på [!UICONTROL Gantt chart].\

     Mer information finns i [Visa information i [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

     Hur tidsperioden visas i exportfilen beror på om du väljer **[!UICONTROL What I see]** eller **[!UICONTROL Multiple pages]** i ett senare steg.

1. (Valfritt) Om du bara vill ta med vissa uppgifter i det exporterade PDF markerar du de uppgifter som du vill ta med.

   Om du inte markerar några uppgifter inkluderas alla uppgifter i det exporterade PDF.

   Om du till exempel visar [!UICONTROL Gantt chart] för ett projekt som innehåller 50 uppgifter, men bara vill visa 10 uppgifter för den exporterade [!UICONTROL Gantt chart], markerar du de 10 uppgifter som du vill visa.

1. Klicka på skrivarikonen.\
   Dialogrutan **[!UICONTROL Export to PDF]** visas.\
   ![exported_gantt_UI.png](assets/exported-gantt-ui-350x225.png)

1. Välj om du bara vill exportera det du ser eller hela [!UICONTROL Gantt chart]:

   * **[!UICONTROL What I see]:** Exporterar alla aktiviteter (inklusive alla underaktiviteter) som visas på skärmen innan upp till 500 objekt exporteras. (Detta är inte vad som visas i avsnittet **[!UICONTROL Preview]**. Avsnittet [!UICONTROL Preview] innehåller bara exempeldata.)

     Underaktiviteter tas med i det exporterade PDF även om den överordnade aktiviteten är komprimerad och underaktiviteterna inte visas. Om du bara vill ta med överordnade uppgifter markerar du de överordnade uppgifter som du vill ta med och låter alla underaktiviteter vara omarkerade.

     Du kan använda den nedrullningsbara menyn **[!UICONTROL Zoom To]** eller skjutreglaget för att endast visa en del av [!UICONTROL Gantt chart], vilket beskrivs i [Visa information i [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md) .

   * **[!UICONTROL Multiple pages]:** Exporterar hela [!UICONTROL Gantt chart], även det som inte visas på den aktuella skärmen, upp till 500 objekt.\

     Du kan använda den nedrullningsbara menyn **[!UICONTROL Zoom To]** eller skjutreglaget för att bestämma hur mycket information som ska visas på varje sida, enligt beskrivningen i [Konfigurera hur information ska visas på [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). Välj ett mer detaljerat alternativ om du vill visa fler sidor att exportera, eller välj ett mindre detaljerat alternativ om du vill visa färre sidor att exportera.

     >[!NOTE]
     >
     >Om du behöver exportera en [!UICONTROL Gantt chart] som innehåller fler än 500 objekt ska du tillämpa ett filter på listan innan du visar [!UICONTROL Gantt chart] så att färre än 500 objekt eller 250 sidor visas. Mer information om hur du använder ett filter finns i [Översikt över filter](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
     >
     >
     >Du kan inte exportera hela Gantt-schemat under följande omständigheter:
     >
     >   
     >   
     >   * När den sträcker sig över mer än 250 sidor
     >   * När den innehåller mer än 500 objekt




1. Om PDF skrivs ut efter att det har exporterats till PDF väljer du den pappersstorlek du vill skriva ut till i listrutan **[!UICONTROL Page Size]**.\
   Du kan välja **[!UICONTROL Letter]**, **[!UICONTROL Legal]**, **[!UICONTROL Ledger]**, **[!UICONTROL A1]**, **[!UICONTROL A2]**, **[!UICONTROL A3]** (endast tillgängligt för vissa språk) eller **[!UICONTROL A4]**.
1. I avsnittet **[!UICONTROL Page Orientation]** väljer du om du vill att PDF ska exporteras i liggande eller stående orientering.
1. Välj **[!UICONTROL Show Legend]** om du vill inkludera förklaringen i den exporterade PDF.
1. Klicka på **[!UICONTROL Export]**.

   PDF-filen för [!UICONTROL Gantt chart] skapas och hämtas till datorn.

   Lägg märke till teckenförklaringen längst ned i den exporterade filen. Den förklarar endast de alternativ som du har aktiverat i [!UICONTROL Gantt chart] och som är tillgängliga i uppgiftslistan.

   Delmål visas t.ex. bara i förklaringen om du har minst en uppgift som är kopplad till en milstolpe.

   ![gantt_chart_with_updated_limited_förklard.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)

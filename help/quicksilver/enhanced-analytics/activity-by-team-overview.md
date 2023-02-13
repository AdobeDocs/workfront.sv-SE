---
title: Visa aktivitetsbaserad teamvisualisering i Förbättrad analys
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: I Activity by team-visualisering visas aktiviteter som inträffar under en viss tidsperiod för ett hemteam, så att du kan förstå hur olika hemteam tillbringade sin tid i Adobe Workfront. Beroende på hur ditt hemteam är konfigurerat i Workfront kan den här visualiseringen ge dig olika insikter och svara på olika frågor.
author: Nolan
feature: Reports and Dashboards
exl-id: c4f9886c-ce76-43a8-bd43-cb64fff27e79
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# Visa aktivitetsbaserad teamvisualisering i Förbättrad analys

I Activity by team-visualisering visas aktiviteter som inträffar under en viss tidsperiod för ett hemteam, så att du kan förstå hur olika hemteam tillbringade sin tid i Adobe Workfront. Beroende på hur ditt hemteam är konfigurerat i Workfront kan den här visualiseringen ge dig olika insikter och svara på olika frågor.

>[!NOTE]
>
>Visualiseringen av projektaktiviteten liknar den här visualiseringen, men den visar aktivitet baserat på personer som har tilldelats till projekt i stället för personer som har tilldelats till ett hemteam.\
>Mer information om projektaktivitetsvisualisering finns i [Visa projektaktivitetsvisualisering i Förbättrad analys](../enhanced-analytics/project-activity-overview.md).

![](assets/activity-by-team-350x113.png)

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Workfront</a>*</td> 
   <td> <p>Företag eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Översikt över Adobe Workfront-licenser</a>*</td> 
   <td> <p>Granska eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa åtkomst till projekt</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå.<br>Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Information om krav för att använda Förbättrad analys finns i avsnittet Krav i [Förbättrad analys - översikt](../enhanced-analytics/enhanced-analytics-overview.md).

## Förstå aktivitetsbaserad teamvisualisering

De olika aktiviteterna visas i olika färger för att sammanfatta specifika händelser under den filtrerade tidsperioden:

* **Användare som är inloggade**: Lila rutor visar att personer i hemteamet loggade in den dagen. En mörkare ton anger att fler personer loggar in.

   ![](assets/project-activity-users-logged-in.png)

* **Ändring av aktivitetsstatus**: Rutor visar att personer i hemteamet ändrade status för en uppgift den dagen. En mörkare ton anger att ett högre antal uppgiftsstatusvärden ändras.

   ![](assets/project-activity-task-status-changes.png)

* **Slutförda uppgifter**: Blå rutor visar att folk i hemteamet slutförde en uppgift den dagen. En mörkare ton anger att fler uppgifter slutförs.

   ![](assets/project-activity-tasks-completed.png)

När du hovrar över en ruta visas det exakta antalet gånger som åtgärden har slutförts under en viss dag. Du kan välja ett team för att se en beskrivning av dessa aktiviteter för varje person i hemteamet.

Om du ser den här informationen blir det lättare att avgöra:

* Vilka aktiviteter finns inom ett hemteam och i vilken takt.
* Vilka hemteam som jobbar för mycket eller använder systemet mer.
* Om arbetsfördelningen är lämplig för hemteamet.

Om du vill veta hur du får de bästa data för den här visualiseringen kan du läsa [Förbättrad analys - översikt](../enhanced-analytics/enhanced-analytics-overview.md).

## Visa Aktivitet efter teamvisualisering

1. Klicka på ikonen Huvudmeny ![](assets/main-menu-icon-16x12.png)väljer **Analyser**.
1. Välj **Folk**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (Valfritt) Om du vill använda ett annat datumintervall väljer du nya start- och slutdatum från datumintervallfiltret.

   ![](assets/filters-select-date-range-350x344.png)

   Mer information om hur du använder datumintervallfiltret finns i [Använd filter i Förbättrad analys](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Villkorligt) Om du inte har ställt in teamfiltret lägger du till teamfiltret och väljer varje team som du vill se data för.

   Mer information om hur du lägger till filter i Förbättrad analys finns i [Använd filter i Förbättrad analys](../enhanced-analytics/use-enhanced-analytics-filters.md).

   När du har lagt till filter visas data för upp till 50 projekt och filtren förblir aktiva även när du lämnar sidan eller loggar ut från Workfront.

1. (Valfritt) Om du vill zooma in ett datumintervall markerar du en punkt i visualiseringen för början av datumintervallet och drar till slutet av datumintervallet.

   Alla andra visualiseringar uppdateras till samma datumintervall och ett tidsramsfilter skapas.

   ![](assets/timeframe-filter-350x220.png)

1. Klicka på ett teamnamn

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   or role
   </MadCap:conditionalText>
   -->

   om du vill ha mer information om de aktiviteter som har slutförts av hemteamet.

   Listan utökas för att visa aktiviteterna för varje person som tilldelats hemteamet.

   <!--
   <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Role not available</span>
   -->

1. Håll markören över en färgad ruta för att se när användaren slutförde en åtgärd samt hur många gånger åtgärden slutfördes den dagen.

   Mörkare färger anger högre aktivitet.

   ![](assets/activity-by-team-activity-pop-up-350x155.png)

1. (Valfritt) Om du vill exportera visualiseringsdata klickar du på ikonen Exportera ![](assets/export.png) i det övre högra hörnet av visualiseringen väljer du exportformat:

   * **Diagram (PNG)**
   * **Datatabell (XSLX)**


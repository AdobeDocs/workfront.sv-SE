---
title: Visa aktivitetsbaserad teamvisualisering i Förbättrad analys
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: I Activity by team-visualisering visas aktiviteter som inträffar under en viss tidsperiod för ett hemteam, så att du kan förstå hur olika hemteam tillbringade sin tid i Adobe Workfront. Beroende på hur ditt hemteam är konfigurerat i Workfront kan den här visualiseringen ge dig olika insikter och svara på olika frågor.
author: Nolan
feature: Reports and Dashboards
exl-id: c4f9886c-ce76-43a8-bd43-cb64fff27e79
source-git-commit: 59e021aa3ae66e4fc8d9ce9eb57616f948e6cd90
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 0%

---

# Visa aktivitetsbaserad teamvisualisering i Förbättrad analys

>[!IMPORTANT]
>
>Förbättrad analys kommer att tas bort från Workfront den 26 maj. Workfront Data Connect är en ny alternativ lösning som kan användas för att replikera de utökade analyser du använder just nu. <br>Mer information finns i guiden [Borttagning av utökad analys](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md).



<!-- Audited: 12/2023 -->

I Activity by team-visualisering visas aktiviteter som inträffar under en viss tidsperiod för ett hemteam, så att du kan förstå hur olika hemteam tillbringade sin tid i Adobe Workfront. Beroende på hur ditt hemteam är konfigurerat i Workfront kan den här visualiseringen ge dig olika insikter och svara på olika frågor.

>[!NOTE]
>
>Visualiseringen av projektaktiviteten liknar den här visualiseringen, men den visar aktivitet baserat på personer som har tilldelats till projekt i stället för personer som har tilldelats till ett hemteam.\
>Mer information om visualisering av projektaktivitet finns i [Visa visualisering av projektaktivitet i Förbättrad analys](../enhanced-analytics/project-activity-overview.md).

![Aktivitet per team](assets/activity-by-team-350x113.png){width="700"}

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Workfront</a></td> 
   <td> <p>Företag eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Översikt över Adobe Workfront-licenser</a></td> 
   <td>
      <p>Nytt:</p> 
         <ul><li>Ljus eller högre</li></ul>
      <p>Aktuell:</p>
         <ul><li>Granska eller högre</li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa åtkomst till projekt</p> <!--<p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level.<br>For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p>--> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa</p> <!--<p>For information on requesting additional access, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p>--> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Förutsättningar för att använda Förbättrad analys finns i avsnittet Förutsättningar i [Översikt över förbättrade analyser](../enhanced-analytics/enhanced-analytics-overview.md).

## Förstå aktivitetsbaserad teamvisualisering

De olika aktiviteterna visas i olika färger för att sammanfatta specifika händelser under den filtrerade tidsperioden:

* **Användare som är inloggade**: lila rutor visar att personer i hemteamet är inloggade den dagen. En mörkare ton anger att fler personer loggar in.

  ![Användare som är inloggade](assets/project-activity-users-logged-in.png)

* **Statusändring för aktivitet**: Rutor för rosa visar att personer i hemteamet ändrade status för en uppgift den dagen. En mörkare ton anger att ett högre antal uppgiftsstatusvärden ändras.

  ![Aktivitetsstatus ändras](assets/project-activity-task-status-changes.png)

* **Aktiviteter slutförda**: Blå rutor visar att personer i hemteamet slutförde en uppgift den dagen. En mörkare ton anger att fler uppgifter slutförs.

  ![Aktiviteter har slutförts](assets/project-activity-tasks-completed.png)

När du hovrar över en ruta visas det exakta antalet gånger som åtgärden har slutförts under en viss dag. Du kan välja ett team för att se en beskrivning av dessa aktiviteter för varje person i hemteamet.

Om du ser den här informationen blir det lättare att avgöra:

* Vilka aktiviteter finns inom ett hemteam och i vilken takt.
* Vilka hemteam som jobbar för mycket eller använder systemet mer.
* Om arbetsfördelningen är lämplig för hemteamet.

Om du vill lära dig hur du får bästa möjliga data för den här visualiseringen kan du läsa [Översikt över förbättrade analyser](../enhanced-analytics/enhanced-analytics-overview.md).

## Visa Aktivitet efter teamvisualisering

1. Klicka på ikonen Huvudmeny ![Huvudmeny](assets/main-menu-icon-16x12.png) och välj sedan **Analys**.
1. Välj **Personer** i den vänstra panelen.

   ![Området Personer](assets/people-area-cropped-qs-350x276.png)

1. (Valfritt) Om du vill använda ett annat datumintervall väljer du nya start- och slutdatum från datumintervallfiltret.

   ![Välj datumintervall](assets/filters-select-date-range-350x344.png)

   Mer information om hur du använder datumintervallfiltret finns i [Använda filter i Förbättrad analys](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Villkorligt) Om du inte har ställt in teamfiltret lägger du till teamfiltret och väljer varje team som du vill se data för.

   Mer information om hur du lägger till filter i Förbättrad analys finns i [Använda filter i Förbättrad analys](../enhanced-analytics/use-enhanced-analytics-filters.md).

   När du har lagt till filter visas data för upp till 50 projekt och filtren förblir aktiva även när du lämnar sidan eller loggar ut från Workfront.

1. (Valfritt) Om du vill zooma in ett datumintervall markerar du en punkt i visualiseringen för början av datumintervallet och drar till slutet av datumintervallet.

   Alla andra visualiseringar uppdateras till samma datumintervall och ett tidsramsfilter skapas.

   ![Tidsbildrutefilter](assets/timeframe-filter-350x220.png)

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

   ![Aktivitet per team](assets/activity-by-team-activity-pop-up-350x155.png)

1. (Valfritt) Om du vill exportera visualiseringsdata klickar du på ikonen Exportera ![på ikonen Exportera](assets/export.png) i det övre högra hörnet av visualiseringen och väljer sedan exportformat:

   * **Diagram (PNG)**
   * **Datatabell (XSLX)**


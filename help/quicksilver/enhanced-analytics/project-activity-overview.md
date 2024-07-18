---
title: Visa projektaktivitetsvisualisering i Förbättrad analys
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: I projektaktivitetsvisualiseringen visas en sammanställd vy över aktiviteter på projektnivå - aktiviteterna för varje person som tilldelats projektet - som inträffade under en viss tidsperiod. Du kan begränsa ditt fokus för att förstå aktiviteterna i ett projekt eller jämföra projektaktiviteter med andra projekt i Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 9ef52be8-48d0-4f83-a214-dd32e794c73e
source-git-commit: 4e928defe9b6271cef64f6554e91af4fc31ddeca
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 0%

---

# Visa projektaktivitetsvisualisering i Förbättrad analys

<!-- Audited: 12/2023 -->

I projektaktivitetsvisualiseringen visas en sammanställd vy över aktiviteter på projektnivå - aktiviteterna för varje person som tilldelats projektet - som inträffade under en viss tidsperiod. Du kan begränsa ditt fokus för att förstå aktiviteterna i ett projekt eller jämföra projektaktiviteter med andra projekt i Adobe Workfront.

>[!NOTE]
>
>Aktivitet per team-visualisering fungerar på liknande sätt som den här visualiseringen, men med Aktivitet per team visas teamaktiviteter hemma för alla projekt.\
>Mer information om visualisering av aktivitet per team finns i [Visa visualisering av aktivitet per team i Förbättrad analys](../enhanced-analytics/activity-by-team-overview.md).

## Åtkomstkrav

Du måste ha följande:

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
   <td>   <p>Nytt:</p> 
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

## Förutsättningar

Förutsättningar för att använda Förbättrad analys finns i avsnittet Förutsättningar i [Översikt över förbättrade analyser](../enhanced-analytics/enhanced-analytics-overview.md).

## Förstå projektaktivitetsvisualisering

Projektaktiviteter visas i olika färger för att sammanfatta specifika händelser i ett projekt under en tidsperiod:

* **Användare som är inloggade**: lila rutor visar att personer som tilldelats projektet är inloggade den dagen. En mörkare ton anger att fler personer loggar in.

  ![](assets/project-activity-users-logged-in.png)

* **Statusändring för aktivitet**: Rutor för rosa visar att personer har ändrat status för en aktivitet för projektet den dagen. En mörkare ton anger att ett högre antal uppgiftsstatusvärden ändras.

  ![](assets/project-activity-task-status-changes.png)

* **Aktiviteter slutförda**: Blå rutor visar att personer har slutfört en aktivitet för projektet. En mörkare ton anger att fler uppgifter slutförs.

  ![](assets/project-activity-tasks-completed.png)

När du hovrar över en ruta visas det exakta antalet gånger som åtgärden har slutförts under en viss dag. Du kan välja ett projekt om du vill se en beskrivning av aktiviteterna för varje enskild deltagare i projektet.

Om du ser den här informationen blir det lättare att avgöra:

* Aktiviteten i ett visst projekt.
* Ett projekts aktivitet jämfört med andra projekt.
* Vilka användare som arbetar med ett projekt och med vilken frekvens.

Om du vill lära dig hur du får bästa möjliga data för den här visualiseringen kan du läsa [Översikt över förbättrade analyser](../enhanced-analytics/enhanced-analytics-overview.md).

## Visa projektaktivitetsvisualisering

1. Klicka på ikonen Huvudmeny ![](assets/main-menu-icon-16x12.png) och välj sedan **Analys**.
1. (Valfritt) Om du vill använda ett annat datumintervall väljer du nya start- och slutdatum från datumintervallfiltret.

   ![](assets/filters-select-date-range-350x344.png)

   Mer information om hur du använder datumintervallfiltret finns i [Använda filter i Förbättrad analys](../enhanced-analytics/use-enhanced-analytics-filters.md).

   >[!NOTE]
   >
   >Om du väljer ett datumintervall för en period som är längre än tre månader visas inga data i projektaktivitetsvisualiseringen.

1. (Villkorligt) Om du behöver begränsa projektdatauppsättningen markerar och tillämpar du de filter som du vill använda.

   Mer information om hur du lägger till filter i Förbättrad analys finns i [Använda filter i Förbättrad analys](../enhanced-analytics/use-enhanced-analytics-filters.md).

   När du har lagt till filter visas data för upp till 50 projekt och filtren förblir aktiva även när du lämnar sidan eller loggar ut från Workfront.

1. (Valfritt) Om du vill zooma in ett datumintervall markerar du en punkt i visualiseringen för början av datumintervallet och drar till slutet av datumintervallet.

   Alla andra visualiseringar uppdateras till samma datumintervall och ett tidsramsfilter skapas.

   ![](assets/timeframe-filter-350x220.png)

1. (Valfritt) Om du vill ändra hur projekten sorteras klickar du på menyn **Sortera efter** och väljer sedan ett nytt sorteringsalternativ:

   * **A - Z**
   * **Z - A**
   * **Planerat slutförandedatum**
   * **Planerat startdatum**

   Alla andra visualiseringar på sidan uppdateras för att matcha din sorteringsmarkering.

1. (Villkorligt) Om det finns fler än 50 projekt i datauppsättningen använder du pilarna i det nedre vänstra hörnet av visualiseringen för att navigera mellan 50 projekt i en grupp.

   Alla andra visualiseringar på sidan uppdateras så att de matchar sidans val.

   ![](assets/pagination-350x118.png)

1. Klicka på ett projekt i visualiseringen för att se mer information om projektet.

   Listan utökas för att visa aktiviteterna för varje enskild deltagare i projektet.

1. För musen över en ruta för att se vilket datum användaren slutförde en åtgärd samt hur många gånger åtgärden slutfördes för den dagen.

   ![](assets/project-activity-activity-pop-up-350x137.png)

1. (Valfritt) Om du vill exportera visualiseringsdata klickar du på ikonen **Exportera** ![](assets/export.png) i det övre högra hörnet av visualiseringen och väljer sedan exportformat:

   * **Diagram (PNG)**
   * **Datatabell (XSLX)**


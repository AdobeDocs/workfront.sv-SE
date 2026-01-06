---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visa faktiska timmar
description: De timmar du loggar in på dina arbetsuppgifter i Adobe Workfront räknas som faktiska timmar. Faktiska timmar representerar den faktiska tid det tog för dig att slutföra en uppgift, ett ärende eller ett projekt.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1276'
ht-degree: 0%

---

# Visa faktiska timmar

<!-- Audited: 5/2025 -->

De timmar du loggar in på dina arbetsuppgifter i Adobe Workfront räknas som faktiska timmar.

Faktiska timmar representerar den faktiska tid det tog för dig att slutföra en uppgift, ett ärende eller ett projekt.

Vi rekommenderar att timmar loggas på arbetsuppgifter, som är uppgifter och problem. Som Workfront-administratör kan du dock tillåta användare att även logga in på projekt beroende på organisationens arbetsflöden.

Mer information om hur du konfigurerar systemet så att användare kan logga in på projekt finns i [Konfigurera tidrapport och timinställningar](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

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
   <p>Standard<p>
   <p>Arbeta eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa eller ge senare åtkomst till uppgifter, projekt eller ärenden</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter för en aktivitet, ett projekt eller ett problem</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
 
 <table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   <p>New: Standard<p>
   <p>Or</p>
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to Tasks, Projects, or Issues</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a task, a project, or an issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Faktiska timmar kontra äldre faktiska timmar

Beroende på vilket område av Workfront du kommer åt de faktiska timmarna från kan de hänvisa till någon av följande loggade timmar:

* I projekt, uppgifter och utfärda rapporter och listor:

   * **Faktiska timmar**: Timmar som loggats för projekt, uppgifter eller problem mellan maj 2021 och idag. De lagras i Workfront-databasen i timmar och deras värdefält är `actualWorkRequiredDouble`.
   * **Tidigare faktiska timmar**: Timmar som loggats för projekt, uppgifter eller utgåvor när som helst, mellan ett datum före maj 2021 och idag. De lagras i Workfront-databasen som minuter och deras värdefält är `actualWorkRequired`.

     Timmar som loggas för närvarande uppdaterar både den faktiska och den gamla faktiska timmen.

     >[!IMPORTANT]
     >
     >Projektets faktiska kostnad använder äldre faktiska timmar för beräkning.

* I området med projekt-, uppgifts- eller utleveransinformation kan faktiska timmar visas i följande fält:

   * **Faktiska timmar**: På fliken Detaljer är detta timmar som loggats för projekt, uppgifter eller problem mellan maj 2021 och idag. De lagras i Workfront-databasen i timmar och deras värdefält är `actualWorkRequiredDouble`.
   * **Faktiska timmar**: I ett projekt, en aktivitet eller ett utleverans i ett anpassat formulär, när de öppnas med hjälp av ett anpassat fält för intern fältreferens som refererar till fältet för faktiska timmar. Detta är timmar som loggats för projekt, uppgifter eller problem mellan ett datum före maj 2021 och idag. De lagras i Workfront-databasen i timmar och deras värdefält är `actualWorkRequiredDouble`.

     Timmar som loggas för närvarande uppdaterar både den faktiska och den gamla faktiska timmen.

>[!NOTE]
>
>Vi rekommenderar att du använder fältet Faktiska timmar när det är möjligt, eftersom fältet Gammalt antal faktiska timmar kan visa felaktiga timmar på grund av det sätt på vilket ökningar avrundas när timmar lagras i minuter.

## Faktiska timmar för uppgifter och ärenden jämfört med faktiska timmar för projekt

De faktiska timmarna för uppgifter och problem representerar antalet timmar som loggas direkt på uppgifter och problem.

Faktiska timmar från underordnade uppgifter summeras till Faktiska timmar för den överordnade aktiviteten. Följande formel gäller för de faktiska timmarna för en överordnad uppgift:

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

Faktiska timmar för projekt representerar totalt antal faktiska timmar från alla projektaktiviteter (inklusive timmar som loggas direkt på överordnade aktiviteter), alla projektfrågor och faktiska timmar som loggats på själva projektet.

Följande formel gäller för de faktiska timmarna i ett projekt:

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## Hitta faktiska timmar

Att hitta värdet för Faktiska timmar för ett objekt är identiskt för uppgifter, projekt och utgåvor.

### Faktiska timmar i detaljavsnittet {#actual-hours-in-the-details-section}

Att hitta faktiska timmar i detaljavsnittet är identiskt för projekt, uppgifter och ärenden.

Så här hittar du faktiska timmar i Uppgiftsinformation:

1. Gå till en uppgift som du vill granska de faktiska timmarna för.
1. Klicka på **Uppgiftsinformation** i den vänstra panelen. Avsnittet **Översikt** visas.
1. Leta reda på värdet **Faktiska timmar** i avsnittet **Arbetstid**. Detta är det totala antalet timmar som loggats för den här aktiviteten.
1. (Valfritt och villkorligt) Om den inbyggda fältreferensen för faktiska timmar har lagts till i ett anpassat formulär för ett projekt, en uppgift eller ett ärende går du till det anpassade formuläret och letar upp de faktiska timmarna i det anpassade fältet. Detta är det totala antalet loggade timmar för objektet.

### Faktiska timmar i timavsnittet {#actual-hours-in-the-hours-section}

Att hitta faktiska timmar i avsnittet Timmar är identiskt för projekt, uppgifter och ärenden.

Så här hittar du faktiska timmar under Timmar för en uppgift:

1. Gå till en uppgift som du vill granska de faktiska timmarna för.

1. Klicka på **Timmar** i den vänstra panelen. En lista med timposter som är inloggade på aktiviteten visas, med kolumnen **Timmar** som visar det totala antalet faktiska timmar för aktiviteten.

1. Se till att grupperingen **Standard** och **Project** används i den här listan.
1. Aktivitetens faktiska timmar visas på grupperingsraden för kolumnen **Faktiska timmar**.

### Faktiska timmar och faktiska/gamla timmar i rapporter

När du skapar uppgifter, utgåvor eller projektrapporter kan du visa värdena för Faktiska timmar och Gammal faktisk timme för varje uppgift, utgåva eller projekt i rapporten.

Mer information om skillnaden mellan faktiska timmar och gamla faktiska timmar finns i avsnittet [Faktiska timmar kontra äldre faktiska timmar](#actual-hours-vs-legacy-actual-hours) i den här artikeln.

Så här visar du faktiska timmar och faktiska/gamla timmar i en uppgiftsrapport:

{{step1-to-reports}}

1. Klicka på **Ny rapport** på sidan **Rapporter** och välj sedan **Aktivitet** som objekt.
1. Klicka på **Lägg till kolumn** längst ned till höger på sidan.
1. I listrutan **Visa i den här kolumnen** börjar du skriva **Faktiska timmar** och markerar sedan fältet när det visas i listan.
1. Upprepa steget ovan om du vill lägga till fältet **Äldre faktiska timmar** i rapporten.

1. Klicka på **Spara + stäng** längst ned till vänster på sidan för att spara rapporten.

1. Ange ett nytt rapportnamn i dialogrutan **Namnge den här rapporten för att spara den** och klicka sedan på **Använd**.
1. Upprepa samma steg för ett projekt eller en problemrapport.

### Faktiska timmar i resurshanteringsverktyg {#actual-hours-in-resource-management-tools}

Om du vill se hur arbetet med tilldelade uppgifter och ärenden fortskrider kan du visa dem i följande verktyg för resurshantering:

* Användningsrapporten.\
  Mer information finns i [Översikt över resursanvändningsrapporten](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* Resursplaneraren.

  Mer information finns i [Visa tillgängliga, planerade och faktiska timmar eller FTE i resursplaneraren när du använder användarvyn](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).


### Faktiska timmar i Workfront API

<!--this section was added as a result to this issue: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/6810910e0001b932e0948336208e76f2/overview-->

De flesta fält i Workfront som lagrar timmar sparas i Workfront-databasen på några minuter. Namnet på fältet Planerade timmar för en aktivitet är till exempel `workRequired` i Workfront-databasen och lagras i minuter.

Du måste ta hänsyn till konverteringen från minuter till timmar när du får åtkomst till dessa fält i API-anrop eller i beräknade anpassade fält eller kolumner.

De faktiska timmarna som loggats för projekt, uppgifter eller utgåvor lagras för närvarande i Workfront-databasen som minuter och deras värdefält är `actualWorkRequired`.

Med följande version av Workfront API som ska släppas senare under 2025 lagras Faktiska timmar i följande fält och enheter i databasen:

* **Faktiska timmar**: Timmar som loggats för projekt, uppgifter eller problem efter maj 2021. De lagras i Workfront-databasen i timmar och deras värdefält är `actualWorkRequiredDouble`.
* **Tidigare faktiska timmar**: Timmar som loggats för projekt, uppgifter eller problem när som helst, inklusive före maj 2021. De lagras i Workfront-databasen som minuter och deras värdefält är `actualWorkRequired`.

Mer information om API-versioner finns i [API-versionshantering och supportschema](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

>[!IMPORTANT]
>
>Projektets faktiska kostnad använder äldre faktiska timmar för beräkning.

Mer information om hur du använder Faktiska timmar i beräknade kolumner eller fält finns i [Rapportera vanliga frågor och svar](/help/quicksilver/reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md).

## Loggtid

Du kan logga tid på uppgifter, problem och projekt på flera sätt.

Mer information finns i [Loggtid](../../../timesheets/create-and-manage-timesheets/log-time.md).

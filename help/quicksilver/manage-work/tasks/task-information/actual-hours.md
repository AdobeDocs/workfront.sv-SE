---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visa faktiska timmar
description: De timmar du loggar in på dina arbetsuppgifter i Adobe Workfront räknas som faktiska timmar.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: 3827e834a71084f14a99cb27aadefd97327b02d7
workflow-type: tm+mt
source-wordcount: '759'
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

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> 
   <p>Nytt: Standard<p>
   <p>eller</p>
   <p>Aktuell: Arbete eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa eller ge senare åtkomst till uppgifter, projekt eller ärenden</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter för en aktivitet, ett projekt eller ett problem</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

Information om faktiska timmar finns på följande platser:

* [Faktiska timmar i detaljavsnittet](#actual-hours-in-the-details-section)
* [Faktiska timmar i timavsnittet](#actual-hours-in-the-hours-section)
* [Faktiska timmar i rapporter](#actual-hours-in-reports)
* [Faktiska timmar i resurshanteringsverktyg](#actual-hours-in-resource-management-tools)

### Faktiska timmar i detaljavsnittet {#actual-hours-in-the-details-section}

Att hitta faktiska timmar i detaljavsnittet är identiskt för projekt, uppgifter och ärenden.

Så här hittar du faktiska timmar i Uppgiftsinformation:

1. Gå till en uppgift som du vill granska de faktiska timmarna för.
1. Klicka på **Uppgiftsinformation** i den vänstra panelen. Avsnittet **Översikt** visas.
1. Leta reda på värdet **Faktiska timmar** i avsnittet **Arbetstid**. Detta är det totala antalet timmar som loggats för den här aktiviteten.

### Faktiska timmar i timavsnittet {#actual-hours-in-the-hours-section}

Att hitta faktiska timmar i avsnittet Timmar är identiskt för projekt, uppgifter och ärenden.

Så här hittar du faktiska timmar i avsnittet Timmar:

1. Gå till en uppgift som du vill granska de faktiska timmarna för.

1. Klicka på **Timmar** i den vänstra panelen. En lista med timposter som är inloggade på aktiviteten visas, med kolumnen **Timmar** som visar det totala antalet faktiska timmar för aktiviteten.

1. Se till att grupperingen **Standard** och **Project** används i den här listan.

### Faktiska timmar i rapporter {#actual-hours-in-reports}

När du skapar aktiviteter, utgåvor eller projektrapporter kan du visa värdet för Faktiska timmar för varje uppgift, utgåva eller projekt i rapporten.

Så här visar du faktiska timmar i en uppgiftsrapport:

{{step1-to-reports}}

1. Klicka på **Ny rapport** på sidan **Rapporter** och välj sedan **Aktivitet** som objekt.
1. Klicka på **Lägg till kolumn** längst ned till höger på sidan.
1. I listrutan **Visa i den här kolumnen** som visas börjar du skriva **Faktiska timmar** och markerar sedan fältet när det visas i listan.

1. Klicka på **Spara + stäng** längst ned till vänster på sidan för att spara rapporten.

1. Ange ett nytt rapportnamn i dialogrutan **Namnge den här rapporten för att spara den** och klicka sedan på **Använd**.

### Faktiska timmar i resurshanteringsverktyg {#actual-hours-in-resource-management-tools}

Om du vill se hur arbetet med tilldelade uppgifter och ärenden fortskrider kan du visa dem i följande verktyg för resurshantering:

* Användningsrapporten.\
  Mer information finns i [Översikt över resursanvändningsrapporten](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* Resursplaneraren.

  Mer information finns i [Visa tillgängliga, planerade och faktiska timmar eller FTE i resursplaneraren när du använder användarvyn](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).

## Loggtid

Du kan logga tid på uppgifter, problem och projekt på flera sätt.

Mer information finns i [Loggtid](../../../timesheets/create-and-manage-timesheets/log-time.md).

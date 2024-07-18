---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visa faktiska timmar
description: De timmar du loggar in på dina arbetsuppgifter i Adobe Workfront räknas som faktiska timmar.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# Visa faktiska timmar

De timmar du loggar in på dina arbetsuppgifter i Adobe Workfront räknas som faktiska timmar.

Faktiska timmar representerar den faktiska tid det tog för dig att slutföra en uppgift, ett ärende eller ett projekt.

Vi rekommenderar att timmar loggas på arbetsuppgifter, som är uppgifter och problem.

Som Workfront-administratör kan du dock även tillåta användare att logga in på projekt, beroende på vilka arbetsflöden som finns i organisationen.

Mer information om hur du konfigurerar systemet så att användare kan logga in på projekt finns i [Konfigurera tidrapport och timinställningar](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

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
   <td> <p>Arbeta eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa eller ge senare åtkomst till uppgifter, projekt eller ärenden</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter för en aktivitet, ett projekt eller ett problem</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Faktiska timmar för uppgifter och ärenden jämfört med faktiska timmar för projekt

De faktiska timmarna för uppgifter och problem representerar antalet timmar som loggas direkt på uppgifter och problem.

>[!NOTE]
>
>Faktiska timmar från underordnade uppgifter summeras till Faktiska timmar för den överordnade aktiviteten. Följande formel gäller för de faktiska timmarna för en överordnad uppgift:

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

Faktiska timmar för projekt representerar totalt antal faktiska timmar från alla aktiviteter i projektet (inklusive timmar som loggas direkt på överordnade aktiviteter), alla problem i projektet samt faktiska timmar som loggats i själva projektet.

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
1. Klicka på **Uppgiftsinformation** i den vänstra panelen.
1. Klicka på **Översikt** och observera värdet för **Faktiska timmar**.

   Detta är det totala antalet timmar som loggats för den här aktiviteten.

### Faktiska timmar i timavsnittet {#actual-hours-in-the-hours-section}

Att hitta faktiska timmar i avsnittet Timmar är identiskt för projekt, uppgifter och ärenden.

Så här hittar du faktiska timmar i avsnittet Timmar:

1. Gå till en uppgift som du vill granska de faktiska timmarna för.
1. Klicka på **Timmar** i den vänstra panelen.

   Beroende på din konfiguration kan avsnittet Timmar visas under **Visa mer**.

   Här visas en lista med timposter som är inloggade på uppgiften.

1. Se till att grupperingen **Standard** och **Project** används i den här listan.

   Numret som visas i grupperingsraden för kolumnen **Timmar** är det totala antalet faktiska timmar för aktiviteten.

### Faktiska timmar i rapporter {#actual-hours-in-reports}

När du skapar aktiviteter, utgåvor eller projektrapporter kan du visa värdet för Faktiska timmar för varje uppgift, utgåva eller projekt i rapporten.

Att lägga till kolumnen Faktiska timmar i en uppgiftsvy liknar att skapa en vy i en rapport.

Så här visar du faktiska timmar i en uppgiftsrapport:

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Rapporter**.
1. Klicka på **Ny rapport** och välj sedan **Aktivitet** som objekt.

1. Klicka på **Lägg till kolumn** och börja skriva **Faktiska timmar** när listrutan **Visa i den här kolumnen** visas. Markera fältet när det visas i listan.

1. Klicka på **Spara + stäng** för att spara rapporten.

   I kolumnen Faktiska timmar visas antalet timmar som loggats för varje uppgift.

### Faktiska timmar i resurshanteringsverktyg {#actual-hours-in-resource-management-tools}

Om du vill se hur arbetet med tilldelade uppgifter och ärenden fortskrider kan du visa dem i följande verktyg för resurshantering:

* Användningsrapport.\
  Mer information om användningsrapporten finns i [Översikt över resursanvändningsrapporten](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* Resursplanering.

  Information om hur du visar faktiska timmar i resursplaneraren finns i [Visa tillgängliga, planerade och faktiska timmar eller FTE i resursplaneraren när du använder användarvyn](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).

## Loggtid

Du kan logga tid på uppgifter, problem och projekt på flera sätt.

Mer information om loggningstid i Workfront finns i [Loggtid](../../../timesheets/create-and-manage-timesheets/log-time.md).

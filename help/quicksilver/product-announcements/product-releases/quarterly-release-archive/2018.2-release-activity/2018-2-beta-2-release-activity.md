---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 Beta 2 - versionsaktivitet
description: Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i 2018.2 Beta 2. Funktionerna gjordes tillgängliga i förhandsvisningsmiljön den 5 april 2018. Den kommer att göras tillgänglig i produktionsmiljön i juni 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: c8ef68f5-53db-4c3c-af0f-e1c98521ec27
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# 2018.2 Beta 2 - versionsaktivitet

Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i 2018.2 Beta 2. Funktionerna gjordes tillgängliga i förhandsvisningsmiljön den 5 april 2018. Den kommer att göras tillgänglig i produktionsmiljön i juni 2018.

>[!IMPORTANT]
>
> Funktionerna som beskrivs på den här sidan kan ändras innan de är tillgängliga i produktionsmiljön.

En lista över alla ändringar som gjorts under 2018.2 finns på  [Aktivitetsöversikt för 2018.2-utgåvan](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

Beta 2-versionen från 2018.2 innehåller följande förbättringar:

* [Redigera fält direkt från hemområdet](#edit-fields-directly-from-the-home-area)
* [Loggtid i dagar](#log-time-in-days)
* [Visa korsprojektsrelationer i Gantt-schemat i en projektlista](#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects)
* [Använd budgeterad kostnad i Portfolio-optimering för att beräkna Portfolio-ekonomi](#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances)
* [Användningsrapport: Fyller i budgeterade timmar från det nya resursbudgeteringsområdet](#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area) (Endast förhandsvisning)

* [Användningsrapport: Visa budgeterade timmar per användare i ett projekt](#utilization-report-view-budgeted-hours-by-user-on-a-project) (Endast förhandsvisning)

* [Korrekturstatus från dokumentlistan som är tillgänglig för icke-språkliga användare](#proof-progress-from-the-document-list-available-to-non-proofing-users)
* [Mobilförbättringar](#mobile-improvements)

## Redigera fält direkt från hemområdet {#edit-fields-directly-from-the-home-area}

När du nu markerar ett objekt i området Hem kan du redigera fält som är kopplade till det objektet direkt från den högra panelen i området Hem. 

Före den här ändringen gick det bara att visa information i hemområdet, inte redigerad.

Mer information finns i [Uppdatera eller redigera en arbetsuppgift i hemområdet](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md) i artikeln  [Uppdatera eller redigera en arbetsuppgift i hemområdet](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).

## Loggtid i dagar {#log-time-in-days}

Workfront-administratörer kan nu konfigurera om användare i sin organisations loggtid i dagar eller timmar. Användare med en planeringslicens kan konfigurera den här inställningen för sig själva.

Före den här ändringen kunde användaren bara logga tiden i timmar.

Du kan konfigurera den här inställningen genom att redigera användarprofilen. Mer information finns i [Konfigurera om tid är inloggad i timmar eller dagar](../../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md).

Mer information om hur användare kan logga tid i dagar efter att den här inställningen har uppdaterats finns i [Loggtid](../../../../timesheets/create-and-manage-timesheets/log-time.md).

## Visa korsprojektsrelationer i Gantt-schemat i en projektlista {#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects}

Du kan nu visa korsprojektsrelationer i Gantt-diagrammet i följande projektlistor:

* Fliken Projekt i en portfölj eller ett program
* I en projektrapport

Före den här ändringen kunde du bara visa korsprojektsrelationer för enskilda uppgifter på projektnivå.

Mer information finns i [Konfigurera hur information visas i Gantt-schemat](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). 

## Använd budgeterad kostnad i Portfolio-optimering för att beräkna Portfolio-ekonomi {#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances}

I nya Portfolio Optimizer används nu den budgeterade kostnaden från det nya området Resursbudgetering i affärsärendet eller från resursplaneraren för att beräkna följande fält:

* Nettovärde
* Avkastning på investering
* Kostnad

Tidigare använde både den nya och den gamla Portfolio-optimeraren den gamla budgeterade kostnaden. Den gamla Portfolio-optimeraren använder fortfarande den gamla budgeterade kostnaden för att beräkna nettovärde, avkastning på investering och kostnad.

Vi har också lagt till två nya fält i Portfolio Financial Fields: Legacy ROI och Legacy Net Value för att hämta in de nya värdena från de nya resurshanteringsverktygen.

Mer information finns i [Portfolio Optimizer - översikt](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md) i artikeln  [Portfolio Optimizer - översikt](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

## Användningsrapport: Fyller i budgeterade timmar från det nya resursbudgeteringsområdet {#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area}

>[!NOTE]
>
>Den här funktionen kommer inte att ingå i den officiella versionen till förhandsvisningsmiljön i version 2018.2. Den kommer att återinföras under betaperioden för version 2018.3 och kommer att släppas ut i produktionsmiljön i version 2018.3. 

Budgeterade timmar i utnyttjanderapporten fylls nu i från information som är tillgänglig i det nya området Resursbudgetering i affärsärendet.

Före den här ändringen användes information från det tidigare området Resursberäkning.

Mer information finns i [Översikt över resursanvändningsrapporten](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) i artikeln  [Översikt över resursanvändningsrapporten](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Användningsrapport: Visa budgeterade timmar per användare i ett projekt {#utilization-report-view-budgeted-hours-by-user-on-a-project}

>[!NOTE]
>
>Den här funktionen kommer inte att ingå i den officiella versionen till förhandsvisningsmiljön i version 2018.2. Den kommer att återinföras under betaperioden för version 2018.3 och kommer att släppas ut i produktionsmiljön i version 2018.3. 

Användningsrapporten för ett projekt visar nu Budgeterade timmar per användare.

Före den här ändringen visade användningsrapporten endast budgeterade timmar per jobbroll. 

Mer information finns i [Översikt över resursanvändningsrapporten](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) i artikeln [Översikt över resursanvändningsrapporten](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Korrekturstatus från dokumentlistan som är tillgänglig för icke-språkliga användare {#proof-progress-from-the-document-list-available-to-non-proofing-users}

Bevisföringsindikatorer (Skickat, Öppnad, Kommentarer gjorda och Beslut) visas nu för alla användare när dokumentlistan visas. Detta gäller även användare som inte kan generera korrektur (mer information om hur du aktiverar användare för att generera korrektur finns i avsnittet .

Före den här ändringen fanns det bara bevis på förloppsindikatorer tillgängliga för användare som kunde generera korrektur.

Mer information finns i [Översikt över korrektur och status](../../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md).

## Mobilförbättringar {#mobile-improvements}

Mobilappen innehåller följande förbättringar:

* Länkar som delas med dig i andra mobilprogram öppnas nu i Workfront mobilapp.

  Mer information om delning av länkar finns i .

  Den här uppdateringen är nu tillgänglig på iOS och Android.

* Vi har uppdaterat våra supportkrav för iOS-plattformen för iPhone X.

  Mer information om vilka mobila enheter och operativsystem som stöds finns i . 

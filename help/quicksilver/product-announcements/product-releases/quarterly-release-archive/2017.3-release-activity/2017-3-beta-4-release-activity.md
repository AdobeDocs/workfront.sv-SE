---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.3 Beta 4 - versionsaktivitet
description: Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i 2017.3 Beta 4. Funktionerna på den här sidan var tillgängliga i förhandsvisningsmiljön den 25 september 2017. Den kommer att göras tillgänglig i produktionsmiljön i början av november 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d6bb889c-a057-453f-8f80-761cfb1ad4a1
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '1676'
ht-degree: 0%

---

# 2017.3 Beta 4 - versionsaktivitet

Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i 2017.3 Beta 4. Funktionerna på den här sidan var tillgängliga i förhandsvisningsmiljön den 25 september 2017. Den kommer att göras tillgänglig i produktionsmiljön i början av november 2017.

>[!IMPORTANT]
>
> Funktionerna som beskrivs på den här sidan kan ändras innan de är tillgängliga i produktionsmiljön.

En lista över alla ändringar som gjorts under 2017.3 finns på  [Aktivitetsöversikt för version 2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

2017.3 Beta 4 innehåller förbättringar för både Workfront-administratörer och andra användare:

**För administratörer**

* [Nytt inställningsområde för resurshantering i inställningsområdet](#new-resource-management-preferences-area-in-the-setup-area)

**För alla användare**

* [Duplicera aktiviteter](#duplicate-tasks)
* [Automatisera tilldelningar vid schemaläggning av resurser](#automate-assignments-when-scheduling-resources)
* [Ändra tilldelningar för flera aktiviteter vid schemaläggning av resurser](#modify-assignments-for-multiple-tasks-when-scheduling-resources)
* [Använd FTE-distribution i resursplaneraren](#apply-fte-distribution-to-the-resource-planner)
* [Avsnitt för jobbroll för användarinställningar inkluderar procent av FTE-tillgänglighet](#job-role-section-for-user-settings-includes-percentage-of-fte-availability)
* [Spara och hantera filter i användningsrapporten för ett projekt](#save-and-manage-filters-in-the-utilization-report-on-a-project)
* [Ytterligare filteralternativ i användningsrapporten](#additional-filtering-options-in-the-utilization-report)
* [Visa användningsrapporten per program eller Portfolio](#view-the-utilization-report-by-program-or-portfolio)
* [Visa ursprunglig probleminformation i projekt- och aktivitetsrapporter](#show-original-issue-information-in-project-and-task-reports)
* [Filtersystemsuppdateringar i uppdateringsströmmen är nu beständiga över objekt](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [Rapport om aktiva korrekturstadier i Workfront](#report-on-active-proof-stages-within-workfront)
* [Tilldela anpassade Workfront Proof-behörighetsprofiler till användare i Workfront](#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront)
* [Timresurs tillagd i händelseprenumerationer](#hour-resource-added-to-event-subscriptions)

## Duplicera uppgifter {#duplicate-tasks}

Nu kan du snabbt duplicera en uppgift eller en uppsättning uppgifter i ett projekt. Den här åtgärden skapar en identisk uppgift med den ursprungliga. Det finns inga ytterligare alternativ under dupliceringsprocessen som gör att du kan göra ändringar i den nya uppgiften.  

Före den här ändringen kan du kopiera en uppgift till antingen ett nytt projekt eller det befintliga projektet och ändra viss information medan du kopierade den.

För  Mer information om att duplicera uppgifter finns i [Kopiera och duplicera uppgifter](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

## Automatisera tilldelningar vid schemaläggning av resurser {#automate-assignments-when-scheduling-resources}

>[!NOTE]
>
>Verktygen för resursschemaläggning har tagits bort från Workfront i version 23.1. Mer information om att schemalägga resurser med hjälp av belastningsutjämnaren finns i [Översikt över belastningsutjämnaren](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Nu kan du låta Workfront automatiskt föreslå tilldelningar för ej tilldelade uppgifter och ärenden när resurser för flera projekt schemaläggs (från fliken Schemaläggning) eller när resurser för ett enskilt projekt schemaläggs (från fliken Personal).

Workfront analyserar aktuella arbetsuppgifter för alla era tillgängliga användare och föreslår intelligenta, logiska tilldelningar för uppgifter och ärenden som ännu inte har tilldelats. Du kan ändra alla föreslagna eller befintliga tilldelningar innan du slutför tilldelningarna.

Mer information finns i &quot;Tilldela ej tilldelade uppgifter och ärenden manuellt i schemaläggningsområden&quot;.

## Ändra tilldelningar för flera aktiviteter vid schemaläggning av resurser {#modify-assignments-for-multiple-tasks-when-scheduling-resources}

När du tilldelar, byter eller frigör flera användare samtidigt när du schemalägger resurser (antingen från fliken Schemaläggning eller från fliken Tillstånd) kan du nu ändra tilldelningar för specifika uppgifter som du anger (inklusive alla underaktiviteter och tillhörande ärenden) i ett eller flera projekt.

Före den här ändringen kan du bara ändra tilldelningar till aktiviteter och ärenden i hela projekt (du kunde inte ange specifika uppgifter i ett projekt).

Mer information finns i &quot;Tilldela ej tilldelade uppgifter och ärenden manuellt i schemaläggningsområden&quot;.

## Tillämpa FTE-distribution på resursplaneraren {#apply-fte-distribution-to-the-resource-planner}

>[!NOTE]
>
>Den här funktionen är för närvarande inte tillgänglig i Förhandsgranska i alla kluster.

Nu kan du visa rätt antal tillgängliga timmar för varje roll för användaren baserat på procentandelen FTE-tillgänglighet för varje roll när användare har mer än en roll.

Om schemat för en användare till exempel visar att de är tillgängliga för arbete 100 timmar på en månad och deras procentuella FTE-tillgänglighet för den primära rollen är 75 % och procentandelen FTE-tillgänglighet för den andra rollen är 25 %, visas i resursplaneraren 75 tillgängliga timmar under den primära rollen och med 25 tillgängliga timmar under deras andra roll.

Innan den här ändringen utfördes associerades namnet på användaren som endast visades i resursplaneraren för den primära rollen, och användarens fullständiga tillgänglighet baserat på användarens schema (100 timmar) endast med den primära rollen. Användarens Andra roll visas bara i resursplaneraren om användaren har tilldelats en aktivitet i den rollen och de tillgängliga timmarna för användaren i den andra rollen var noll.

Mer information om hur tillgängliga timmar och tillgängliga heltidsanställda beräknas för användare och roller i resursplaneraren finns i [Översikt över beräkning av timmar och heltidsanställda för användare och roller i resursplaneraren](../../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

## Avsnitt för jobbroll för användarinställningar inkluderar procent av FTE-tillgänglighet {#job-role-section-for-user-settings-includes-percentage-of-fte-availability}

>[!NOTE]
>
>Den här funktionen är för närvarande inte tillgänglig i Förhandsgranska i alla kluster.

När du nu uppdaterar en användarprofil kan du lägga till ytterligare jobbroller till en användare och definiera procentandelen FTE som tilldelats till varje jobbroll.

Före den här ändringen kunde du inte tilldela en viss mängd FTE till någon av de jobbroller som användaren var associerad med.

Mer information om hur du uppdaterar procentandelen FTE-tillgänglighet för användarens jobbroller finns i [Redigera en användares profil](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) eller [Konfigurera mina inställningar](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

## Nytt inställningsområde för resurshantering i inställningsområdet {#new-resource-management-preferences-area-in-the-setup-area}

Du kan nu hitta ett nytt område under Resurshantering i installationsprogrammet. I det här området har vi infört en inställning som gör att du kan ange hur användartillgängligheten ska beräknas i resursplaneraren. Du kan beräkna den på följande sätt:

* Manuellt: Standardschemat för systemet används tillsammans med användarens enskilda FTE för att avgöra användarens tillgänglighet per timme i Resursplaneraren. Användarens schema ignoreras.
* Automatiskt: Användarens schema används för att avgöra användarens tillgänglighet per timme i resursplaneraren. FTE-tillgängligheten beräknas baserat på användarens schema och standardschema. Värdet för användarens FTE ignoreras. 

Mer information om hur du konfigurerar inställningar för resurshantering för ditt system finns i [Konfigurera inställningar för resurshantering](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Spara och hantera filter i användningsrapporten för ett projekt {#save-and-manage-filters-in-the-utilization-report-on-a-project}

Nu kan du spara filter som du skapar i användningsrapporten. Dessutom kan du byta namn på ett sparat filter, duplicera ett sparat filter, ta bort ett sparat filter eller ändra ett sparat filter.

Tidigare var du tvungen att ange individuella filteralternativ varje gång du filtrerade användningsrapporten.

Mer information om att spara och hantera filter i användningsrapporten finns i [Översikt över resursanvändningsrapporten](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) i [Översikt över resursanvändningsrapporten](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Ytterligare filteralternativ i användningsrapporten {#additional-filtering-options-in-the-utilization-report}

När du kör användningsrapporten är nu nya filtreringsfält för Portfolio, Program och Projekt tillgängliga när du skapar filtret, utöver de uppgifter, ärenden och roller som tidigare fanns tillgängliga.

Före den här ändringen kunde du bara filtrera efter portfölj, program och projekt genom att lägga till en ny filterregel.

Mer information finns i [Översikt över resursanvändningsrapporten](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) i [Översikt över resursanvändningsrapporten](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Visa användningsrapporten per program eller Portfolio {#view-the-utilization-report-by-program-or-portfolio}

Nu kan du visa en användningsrapport per program eller portfölj. På så sätt kan du se information från flera projekt i en enda användningsrapport.

För att underlätta den här ändringen är fliken Användning nu tillgänglig både i rapportområdet inom Workfront och i ett enskilt projekt.

Innan den här ändringen utfördes gick det endast att få åtkomst till användningsrapporter inom ett projekt.

Mer information finns i  [Översikt över resursanvändningsrapporten](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md). 

## Visa ursprunglig probleminformation i projekt- och aktivitetsrapporter {#show-original-issue-information-in-project-and-task-reports}

>[!NOTE]
>
>Den här funktionen är för närvarande inte tillgänglig i Förhandsgranska i alla kluster.

Du kan nu hitta följande information om det ursprungliga problemet i ett projekt eller en uppgiftsrapport för de projekt och uppgifter som skapades när ett problem konverterades:

* Ursprungligt utgivningsdatum
* Ursprungligt problemnamn
* Originalnummer för utgåvans upphovsman-ID

Den här informationen kan visas i en uppgifts- eller projektrapport eller i en lista genom att skapa en anpassad vy i textläge.

Före den här ändringen kunde du inte rapportera om den här informationen.

Mer information om hur du skapar den anpassade textlägesvyn som hämtar information från det ursprungliga problemet finns i [Visa information om ursprungliga problem i uppgifts- eller projektlistor](../../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

## Filtersystemsuppdateringar i uppdateringsströmmen är nu beständiga över objekt {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

>[!NOTE]
>
>Den här funktionen släpptes inte i förhandsvisningsmiljön med Beta 4. Det kommer att vara tillgängligt i Förhandsgranska under första halvan av oktober.

Alternativet Filtersystemuppdateringar är nu beständigt över objekt på hela Workfront-webbplatsen. På så sätt kan du dölja systemuppdateringar och endast visa användarkommentarer i uppdateringsströmmen för ett objekt, och du behåller den inställningen när du bläddrar till andra objekt.

Innan den här ändringen genomfördes var du tvungen att välja att filtrera bort systemuppdateringar för varje objekt när du surrade på Workfront webbplats.

Mer information finns i [Uppdatera arbete](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Rapport om Active Proof Stages i Workfront {#report-on-active-proof-stages-within-workfront}

När du skapar en dokumentversionsrapport i Workfront finns det nu en kolumn som heter&quot;Active Proof Stages&quot;. I den här kolumnen kan du visa korrekturscenen som är aktiv för varje dokumentversion i rapporten. Scenens namn visas i kolumnen &quot;Aktiva korrekturstadier&quot;. Om ingen scen är aktiv i dokumentversionen är kolumnen tom.

Mer information om tillgängliga fält i vyer och rapporter finns i [Ordlista för Adobe Workfront-terminologi](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Tilldela anpassade Workfront Proof-behörighetsprofiler till användare i Workfront {#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront}

När du nu aktiverar språkfunktioner för en användare i Workfront kan du tilldela en anpassad Workfront Proof-behörighetsprofil. 

Före den här ändringen var endast följande behörighetsprofiler tillgängliga: Ansvarig, Hanterare, Administratör.

## Timresurs tillagd i händelseprenumerationer {#hour-resource-added-to-event-subscriptions}

Med den nya timresursen kan du nu skapa en evenemangsprenumeration som håller faktureringsprogrammet synkat med Workfront.

Mer information om händelseprenumerationer finns i [API för händelseprenumeration](../../../../wf-api/general/event-subs-api.md).

---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 Beta 1 - versionsaktivitet
description: Den här sidan beskriver alla ändringar som är tillgängliga i förhandsvisningsmiljön i 2017.2 Beta 1. Funktionerna på den här sidan gjordes tillgängliga i förhandsvisningsmiljön den 10 maj 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 99812ed3-a300-478e-973f-b957382d934b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 0%

---

# 2017.2 Beta 1 - versionsaktivitet

Den här sidan beskriver alla ändringar som är tillgängliga i förhandsvisningsmiljön i 2017.2 Beta 1. Funktionerna på den här sidan gjordes tillgängliga i förhandsvisningsmiljön den 10 maj 2017.

>[!IMPORTANT]
>
>Funktionerna som beskrivs på den här sidan kan ändras innan de är tillgängliga i produktionsmiljön.

2017.2 Beta 1 innehåller förbättringar både för Workfront-administratörer och andra användare:

**För administratörer:**

* [Återställ dokument](#restore-documents)
* [Ny förhandsvisningsbanderoll med versionsinformation](#new-preview-banner-with-release-information) 
* [API 7-tillgänglighet](#api-7-availability)

**För alla användare:**

* [Prenumerera på uppgifter och problem](#subscribe-to-tasks-and-issues)
* [Förbättringar av resursplanering](#resource-scheduling-improvements)
* [Jämför korrektur](#compare-proofs)
* [Nytt fält för resurspooler för användare och projekt](#new-field-for-resource-pools-for-users-and-projects)
* [Uppdaterat utseende och känsla i instrumentpanelslistan](#updated-look-and-feel-in-the-dashboard-list)
* [Tar bort slutredigeringsfunktionerna i Workfront](#removing-the-endorsements-functionality-in-workfront)
* [Ändra ordning på kolumner i en lista med dra och släpp (funktionen tas bort)](#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed)

## Återställ dokument {#restore-documents}

Workfront-administratörer kan nu återställa enskilda dokument som har tagits bort under de senaste 30 dagarna. 

Före den här ändringen kunde Workfront-administratörer bara återställa projekt, uppgifter och ärenden (inklusive dokument som tagits bort i samband med det borttagna projektet, uppgiften eller problemet).

Mer information finns i [Återställ borttagna objekt](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Ny förhandsvisningsbanderoll med versionsinformation {#new-preview-banner-with-release-information}

Den blå banderollen högst upp i förhandsvisningssandlådemiljön visar nu släppningsnamnet och versionsnumret för förhandsvisningsmiljön. Om du klickar på namnet på releasen kommer du till en hjälpartikeln där du hittar mer information om den aktuella förhandsversionen. Mer information om sandlådemiljön för förhandsgranskning finns i [Sandlådemiljön för Adobe Workfront Preview](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) 

## API 7-tillgänglighet {#api-7-availability}

API 7 finns nu och innehåller nya och uppdaterade objekt.

Mer information finns i [Nyheter i API-version 7](../../../../wf-api/api/new-api-version-7.md).

## Prenumerera på uppgifter och problem {#subscribe-to-tasks-and-issues}

Workfront skickar meddelanden om objekt som du har tilldelats eller som du äger.

Från och med den aktuella versionen kan du prenumerera på objekt som inte har tilldelats dig men som kan påverka ditt arbete.

Du kan prenumerera på utgåvor och uppgifter som du har behörighet att åtminstone visa. När en ny kommentar läggs till i det ärende eller den uppgift du prenumererar på får du ett e-postmeddelande om kommentaren.

Mer information om att prenumerera på problem och uppgifter finns i [Prenumerera på objekt i Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Förbättringar av resursplanering {#resource-scheduling-improvements}

>[!NOTE]
>
>Verktygen för resursschemaläggning har tagits bort från Workfront i version 23.1. Mer information om att schemalägga resurser med hjälp av belastningsutjämnaren finns i [Översikt över belastningsutjämnaren](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Följande förbättringar är tillgängliga vid planering av resurser:

* [Visa fler objekt på tidslinjen för resursplanering i en enda vy](#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view)
* [Konfigurera projektnamnet som ska visas i aktiviteter och ärenden på tidslinjen för schemaläggning](#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline)
* [Konfigurera om överordnade aktiviteter ska visas på tidslinjen ](#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline)
* [Utöka eller komprimera enkelt alla aktiviteter och ärenden på tidslinjen ](#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline)
* [Roll- och användarinformation finns kvar högst upp i tidslinjen för schemaläggning vid rullning](#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling)

### Visa fler objekt på tidslinjen för resursplanering i en enda vy {#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view}

När du schemalägger resurser för ett team eller för projekt som du är resurshanterare för, förbrukar aktiviteter och utleveranser nu mindre vertikalt utrymme på tidslinjen för schemaläggningen. På så sätt kan du se fler uppgifter och problem i en och samma vy.

Om du bestämmer dig för att visa projektnamn för varje aktivitet och problem på tidslinjen för schemaläggning, expanderas det lodräta utrymmet för varje uppgift och problem, vilket resulterar i att färre uppgifter och problem visas i en enda vy.

Mer information om att schemalägga resurser finns i  &quot;Kom igång med resursplanering&quot;.

### Konfigurera projektnamnet som ska visas i aktiviteter och ärenden på tidslinjen för schemaläggning {#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline}

När du schemalägger resurser för ett team eller för projekt som du är resurshanterare för, kan du nu konfigurera projektnamnet så att det visas för varje aktivitet och problem på tidslinjen för schemaläggningen. På så sätt kan användare som visar tidslinjen snabbt se namnet på det projekt där uppgiften eller utgåvan finns.

Mer information finns i Kom igång med resursschemaläggning.

### Konfigurera om överordnade aktiviteter ska visas på tidslinjen för schemaläggning {#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline}

När du schemalägger resurser för projekt som du är resurshanterare för, kan du nu konfigurera om överordnade uppgifter ska visas på tidslinjen när alternativet Sammanfattande slutföringsläge för projektet är inställt på Manuellt.

Före den här ändringen visas alltid överordnade aktiviteter på tidslinjen för schemaläggning när läget Sammanfattning av slutförande i projektet har angetts till Manuell. 

När läget Sammanfattning av slutförande i projektet är inställt på Automatisk kan inte överordnade aktiviteter visas på tidslinjen för schemaläggningen. Den här upplevelsen har inte förändrats.

Mer information finns i Kom igång med resursschemaläggning.

### Expandera eller komprimera enkelt alla aktiviteter och ärenden på tidslinjen {#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline}

Det finns en ny länk som gör att du enklare kan komprimera alla aktiviteter och ärenden på tidslinjen i tidsplanen.

Mer information finns i Kom igång med resursschemaläggning.

### Roll- och användarinformation finns kvar högst upp i tidslinjen för schemaläggning vid rullning {#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling}

När du nu bläddrar nedåt på tidslinjen för schemaläggning för att visa ytterligare information finns rollnamnet och användarnamnet kvar överst i området Användare och roller på tidslinjen för schemaläggningen, vilket gör det enklare att se vilken användare och roll som uppgifterna och problemen är kopplade till.

Före den här ändringen rullas rollnamnet och användarnamnet ut ur den aktuella vyn.

Mer information om att schemalägga resurser finns i  &quot;Kom igång med resursplanering&quot;.

## Jämför korrektur {#compare-proofs}

Nu kan du jämföra två dokumentkorrektur i en enda dokumentlista, t.ex. på fliken Dokument i ett projekt, en uppgift, utgåva, en portfölj eller i huvuddelen av Dokument i det globala navigeringsfältet. 

De två korrekturen visas i gransknings- och godkännandeverktyget, och du kan korrekturgranska varje dokument samtidigt som du jämför dem i en sida vid sida-vy.

Mer information finns i [Jämför korrektur](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md).

## Nytt fält för resurspooler för användare och projekt {#new-field-for-resource-pools-for-users-and-projects}

I R1.5-versionen introducerades nya funktioner för resursplanering i förhandsvisningsmiljön. Med den här funktionen kan du skapa nya resurspooler, som är användarsamlingar.

Nu kan du associera resurspoolerna med projekt och med användare. Nu visas ett nytt fält med namnet&quot;Resurspooler&quot; i projektet samt på användarobjektet.

Mer information om de nya resurspoolerna och hur de kan associeras med projekt och användare finns i [Översikt över resurspooler](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

## Uppdaterad Look and Feel i kontrollpanelslistan {#updated-look-and-feel-in-the-dashboard-list}

Nu när du visar en kontrollpanelslista är utseendet mer modernt och skalbart.

Den här funktionen var tidigare endast tillgänglig för användare som är registrerade i tidig åtkomst. Detta är nu tillgängligt för alla användare i förhandsvisningsmiljön. Den kommer att vara tillgänglig för alla användare i produktionsmiljön i version 2017.2. 

Mer information om instrumentpaneler finns i [Skapa en instrumentpanel](../../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Ta bort slutredigeringsfunktionen i Workfront {#removing-the-endorsements-functionality-in-workfront}

När vi utvärderar funktionaliteten i uppdateringsströmmen har vi identifierat att Endors är en låg implementering och en låg användningsfunktion. Under 2017.2 kommer följande funktioner runt slutkommentarer att tas bort från Workfront från och med version 2017.2 (den här funktionen är inte längre tillgänglig i förhandsversionen):

* Fliken Slutsatser i användarprofilområdet;
* Objektet Endorsements tas bort från API-utforskaren. Om du för närvarande drar in API-rapporter för objekten &quot;Endorption&quot; eller &quot;Endorcement Share&quot;, blir anropen ogiltiga när det här objektet har tagits bort.

Följande funktionalitet finns kvar i webbprogrammet:

* En annan användares godkännande av en användare som gjordes innan den här funktionen togs bort, kommer att finnas kvar i underskriftens uppdateringsström. 

Slutsatser har inte varit ett rapporteringsobjekt och därför finns det inga ändringar i rapporteringen för det här objektet.

## Ändra ordning på kolumner i en lista med dra och släpp (funktionen tas bort) {#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed}

Funktionen för att ändra ordningen på kolumner i en lista genom att dra en kolumn från en plats och släppa den i en annan tas bort från Tidig åtkomst i produktionsmiljön med version 2017.2 och är inte längre tillgänglig för någon användare. 

Mer information om den här funktionen finns i [Ändra kolumnbredd och ordning](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

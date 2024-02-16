---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.3 Beta 2-lanseringsaktivitet
description: Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i 2018.3 Beta 2. Funktionerna kommer att vara tillgängliga i förhandsvisningsmiljön den 1 augusti 2018. Förbättrade korrekturfunktioner som lanseras med Beta 2 kommer att vara tillgängliga i förhandsvisningsmiljön onsdagen den 18 juli. Den kommer att göras tillgänglig i produktionsmiljön i november 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 97945661-e97d-43c8-b564-624c4388de2f
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# 2018.3 Beta 2-lanseringsaktivitet

Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i 2018.3 Beta 2. Funktionerna kommer att vara tillgängliga i förhandsvisningsmiljön den 1 augusti 2018. Förbättrade korrekturfunktioner som lanseras med Beta 2 kommer att vara tillgängliga i förhandsvisningsmiljön onsdagen den 18 juli. Den kommer att göras tillgänglig i produktionsmiljön i november 2018.

>[!NOTE]
>
> Funktionerna som beskrivs på den här sidan kan ändras innan de är tillgängliga i produktionsmiljön.

En lista över alla ändringar som gjorts under 2018.3 finns på  [Aktivitetsöversikt för version 2018.3](../../../../product-announcements/product-releases/quarterly-release-archive/2018.3-release-activity/2018-3-release-activity-overview.md).

Beta 2-versionen från 2018.3 innehåller förbättringar både för Workfront-administratörer och andra användare:

**För administratörer**

* [Uppdatera e-postadressen i användarprofilen som gruppadministratör](#update-the-email-address-in-the-user-profile-as-a-group-administrator)

**För alla användare**

* [Visa godkännanden som delegerats till mig i hemområdet](#view-approvals-delegated-to-me-in-the-home-area)
* [Exportera data för en viss period i resursplaneraren](#export-data-for-a-given-period-in-the-resource-planner)
* [Dagliga summor visas nu i rött när användaren är överallokerad](#daily-totals-now-display-in-red-when-the-user-is-overallocated)
* [Aktiviteter och problem döljs på tidslinjen för schemaläggning när de minimeras](#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized)
* [Filtrera kommentarer och svar efter användare i korrekturläsaren](#filter-comments-and-replies-by-user-in-the-proofing-viewer)
* [Kommentera ett intervall med tagningar i ett videoklipp](#comment-on-a-range-of-footage-in-a-video-proof)
* [Nytt verktyg för kommentarmarkering i korrekturläsaren](#new-polyline-tool-for-comment-markup-in-the-proofing-viewer)
* [Borttagning av Flash för rapport-, kalender- och dokumentdelning](#flash-removal-for-report-calendar-and-document-sharing)

## Uppdatera e-postadressen i användarprofilen som gruppadministratör {#update-the-email-address-in-the-user-profile-as-a-group-administrator}

Du kan nu uppdatera e-postadresser för användare som tillhör en grupp som du administrerar. 

Tidigare kunde bara Workfront-administratörer uppdatera e-postadresser för andra användare. 

Mer information finns i [Gruppadministratörer](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

## Visa godkännanden som delegerats till mig i hemområdet {#view-approvals-delegated-to-me-in-the-home-area}

Nu kan du använda Hem-området för att visa projekt, uppgifter och godkännanden av utleveranser som har delegerats till dig.

Före den här ändringen kunde du bara visa delegerade godkännanden på arbetsytan Mitt arbete.

Mer information finns i [Delegera godkännandebegäran](../../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

## Exportera data för en viss period i resursplaneraren {#export-data-for-a-given-period-in-the-resource-planner}

Ett nytt fönster visas nu när du exporterar informationen i Resursplaneraren där du kan välja en viss tidsram för den exporterade filen.

Före den här förbättringen kunde du bara exportera den information som visas på skärmen.

Mer information om hur du exporterar data från resursplaneraren finns i [Översikt över navigering i resursplanering](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md) i artikeln [Översikt över navigering i resursplanering](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Dagliga summor visas nu i rött när användaren är överallokerad {#daily-totals-now-display-in-red-when-the-user-is-overallocated}

>[!NOTE]
>
>Verktygen för resursschemaläggning har tagits bort från Workfront i version 23.1. Mer information om att schemalägga resurser med hjälp av belastningsutjämnaren finns i [Översikt över belastningsutjämnaren](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

När en användare är överallokerad visas de dagliga summorna för de dagar då användaren är överallokerad nu i rött. Det här alternativet visas bara när alternativet Visa summor för Dagligt planerade timmar är aktiverat i tidslinjeinställningarna för tidslinjen för schemaläggning. Före den här förbättringen fanns det en röd streckindikator för de dagar då användaren överallokerades, men de dagliga summorna visades utan röd markering.

Mer information om användartilldelningar finns i Hantera användartilldelningar i schemaläggningsområdena.

## Aktiviteter och problem döljs på tidslinjen för schemaläggning när de minimeras {#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized}

När du minimerar uppgifter och problem på tidslinjen för schemaläggning döljs de nu för användare och roller om alternativet Visa summor för planerade timmar per dag är aktiverat i inställningarna. Uppgifter och ärenden i området Ej tilldelade visas i en komprimerad vy.

Tidigare när uppgifter och problem minimerades fanns uppgifterna och problemen kvar på tidslinjen för schemaläggning för användare och roller, men de skulle visas i en komprimerad vy.

Mer information om hur du minimerar aktiviteter och problem i tidslinjen för schemaläggning finns i&quot;Kom igång med resursschemaläggning&quot;.

## Filtrera kommentarer och svar efter användare i korrekturläsaren {#filter-comments-and-replies-by-user-in-the-proofing-viewer}

Nu kan du inkludera svar när du filtrerar kommentarer som gjorts av användare som du anger. Det här är användbart när du vill fokusera på all feedback från en viktig granskare, till exempel en klient- eller projektledare.

Tidigare var filtrering per användare begränsad till endast de kommentarer som författats (startats) av de granskare som du anger.

## Kommentera ett intervall med tagningar i ett videoklipp {#comment-on-a-range-of-footage-in-a-video-proof}

Du kan skapa en kommentar för ett intervall av tagningar i ett videoklipp. Det här är användbart när du till exempel behöver ange att ett segment i en tagning måste tas bort eller tas bort.

Tidigare kunde du bara skapa en kommentar för en enda punkt på en tidslinje för video.

## Nytt verktyg för kommentarmarkering i korrekturläsaren {#new-polyline-tool-for-comment-markup-in-the-proofing-viewer}

Nu kan du använda polylinjemarkering för att rita segmenterade linjer och former när du lägger till en kommentar i ett korrektur. Du kan skapa en öppen segmenterad linje eller en sluten form. Det här verktyget är särskilt användbart när du arbetar med komplicerade bilder, t.ex. tekniska bilder eller arkitektoniska bilder.

Tidigare kunde du rita en rektangel, en rak linje, en frihandslinje eller form eller en pil när du kommenterade ett korrektur för att lägga till en kommentar.

## Borttagning av Flash för rapport-, kalender- och dokumentdelning {#flash-removal-for-report-calendar-and-document-sharing}

Vi har tagit bort Flash från följande delningsdialogrutor i Workfront:

* Rapporter
* Kalendrar
* Dokument

Du kan fortfarande dela de här objekten som du gjorde tidigare, men nu är Flashen inte längre något som behövs.

---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 Beta 3 - versionsaktivitet
description: Den här sidan beskriver alla ändringar som är tillgängliga i förhandsvisningsmiljön i 2017.2 Beta 2. Funktionerna på den här sidan gjordes tillgängliga i förhandsvisningsmiljön den 24 maj 2017. Den kommer att finnas tillgänglig i produktionsmiljön mellan slutet av juli och början av augusti 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9647f3c6-f287-426c-a5e7-eb33b8b22a34
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 0%

---

# 2017.2 Beta 3 - versionsaktivitet

Den här sidan beskriver alla ändringar som är tillgängliga i förhandsvisningsmiljön i 2017.2 Beta 2. Funktionerna på den här sidan gjordes tillgängliga i förhandsvisningsmiljön den 24 maj 2017. Den kommer att finnas tillgänglig i produktionsmiljön mellan slutet av juli och början av augusti 2017.

>[!IMPORTANT]
>
>Funktionerna som beskrivs på den här sidan kan ändras innan de är tillgängliga i produktionsmiljön.

En lista över alla ändringar som gjorts under 2017.2 finns i [Översikt över versionsaktivitet för 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

2017.2 Beta 2 innehåller förbättringar både för Workfront-administratörer och andra användare:

**För administratörer:**

* [Återställer objekt i grupp från papperskorgen](#restoring-items-in-bulk-from-the-recycle-bin)
* [Användarinformationen synkroniseras från Workfront till KorrekturHQ (ProofHQ och Workfront)](#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront)

**För alla användare:** 

* [Visa prenumererade användare](#view-subscribed-users)
* [Konfigurera hur milstolpar visas i Gantt-schemat](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [Inkludera Gantt-schemats förklaring vid export till PDF](#include-the-gantt-chart-legend-when-exporting-to-pdf)
* [Visa korrekturgodkännanden i Min arbetsyta (Workfront)](#view-proof-approvals-in-the-my-work-area-workfront)
* [Visa användarnamn när språkverifieringsbegäranden från Min arbetsyta (Workfront) hanteras](#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront)
* [Förbättrat korrekturläsare för videokorrektur (ProofHQ och Workfront)](#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront)
* [Visa korrektur för multimedia i alternativa upplösningar (Korrektur, HQ och Workfront)](#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront)
* [Nytt Proof Creator-objekt i dokumentversionsrapport (Workfront)](#new-proof-creator-object-in-document-version-report-workfront)
* [Ny resurspoolfunktion som tillfälligt tagits bort från förhandsgranskningen](#new-resource-pool-functionality-temporarily-removed-from-preview)

## Återställa objekt i grupp från papperskorgen {#restoring-items-in-bulk-from-the-recycle-bin}

Du kan nu återställa upp till 10 borttagna projekt, uppgifter, utgåvor eller dokument åt gången.

Före den här ändringen kunde du bara återställa ett borttaget objekt i taget.

Mer information om hur du återställer objekt finns i [Återställa borttagna objekt](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Visa prenumererade användare {#view-subscribed-users}

Nu kan du se vem som prenumererar på ett objekt genom att utöka antalet prenumeranter som visas bredvid prenumerationslänken.

Före den här förbättringen hade du ingen insyn i vem som prenumererar på några objekt.

Mer information om att prenumerera på objekt finns i [Prenumerera på objekt i Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md). 

## Konfigurera hur milstolpar visas i Gantt-schemat {#configure-how-milestones-are-displayed-on-the-gantt-chart}

Det finns nu två alternativ för att visa information om milstolpar i ett Gantt-schema. Du kan konfigurera någon av eller båda följande milstolpeindikatorer:

* Milstolpediamanter (ikon)

  Den här ikonen visas i Gantt-schemat efter en uppgift som är associerad med en milstolpe.

* Milstolpslinjer

  En linje visas efter en uppgift som är associerad med milstolpen och som täcker alla uppgifter i Gantt-schemat.

Före den här ändringen fanns det bara ett alternativ för att aktivera att milstolpar visas i ett Gantt-schema, som kallas&quot;milstolpar&quot;. Med det här alternativet aktiverades både milstolpdiamantikonen och milstolpslinjen. Dessa indikatorer kunde inte separeras.

Mer information om hur du konfigurerar hur information visas i Gantt-schemat finns i [Konfigurera hur information visas i Gantt-schemat](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Inkludera Gantt-schemats förklaring vid export till PDF {#include-the-gantt-chart-legend-when-exporting-to-pdf}

När du exporterar Gantt-diagrammet till PDF kan du nu välja om du även vill exportera teckenförklaringen till diagrammet tillsammans med själva diagrammet. Objekten i förklaringen är bara de alternativ som du har aktiverat för att visas i Gantt-diagrammet i användargränssnittet. De här alternativen inkluderas i förklaringen om de finns i aktiviteterna i projektet. Om du t.ex. aktiverar att visa milstolpar i Gantt-schemat, visas även dem i teckenförklaringen, men bara om det finns minst en aktivitet som är associerad med en milstolpe.

Före den här ändringen kunde du inte utesluta teckenförklaringen från det exporterade PDF, och teckenförklaringen innehöll alla möjliga alternativ och markörer för Gantt, oavsett om de var aktiverade eller fanns i användargränssnittet.

Mer information om hur du exporterar Gantt-schemat finns i [Exportera Gantt-schemat till PDF](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

## Användarinformationen synkroniseras från Workfront till KorrekturHQ (ProofHQ och Workfront) {#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront}

Användarinformation (namn och e-postadress) synkroniseras nu från Workfront till KorofHQ när användare skapas eller uppdateras i Workfront. 

Mer information om användarsynkronisering från Workfront till ProofHQ finns i .

## Nytt Korrekturskaparobjekt i dokumentversionsrapport (Workfront)

{#new-proof-creator-object-in-document-version-report-workfront}

Nu när du skapar en dokumentversionsrapport finns det ett nytt Korrekturskaparobjekt. Med det här objektet kan du rapportera information om den användare som skapade korrekturet. 

Det nya objektet Korrekturskapare i dokumentversionsrapporten innehåller alla fält som är tillgängliga med det befintliga användarobjektet i andra typer av objektrapporter.

>[!NOTE]
>
> Den här informationen är endast tillgänglig i rapporten från den tidpunkt då den här funktionen först introducerades i respektive förhandsgransknings- eller produktionsmiljö. Information i rapporter om objektet Requester innan den här funktionen introducerades är inte tillgänglig.

Du kommer åt objektet Korrekturskapare när du skapar en dokumentversionsrapport, vilket beskrivs i [Skapa en anpassad rapport](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Mer information om objektrapporten för dokumentversionen finns i avsnittet [Förstå objekt i Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) i [Förstå objekt i Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Visa korrekturgodkännanden på arbetsytan (Workfront) {#view-proof-approvals-in-the-my-work-area-workfront}

Alla korrekturgodkännanden som du har skickat in för godkännande visas nu på arbetsytan Mitt i fliken **Arbete som jag har skickat in för godkännande**.

Före den här ändringen fanns inga korrekturgodkännanden på fliken **Arbete som jag skickat in för godkännande**.

Godkännanden av korrektur visas endast när följande villkor uppfylls:

* Godkännandet väntar för närvarande på godkännande
* Godkännandeprocessen tilldelas en användare som är en licensierad Workfront-användare (Godkännandeprocesser som tilldelats användare som inte är licensierade Workfront-användare visas inte)
* Godkännandeprocesserna startades efter att den här funktionen släpptes (godkännandeprocesser som startades innan den här funktionen släpptes visas inte)

Mer information finns i [Visa godkännanden](../../../../review-and-approve-work/manage-approvals/view-approvals.md) i [Visa godkännanden](../../../../review-and-approve-work/manage-approvals/view-approvals.md).

## Visa användarnamn när språkverifieringsbegäranden adresseras från Min arbetsyta (Workfront) {#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront}

När du godkänner korrekturgodkännanden från Min arbetsyta visas nu namnet på den användare som begärde godkännandet.

Mer information finns i [Godkänna arbete](../../../../review-and-approve-work/manage-approvals/approving-work.md) i [Godkänna arbete](../../../../review-and-approve-work/manage-approvals/approving-work.md). 

## Förbättrat korrekturläsare för videokorrektur (ProofHQ och Workfront) {#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront}

Språkvisningsprogrammet i både Workfront och ProofHQ uppdateras med ett nytt utseende och en ny känsla, HTML5-arkitektur för bättre prestanda och stöd för nya funktioner.

Det nya korrekturläsaren innehåller följande förbättringar:

* Korrektur bildruta för bildruta
* Videobuffring
* Sökfunktionen i kommentarlistan
* Alla åtgärder som anges för kommentaren visas för varje kommentar i kommentarlistan
* Helskärmsläge
* Granska materialet snabbare eller långsammare
* Stavningskontroll när kommentarer och svar läggs till

### Förhandsgranska

Det nya korrekturläsaren är tillgänglig för test i följande förhandsvisningsmiljöer:

* Korrektur för HQ-förhandsvisningsmiljö

  Mer information om förhandsvisningsmiljön för Korrektur för högdagrar finns i [Testmiljö för förhandsgranskning av sandlådor - Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).

* Workfront förhandsgranskningsmiljö, när ditt konto är aktiverat med språkkontroll

  Mer information om Workfront Preview finns i  [Sandlådemiljön för Adobe Workfront Preview](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

I den här versionen har det nya korrekturläsaren bara stöd för videofärgning. Det innebär att alla videokorrektur använder det nya korrekturläsaren, medan alla statiska korrektur- och multimediekorrektur fortfarande använder det befintliga korrekturläsaren.

### Produktion

När det släpps i produktionsmiljön med version 17.2 kan administratören välja om det nya eller gamla korrekturläsaren passar för användarna i organisationen. Som standard används det äldre korrekturläsaren.

Mer information om hur du använder det nya visningsprogrammet för videokorrektur finns i  

## Visa korrektur för multimedia i alternativa upplösningar (ProofHQ och Workfront) {#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront}

Nu kan du justera upplösningen för korrektur för multimedia antingen genom att ange en anpassad upplösning eller genom att dra bilden till önskad upplösning.

Före den här ändringen kunde du granska korrektur endast med den inbyggda upplösningen för den skärm eller enhet där du granskade innehållet.

Du kan använda läget Jämför för att jämföra olika korrekturupplösningar.

Mer information finns i [Öppna korrektur i Desktop Proofing Viewer](../../../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/open-proofs-in-dpv.md). 

## Ny resurspoolfunktion som tillfälligt tagits bort från förhandsgranskningen {#new-resource-pool-functionality-temporarily-removed-from-preview}

På grund av utvecklingsproblem har vi beslutat att ta bort den nya fliken Resursplanering och ändra namnet på den äldre fliken Resursplanering till det ursprungliga namnet&quot;Resursplanering&quot;.

Den nya funktionen Resurspooler har också tagits bort med den här ändringen. Den nya fliken Resursplanering och funktionaliteten för resurspoolerna återgår till förhandsgranskningssandlådemiljön i slutet av juni 2017.

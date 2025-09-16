---
product-area: documents
navigation-topic: approvals
title: Bildruta.io - integreringsöversikt
description: Bildruta.io - integreringsöversikt
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 701f3fc2c885363b5f61fb9d77049c7d4c41963d
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---


# Bildruta.io - integreringsöversikt

Tack vare integreringen mellan Workfront och Frame.io kan projektsamordnare hantera projekt och planera arbetet i Workfront, medan kreatörer, marknadsförare och intressenter kan granska och godkänna mediefiler i Frame.io.

## Byggt på Adobe Enterprise Storage Management

Kärnan i denna integrering är Adobe Enterprise Storage Management (ESM) - en molnbaserad lagringslösning som fungerar som central lagringsplats för resurser i Adobe företagsprodukter, inklusive Workfront och Frame.io.

Några av fördelarna med Adobe Enterprise Storage Management:

* Enhetligt lagringslager för kreativa resurser och resurser för arbetshantering
* Centraliserade behörigheter via Adobe IMS för säker åtkomstkontroll
* Synlighet från början till slut i Workfront-, Frame.io- och Creative Cloud-apparna <!--coming soon?-->
* Skalbar lagring och kvothantering för företagsbehov

Mer information finns i [Adobe Enterprise Storage Management - översikt](help/quicksilver/review-and-approve-work/esm-overview.md).

## Enhetlig granskning och godkännande

Integreringen av Workfront och Frame.io använder Workfront enhetliga godkännandefunktioner för att hantera granskningar och godkännanden. Med enhetliga godkännanden kan ni

* Skapa och hantera granskningar och godkännanden direkt från Workfront
* Spåra status för granskningar och godkännanden i realtid
* Centralisera feedback och godkännanden på ett och samma ställe
* Se till att alla intressenter har tillgång till de senaste versionerna av mediefiler
* Använd AI-granskare för att automatisera varumärkesgranskningar
* med mera

Mer information finns i [Enhetliga dokumentgodkännanden: artikelindex](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md).


### Använda visningsprogrammet Frame.io

Integrationen kopplas även till Frame.io-visningsprogrammet. Visningsprogrammet Frame.io innehåller

* Markerings- och kommentarverktyg
* Versionshistorik och jämförelse
* Tidsstämplade kommentarer för videogranskningar
* Mobil åtkomst till granskningar och godkännanden oavsett var du är

Mer information finns i [Kom igång med Frame.io-integreringen](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/get-started-with-frame-integration.md).

#### Gränser för videogranskning

<!--need to confirm these-->

#### Filtyper som stöds i Frame.io-visningsprogrammet

Visningsprogrammet Frame.io har stöd för alla vanliga typer av video, bilder, ljud, PDF och MS® Office. En detaljerad lista över filer som stöds finns i [Typer i Frame.io](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

#### Åtkomst och licensiering för Frame.io-visningsprogrammet

Visningsprogrammet Frame.io är tillgängligt för alla Workfront-användare med en betald licens. Ingen ytterligare Frame.io-licens krävs för att använda Frame.io-visningsprogrammet för granskningar och godkännanden med den här integreringen.

Om din organisation vill dra nytta av den extra Frame.io-funktionen, som att överföra resurser direkt till projekt i Frame.io, kan du köpa en företagslicens för Frame.io. <!--link to Frame.io enterprise license info or who to contacT?-->

Workfront korrekturfunktioner är inte tillgängliga med den här integreringen.

## Kraftfull projekthantering i Workfront

Tack vare integreringen mellan Workfront och Frame.io kan projektsamordnarna utnyttja Workfront kraftfulla projekthanteringsfunktioner för att planera, spåra och hantera arbetet.

Mer information om hur du hanterar projekt i Workfront finns i [Projekt: artikelindex](/help/quicksilver/manage-work/projects/projects-toc.md).

### Tvingad struktur och namnkonventioner

Eftersom integreringen byggs med ESM finns det vissa tvingande struktur- och namnkonventioner som du bör känna till när du hanterar projekt och dokument.

* Objektnamn måste vara unika och kan inte dupliceras
* ESM kräver unika namn för peer-objekt med samma överordnade i hierarkiträdet
* Dokument kan inte ha samma namn om de tillhör samma projekt

Med dessa begränsningar i åtanke byter Workfront automatiskt namn på objekt och dokument efter behov för att förhindra konflikter.

### Dokumenthantering i Workfront

Dokument hanteras på projektnivå med den här integreringen och kan för närvarande inte överföras till aktiviteter eller problem.

Åtkomst till dokument hanteras också på projektnivå. Om en användare har åtkomst till ett projekt kan han/hon få åtkomst till alla dokument som är kopplade till det projektet.

<!--Documents can't be dragged as full folders.-->

### Begränsningar i dokumentupplevelsen

Eftersom den här integreringen byggs med ESM finns det vissa begränsningar i den ursprungliga dokumentupplevelsen i Workfront:

#### Begränsningar

Följande funktioner kommer inte att ingå i den här integreringen:

* Externa dokumentleverantörer
* Åtkomst till korrektur
* Dokumentvisningsprogram i Workfront


#### Tillfälliga begränsningar

För närvarande finns inte följande funktioner:

* Favoritdokument
* Begär dokument
* Skicka dokument till Adobe Experience Manager Assets
* Godkännanden i flera steg
* Ladda upp dokument till kommentarer eller uppdateringar i Workfront
* Överföra dokument till uppgifter eller problem i Workfront




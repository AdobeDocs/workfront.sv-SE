---
product-area: documents
navigation-topic: approvals
title: Enhetlig översikt över granskning och godkännande
description: Läs mer om enhetlig granskning och godkännanden från Workfront och Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: b5f0150b-40b5-4386-98bc-374e7ca65b74
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 2b3e2ac00126facab9cc45ba8fb193d8951a37ec
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---

# Enhetlig översikt över granskning och godkännande

Med enhetlig granskning och godkännande som bygger på Workfront och Frame.io kan projektsamordnare hantera projekt och planera arbetet i Workfront, medan kreatörer, marknadsförare och intressenter kan granska och godkänna mediefiler i Frame.io.

## Integrationskrav

* Workfront och Frame.io måste distribueras till samma Identity Management-systemorganisation (IMS).

* Användare kan bara tillhöra en Workfront-instans inom IMS-organisationen.

* Workfront-instansen måste aktiveras för Adobe Unified Experience och Adobe Enterprise-lagring.

* Integreringen måste konfigureras av Adobe Professional Services.


## Byggt på Adobe Enterprise-lagring

Enhetlig granskning och godkännande bygger på Adobe Enterprise-lagring - en molnbaserad lagringslösning som fungerar som central lagringsplats för resurser i Adobe företagsprodukter, inklusive Workfront och Frame.io. <!--, and Creative Cloud.-->

Några av fördelarna med Adobe Enterprise-lagring:

* Enhetligt lagringslager för kreativa resurser och resurser för arbetshantering
* Centraliserad behörighet via Adobe Identity Management-system (IMS) för säker åtkomstkontroll
* Synlighet från början till slut för resurser i Workfront och Frame.io <!--, and Creative Cloud apps -->
* Skalbar lagring och kvothantering för företagsbehov

Mer information finns i [Adobe Enterprise-lagringsöversikt](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Enhetlig granskning och godkännande

Med enhetlig granskning och godkännande kan man

* Skapa och hantera granskningar och godkännanden direkt från Workfront
* Spåra status för granskningar och godkännanden i realtid
* Centralisera feedback och godkännanden på ett och samma ställe
* Se till att alla intressenter har tillgång till de senaste versionerna av mediefiler
* Automatisera varumärkesgranskningar
* med mera

Mer information finns i [Enhetliga dokumentgodkännanden: artikelindex](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md).


### Använda visningsprogrammet Frame.io

Använd Frame.io-visningsprogrammet för att granska och godkänna resurser. Visningsprogrammet Frame.io innehåller

* Markerings- och kommentarverktyg
* Versionshistorik och jämförelse
* Tidsstämplade kommentarer för videogranskningar
* Mobil åtkomst till granskningar och godkännanden oavsett var du är

Mer information finns i [Kom igång med enhetlig granskning och godkännande](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).

#### Gränser för videogranskning

Det finns ett årligt tak för videokorrektur som sätts till 10 % av en organisations totala betalda Workfront-användarlicenser - Standard och Light. Denna övre gräns tillämpas på organisationsnivå.

Workfront-administratörer får meddelanden när användningen når 80 % och 100 % av taket.

Denna gräns gäller inte för Frame.io Enterprise-kunder.

#### Filtyper som stöds i Frame.io-visningsprogrammet

Visningsprogrammet Frame.io har stöd för alla vanliga typer av video, bilder, ljud, PDF och MS® Office. En detaljerad lista över filer som stöds finns i [Filtyper som stöds i Frame.io](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

#### Åtkomst och licensiering för Frame.io-visningsprogrammet

Visningsprogrammet Frame.io är standardvisningsprogram för alla Workfront arbetsflöden för granskning och godkännande. Den ingår automatiskt för alla Workfront-användare med en betald licens. Ingen ytterligare Frame.io-licens krävs för att använda Frame.io-visningsprogrammet för granskningar och godkännanden.

Om din organisation vill dra nytta av den extra Frame.io-funktionaliteten som är tillgänglig med den här integreringen, till exempel att överföra resurser direkt till projekt i Frame.io, kan du köpa en Frame.io-företagslicens. Kontakta din kontorepresentant på Adobe för att boka en demo och utforska fördelarna med Frame.io-lösningen.

Workfront språkfunktioner är inte tillgängliga med den här integreringen.

## Kraftfull projekthantering i Workfront

Projektsamordnare kan utnyttja Workfront kraftfulla projekthanteringsfunktioner för att planera, spåra och hantera arbeten.

Mer information om hur du hanterar projekt i Workfront finns i [Projekt: artikelindex](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

### Tvingad struktur och namnkonventioner

Eftersom enhetliga gransknings- och godkännandeprocesser byggs med Adobe Enterprise-lagring, finns det vissa tvingande struktur- och namnkonventioner som du bör känna till när du hanterar projekt och dokument.

* Objektnamn måste vara unika och kan inte dupliceras
* Adobe Enterprise-lagring kräver unika namn för peer-objekt med samma överordnade i hierarkiträdet
* Dokument kan inte ha samma namn om de tillhör samma projekt
* Dokumentnamn får inte innehålla något av följande specialtecken: \ / : * ? &quot; | &lt; >
* Dokumentnamn får innehålla högst 255 tecken

Med dessa begränsningar i åtanke byter Workfront automatiskt namn på objekt och dokument efter behov för att förhindra konflikter.

### Delning och behörigheter

Som en del av integreringen styrs användarbehörigheterna i Workfront och går ned till Frame.io. Det innebär att du inte kan bjuda in en användare till ett projekt i Frame.io eller ändra användarbehörigheter i Frame.io. Dessa åtgärder måste utföras via Project Share modal i Workfront.

Följande tabell visar hur Workfront-behörigheter mappas till Frame.io-behörigheter:

<table>
<tr>
<th>Användarbehörighet för Workfront</th>
<th>Frame.io-användarbehörighet</th>
</tr>
<tr>
<td>Hantera</td>
<td>Redigera och dela</td>
</tr>
<tr>
<td>Contribute</td>
<td>Redigera och dela</td>
</tr>
<tr>
<td>Visa</td>
<td>Endast kommentarer</td>
</tr>
</table>



### Dokumenthantering i Workfront

Dokument som överförs till Workfront lagras i Adobe Enterprise och är tillgängliga i både Workfront och Frame.io. När du överför ett dokument till en uppgift eller ett problem i Workfront skapas en systemgenererad mapp i Adobe Enterprise-lagring som ärver behörigheter från uppgiften eller problemet. Alla dokument som överförs till den uppgiften eller utgåvan lagras i den mappen och ärver behörigheter från den. Mer information om dokument i Workfront finns i [Översikt över det nya dokumentområdet](/help/quicksilver/documents/managing-documents/documents-area.md) och [Objektbehörigheter och översikt över åtkomstnivån för Adobe Enterprise-lagringsmodell](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).

### Begränsningar i dokumentupplevelsen

Följande dokumentfunktioner ingår inte:

<!--* External document providers-->
* Åtkomst till korrektur i Workfront
* Dokumentvisningsprogram i Workfront
* Favoritdokument
* Begär dokument
---
product-area: documents
navigation-topic: approvals
title: Bildruta.io - integreringsöversikt
description: Bildruta.io - integreringsöversikt
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b5f0150b-40b5-4386-98bc-374e7ca65b74
source-git-commit: 9825f095a7be7debb5150ca4bd50f7cf6fd12295
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 0%

---

# Bildruta.io - integreringsöversikt

Tack vare integreringen mellan Workfront och Frame.io kan projektsamordnare hantera projekt och planera arbetet i Workfront, medan kreatörer, marknadsförare och intressenter kan granska och godkänna mediefiler i Frame.io.

## Byggt på Adobe Enterprise-lagring

Kärnan i denna integrering är Adobe Enterprise-lagring - en molnbaserad lagringslösning som fungerar som central lagringsplats för resurser i Adobe företagsprodukter, inklusive Workfront och Frame.io. <!--, and Creative Cloud.-->

Några av fördelarna med Adobe Enterprise-lagring:

* Enhetligt lagringslager för kreativa resurser och resurser för arbetshantering
* Centraliserade behörigheter via Adobe IMS för säker åtkomstkontroll
* Synlighet från början till slut för resurser i Workfront och Frame.io <!--, and Creative Cloud apps -->
* Skalbar lagring och kvothantering för företagsbehov

Mer information finns i [Adobe Enterprise-lagringsöversikt](/help/quicksilver/review-and-approve-work/esm-overview.md).

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

Det finns ett årligt tak för videokorrektur som sätts till 10 % av en organisations totala betalda Workfront-användarlicenser - Standard och Light. Denna övre gräns tillämpas på organisationsnivå.

Workfront-administratörer får meddelanden när användningen når 80 % och 100 % av taket.

Denna gräns gäller inte för Frame.io Enterprise-kunder.

#### Filtyper som stöds i Frame.io-visningsprogrammet

Visningsprogrammet Frame.io har stöd för alla vanliga typer av video, bilder, ljud, PDF och MS® Office. En detaljerad lista över filer som stöds finns i [Typer i Frame.io](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

#### Åtkomst och licensiering för Frame.io-visningsprogrammet

Visningsprogrammet Frame.io är standardvisningsprogram för alla Workfront arbetsflöden för granskning och godkännande. Den ingår automatiskt för alla Workfront-användare med en betald licens. Ingen ytterligare Frame.io-licens krävs för att använda Frame.io-visningsprogrammet för granskningar och godkännanden.

Om din organisation vill dra nytta av den extra Frame.io-funktionaliteten som är tillgänglig med den här integreringen, till exempel att överföra resurser direkt till projekt i Frame.io, kan du köpa en Frame.io-företagslicens. Kontakta din kontorepresentant på Adobe för att boka en demo och utforska fördelarna med Frame.io-lösningen.

Workfront språkfunktioner är inte tillgängliga med den här integreringen.

## Kraftfull projekthantering i Workfront

Tack vare integreringen mellan Workfront och Frame.io kan projektsamordnarna utnyttja Workfront kraftfulla projekthanteringsfunktioner för att planera, spåra och hantera arbetet.

Mer information om hur du hanterar projekt i Workfront finns i [Projekt: artikelindex](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

### Tvingad struktur och namnkonventioner

Eftersom integreringen byggs med ESM finns det vissa tvingande struktur- och namnkonventioner som du bör känna till när du hanterar projekt och dokument.

* Objektnamn måste vara unika och kan inte dupliceras
* ESM kräver unika namn för peer-objekt med samma överordnade i hierarkiträdet
* Dokument kan inte ha samma namn om de tillhör samma projekt

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

Dokument hanteras på projektnivå med den här integreringen och kan för närvarande inte överföras till aktiviteter eller problem.

Åtkomst till dokument hanteras också på projektnivå. Om en användare har åtkomst till ett projekt kan han/hon få åtkomst till alla dokument som är kopplade till det projektet.

### Begränsningar i dokumentupplevelsen

Eftersom den här integreringen byggs med Adobe Enterprise-lagring finns det vissa begränsningar i den ursprungliga dokumentupplevelsen i Workfront:

#### Begränsningar

Följande funktioner kommer inte att ingå i den här integreringen:

<!--* External document providers-->
* Åtkomst till korrektur i Workfront
* Dokumentvisningsprogram i Workfront
* Favoritdokument
* Begär dokument


<!--#### Temporary limitations

For now, the following capabilities are not available:

* Send documents to Adobe Experience Manager Assets
* Multi-stage approvals
* Upload documents to comments or updates in Workfront
* Upload documents to tasks or issues in Workfront-->

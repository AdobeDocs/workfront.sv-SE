---
product-area: documents
navigation-topic: approvals
title: Enhetlig översikt över granskning och godkännande
description: Läs mer om enhetlig granskning och godkännande från Workfront och Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 32cb95c2-8d12-492b-ad89-b38e2a337fc5
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 93eab1106953bfc7324f4b7cc99d3442364a56cd
workflow-type: tm+mt
source-wordcount: '3865'
ht-degree: 0%

---


# Enhetlig översikt över granskning och godkännande

Enhetlig granskning och godkännande sammanför Adobe Workfront och Adobe Frame.io till en enda, sammanhängande upplevelse - som överbryggar klyftorna mellan hantering av marknadsföring, granskning och innehållsleverans.
Projektsamordnarna hanterar arbetet i Workfront medan kreatörer, marknadsförare och intressenter granskar och godkänner resurser i den professionella versionen av Frame.io-visningsprogrammet, utan att behöva flytta filer mellan olika verktyg.

![Bild som visar det enhetliga arbetsflödet för granskning och godkännande, där projektsamordnare hanterar arbetet i Workfront och granskare och godkännare som ger feedback och fattar beslut i Frame.io-visningsprogrammet.](assets/Unified-Review-Approvals-Image.png)


## Integrationskrav

* Workfront och Frame.io måste distribueras till samma Identity Management-systemorganisation (IMS).

* Användare kan bara tillhöra en Workfront-instans inom IMS-organisationen.

* Workfront-instansen måste aktiveras för Adobe Unified Experience och Adobe Enterprise-lagring.


## Byggt på Adobe Enterprise-lagring

Enhetlig granskning och godkännande bygger på Adobe Enterprise-lagring - en molnbaserad lagringslösning som fungerar som central lagringsplats för resurser i Adobe företagsprodukter, inklusive Workfront och Frame.io. <!--, and Creative Cloud.-->

Några av fördelarna med Adobe Enterprise-lagring:

* Enhetligt lagringslager för kreativa resurser och resurser för arbetshantering
* Centraliserad behörighet med Adobe Identity Management-system (IMS) för säker åtkomstkontroll
* Synlighet från början till slut för resurser i Workfront och Frame.io <!--, and Creative Cloud apps -->
* Skalbar lagring och kvothantering för företagsbehov

Mer information finns i [Adobe Enterprise-lagringsöversikt](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Enhetlig granskning och godkännande

Med enhetlig granskning och godkännande kan man

* Skapa och hantera granskningar och godkännanden direkt från Workfront
* Spåra status för granskningar och godkännanden i realtid
* Centralisera feedback och godkännanden på ett och samma ställe
* Se till att alla intressenter har tillgång till de senaste versionerna av mediefiler
* Använd AI-granskare för att automatisera varumärkesgranskningar
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

Om din organisation vill dra nytta av den extra Frame.io-funktionaliteten som är tillgänglig med den här integreringen, till exempel att överföra resurser direkt till projekt i Frame.io, kan du köpa en Frame.io Enterprise-licens. Kontakta din kontorepresentant på Adobe för att boka en demo och utforska fördelarna med Frame.io-lösningen.

Workfront språkfunktioner är inte tillgängliga med den här integreringen.

## Kraftfull projekthantering i Workfront

Projektsamordnare kan utnyttja Workfront kraftfulla projekthanteringsfunktioner för att planera, spåra och hantera arbeten.

Mer information om hur du hanterar projekt i Workfront finns i [Projekt: artikelindex](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

### Tvingad struktur och namnkonventioner

Eftersom en enhetlig granskning och godkännande byggs med Adobe Enterprise-lagring finns det vissa tvingande struktur- och namnkonventioner som du bör känna till när du hanterar projekt och dokument.

* Adobe Enterprise-lagring kräver unika namn för peer-objekt med samma överordnade objekt i hierarkiträdet.
* Dokument kan inte ha samma namn om de tillhör samma projekt.
* Objektnamn får inte innehålla något av följande specialtecken: \ / : * ? &quot; | &lt; >
* Objektnamn får innehålla högst 255 tecken.

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

## Kom igång med enhetlig granskning och godkännande

Information om hur du kommer igång med enhetlig granskning och godkännande finns i [Kom igång med enhetlig granskning och godkännande](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).

## Vanliga frågor

### Komma igång med enhetlig granskning och godkännande

+++ Expandera om du vill visa vanliga frågor och svar om hur du kommer igång med enhetlig granskning och godkännande.

**Vad är enhetlig granskning och godkännande?**

Enhetlig granskning och godkännande är en inbyggd integrering mellan Adobe Workfront och Adobe Frame.io som sammanför arbetshantering och kreativ granskning i ett enda, uppkopplat system. Projektsamordnarna planerar och håller reda på arbetet i Workfront, medan granskare och godkännare använder det professionella visningsprogrammet Frame.io för att ge feedback, kommentera i materialet och fatta beslut om godkännande - utan att behöva växla mellan olika verktyg eller flytta filer manuellt.

Gransknings- och godkännandeplatserna är i centrum för varje innehållsåtgärd. Det är där kreativt arbete, synpunkter från intressenter och affärsbeslut sammanfaller. När den processen sprids över verktyg som inte är kopplade till varandra - e-posttrådar, chattmeddelanden, skärmbildsmarkeringar - sammanföll resultatet: långsammare time to market, förlorad feedback, versionskonflikter och tidsåtgång för att hantera filer i stället för att skapa innehåll.

Enhetlig granskning och godkännande åtgärdar detta genom att ersätta lapptäcket med verktyg för granskning som inte är kopplade till varandra med ett modernt system - en enda källa till sanning där arbetet redan pågår.

**Vilka är kraven för att använda den här integreringen?**

För att använda enhetlig granskning och godkännande måste följande villkor vara uppfyllda:

* Workfront och Frame.io måste distribueras till samma Adobe Identity Management System-organisation (IMS).

* Användare kan bara tillhöra en Workfront-instans inom IMS-organisationen.

* Workfront-instansen måste aktiveras för Adobe Unified Experience och Adobe Enterprise-lagring.

* Workfront-kunder måste befinna sig på en V2 SKU (detta kan kräva en avtalshändelse - kontakta din Adobe-kontorepresentant).

**Behöver jag en Frame.io-licens för att kunna använda den här integreringen?**

Nej. Visningsprogrammet Frame.io ingår automatiskt för alla Workfront-användare med en betald licens utan extra kostnad. Du behöver ingen separat Frame.io-licens för att granska och godkänna mediefiler via Workfront.

Om din organisation vill ha tillgång till ytterligare Frame.io-funktioner - som att överföra resurser direkt till projekt i Frame.io - kan du köpa en Frame.io Enterprise-licens. Kontakta din Adobe-kontorepresentant om du vill veta mer.

**Ersätter detta Workfront Proof?**

Ja. När enhetlig granskning och godkännande är aktiverat blir Frame.io-visningsprogrammet den primära granskningsytan i Workfront och ersätter Workfront Proof.

Befintliga kunder har fortfarande tillgång till Workfront språkfunktioner för projekt som skapats innan integreringen aktiverades.

**Hur får jag åtkomst till enhetlig granskning och godkännande?**

**Vad behöver jag göra för att få åtkomst?**

För att få tillgång till enhetlig granskning och godkännande måste ni ha en Workfront V2 SKU. Om du inte redan använder en V2 SKU måste du ha en avtalshändelse med Adobe. Så här kommer du igång:

* Kontakta Adobe för att få veta om din nuvarande Workfront-plan har stöd för enhetlig granskning och godkännande.

* Om en SKU-uppgradering behövs kommer er kontorepresentant att hjälpa er genom avtalsprocessen.

* När ditt konto finns på rätt SKU konfigurerar Adobe Professional Services integreringen för din organisation.

   * Om du är osäker på vem som är din Adobe-kontorepresentant kan du kontakta Adobe supportportal eller gå till Experience League för kontaktalternativ.

+++

### Hur enhetlig granskning och godkännande fungerar

+++ Expandera om du vill visa vanliga frågor om hur enhetlig granskning och godkännande fungerar.

**Hur fungerar arbetsflödet för granskning och godkännande?**

Arbetsflödet följer dessa allmänna steg:

1. En projektsamordnare skapar ett projekt i Workfront och överför eller länkar resurser.

1. När en resurs är klar för granskning skapar koordinatorn ett arbetsflöde för godkännande - antingen ett enstaka godkännande eller genom att använda en återanvändbar godkännandemall.

1. Tilldelade granskare och godkännare meddelas via e-post och kan öppna resursen direkt i Frame.io-visningsprogrammet.

1. Granskare kan lägga in kommentarer och markeringar. Godkännarna måste fatta ett formellt beslut.

1. Koordinatorn spårar status i realtid från Workfront.

**Vad är skillnaden mellan en granskare och en godkännare?**

Granskare kan lägga till kommentarer och kommentera resurser i Frame.io-visningsprogrammet. När de är klara markerar de sin granskning som slutförd. De behöver dock inte utföra någon åtgärd för att godkännandearbetsflödet ska gå framåt.

Godkännare måste göra något av följande för att flytta godkännandearbetsflödet framåt:

* **Godkänn**: Resursen är klar att användas som den är.

* **Kräver arbete**: Resursen kräver ändringar och måste skickas in på nytt som en ny version för omgodkännande.

**Vilka typer av arbetsflöden för godkännande kan jag skapa?**

* **Engångsgodkännanden**: Du kan skapa ett engångsgodkännande direkt i ett dokument i ett projekt, en uppgift eller ett ärende. Du kan tilldela granskare och godkännare, ange deadlines och konfigurera flera steg om det behövs. Automatiserade e-postpåminnelser skickas 72 timmar före, 24 timmar före och efter ansökningsdeadline.

* **Godkännandemallar**: Du kan skapa återanvändbara mallar i Workfront Setup. En mall definierar granskarna, godkännarna och en relativ tidsram för slutförande. Du kan skapa flera steg om det behövs. När en mall har tillämpats på en tillgång beräknas tidsgränsen automatiskt.

**Hur deltar externa användare i granskningar?**

Externa Workfront-användare meddelas via e-post när de tilldelas en granskning eller godkännande. De uppmanas att skapa en Frame.io-inloggning för att få åtkomst till visningsprogrammet och delta i granskningsprocessen.

**Hur spårar jag gransknings- och godkännandeprocessen?**

Projektsamordnare kan övervaka alla pågående godkännanden på flera sätt:

* Widgeten Mina godkännanden i Workfront Home ger en realtidssammanfattning av väntande och försenade godkännanden.

* Widgeten Dokumentgodkännandemått visar genomsnittliga godkännandetider och beslutsindelningar.

* Anpassade rapportpaneler kan byggas in i Canvas Dashboards för att få större insyn i gransknings- och godkännandeaktiviteter.

+++


### Granska och godkänna resurser och videor

+++ Expandera om du vill visa vanliga frågor om granskning och godkännande av resurser och videoklipp.

**Finns det några begränsningar för videogranskningar?**

Ja. Det finns ett årligt tak för videokorrektur som sätts till 10 % av din organisations totala betalda Workfront-användarlicenser (Standard och Light). Denna övre gräns gäller på organisationsnivå.

Workfront-administratörer får meddelanden i appen när användningen når 80 % och 100 % av taket.

Denna gräns gäller inte för Frame.io Enterprise-kunder. Om din organisation regelbundet granskar stora volymer videoinnehåll kan du kontakta din Adobe-kontorepresentant för att få reda på mer om Frame.io Enterprise-licensiering.

**Kan samma användare visas i flera steg i ett godkännandearbetsflöde?**

Ja. En användare kan tilldelas till flera steg i samma arbetsflöde för godkännande.

**Kan jag lägga till faser för att skapa ett arbetsflöde för godkännande i flera steg?**

Ja. Arbetsflöden för godkännande i flera steg stöds, vilket gör att du kan dirigera resurser genom sekventiella gransknings- och godkännanderundor med olika deltagare i varje steg.

<!--
**Can I modify the trigger for a later stage---for example, based on all approved versus the due date ending?**

Stages in a multi-stage approval workflow proceed sequentially based on all required decisions being made in the current stage. When all assigned approvers in a stage have made their decisions, the next stage begins and the previous stage is locked. There is no option to trigger a stage based on the due date ending. If the "One decision required" toggle is enabled on a stage, the first approver decision completes that stage and advances the workflow.

**Can I remove the due date from an approval?**

Yes. Due dates are optional for both single-use approvals and approval templates. When creating a single-use approval, you can leave the deadline field empty. For approval templates, the relative completion timeframe is also optional.

**Can I change the default due date on new approval templates?**

Yes. When creating or editing an approval template, the timeframe (or "Workdays until due date" for multi-stage templates) can be adjusted per stage or left empty. The deadline is calculated automatically from this timeframe when the template is applied to an asset, so updating the template changes the default for all future approvals that use it.

**What happens when the deadline is reached for a review stage?**

For both single-stage and multi-stage reviews, automated reminder emails are sent at 72 hours, 24 hours, and on the deadline. However, reaching the deadline does not automatically reject the asset, lock the stage, or advance the workflow. Approvers and reviewers can still make decisions or complete their review after the deadline has passed. In a multi-stage workflow, each stage has its own independent deadline, and stages still advance based on all required decisions being made---not based on the deadline.
-->

**Kan mallar för godkännande innehålla grupper eller team, eller bara enskilda användare?**

Godkännandemallar har stöd för enskilda användare och team.

**Meddelas godkännare via e-post när de har något att granska?**

Ja. Godkännare och granskare får e-postmeddelanden när de tilldelas till en granskning eller godkännande. Automatiserade påminnelsemeddelanden skickas också 72 timmar före ansökningsdeadline, 24 timmar före och efter själva deadline.

Det går för närvarande inte att anpassa e-postmeddelanden, men det finns på produktfärdplanen.

<!--
**Can I change the notification frequency for a unified approver or reviewer (for example, all comments, replies to my comments, or daily summaries)?**

No. Notification frequency settings such as receiving all comments, only replies to your comments, or daily digest summaries are not currently available for unified review and approval. The system sends email notifications automatically when a user is assigned as a reviewer or approver, and automated reminder emails are sent at 72 hours, 24 hours, and on the deadline. The ability to customize notification messages and frequency is on the product roadmap.
-->

**Kan jag hålla en granskningsfas privat från andra deltagare?**

Det finns för närvarande ingen privat scenfunktion. För att hålla en granskning privat från andra deltagare rekommenderar vi att du skapar en separat kopia av resursen specifikt för den granskningsgruppen. Kommentarer segmenteras för närvarande inte av en deltagargrupp i en enskild tillgång.

Observera att versionshistorik, inklusive tidigare och aktuella versioner, alltid är synlig för alla som har tillgång till den resursen.

**Kan kommentarer markeras som lösta?**

Ja. Kommentarer kan markeras som lösta i Frame.io-visningsprogrammet.

**Vilka markerings- och anteckningsverktyg finns i Frame.io-visningsprogrammet?**

Visningsprogrammet Frame.io innehåller en komplett uppsättning visuella markeringsverktyg, inklusive frihandsritning och standardformer som cirklar, pilar och fyrkanter. För videomaterial tidstämplas kommentarerna med bildruteexakt precision, så feedback är alltid knuten till det exakta ögonblicket i klippet och inte bara till en allmän tidsstämpel.

**Kommer kommentarer som gjorts i Frame.io-visningsprogrammet att visas i Workfront-projektet?**

Kommentarer och anteckningar finns kvar i Frame.io-visningsprogrammet så att de behåller sitt fullständiga sammanhang, inklusive tidsstämplar och visuella markeringar. Detta kan komma att utvecklas i framtida versioner.

**Går det att lägga till kommentarer i en hämtad version av en resurs (t.ex. en PDF)?**

Detta stöds för närvarande inte, men det är en vanlig begärd funktion som är under övervägande för en framtida version.

**Kan jag granska flera resurser tillsammans som en grupp?**

Utökade alternativ för massgranskning kommer snart. Under tiden kan resurser av olika filtyper, t.ex. en video och ett Word-dokument, inkluderas i en grupperad resursgranskning.

**Är granskning och godkännande endast för video enhetlig, eller stöder det andra filtyper?**

Enhetlig granskning och godkännande är utformat för alla resurstyper, inte bara video. Visningsprogrammet Frame.io har uppdaterats avsevärt för att förutom video även stödja bilder, dokument, PDF-filer och andra vanliga filformat.

En fullständig lista över filtyper som stöds finns i dokumentationen för filtyper som stöds i Frame.io på Experience League.

**Kan jag dela resurser externt med intressenter som inte har tillgång till Workfront?**

Ja. Assets kan delas externt. Externa användare meddelas via e-post och uppmanas att skapa en Frame.io-inloggning för att få åtkomst till visningsprogrammet och delta i granskningen.

<!--
**Before unified review and approval, is a reviewer just directed to a proof?**

Yes. In the legacy proofing workflow (prior to unified review and approval), when a user was assigned as a reviewer they were directed to the Workfront Proof viewer (ProofHQ) to review the proof. With unified review and approval, reviewers are instead directed to the Frame.io viewer, which replaces the Workfront Proof viewer as the primary review surface.

**When I upload a document and not a proof, a proof gets generated. Will a proof always be generated?**

No. With unified review and approval enabled and Adobe enterprise storage active, uploading a document does not automatically generate a proof. Documents are stored in Adobe enterprise storage and are reviewed using the Frame.io viewer. A proof is only generated if you explicitly create one using the legacy proofing workflow. The Frame.io viewer serves as the primary review surface, so a separate proof is not needed for standard review and approval workflows.

**What is the difference between uploading a document and a proof after the 26.2 release?**

With unified review and approval enabled, uploading a document stores it in Adobe enterprise storage and makes it available for review in the Frame.io viewer. A unified approval workflow can be created directly on the document. Uploading a proof, by contrast, uses the legacy Workfront Proof viewer (ProofHQ) and its own proofing workflow. Both options are available for projects created before the integration was enabled, but the Frame.io viewer is the primary review surface going forward. The key difference is that a document uses the unified approval workflow and Frame.io viewer, while a proof uses the legacy proofing workflow and viewer.

**Reviews under My Approvals only show a "Complete my review" button and no link to the proofing viewer or the document. Is this intended?**

For unified review and approval, the My Approvals widget provides an "Open review" button that opens the asset in the Frame.io viewer, as well as action buttons to approve, request changes, or complete a review. Reviewers can complete their review directly from the widget. If you are only seeing a "Complete my review" button without a link to the viewer, this may reflect the reviewer role behavior---reviewers are not required to open the asset to mark their review as complete, though they can choose to open it in the Frame.io viewer to provide feedback before completing.

**Before unified review and approval, if a user is both an approver in a document approval and a reviewer/approver on a proof, both show up in the proof window. How do these work together?**

When using unified approvals alongside legacy proofing on the same document, the two workflows operate independently. Document approval participants are shown in the Document Summary panel, while proof participants are shown in the proofing workflow. The SOCD (Sent, Opened, Comment, Decision) indicators in the document list are proofing-related and do not reflect the unified approval decision status. These two workflows do not automatically sync---a decision made in one does not carry over to the other.

**If you upload a new version, the document approval users do not get repopulated. Is that intended?**

Yes. When a new version is uploaded, previous approval participants are not automatically repopulated. The previous version's approval process is closed and any outstanding approvals are marked as "Withdrawn." The document owner must manually add participants to the new version's approval workflow. An "Add all" button is available to quickly repopulate all participants from the previous version, and you can also selectively add previous participants or add new ones.
-->

+++

### Lagring och filhantering

+++ Expandera om du vill visa vanliga frågor om lagring och filhantering.

**Vad är Adobe Enterprise-lagring och hur hör det ihop med den här integreringen?**

Adobe Enterprise-lagring är det vanliga lagringsskiktet som ansluter Workfront, Frame.io och Adobe Creative Cloud. Assets finns på ett och samma ställe och är tillgängligt för alla verktyg utan manuell filöverföring. Kreatörerna kan arbeta på plats, och granskarna ser alltid den senaste versionen.

Några av fördelarna med Adobe Enterprise-lagring:

* Ett enda lager för alla resurser som är under arbete i Workfront och Frame.io

* Central åtkomstkontroll som hanteras via Adobe Identity Management System (IMS)

* Komplett synlighet - ingen versionslogik, inga förlorade metadata

* Skalbar lagringshantering i enterpriseklass

**Finns det namngivnings- eller strukturkrav för filer och projekt?**

Ja. Eftersom integreringen använder Adobe Enterprise-lagring gäller följande konventioner:

* Objekt- och dokumentnamn måste vara unika inom samma överordnade i mapphierarkin.

* Dokument i samma projekt kan inte ha samma namn.

* Program, portföljer, projekt, mallar, uppgifter, utgåvor, dokument, dokumentmappsnamn får inte innehålla följande specialtecken: `\ / : * ? " | < >` och får innehålla högst 255 tecken.

Workfront byter automatiskt namn på objekt och dokument efter behov för att förhindra konflikter.

**Vilka filtyper stöds i Frame.io-visningsprogrammet?**

Visningsprogrammet Frame.io har stöd för över 40 filformat, inklusive alla vanliga typer av video, bilder, ljud, PDF och Microsoft Office. Videofunktionen innehåller inbyggd uppspelning för professionella format som ProRes, H.265 och DNxHD, med stöd för filer på upp till 500 GB.

Frame.io har tagits fram för kreativ granskning, vilket innebär att den hanterar alla typer av mediefiler som marknadsförare och kreativa team arbetar med.

+++

### Behörigheter och åtkomst

+++ Expandera om du vill visa vanliga frågor om behörigheter och åtkomst.

**Hur hanteras användarbehörigheter?**

Användarbehörigheter anges och styrs i Workfront och flödar automatiskt till Frame.io. Du kan inte bjuda in användare eller ändra behörigheter direkt i Frame.io för den här integreringen. All åtkomsthantering måste utföras med projektdelningstekniken i Workfront.

Tabellen nedan visar hur Workfront-behörigheter mappas till Frame.io-behörigheter:

<table>
  <thead>
    <tr>
      <th>Workfront Permission</th>
      <th>Ram.io - behörighet</th>
    </tr>
  </thead>
  <tbody>
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
  </tbody>
</table>

+++


### Integrering och avancerade funktioner

+++ Expandera om du vill visa vanliga frågor om integreringar och avancerade funktioner.

**Hur påverkar detta integreringar mellan Creative Cloud och GenStudio?**

Integrationer som stöder Frame.io-visningsprogrammet är under utveckling för Adobe Express och GenStudio Performance Marketing. De nya integreringarna kommer att bygga på samma enhetliga gransknings- och godkännandesystem, så de kommer att utnyttja Frame.io-visningsprogrammet för en konsekvent granskningsupplevelse för alla tre produkterna.

**Är Frame.io integrerat i Workfront, eller navigerar användare till ett separat gränssnitt?**

Användare kan starta Frame.io-visningsprogrammet direkt från Workfront. Alla gransknings- och godkännandeaktiviteter äger rum i Frame.io-visningsprogrammet och synkroniseras automatiskt tillbaka till Workfront.

**Kan jag skicka godkända mediefiler till Adobe Experience Manager (AEM)?**

Ja. När en mediefil har granskats och godkänts kan du överföra den till Adobe Experience Manager Assets för slutlig lagring och distribution. Detta kopplar ihop Workfront för arbetshantering, Frame.io för granskning och AEM för hantering av digitala resurser till ett enhetligt supply chain-innehåll.

Mer information finns i [Använda Adobe Experience Manager med Frame.io-integrering](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

**Hur passar en enhetlig granskning och godkännande in i Adobe GenStudio?**

Enhetlig granskning och godkännande är en grundläggande komponent i Adobe GenStudio - Adobe bredare vision för ett uppkopplat material i supply chain. GenStudio kopplar ihop Workfront, Frame.io, Creative Cloud, Adobe Express, Adobe Experience Manager Assets och GenStudio for Performance Marketing i ett enhetligt arbetsflöde från kampanjrapporter till innehållsleverans.

Inom det ekosystemet fungerar granskning och godkännande som den kritiska utgångspunkten mellan skapande och leverans. Det är där det kreativa arbetet möter intressenternas synpunkter, kvaliteten valideras och innehållet klargörs för publicering. När överföringen är snabb, synlig och tillförlitlig låser den upp hastigheten i hela det material som supply chain har - AI kan snabba upp framtagningen, automatiseringen kan hantera distributionen, men en flaskhals i granskningen kan maximera vinsten på båda sidor. När du ansluter Workfront och Frame.io tas flaskhalsen bort.

**Vad är AI Reviewer-funktionen?**

Enhetlig granskning och godkännande innefattar en AI Reviewer-funktion som automatiserar märkeskompatibilitetskontroller som en del av granskningsprocessen. AI Reviewer kan utvärdera resurser mot varumärkesriktlinjer och flagga potentiella problem innan granskarna är engagerade, så att teamen kan fånga upp problem tidigare och agera snabbare.

Mer information om hur du konfigurerar och använder AI Reviewer finns i Workfront-dokumentationen för Experience League.

+++

### Kontrakt, SKU och lagring

+++ Expandera om du vill visa vanliga frågor om kontrakt, SKU:er och lagring.

**När blir en enhetlig granskning och godkännande tillgänglig för mig?**

Nu finns enhetlig granskning och godkännande. För åtkomst krävs en uppgradering till en Workfront V2 SKU. Om ditt kontrakt undertecknades innan V2-SKU:erna var tillgängliga kan du få åtkomst på något av följande två sätt:

* När avtalet förnyas: Åtkomst aktiveras vid nästa förnyelsedatum.

* Tidig omkontraktshantering: Adobe-kontoteamet kan omsluta dig tidigt för att lägga till de nya SKU-berättigandena samtidigt som det befintliga slutdatumet för kontraktet behålls. Ingen prisökning sker vid byte till ett motsvarande paket.

Kontakta din Adobe-kontorepresentant för att fastställa den bästa vägen för din organisation.

<!--
**Before we sign the contract, what changes will we see in Workfront?**

Before signing the V2 SKU contract, your Workfront instance will continue to operate using the existing document and proofing experience. No unified review and approval features---such as the Frame.io viewer, Adobe enterprise storage, or multi-stage approval templates---will be available until the V2 SKU is contracted and Adobe Professional Services configures the integration for your organization.
-->

**Ger uppgradering till V2 SKU mer lagringsutrymme?**

Ja. Med V2 SKU får varje licensierad användare 60 GB lagringsutrymme, vilket är en ökning från 30 GB i den tidigare versionen.

**Hur väljer jag mellan Adobe Enterprise-lagring och äldre Workfront-lagring?**

Enterprise Storage möjliggör Frame.io-visning och krävs för enhetlig granskning och godkännande. Äldre lagring fortsätter att använda Workfront Proof Viewer (ProofHQ) som standard.

Om din organisation har en blandning av enkla arbetsflöden och mer komplicerade korrekturarbetsflöden kan du prioritera vilka arbetsflöden som ska migreras först.

Enterprise Storage ger er flexibilitet att lansera den nya upplevelsen stegvis, med början i de arbetsflöden som kommer att vara till störst nytta.

**Hur hanteras Frame.io-licenser?**

När V2-SKU:n har signerats får alla Workfront-användare tillgång till Frame.io-visningsprogrammet för granskning och godkännande - det krävs ingen separat licens för Frame.io Enterprise.

Om din organisation behöver fler Frame.io Enterprise-funktioner som

* Avancerad vattenstämpel (dynamisk och kriminalteknisk)
* Hantering av digitala rättigheter med automatisk borttagning av resurser
* Inloggningsuppgifter för AI-genererat innehåll
* Egna kreativa metadata
* Integreringar mellan kamera och moln
* Din egen arbetsyta för pågående kreativt arbete

kan du samarbeta med ditt Adobe-kontoteam för att fastställa rätt antal Frame.io Enterprise-licenser. Alla licenser hanteras via Adobe Admin Console.

+++

### Sandbox och rollout

+++ Expandera om du vill visa vanliga frågor om sandlådor och utrullningar.

**Kan jag testa enhetlig granskning och godkännande i en sandlådemiljö?**

Delvis. Arbetsflöden för godkännande kan testas i Workfront sandlådemiljö. Visningsprogrammet Frame.io är dock inte tillgängligt i sandlådan. Själva granskningsytan måste testas i en produktionsmiljö.

Om du vill begränsa exponeringen under utrullningen kan du aktivera enhetlig granskning och godkännande för en viss grupp i Workfront produktionsmiljö. På så sätt kan du köra en riktad pilot med en mindre uppsättning användare innan du distribuerar den vidare.

<!--
**How should we test future quarterly releases involving unified review and approval if the Frame.io viewer is not available in sandbox?**

Because the Frame.io viewer experience is not available in the Workfront sandbox environment, testing future quarterly releases should be done using a controlled pilot group in your production environment. You can enable unified review and approval for a specific group within your Workfront production instance, allowing a smaller set of users to validate new features as they release. Approval workflow configuration and template setup can still be tested in sandbox, but the full review experience---including the Frame.io viewer---must be validated in production.
-->

+++

### Interaktiva korrektur och HTML

+++ Expandera om du vill visa vanliga frågor om interaktiva korrektur och HTML.

**Har enhetlig granskning och godkännande stöd för interaktiva korrektur eller HTML URL:er?**

Zip HTML-filer stöds för närvarande för interaktiv granskning. Stöd för HTML URL (live web URL review) finns på färdplanen och förväntas under tredje kvartalet.

Läs Workfront versionsinformation om Experience League för att få uppdateringar.

+++

### Fusion och automatisering

+++ Expandera för att visa vanliga frågor om Fusion och automatisering.

**Behöver jag Workfront Fusion för att använda enhetlig granskning och godkännande?**

Nej. Enhetlig granskning och godkännande är en inbyggd produktintegrering och kräver inte Fusion. Arbetsflödet är inbyggt direkt i Workfront.

**Kommer Fusion-anslutningar att vara tillgängliga för enhetlig granskning och godkännande?**

Ja. Fusion-åtgärder för enhetlig granskning och godkännande håller för närvarande på att utvecklas och förväntas bli tillgängliga under tredje kvartalet. Läs Workfront versionsinformation om Experience League för att se om det finns uppdateringar när de blir tillgängliga.

**Kan Fusion användas för att automatiskt starta en granskning när ett dokument överförs?**

Ja. Den här typen av automatisering är möjlig med Workfront webhooks i kombination med Fusion.

**Hur kommer befintliga Fusion-arbetsflöden som bygger på Workfront Proof att påverkas?**

Effekten varierar beroende på hur varje arbetsflöde skapas. I allmänhet:

* **Redigera eller uppdatera**: Arbetsflöden där den befintliga korrekturrelaterade åtgärden har en direkt motsvarighet i enhetliga godkännanden kan uppdateras för att använda den nya åtgärden.

* **Återskapa**: Arbetsflöden där de underliggande stegen har ändrats avsevärt, eller där det finns nya funktioner, kan behöva återskapas från grunden.

En tydligare bild kommer att uppstå när Fusion API:er för enhetliga godkännanden är tillgängliga. Vi rekommenderar att du granskar dina befintliga Fusion-arbetsflöden och utvärderar dem mot de nya enhetliga godkännandefunktionerna vid den tidpunkten.

+++







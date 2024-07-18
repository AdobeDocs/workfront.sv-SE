---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Final
description: Versionsaktivitet 2018.3
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 38974e97-dea3-4c9e-bc32-bd55665370c7
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1177'
ht-degree: 0%

---

# R1 Final

Följande funktionalitet är för närvarande inte tillgänglig i Preview eller Beta, men släpps till produktionsmiljön i R1:

## Utför godkännandebeslut för korrektur från Min arbetsyta (Workfront)

När en användare lägger till dig i ett korrektur och ger dig rollen Godkännare eller rollen Granskare och godkännare (antingen från det fristående Korrektur-HQ-programmet eller genom att använda automatiserat arbetsflöde i Workfront) visas godkännandebegäran på fliken Godkännanden i arbetsytan Mitt arbete. Sedan kan du titta på beviset och godkänna det direkt från Workfront.

Mer information om hur du lägger till användare i ett korrektur med Automated Workflow finns i [Dela ett korrektur i Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) i [Dela ett korrektur i Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

Mer information om hur du fattar beslut om godkännande på arbetsytan Mitt arbete finns i [Godkänna arbete](../../../../review-and-approve-work/manage-approvals/approving-work.md) i [Godkänna arbete](../../../../review-and-approve-work/manage-approvals/approving-work.md). 

## Rapport om korrekturgodkännanden på arbetsytan My Work (Workfront)

Nu kan du skapa en rapport baserad på objektet Korrektur för godkännande. Med den här rapporten kan du rapportera om korrekturgodkännanden från användarnas arbetsytor där beslut ännu inte har fattats.

Godkännanderapporter innehåller följande information:

* Dokument som har skickats för godkännande
* Godkännarens namn
* Korrekturversion
* Korrektur-ID
* Datum för korrekturskapande

Du får åtkomst till det här godkännandet när du skapar en rapport baserad på ett objekt, vilket beskrivs i [Skapa en anpassad rapport](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Mer information om objektrapporten för korrekturgodkännanden finns i avsnittet [Förstå objekt i Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) i [Förstå objekt i Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Generera automatiskt en ny version av ett dokumentkorrektur med dra-och-släpp (Workfront)

När du använder dra och släpp-metoden för att lägga till en ny version av ett dokument som kräver korrektur, genereras ett korrektur automatiskt. Korrekturkorrekturet har samma alternativ och arbetsflöden som det ursprungliga korrekturet eller den tidigare versionen.

När du tidigare lade till en ny version av dokumentet genererades inte korrekturet automatiskt i den nya versionen och du var tvungen att generera om korrekturet för den nya versionen.

När du använder menyn Dokument, mer för att överföra en ny version, genereras inget korrektur automatiskt.

Mer information finns i  avsnitt i

## Ge alla korrekturanvändare tillgång till Korrektur på högdagrar direkt från Workfront-gränssnittet (Workfront)

Nu kan du ge alla språkanvändare i ditt system smidig åtkomst till ditt ProofHQ Premium-konto direkt från Workfront gränssnitt. När det här alternativet är aktiverat visas en Korrektur-HQ-ikon i det globala navigeringsfältet som dirigerar dem till webbplatsen för Korrektur.

Det här alternativet är inte aktiverat som standard. Om du vill aktivera det här alternativet kontaktar du Workfront tekniska support och begär åtkomst för alla språkanvändare i ditt system.

Mer information finns i [Åtkomst till Workfront Proof från Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md) i  [Öppna Workfront Proof från Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

Före den här ändringen kunde bara Workfront-administratören ha direktåtkomst till webbplatsen ProofHQ från Workfront gränssnitt.

## Nytt alternativ för TLS Secure Connection för utgående e-post (Workfront)

När du väljer att hantera din Workfront-kommunikation med din egen e-postserver kan du nu aktivera din utgående e-post för att använda en säker TLS-anslutning.

Före den här förbättringen kunde du bara aktivera utgående e-post via en säker SSL-anslutning.

Mer information om hur du konfigurerar utgående e-post finns i .

## Nytt fält för att hantera e-postmeddelanden i förhandsgranskningssandlådemiljön

Workfront inaktiverar nu all e-postkommunikation från sandlådemiljön Preview och den anpassade uppdateringsmiljön. Om du vill få e-postmeddelanden från förhandsgranskningssandlådan eller anpassade uppdateringsmiljöer måste du aktivera den här funktionen i dina användarinställningar.

Mer information finns i följande information:

* [Sandlådemiljön Adobe Workfront Preview](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) i [Sandlådemiljön Adobe Workfront Preview](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

* &quot;Tar emot e-postmeddelanden från den anpassade uppdateringssandlådan&quot; i [den anpassade uppdateringssandlådemiljön i Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)

## Outlook för Office 365 (Workfront)

Workfront-tillägget för Outlook 365 är nu tillgängligt. 

Mer information om hur du använder tillägget finns i [Använda Workfront-tillägget med Outlook för Office 365.](https://support.workfront.com/hc/en-us/sections/205046167)

## Sök i mobilappen (Workfront)

Nu kan du söka efter objekt i mobilappen, på samma sätt som du söker i webbprogrammet. Den nya sökfunktionen söker först efter objekt i listan Senaste objekt samt de objekt som tidigare har laddats ned till din mobila enhet. Listan med de senaste objekten är den som du ser i webbprogrammet.

>[!NOTE]
>
>Den här funktionen kommer att vara tillgänglig den första veckan i maj 2017.

Mer information om mobilappen finns i avsnittet Söka i mobila enheter i  

## Förbättrad hjälp i mobilappen: Tutorials (Workfront)

Från och med mobilversionen i april kommer du att se nya självstudiekurser som vägleder dig genom din mobila upplevelse. När du loggar in i mobilappen för första gången och använder en funktion för första gången visas en kort självstudiekurs som förklarar hur funktionen fungerar. Självstudiekursen visas bara en gång, första gången du använder en viss funktion.

Mer information om mobilappen finns i .

## Sök i PDF-dokument (ProofHQ)

Nu kan du söka i PDF-dokument, Office-dokument och statiska webbsidor.

Mer information finns i  [Sök efter innehåll i ett korrektur](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/search-in-a-proof.md).

## Uppdaterat globalt navigeringsfält (ProofHQ)

ProofHQ Premium-konton som är integrerade med Workfront ser nu följande förbättringar i Global Navigation Bar i ProofHQ:

* Ny användarprofilbild 
* Uppdaterat utseende och känsla

## Inkludera ytterligare information i anpassade vyer (KorrekturHQ)

Du kan nu inkludera följande ytterligare information i anpassade vyer:

* **Data på mottagarnivå**\
  Du kan konfigurera anpassade vyer så att de omfattar följande kolumner som är relaterade till data på mottagarnivå: Roll, Position, E-postaviseringar, Min deadline, Datum tillagd i korrektursökning och Mottagarsökning.\
  Mer information finns i [Skapa och hantera anpassade vyer i Workfront Proof-korrektur](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **Språkdata**\
  Du kan konfigurera anpassade vyer så att de innehåller följande kolumner som är relaterade till korrekturdata: antal kommentarer (alla versioner), storlek på disk, korrekturtyp, antal filer per version, data för bifogade kommentarer (storlek på disk, filnamn) och filtrering efter undermapp.\
  Mer information finns i [Skapa och hantera anpassade vyer i Workfront Proof-korrektur](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **Data på scennivå relaterade till automatiserade arbetsflöden**\
  Du kan konfigurera anpassade vyer så att de omfattar följande kolumner som är relaterade till enskilda steg i automatiserade arbetsflöden: SOCD-status, Stage Deadlines, Active Stage Name, Next Stage Name, Stage name och Template.\
  Mer information finns i [Skapa och hantera anpassade vyer i Workfront Proof-korrektur](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## Förbättringar av korrekturrapporter (tidigare analyser) (Korrektur, högdagrar)

Rapporteringsfunktionen (tidigare Analytics) innehåller följande förbättringar:

* Nya standardrapporttyper:

   * Korrekturstid
   * Procent för sent godkännande
   * Korrektur för första aktivitetstiden
   * Antal kommentarer och svar

* Skriv ut rapporter
* Uppdaterat utseende och känsla

## Visa Korrektur för högdagrar i förhandsvisningsmiljön (ProofHQ)

Funktioner som släpps till ProofHQ är först tillgängliga för testning i förhandsvisningsmiljön innan de släpps till produktionsmiljön.

Det nya arbetsflödet med att släppa funktionalitet till Förhandsgranska före produktion gör att du kan vara mer förberedd för framtida uppdateringar av produktionsmiljön för korrektur och högkvarter.

Mer information om förhandsvisningsmiljön för Korrektur för högdagrar finns i [Testmiljö för förhandsgranskning av sandlådor - Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).

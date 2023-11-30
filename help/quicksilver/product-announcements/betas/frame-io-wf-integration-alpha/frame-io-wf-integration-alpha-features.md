---
content-type: reference
navigation-topic: betas
title: "Adobe Workfront och Frame.io inbyggd integration alpha: features"
description: Planerade funktioner för Adobe Workfront och Frame.io, inbyggd integration alpha
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
exl-id: a1603a06-957b-4d52-89f3-f0cec1a4e02c
source-git-commit: 15e2869417d8315bf8e96f7d9d537cd70a5e39df
workflow-type: tm+mt
source-wordcount: '1204'
ht-degree: 0%

---

# Adobe Workfront och Frame.io, inbyggd integration alpha: funktioner och testning

Med den här integreringen är vårt mål att göra det möjligt för kreatörer att behålla sina valfria verktyg (CC eller Frame.io) för att skapa innehåll och utföra peer-granskningar, samtidigt som projektledare koordinerar arbetet och initierar och övervakar den formella granskningsprocessen inifrån Workfront. Detta kan uppnås genom att man använder det bästa av båda lösningarna: Workfront nya dokumentgodkännanden för att hantera innehållsgodkännanden, tillsammans med de innehållsgranskningsfunktioner som Frame.io erbjuder. De nya dokumentgodkännandena och Frame.io kommer tillsammans att utgöra vår nya heltäckande upplevelse för granskning och godkännande av innehåll. 

Mer information om hur alfavärdet fungerar och hur du kan delta finns i [Integreringsalfa för Adobe Workfront och Frame.io: översikt](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)


>[!NOTE]
>
>Om du kommer på dessa sidor utan att ditt företag deltar i det här alfaversionsprogrammet, var noga med att behandla informationen här och kontakta din Workfront- eller Frame.io-administratör för mer information.

## Grundläggande testscenario

För att du enkelt ska kunna testa de nya funktionerna i alfaversionen har vi skapat ett nytt test-konto för Frame.io och kopplat det till en ny grupp som kallas `Frame.io alpha testing` i Workfront Preview- eller Sandbox-miljö.

Om du vill testa funktionen loggar du in på Workfront Preview eller Sandbox och utför följande steg:

>[!NOTE]
>
><span class="preview">Markerad text</span> Nedan beskrivs funktioner som ännu inte har implementerats för testning, men som kommer att ingå i en senare version.
>

1. **Koordinatorer:** Skapa ett projekt i Workfront med `Frame.io alpha testing` grupp tilldelad som projektgrupp.

1. **Koordinatorer:** Inom Workfront kan du tilldela dina kreatörer till projektet <span class="preview">eller Aktiverade bildruteuppgifter</span> och ändra projektstatus till Aktuell.

1. **Kreatörer:** Kontrollera dina e-postmeddelanden om det finns en inbjudan till det nyligen skapade Frame.io-projektet

1. **Kreatörer:** Klicka på knappen&quot;Gå med i projekt&quot; i e-postmeddelandet med en inbjudan om att gå med i Frame.io-projektet, granska det kreativa utkastet i projektet och börja skapa ditt innehåll i valfritt verktyg på Creative Cloud.

1. **Kreatörer:** Överför dina skapade resurser till Frame.io och lägg till dem i det länkade Workfront-projektet <span class="preview">(eller tilldelade bildruteaktiverade uppgifter).</span>

1. **Koordinatorer:** I Workfront hittar du de länkade Frame.io-resurserna i ditt projekt och tilldelar granskare/godkännare (mer information om hur du tilldelar granskningar/godkännare finns i [Lägga till ytterligare godkännare eller granskare i ett dokument](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/add-additional-reviewers-or-approvers.md)).

1. **Intressenter:** I Workfront kan du visa din godkännandebegäran i Hem- eller Dokumentinformation och granska dokumentet Frame.io Viewer. Lämna sedan en kommentar med feedback.

1. <span class="preview">**Koordinatorer:** I Workfront kan du visa de kommentarer som har skapats av berörda parter i uppdateringsavsnittet i det dokument som är kopplat till Frame.io.</span>

1. <span class="preview">**Intressenter:** Fatta ett beslut inifrån Frame.io Viewer.</span>

1. <span class="preview">**Kreatörer:** I Frame.io ser du det övergripande godkännandebeslutet för dina tillgångar.</span>

1. **Kreatörer:** I Frame.io tillämpar du de begärda ändringarna genom att lägga till den uppdaterade versionen i den anslutna resursens versionsstack.

1. **Koordinatorer:** I Workfront tilldelar du godkännare/granskare till den nyligen överförda versionen och övervakar förloppet tills den har signerat.

## Funktionsplaner

Nedan finns information om de primära användningsområdena som vi vill ta upp och de funktioner vi planerar att göra det. <!--, along with documentation to get you started testing.-->

>[!NOTE]
>
><span class="preview">Markerad text</span> Nedan beskrivs funktioner som ännu inte har implementerats, men som kommer att ingå i en senare version.
>
>Punkter under en **&quot;Potentiella förbättringar i framtida releaser&quot;** sidhuvudet kan, eller behöver inte, ingå i en framtida release, beroende på feedback och våra utvecklingsplaner.
>


### Workfront-administratörer kan skapa en anslutning mellan Workfront-grupper och Frame.io-konton

* <span class="preview">I Workfront kan du ansluta en Workfront-grupp till ett Frame.io-konto</span>

* Ett nytt Frame.io-team skapas i Frame.io som representerar den anslutna Workfront-gruppen

**Potentiella förbättringar i framtida versioner:**

* Koppla från en Workfront-grupp från ett Frame.io-konto

* Koppla en Workfront-grupp till ett befintligt Frame.io-team

### Projektsamordnare kan konfigurera vilka Workfront-projekt som skickas till Frame.io och lägga till de tilldelade kreativa i Workfront i projektet Frame.io

* Möjlighet att markera Workfront-projekt som Frame.io aktiverat genom att tilldela en bildruteansluten grupp

* <span class="preview">Förbättring: Möjlighet att växla aktiviteter i Workfront-projekt till Frame-åtgärder som i sin tur skapar uppgiftsmappar i Frame.io</span>

* När statusen för ett Workfront-projekt är Aktuell skapas ett motsvarande anslutet projekt i bildrutan, användare som tilldelats Workfront läggs till i bildruteprojektet och ett e-postmeddelande skickas till dem från Frame.io

   * Alla Workfront Project-medlemmar (användare och team) läggs till som medarbetare i Frame.io-projektet (när projekt skapas och senare)

   * <span class="preview">Ändra: Användare och team som är tilldelade till bildruteaktiverade Workfront-uppgifter läggs till som medarbetare i Frame.io-projektet och meddelas (när projekt skapas och senare)</span>

* Dokument (Creative Brief) som läggs till i projektet och aktiviteter som är aktiverade för bildruta flyttas till Frame.io-projektet (i respektive arbetsmapp) när projektet skapas (utlösare: projektstatus inställd på Aktuell)

   * Vi rekommenderar att du begränsar antalet dokument som läggs till i projektet innan du börjar arbeta med bara dina projektdokument, så att du slipper skicka flera onödiga dokument till Frame.io.

* <span class="preview">Förbättring: Användare/team som uttryckligen inte tilldelats från en bildruteaktiverad Workfront-uppgift tas bort från Frame.io-projektet</span>

**Potentiella förbättringar i framtida versioner:**

* Ramaktiverade uppgifter kan konfigureras för projektmallar

* Nya versionsuppladdningar till kreativa informationsdokument kommer att överföras till Frame

* Optimerad projektsynkronisering (koppla från projekt, synkronisera om projekt och dokument osv.)

### Inom Frame.io kan kreativa personer skicka skapade resurser till Workfront-projektet för formell granskning

* Möjlighet att ansluta en Frame.io-resurs till ett WF-projekt eller en WF-uppgift. En resursreferens kommer att skapas i Workfront

* Överföringar av nya versioner inuti Frame.io skapar automatiskt nya dokumentversioner i Workfront för anslutna resurser

* <span class="preview">Förbättring: Möjlighet att markera de refererade Workfront-åtgärderna som slutförda inifrån Frame.io</span>

* <span class="preview">Förbättring: Om det anslutna Workfront-dokumentet tas bort ligger det kvar i Frame.io och kan återanslutas till samma eller andra projektuppgifter</span>

**Potentiella förbättringar i framtida versioner:**

* Skicka flera Frame.io-resurser till Workfront samtidigt

* Tidsloggning mot Workfront-projekt/uppgifter inifrån Frame.io

### Projektsamordnare kan tilldela den formella godkännandeprocessen till dokument som är länkade från Frame.io

* Workfront-användare och -team kan läggas till i nya dokumentgodkännanden för Frame.io-anslutna dokument

* <span class="preview">Förbättring: När en användare/ett team inte delas från ett dokument som är aktiverat för bildrutor förlorar de även åtkomsten till resursen i Frame.io Viewer</span>

**Potentiella förbättringar i framtida versioner:**

* Skicka flera resurser som en enda granskning

* Tilldela godkännare/granskare gruppvis till Workfront-dokument

### Intressenter kan granska och godkänna dem i Frame.io Viewer

* Intressenterna meddelas och kan visa dokumentet som är kopplat till ramen i Frame.io Viewer

* Frame.io Viewer kan nås från olika platser i Workfront, t.ex. Dokumentlista, Dokumentinformation, Workfront startsida

* Möjlighet att utnyttja de gransknings- och kommentarfunktioner som finns i Frame.io Viewer, som kommer att synkroniseras med Workfront Update Stream

* <span class="preview">Möjlighet att fatta ett beslut om godkännande av ett nytt dokument inifrån Frame.io Viewer</span>

### Inom Frame.io kommer kreatörerna att informeras om det övergripande beslutet som fattats om den anslutna Frame.io-resursen

* <span class="preview">Förbättring: Den övergripande statusen för dokumentgodkännande visas för resurser i Frame.io</span>

### Projektsamordnare kan skicka det slutliga materialet till AEM

* <span class="preview">Förbättring: Ramanslutna dokument, inklusive metadata, kan skickas till AEM med den befintliga Workfront + AEM Asset CS-kopplingen</span>

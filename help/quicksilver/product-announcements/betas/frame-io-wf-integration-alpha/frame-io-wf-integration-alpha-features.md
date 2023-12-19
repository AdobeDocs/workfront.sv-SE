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
source-git-commit: 9e6033e495e83afa994b21996a4026ac484045a0
workflow-type: tm+mt
source-wordcount: '1250'
ht-degree: 0%

---

# Adobe Workfront och Frame.io, inbyggd integration alpha: funktioner och testning

Med den här integreringen är vårt mål att göra det möjligt för kreatörer att behålla sina valfria verktyg (CC eller Frame.io) för att skapa innehåll och utföra peer-granskningar, samtidigt som projektledare koordinerar arbetet och initierar och övervakar den formella granskningsprocessen inifrån Workfront. Detta kan uppnås genom att man använder det bästa av båda lösningarna: Workfront nya dokumentgodkännanden för att hantera innehållsgodkännanden, tillsammans med de innehållsgranskningsfunktioner som Frame.io erbjuder. De nya dokumentgodkännandena och Frame.io kommer tillsammans att utgöra vår nya heltäckande upplevelse för granskning och godkännande av innehåll. 

Mer information om hur alfavärdet fungerar och hur du kan delta finns i [Integreringsalfa för Adobe Workfront och Frame.io: översikt](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md).

>[!NOTE]
>
>Om du kommer på dessa sidor utan att ditt företag deltar i det här alfaversionsprogrammet, var noga med att behandla informationen här och kontakta din Workfront- eller Frame.io-administratör för mer information.
>

## Demonstrationsvideo

>[!VIDEO](https://video.tv.adobe.com/v/3426406/)

## Grundläggande testscenario

För att du enkelt ska kunna testa de nya funktionerna i alfaversionen har vi skapat ett nytt test-konto för Frame.io och kopplat det till en ny grupp som kallas `Frame.io alpha testing` i Workfront Preview- eller Sandbox-miljö.

Om du vill testa funktionen loggar du in på Workfront Preview eller Sandbox och utför följande steg:

1. **Koordinatorer:** Skapa ett projekt i Workfront med `Frame.io alpha testing` grupp tilldelad som projektgrupp.

1. **Koordinatorer:** I Workfront markerar du de uppgifter som kräver kreativt arbete som bildruteaktiverade (i uppgiftsinformationen) och tilldelar dina användare (tilldela dig själv också om du vill testa hela arbetsflödet).

>[!NOTE]
>
>Underaktiviteter kan inte markeras som bildrutor aktiverade.
>

1. **Koordinatorer:** Ladda upp din översikt och ändra projektstatus till Aktuell.

1. **Kreatörer:** Kontrollera dina e-postmeddelanden om det finns en inbjudan till det nyligen skapade Frame.io-projektet

1. **Kreatörer:** Klicka på knappen&quot;Gå med i projekt&quot; i e-postmeddelandet med en inbjudan om att gå med i Frame.io-projektet, granska det kreativa utkastet i projektet och börja skapa ditt innehåll i valfritt verktyg på Creative Cloud.

1. **Kreatörer:** Överför dina skapade resurser till Frame.io och lägg till dem i det länkade Workfront-projektet genom att välja någon av de tilldelade Frame-aktiverade åtgärderna. Välj alternativet för att markera uppgiften som slutförd.

1. **Koordinatorer:** I Workfront söker du efter de länkade Frame.io-resurserna i den bildruteaktiverade aktiviteten och kontrollerar att aktivitetens status har ändrats till&quot;complete&quot;.

1. **Koordinatorer:** Tilldela granskare/godkännare till den länkade Frame.io-resursen. Tilldela dig själv som godkännare också om du vill testa hela arbetsflödet. (Mer information om hur du tilldelar granskningar/godkännare finns i [Lägga till ytterligare godkännare eller granskare i ett dokument](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/add-additional-reviewers-or-approvers.md)).

1. **Intressenter:** I Workfront kan du visa din godkännandebegäran i Hem, Dokumentinformation eller i det mottagna e-postmeddelandet. Öppna resursen i Frame.io Viewer, lämna en kommentar med feedback och fatta ett beslut.

1. **Koordinatorer:** I Workfront kan du läsa de kommentarer som har skapats av berörda parter i uppdateringsavsnittet i det dokument som är kopplat till Frame.io samt beslutet i godkännandeavsnittet eller dokumentsammanfattningsfönstret.

1. **Kreatörer:** I Frame.io ser du det övergripande godkännandebeslutet för dina tillgångar.

1. **Kreatörer:** I Frame.io tillämpar du de begärda ändringarna genom att lägga till den uppdaterade versionen i den anslutna resursens versionsstack.

1. **Koordinatorer:** I Workfront tilldelar du godkännare/granskare till den nyligen överförda versionen och övervakar förloppet tills den har signerat.

## Detaljerat testscenario

För deltagare som vill testa ytterligare funktioner har vi skapat ett mer komplicerat testscenario. En guide för detta detaljerade testscenario kan laddas ned här: [WF + Frame.io Detailed Test Scenario Walkthrough](/help/quicksilver/product-announcements/betas/assets/WF-Frame-Detailed-Test-Scenario-Walkthrough.pdf).

## Funktionsplaner

Nedan finns information om de primära användningsområdena som vi vill ta upp och de funktioner vi planerar att göra det. <!--, along with documentation to get you started testing.-->

>[!NOTE]
>
>Punkter under en **&quot;Potentiella förbättringar i framtida releaser&quot;** sidhuvudet kan, eller behöver inte, ingå i en framtida release, beroende på feedback och våra utvecklingsplaner.
>

### Workfront-administratörer kan skapa en anslutning mellan Workfront-grupper och Frame.io-konton

* I Workfront kan du ansluta en Workfront-grupp till ett Frame.io-konto

* Ett nytt Frame.io-team skapas i Frame.io som representerar den anslutna Workfront-gruppen (observera att den här funktionen bara har aktiverats för kunder som använder integreringen i Production. Kunder som fortfarande testar i sandlådan eller förhandsgranskningen kommer att ha anslutningen konfigurerad av Adobe team.)

**Potentiella förbättringar i framtida versioner:**

* Koppla från en Workfront-grupp från ett Frame.io-konto

* Koppla en Workfront-grupp till ett befintligt Frame.io-team

### Projektsamordnare kan konfigurera vilka Workfront-projekt som skickas till Frame.io och lägga till de tilldelade kreativa i Workfront i projektet Frame.io

* Möjlighet att markera Workfront-projekt som Frame.io aktiverat genom att tilldela en bildruteansluten grupp

* Möjlighet att växla aktiviteter i Workfront-projekt till Frame-uppgifter som i sin tur skapar uppgiftsmappar inuti Frame.io

* Om ett Workfront-projekt har en bildruteansluten grupp tilldelad och minst en bildruteaktiverad uppgift, och Workfront-projektstatus är Aktuell, skapas ett motsvarande anslutet projekt i bildruta, Workfront-tilldelade användare läggs till i bildruteprojektet och ett e-postmeddelande skickas till dem från Frame.io

   * Användare och team som är tilldelade Frame-aktiverade Workfront-uppgifter läggs till som medarbetare till Frame.io-projektet och meddelas (när projekt skapas och senare)

* Dokument (Creative Brief) som läggs till i projektet och aktiviteter som är aktiverade för bildruta flyttas till Frame.io-projektet (i respektive arbetsmapp) när projektet skapas (utlösare: projektstatus inställd på Aktuell)

   * Vi rekommenderar att du begränsar antalet dokument som läggs till i projektet innan du börjar arbeta med bara dina projektdokument, så att du slipper skicka flera onödiga dokument till Frame.io.

   * Dokument/uppgifter som läggs till efter den inledande projektsynkroniseringen överförs inte till Frame.io, endast användare/team

**Potentiella förbättringar i framtida versioner:**

* Ramaktiverade uppgifter kan konfigureras för projektmallar

* Nya versionsuppladdningar till kreativa informationsdokument kommer att överföras till Frame

* Optimerad projektsynkronisering (koppla från projekt, synkronisera om projekt och dokument osv.)

### Inom Frame.io kan kreativa personer skicka skapade resurser till Workfront-projektet för formell granskning

* Möjlighet att ansluta en Frame.io-resurs till ett WF-projekt eller en WF-uppgift. En resursreferens kommer att skapas i Workfront

* Överföringar av nya versioner inuti Frame.io skapar automatiskt nya dokumentversioner i Workfront för anslutna resurser

* Möjlighet att markera de refererade Workfront-aktiviteterna som slutförda inifrån Frame.io

* Om det anslutna Workfront-dokumentet tas bort ligger det kvar i Frame.io och kan återanslutas till samma eller andra projektuppgifter

**Potentiella förbättringar i framtida versioner:**

* Skicka flera Frame.io-resurser till Workfront samtidigt

* Tidsloggning mot Workfront-projekt/uppgifter inifrån Frame.io

### Projektsamordnare kan tilldela den formella godkännandeprocessen till dokument som är länkade från Frame.io

* Workfront-användare och -team kan läggas till i nya dokumentgodkännanden för Frame.io-anslutna dokument

* När en användare/grupp inte delas från ett dokument som är aktiverat för bildrutor förlorar de även åtkomsten till resursen i Frame.io Viewer

**Potentiella förbättringar i framtida versioner:**

* Skicka flera resurser som en enda granskning

* Tilldela godkännare/granskare gruppvis till Workfront-dokument

### Intressenter kan granska och godkänna dem i Frame.io Viewer

* Intressenterna meddelas och kan visa dokumentet som är kopplat till ramen i Frame.io Viewer

* Frame.io Viewer kan nås från olika platser i Workfront, t.ex. Dokumentlista, Dokumentinformation, Workfront startsida

* Möjlighet att utnyttja de gransknings- och kommentarfunktioner som finns i Frame.io Viewer, som kommer att synkroniseras med Workfront Update Stream

* Möjlighet att fatta ett beslut om godkännande av ett nytt dokument inifrån Frame.io Viewer

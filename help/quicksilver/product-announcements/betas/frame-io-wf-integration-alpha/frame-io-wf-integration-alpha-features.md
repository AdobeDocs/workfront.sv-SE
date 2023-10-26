---
content-type: reference
navigation-topic: betas
title: "Adobe Workfront och Frame.io inbyggd integration alpha: features"
description: Planerade funktioner för Adobe Workfront och Frame.io, inbyggd integration alpha
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
source-git-commit: 0ad33f377086f71699c550e2300731056a834e72
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---


# Adobe Workfront och Frame.io, inbyggd integration alpha: features

## Användningsexempel och funktionstestning

Med den här integreringen är vårt mål att göra det möjligt för kreatörer att behålla sina valfria verktyg (CC eller Frame.io) för att skapa innehåll och utföra peer-granskningar, samtidigt som projektledare koordinerar arbetet och initierar och övervakar den formella granskningsprocessen inifrån Workfront. Detta kan uppnås genom att man använder det bästa av båda lösningarna: Workfront nya dokumentgodkännanden för att hantera innehållsgodkännanden, tillsammans med de innehållsgranskningsfunktioner som Frame.io erbjuder. De nya dokumentgodkännandena och Frame.io kommer tillsammans att utgöra vår nya heltäckande upplevelse för granskning och godkännande av innehåll. 

Mer information om hur alfavärdet fungerar och hur du kan delta finns i [Integreringsalfa för Adobe Workfront och Frame.io: översikt](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)


>[!NOTE]
>
>Om du kommer på dessa sidor utan att ditt företag deltar i det här alfaversionsprogrammet, var noga med att behandla informationen här och kontakta din Workfront- eller Frame.io-administratör för mer information.

<!--Initial setup and basic test scenario 

As part of the alpha program, we've provisioned a new test Frame.io account for you and connected it to a new group "Frame.io alpha testing" in your existing Workfront Preview or Sandbox environment. To test the delivered functionality please log in to your Workfront Preview or Sandbox instance and  perform the following steps: 

Coordinators: Within Workfront, create a project with the "Frame.io alpha testing" group assigned as project group 

Coordinators: Within Workfront, assign your creatives to the project or Frame enabled tasks and change the project status to "Current" 

Creatives: Check your emails for an invite to the newly created Frame.io project 

Creatives: Click on the "Join project" button within the invitation email to join the Frame.io project, review the creative brief within the project and start your content creation within your CC tool of choice 

Creatives: Upload your created assets to Frame.io and add them to the linked Workfront project (or assigned Frame enabled tasks)  

Coordinators: Within Workfront, see the linked Frame.io assets in your project and assign reviewers / approvers (new document approvals: More help on this feature) 

Stakeholders: Withing Workfront, view your approval request in Workfront Home or Document Details and review the Frame connected document in the Frame.io Viewer. Leave a comment feedback 

Coordinators: Within Workfront, view the stakeholder created comments within the Updates section of the Frame.io connected document in Workfront 

Stakeholders: Make a decision from within the Frame.io Viewer 

Creatives: Within Frame.io, notice the overall approval decision made for your assets 

Creatives: Within Frame.io, Apply the requested changes by adding the updated version to the version stack of the connected asset 

Coordinators: Within Workfront, assign approvers / reviewers to the new version upload and monitor the progress until it reaches sign-off-->

## Funktionsplaner

Nedan finns information om de primära användningsområdena som vi vill ta upp och de funktioner vi planerar att göra det. <!--, along with documentation to get you started testing.-->


### Workfront-administratörer kan skapa en anslutning mellan Workfront-grupper och Frame.io-konton

* _I Workfront kan du ansluta en Workfront-grupp till ett Frame.io-konto_

* Ett nytt Frame.io-team skapas i Frame.io som representerar den anslutna Workfront-gruppen

**Potentiella förbättringar i framtida versioner:**

* Koppla från en Workfront-grupp från ett Frame.io-konto

* Koppla en Workfront-grupp till ett befintligt Frame.io-team

### Projektsamordnare kan konfigurera vilka Workfront-projekt som skickas till Frame.io och lägga till de tilldelade kreativa i Workfront i projektet Frame.io

* Möjlighet att markera Workfront-projekt som Frame.io aktiverat genom att tilldela en bildruteansluten grupp

* _Förbättring: Möjlighet att växla aktiviteter i Workfront-projekt till Frame-åtgärder som i sin tur skapar uppgiftsmappar i Frame.io_

* När statusen för ett Workfront-projekt är Aktuell skapas ett motsvarande anslutet projekt i bildrutan, användare som tilldelats Workfront läggs till i bildruteprojektet och ett e-postmeddelande skickas till dem från Frame.io

   * Alla Workfront Project-medlemmar (användare och team) läggs till som medarbetare i Frame.io-projektet (när projekt skapas och senare)

   * _Ändra: Användare och team som är tilldelade till bildruteaktiverade Workfront-uppgifter läggs till som medarbetare i Frame.io-projektet och meddelas (när projekt skapas och senare)_

* Dokument (Creative Brief) som läggs till i projektet och aktiviteter som är aktiverade för bildruta flyttas till Frame.io-projektet (i respektive arbetsmapp) när projektet skapas (utlösare: projektstatus inställd på Aktuell)

   * Vi rekommenderar att du begränsar antalet dokument som läggs till i projektet innan du börjar arbeta med bara dina projektdokument, så att du slipper skicka flera onödiga dokument till Frame.io.

* _Förbättring: Användare/team som uttryckligen inte tilldelats från en bildruteaktiverad Workfront-uppgift tas bort från Frame.io-projektet_

**Potentiella förbättringar i framtida versioner:**

* Ramaktiverade uppgifter kan konfigureras för projektmallar

* Nya versionsuppladdningar till kreativa informationsdokument kommer att överföras till Frame

* Optimerad projektsynkronisering (koppla från projekt, synkronisera om projekt och dokument osv.)

### Inom Frame.io kan kreativa personer skicka skapade resurser till Workfront-projektet för formell granskning

* Möjlighet att ansluta en Frame.io-resurs till ett WF-projekt eller en WF-uppgift. En resursreferens kommer att skapas i Workfront

* Överföringar av nya versioner inuti Frame.io skapar automatiskt nya dokumentversioner i Workfront för anslutna resurser

* _Förbättring: Möjlighet att markera de refererade Workfront-åtgärderna som slutförda inifrån Frame.io_

* _Förbättring: Om det anslutna Workfront-dokumentet tas bort ligger det kvar i Frame.io och kan återanslutas till samma eller andra projektuppgifter_

**Potentiella förbättringar i framtida versioner:**

* Skicka flera Frame.io-resurser till Workfront samtidigt

* Tidsloggning mot Workfront-projekt/uppgifter inifrån Frame.io

### Projektsamordnare kan tilldela den formella godkännandeprocessen till dokument som är länkade från Frame.io

* Workfront-användare och -team kan läggas till i nya dokumentgodkännanden för Frame.io-anslutna dokument

* _Förbättring: När en användare/ett team inte delas från ett dokument som är aktiverat för bildrutor förlorar de även åtkomsten till resursen i Frame.io Viewer_

**Potentiella förbättringar i framtida versioner:**

* Skicka flera resurser som en enda granskning

* Tilldela godkännare/granskare gruppvis till Workfront-dokument

### Intressenter kan granska och godkänna dem i Frame.io Viewer

* Intressenterna meddelas och kan visa dokumentet som är kopplat till ramen i Frame.io Viewer

* Frame.io Viewer kan nås från olika platser i Workfront, t.ex. Dokumentlista, Dokumentinformation, Workfront startsida

* Möjlighet att utnyttja de gransknings- och kommentarfunktioner som finns i Frame.io Viewer, som kommer att synkroniseras med Workfront Update Stream

* _Möjlighet att fatta ett beslut om godkännande av ett nytt dokument inifrån Frame.io Viewer_

### Inom Frame.io kommer kreatörerna att informeras om det övergripande beslutet som fattats om den anslutna Frame.io-resursen

* _Förbättring: Den övergripande statusen för dokumentgodkännande visas för resurser i Frame.io_

### Projektsamordnare kan skicka det slutliga materialet till AEM

* _Förbättring: Ramanslutna dokument, inklusive metadata, kan skickas till AEM med den befintliga Workfront + AEM Asset CS-kopplingen_
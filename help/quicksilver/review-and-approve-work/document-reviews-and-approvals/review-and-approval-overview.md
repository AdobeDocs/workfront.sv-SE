---
product-area: documents
navigation-topic: approvals
title: Översikt över resursgranskning och godkännande
description: Läs mer om den formella granskningen och godkännandeprocessen i Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 63160895fc77994fdecd7aca8769b7d236d285d6
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---


# Översikt över resursgranskning och godkännande

Det nya arbetsflödet för granskning och godkännande av resurser bygger på en nära integrering mellan Workfront och Frame.io. Integrationen tar det bästa av det varje produkt har att erbjuda och kombinerar den för att skapa en upplevelse som gör att alla personer som arbetar med innehållsframtagning kan arbeta med sina valfria verktyg, samtidigt som de har tillgång till kommentarer, filer och statusuppdateringar synkroniserade i båda systemen i realtid.

<!-- link to frame docs-->

## Arbetsplanering i Workfront

Projektsamordnaren börjar i Workfront. Projektet skapas, uppgifter tilldelas och instruktioner skickas.

Projektkoordinatorn skapar ett WF-projekt, använder synkroniserad projektmapp för att skicka information och stödmaterial till kreatörer inuti Frame.io

Ställa in arbetsflöde för godkännande från grunden eller via mallar

Tilldela uppgifter

Anger projekt som Aktuell eller lika med för att skapa bildruteprojekt och varningsskapande

### Konfigurera ett standardkonto för Frame.io

Workfront-administratörer initierar integreringen av Workfront och Frame.io genom att lägga till ett standard-konto för Frame.io under Konfigurera i Workfront. När ett Frame.io-standardkonto har konfigurerats kan det användas för att skapa sammankopplade projekt mellan Workfront och Frame.io.

Mer information finns i [].


<!-- in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->


### Aktivera Frame.io-användare

Workfront-användare som regelbundet använder Frame.io bör markeras som Frame.io-användare. Workfront-administratörer kan ange Frame.io-användare i Workfront användarprofil.

När en användare har markerats som en Frame.io-användare i Workfront och läggs till i ett projekt:

* De läggs till som medarbetare i Frame.io
* De kan skicka material från Frame.io till Workfront för granskning och godkännande

Mer information finns i [].

![](assets/Frame-enabled-user.png)

>[!TIP]
>
>Vi rekommenderar att användare som regelbundet arbetar med kreativa verktyg kan aktivera och överföra material för granskning och godkännande som Frame.io-användare.

### Skapa ett projekt som är kopplat till Frame.io

Projektsamordnare kan skapa Workfront-projekt som är kopplade till Frame.io. När du skapar ett anslutet projekt kan du

* **Tilldela Frame.io-användare till uppgifter**: Frame.io-aktiverade användare meddelas via e-post när de tilldelas en uppgift som signalerar till dem att det finns arbete att slutföra.
* **Dela projektet med Frame.io-användare**: Projekt som delas med Frame.io-aktiverade användare ger åtkomst till projektet inuti Frame.io.
* **Dela kreativt material med Frame.io**: Du kan skicka instruktioner och material från Workfront direkt till den kreativa användaren i Frame.io med en envägsprojektmapp för synkronisering.
* **Spåra uppgiftsförloppet**: Kreatörer kan skicka färdigt material och markera uppgifter som slutförda utan att lämna Frame.io.

Mer information finns i [].

<!--Preassign approval templates to asks coming in the future-->


## Skapa och samarbeta kring material i Frame.io

Kreatörerna kan behålla sina valverktyg och ha friheten att skapa, upprepa och genomföra granskningar inifrån Frame.io.

När en kreatör läggs till i ett integrerat projekt kan de göra allt detta utan att lämna Frame.io:

* Åtkomstinstruktioner från projektkoordinatorn
* Utföra informella peer-granskningar
* Skicka det färdiga materialet till Workfront för granskning och godkännande
* Ändra status för en uppgift eller markera den som slutförd
<!-- * Notification of decision
* Upload new versions of connected assets marked as needs more work < will automatically connect>-->


## Granska och godkänn mediefiler i Workfront

När en kreatör skickar en färdig fil till Workfront från Frame.io kan projektsamordnaren starta den formella gransknings- och godkännandeprocessen i Workfront. Alla gransknings- och godkännandeaktiviteter registreras i Workfront.

Alla kommentarer som görs i Frame.io visas även på fliken Uppdateringar i Workfront. Svar som gjorts i Workfront återspeglas inte i Frame.io.

Kommentarer som bara är markerade för Team visas inte på fliken Workfront Updates.

### Starta formella granskningar och godkännanden

Du kan skapa en enstaka granskning och godkännanden, eller så kan du skapa återanvändbara mallar för godkännande under Konfigurera på arbetsytan:

Du kan välja att tilldela granskare, godkännare eller en blandning av båda:

* **Granskare** kan kommentera och markera resurser. När de är klara kan de markera granskningen som slutförd. <!--example of when to add reviewers-->
* **Godkännare** Kan kommentera, kommentera resurser och måste fatta ett beslut om att flytta godkännandeprocessen framåt.

Granskare och godkännare kan läggas till i mallar för enstaka användning eller godkännande:

<!--can also assign teams and set deadline-->

* **Godkännanden för enstaka användning**: Ange godkännandedeadlines

* **Godkännandemallar**
I området Workfront Setup kan användare med en standardlicens skapa återanvändbara godkännandemallar. I en mall kan användarna ange en tidsram och lägga till granskare och godkännare. <!--do we want to mention any upcoming plans here? -->

  När en mall har skapats kan den tillämpas på resurser som skickas från Frame.io för att starta den formella gransknings- och godkännandeprocessen i Workfront.
  ![](assets/assign-template.png)

<!-- can set timreframe which calculates deadline once approval is started. >

    For more information, see [Create and manage Approval Templates](/)<!--don't forget link-->

### Gransknings- och godkännandemeddelanden

Kombinera med andra avsnitt?

Hem i väntan på min widget E-post för godkännande - e-post om deadline 72, 24 och inom deadline.

<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->

### Granska och godkänna resurser

Frame.io-anslutna resurser som intressenter kan granska och godkänna inuti bildrutevisningsprogrammet med kommentarer synkroniserade till uppdateringsströmmen, beslut osv.

<!-- include screenshot from frame.io-->

Externa WF-användare uppmanas att skapa en inloggning för bildruta

Om resursen inte är ansluten till en bildruta kan de visa miniatyrbilder i WF och använda kommentarströmmen. beslut om granskning och godkännande kan fattas.

### Spåra gransknings- och godkännandestatistik

Snabbrapport för godkännande av widget i hemmet

<!--
### Published approved assets to Adobe Experience Manager Assets

Use the native integration to send approved assets to AEM.
-->


* Ladda upp en mediefil från Workfront och skicka den till en bildruta för granskning och godkännande - Kommer snart?

## Exempel på arbetsflöde för godkännande av kampanjresurser

Inro para?

![](assets/example-workflow.png) <!-- probbly need a different version of this but add something similar rather than typing all out?-->
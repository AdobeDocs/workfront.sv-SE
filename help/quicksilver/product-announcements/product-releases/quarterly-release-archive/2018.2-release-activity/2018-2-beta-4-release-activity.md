---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 Beta 4 - versionsaktivitet
description: Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i 2018.2 Beta 4. Funktionerna kommer att vara tillgängliga i förhandsvisningsmiljön den 17 maj 2018. Den kommer att göras tillgänglig i produktionsmiljön i juli 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4b54b9e6-d1bf-4802-9d6c-9c3d3b6a6583
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '1705'
ht-degree: 0%

---

# 2018.2 Beta 4 - versionsaktivitet

Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i 2018.2 Beta 4. Funktionerna kommer att vara tillgängliga i förhandsvisningsmiljön den 17 maj 2018. Den kommer att göras tillgänglig i produktionsmiljön i juli 2018.

>[!IMPORTANT]
>
> Funktionerna som beskrivs på den här sidan kan ändras innan de är tillgängliga i produktionsmiljön.

En lista över alla ändringar som gjorts under 2018.2 finns på  [Aktivitetsöversikt för version 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

2018.2 Beta 4 innehåller förbättringar för Workfront-administratörer och andra användare:

**För administratörer**

* [Systeminställning: Sessionsinformation på externa sidor](#system-setting-session-information-in-external-pages)

**För alla användare**

* [Förbättringar av begränsning av pågående arbete (WIP) för kanban-styrelsen](#work-in-progress-wip-limit-enhancements-on-the-kanban-board)
* [Förbättrat gränssnitt för konfigurering av status för ett team](#improved-interface-for-configuring-statuses-for-an-agile-team)
* [Uppdaterad arbetslista (vänster panel) i hemområdet](#updated-work-list-left-panel-in-the-home-area)
* [Ny Desktop Proofing Viewer för korrektur av interaktivt (multimedia) innehåll](#new-desktop-proofing-viewer-for-proofing-interactive-rich-media-content) 
* [Exportera användarvyn i resursplaneraren](#export-the-user-view-in-the-resource-planner)
* [Stöd för Google Team Drives](#support-for-google-team-drives)
* [Ny exportgräns för Gantt-schemat](#new-export-limit-for-the-gantt-chart)
* [Alternativet Klistra in från Urklipp visas nu som nedtonat när du använder Internet Explorer eller Safari](#paste-from-clipboard-option-now-displays-as-dimmed-when-using-internet-explorer-or-safari)
* [Ny Beta-miljö för Android tillsammans med nya funktioner](#new-beta-environment-for-android-along-with-new-features)
* [Exempel på filter för händelseprenumerationsmeddelanden](#examples-of-filters-for-event-subscriptions-messages)

## Förbättringar av gränsen för pågående arbete för kanban-styrelsen {#work-in-progress-wip-limit-enhancements-on-the-kanban-board}

### Konfigurera PIA-begränsningar (Work in Progress) för varje kolumn i kanban-styrelsen

Nu kan du konfigurera gränserna för pågående arbete (PIA) för varje kolumn på Kanban-tavlan. 

Före den här ändringen kunde du bara konfigurera en PIA-gräns som tillämpades på alla kolumner på Kanban-tavlan. 

Mer information finns i avsnittet  [Konfigurera gränsen för pågående arbete (PIA)](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4) i artikeln  [Konfigurera Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

### Uppdatera PIA-gränsen (Work in Progress) direkt från kanban-styrelsen

Nu kan teammedlemmar med redigeringsbehörighet för teamet uppdatera PIA-gränsen direkt från Kanban-styrelsen.

Innan den här ändringen utfördes kunde du bara uppdatera PIA-gränsen från området Teaminställningar.

Mer information finns i  i artikeln.

## Förbättrat gränssnitt för konfigurering av status för ett Agile-team {#improved-interface-for-configuring-statuses-for-an-agile-team}

Gränssnittet för konfigurering av status för ett Agile-team har uppdaterats med följande förbättringar:

* Nytt utseende
* Ändra ordning på statuskolumner via dra och släpp 

Mer information finns i följande artiklar:

* [Konfigurera Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
* [Konfigurera Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## Uppdaterad arbetslista (vänster panel) i hemområdet {#updated-work-list-left-panel-in-the-home-area}

Arbetslista i Hem-området innehåller följande förbättringar:

* Olästa objekt sticker nu ut med fet och blå punkt.

  Objekt som visas utanför hemområdet visas fortfarande som olästa i hemområdet.

  Mer information finns i [Visa objekt i arbetslistan i hemområdet](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Nu kan du skilja på olika problem med en problemikon som visas bredvid problemet.
* Godkännanden urskiljs nu efter typ av godkännande, med typen av godkännande som visas. Möjliga godkännandetyper är Aktivitet, Projekt, Utgåva, Åtkomst, Dokument, Tidrapport och Korrektur.

  Före den här ändringen särskiljdes godkännanden endast med ordet&quot;Godkännande&quot;.

* Objekten urskiljs nu av om de är klara att starta eller inte. Möjliga alternativ är Klar att starta, Inte klar eller Arbeta på.

  Den här informationen visas inte för godkännanden eftersom godkännanden alltid är klara att starta.

* En dokumentikon visas under objektets namn när ett dokument bifogas till objektet.
* Du kan nu komprimera och expandera grupperingar i arbetslistan för att bättre kontrollera vilken information som visas. Grupperingarna är Sena, Projekt, Datum och Slutfört.

  Avsnittet Den här veckan är som standard utökat och alla andra grupperingar komprimeras.

* Välj om du vill sortera objekt efter planerat slutförandedatum eller Genomför-datum.
* Antalet objekt i varje gruppering visas nu inom parentes bredvid grupperingsrubriken.

  Det här numret är inte tillgängligt för grupperingen Slutfört.

  Mer information finns i [Visa objekt i arbetslistan i hemområdet](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Ändra storlek på arbetslistan genom att dra och släppa. Du kan ändra storlek på arbetslistan så att den förbrukar upp till hälften av skärmen. Storleken som du anger behålls nästa gång du öppnar Home.

  Det gick inte att ändra storleken på arbetslistan före den här ändringen.

* På begäran visas användaravataren för användaren som gjorde begäran med texten [Godkännare_namn].
* När du skapar en ny personlig uppgift får du nu etiketten&quot;Att göra&quot;.

  Mer information finns i [Skapa arbetsobjekt från Hem](../../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md) i artikeln [Skapa arbetsobjekt från Hem](../../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

* Sena objekt anges som sena endast efter en timme efter det planerade slutförandedatumet.

Mer information om Hem-området finns i [Använda Hem-området](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Ny Desktop Proofing Viewer för korrektur av interaktivt material (multimedia) {#new-desktop-proofing-viewer-for-proofing-interactive-rich-media-content}

Med den nya Desktop Proofing Viewer kan du korrekturgranska interaktivt material. Till skillnad från det befintliga korrekturläsaren för äldre versioner och det nya korrekturläsaren som körs i webbläsaren är korrekturläsaren för skrivbordet ett program som körs på din arbetsstation.

Före den nya Desktop Proofing Viewer kunde du bara göra korrektur av interaktivt innehåll i det äldre korrekturläsaren. 

Desktop Proofing Viewer innehåller följande förbättringar jämfört med det äldre korrekturläsaren för korrektur av interaktivt innehåll:

* Granska oskyddade HTTP-platser

  Med det äldre språkvisningsprogrammet kan du endast granska säkra webbplatser (HTTPS)

* Granska iframe-skyddade webbplatser (webbplatser som skyddas från att visas i en iframe).

  Det äldre korrekturläsaren stöder inte granskning för webbplatser som skyddas från att visas i en iframe.

* Visa innehåll med förkonfigurerade upplösningar för olika enheter. Du kan till exempel se hur innehåll visas på olika vanliga skrivbordsupplösningar eller på enskilda enheter som iPhone 8. 

Mer information om hur du hämtar, installerar och använder Desktop Proofing Viewer finns i .

Mer information om skillnader i funktionalitet mellan Desktop Proofing Viewer och webbläsarbaserade korrekturläsare finns i [Skillnader mellan Web Proofing Viewer och Desktop Proofing Viewer - översikt](../../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

## Exportera användarvyn i resursplaneraren {#export-the-user-view-in-the-resource-planner}

Vi hade tillfälligt inaktiverat export av data från resursplaneraren när de visades i användarvyn för att åtgärda vissa prestandaproblem. I den här versionen återaktiveras exporten av data när resursplaneraren visas i användarvyn.

Mer information om hur du exporterar resursplaneringsdata till Excel finns i avsnittet Exportalternativ i [Navigeringsöversikt för resursplanering](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Om du vill delta i vårt aktuella betaprogram för resursplaneraren läser du [Resursplaneringsprestanda för Beta.](https://experienceleaguecommunities.adobe.com/t5/workfront/ct-p/workfront?profile.language=sv)

## Systeminställning: Sessionsinformation på externa sidor {#system-setting-session-information-in-external-pages}

Workfront-administratören kan nu begränsa användningen av sessionsinformation (till exempel sessions-ID) när en extern sida skapas.

Före den här ändringen kunde användare som skapade externa sidor använda vilken sessionsinformation som helst när de bäddade in andra webbplatser i en Workfront-kontrollpanel. 

Mer information om hur du konfigurerar systeminställningarna i Workfront finns i [Konfigurera systemsäkerhetsinställningar](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Stöd för Google Team Drives {#support-for-google-team-drives}

Nu kan du länka ett dokument eller en mapp på en Google Team Drive från Workfront.

Före den här förbättringen kan du länka ett dokument eller en mapp som bara finns på Google My Drive.

Mer information om hur du länkar dokument och mappar från olika program till Workfront finns i [Länka dokument från externa program](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Ny exportgräns för Gantt-schema {#new-export-limit-for-the-gantt-chart}

Du kan nu exportera upp till 500 uppgifter i Gantt-diagrammet.

Tidigare kunde du bara exportera upp till 250 uppgifter.

Mer information finns i [Exportera Gantt-schemat till PDF](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

## Alternativet Klistra in från Urklipp visas nu som nedtonat när du använder Internet Explorer eller Safari {#paste-from-clipboard-option-now-displays-as-dimmed-when-using-internet-explorer-or-safari}

Alternativet Klistra in från Urklipp visas nu som nedtonat när du använder webbläsarna Internet Explorer eller Safari, med ett verktygstips som förklarar att endast webbläsarna Chrome och Firefox stöds för den här funktionen.

Före den här ändringen visades inte det här alternativet när Internet Explorer eller Safari användes. 

Mer information om hur du klistrar in bilder från Urklipp finns i [Klistra in bilder från Urklipp](../../../../documents/managing-documents/paste-image-clipboard.md).

## Nya Beta Environment for Android plus nya funktioner {#new-beta-environment-for-android-along-with-new-features}

Nu kan du uppleva de senaste funktionerna som vårt team arbetar med för mobilappen innan de släpps för allmänheten genom att registrera sig som betatestare. Den här miljön stöds för närvarande endast för Android-telefoner.

Mer information om hur du registrerar dig som betatestare för Workfront mobilapp finns i .

Följande förbättringar är nu tillgängliga i betaversionen av mobilappen:

* Ny kontosida

  Nu kan du visa din kontoinformation, hantera dina mobilinställningar, skicka feedback eller logga ut från den nya kontosidan.

  Innan den här förbättringen kunde du inte visa din kontoinformation för mobilappen och du kan komma åt dina inställningar, skicka feedback och logga ut från Workfront huvudmeny.

* Ny navigeringspanel i nederkant

  Nu finns ett mer framträdande navigeringsfält längst ned på skärmen som visar alla delar av mobilappen.

  Innan den här förbättringen listades funktionsområdena på Workfront huvudmeny. Workfront huvudmeny har tagits bort och ersatts av det nya nedre navigeringsfältet.

  Mer information om hur du konfigurerar det nya navigeringsfältet finns i avsnittet&quot;Konfigurera din mobilapp&quot; i .

* Ny meddelandelistvy

  Tack vare det förbättrade utseendet på meddelandelistan kan du enkelt differentiera meddelandena i listan beroende på vilken typ av meddelanden de är och om de har lästs.

* Sökrutan har flyttats till en mer framträdande plats.

* Ny inloggningsfunktionDet finns en ny, effektivare inloggningsfunktion.

* Ny självstudiekurs

  Nya självstudiekurser finns nu tillgängliga för att kort vägleda användarna genom appen när de loggar in första gången. Före den här erfarenheten startades självstudiekurserna endast när användarna fick åtkomst till specifika funktionsområden.

## Exempel på filter för händelseprenumerationsmeddelanden {#examples-of-filters-for-event-subscriptions-messages}

För att visa hur du kan filtrera händelseprenumerationer så att de bara tar emot meddelanden som är relevanta för din organisation finns nu exempelkodfragment tillgängliga för filtrering av händelseflödet som kommer till slutpunkterna. Mer information om hur du visar filterexemplen finns i [Prenumerationsmeddelanden för filterhändelser](../../../../wf-api/api/filter-event-sub-messages.md).

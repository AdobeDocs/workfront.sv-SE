---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.3 Beta Final release activity
description: Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i den slutliga betaversionen 2017.3. Funktionerna på den här sidan gjordes tillgängliga i förhandsvisningsmiljön den 12 september 2017. Den kommer att göras tillgänglig i produktionsmiljön i början av november 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 880828f4-3908-4ef0-ab1f-774f8dee72b6
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '3821'
ht-degree: 0%

---

# 2017.3 Beta Final release activity

Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i den slutliga betaversionen 2017.3. Funktionerna på den här sidan gjordes tillgängliga i förhandsvisningsmiljön den 12 september 2017. Den kommer att göras tillgänglig i produktionsmiljön i början av november 2017.

>[!IMPORTANT]
>
> Funktionerna som beskrivs på den här sidan kan ändras innan de är tillgängliga i produktionsmiljön.

En lista över alla ändringar som gjorts under 2017.3 finns på  [Aktivitetsöversikt för 2017.3-utgåvan](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

Den slutliga betaversionen 2017.3 innehåller förbättringar för både Workfront-administratörer och andra användare:

**För administratörer**

* [Ny konfiguration för återanrop av begäranden i området Godkännandeinställningar](#new-configuration-for-recalling-requests-in-the-approval-settings-area)
* [Konfigurera standardprofilroller](#configure-default-proof-roles)

**För alla användare**

* [Hem (uppdaterade min arbetsyta)](#home-area-updated-my-work-area)

* [Uppdaterad layoutmall som har stöd för hemområdet](#updated-layout-template-to-support-the-home-area)

* [Kanban för Agile](#kanban-for-agile)
* [Inkludera problem i Scrum-eftersläpningen för ett Agile Team](#include-issues-on-the-scrum-backlog-for-an-agile-team)
* [Inkludera frågor i Scrum Agile Story Board](#include-issues-on-the-scrum-agile-story-board)
* [Använda grupperingar och filter i eftersläpningen för ett Agile-team](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team)
* [Förbättrade @Tagging-funktioner returnerar i förhandsvisningsmiljön](#enhanced-tagging-functionality-returns-in-the-preview-environment)
* [Filtersystemsuppdateringar i uppdateringsströmmen är nu beständiga över objekt](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [Visa data i användningsrapporten](#visualize-data-in-the-utilization-report)
* [Prestandaförbättring för användningsrapporten](#utilization-report-performance-improvement)
* [Förbättrade dokument: Smidigt gränssnitt](#document-enhancements-streamlined-interface)
* [Förbättringar av korrektur i Workfront](#proofing-enhancements-within-workfront)
* [Förbättringar av korrektur i både Workfront och Workfront](#proofing-enhancements-within-both-workfront-proof-and-workfront)
* [RTF-formatering för uppdateringar och e-postmeddelanden](#rich-text-formatting-for-updates-and-emails)
* [Ny Gantt-schemaomdesign](#new-gantt-chart-redesign)
* [Inbyggda rapporter innehåller uppdaterade beskrivningar](#built-in-reports-contain-updated-descriptions)
* [Varumärkning i exporterade rapporter, listor och kontrollpaneler](#branding-in-exported-reports-lists-and-dashboards)
* [Förbättringar när du kopierar uppgifter och flyttar uppgifter eller problem](#improvements-when-copying-tasks-and-moving-tasks-or-issues)
* [Ny gruppering för resursbudgeterade timrapporter: allokeringsdatum](#new-grouping-for-resource-budgeted-hour-reports-allocation-date)
* [Förbättringar av resursplanering](#resource-planner-improvements)
* [Mobilförbättringar](#mobile-improvements)
* [Workfront-integrering med Slack](#workfront-integration-with-slack)
* [Förbättringar i Outlook 365](#outlook-365-improvements)
* [API-ändringar](#api-changes)

## Hem (uppdaterade min arbetsyta) {#home-area-updated-my-work-area}

>[!NOTE]
>
>Den här funktionen kommer inte att släppas till produktionsmiljön i version 17.3. Den kommer att finnas kvar i förhandsversionen fram till början av 2018.

Den nya Hem-området ger en alternativ, förbättrad vy till samma data som för närvarande är tillgängliga i Min arbetsyta. Hem-området ger följande fördelar jämfört med Min arbetsyta:

* Ett smidigare och mer intuitivt gränssnitt
* Förbättrade prestanda

Följande funktionalitet är tillgänglig på arbetsytan Mitt arbete men har ännu inte implementerats i hemområdet:

* Visa din personliga kalender
* Uppdatera uppgifter och problem med formaterad text
* Godkänn korrektur
* Visa en lista över arbeten som du har skickat in för godkännande
* Skapa ett ad hoc-problem i ett projekt
* Visa endast de godkännanden som har delegerats till dig

Mer information om hur du använder den nya hemområdet finns i [Använda området Hem](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Uppdaterad layoutmall som har stöd för hemområdet {#updated-layout-template-to-support-the-home-area}

>[!NOTE]
>
>Den här funktionen kommer inte att släppas till produktionsmiljön i version 17.3. Den kommer att finnas kvar i förhandsversionen fram till början av 2018.

Som Workfront-administratör kan du avgöra om användare i din organisation har tillgång till Hem-området genom att konfigurera den layoutmall de är tilldelade. Användare som inte har tilldelats någon layoutmall har alltid tillgång till Hem-området.

Mer information finns i&quot;Anpassa startsidan&quot; i&quot;Skapa och hantera layoutmallar&quot;.

## Kanban för Agile  {#kanban-for-agile}

Agile Teams kan nu använda en Kanban-metod inom Workfront, utöver den Scrum-flexibla metod som redan stöds.

Metoderna Scrum och Kanban agile i Workfront skiljer sig på följande sätt:

**Fördelar med att använda Kanban i Workfront**

* Visa eftersläpningen på Kanban agile story board.

  Mer information finns i .

* Konfigurera objekt på eftersläpningen så att de automatiskt läggs till i den flexibla artikelpanelen i Kanban när andra objekt flyttas till en status som motsvarar fullständig.

  Mer information finns i [Konfigurera artiklar som automatiskt ska läggas till från eftersläpningen](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) in [Konfigurera Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Konfigurera en PIA-gräns (Work In Progress) som ska visas på den flexibla artikeltavlan för Kanban.

  Mer information finns i [Konfigurera PIA-gränsen (Work in Progress)](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4) in [Konfigurera Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

**Fördelar med att använda Scrum i Workfront**

* Lägg till en uppsättning artiklar i en smidig iteration och skapa en artikelpanel för den iteration som används.
* Inkludera problem på Scrum story board.
* Ta med problem i eftersläpningen för ett smidigt team.

  Mer information finns i [Konfigurera hur datum tillämpas när arbetsobjekt läggs till i en iteration](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) in [Konfigurera Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

* Underuppgifter kan visas på Scrum story board.
* Visa ett nedladdningsbart diagram om du vill se förloppet mot artiklar under upprepningen.

  Mer information finns i [Översikt över Agile-nedladdningsdiagram](../../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

Mer information om att aktivera och konfigurera Kanban för ett team finns i [Bestäm en flexibel metod](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md#deciding) in [Skapa ett smidigt team](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

## Inkludera problem i Scrum-eftersläpningen för ett Agile Team {#include-issues-on-the-scrum-backlog-for-an-agile-team}

>[!NOTE]
>
>Den här funktionen togs bort från produktionsmiljön den 14 november 2017. Den kommer att återinföras i förhandsvisningsmiljön i början av 2018 med förbättrad design och ökad stabilitet. Den kommer att vara tillgänglig i produktionsmiljön med version 2018.1.

Nu kan du inkludera problem i eftersläpningen för ditt mobila team när du använder Scrum-metoden (problemen visas inte i eftersläpningen för ett rörligt team när du använder Kanban-metoden). Befintliga Scrum-team måste aktivera den här funktionen för att problemen ska kunna tas med. Problem tas automatiskt med i eftersläpningen för Scrum-team som skapas efter version 2017.3.

Före den här ändringen kunde bara uppgifter läggas till i efterloggen. Om du ville lägga till ett problem var du först tvungen att konvertera problemet till en uppgift innan det kunde läggas till.

Eftersom du nu har tillgång till mer än bara uppgifter i efterloggen kopieras alla anpassade uppgiftsvyer som tidigare fanns i efterloggen och läggs till i eftersläpningen som anpassade arbetsobjektvyer i eftersläpningen.

Mer information om hur du använder problem i eftersläpningen finns i  [Hantera den flexibla eftersläpningen](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

Information om hur du aktiverar problem som ska vara tillgängliga i eftersläpningen för ett team med flexibla systemkontroller finns i  [Konfigurera hur datum tillämpas när arbetsobjekt läggs till i en iteration](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) in [Konfigurera Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Inkludera frågor i Scrum Agile Story Board {#include-issues-on-the-scrum-agile-story-board}

>[!NOTE]
>
>Den här funktionen togs bort från produktionsmiljön den 14 november 2017. Den kommer att återinföras i förhandsvisningsmiljön i början av 2018 med förbättrad design och ökad stabilitet. Den kommer att vara tillgänglig i produktionsmiljön med version 2018.1.

Nu kan du inkludera problem på artikelpanelen när du använder den flexibla Scrum-metoden.

Mer information finns i [Konfigurera statuskolumner på den flexibla artikelpanelen](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur2) in [Konfigurera Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Använda grupperingar och filter i eftersläpningen för ett Agile-team {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

>[!NOTE]
>
>Den här funktionen togs bort från produktionsmiljön den 14 november 2017. Den kommer att återinföras i förhandsvisningsmiljön i början av 2018 med förbättrad design och ökad stabilitet. Den kommer att vara tillgänglig i produktionsmiljön med version 2018.1.

Grupperings- och filteralternativen är nu tillgängliga i den flexibla eftersläpningen, så att du kan ordna din eftersläpning efter grupperingar samt filtrera efter specifika uppgifter och problem.

Före den här ändringen kan du tillämpa på vyer på den flexibla eftersläpningen.

Mer information finns i  [Hantera den flexibla eftersläpningen](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) in  [Hantera den flexibla eftersläpningen](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## RTF-formatering för uppdateringar och e-postmeddelanden {#rich-text-formatting-for-updates-and-emails}

>[!NOTE]
>
>De formateringsändringar du gör i förhandsvisningsmiljön kan återställas till oformaterad version.

Nu kan du betona viktig information genom att formatera dina kommentarer och uppdateringar i Workfront-objekt. 

Med RTF-verktygen kan du formatera text, skapa punktlistor och numrerade listor samt lägga till hyperlänkar i ytterligare resurser.

Formatering som tillämpas på kommentarer i uppdateringsströmmen visas också i e-postmeddelanden om uppdatering. Mer information om hur du formaterar dina kommentarer finns i [Uppdatera arbete](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Förbättrade @Tagging-funktioner returnerar i förhandsvisningsmiljön {#enhanced-tagging-functionality-returns-in-the-preview-environment}

Du kan återigen använda symbolen @ för att tagga andra användare i uppdateringsflödet för alla objekt i förhandsvisningsmiljön. Tidigare placerade @tagging den taggade användarens för- och efternamn i uppdateringsströmmen. Nu visas bara användarens förnamn i den förbättrade @tagging-funktionen. Mer information om hur du taggar användare i uppdateringar finns i [Tagga andra för uppdateringar](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Filtersystemsuppdateringar i uppdateringsströmmen är nu beständiga över objekt {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

Alternativet Filtersystemuppdateringar är nu beständigt över objekt på hela Workfront-webbplatsen. På så sätt kan du dölja systemuppdateringar och endast visa användarkommentarer i uppdateringsströmmen för ett objekt, och du behåller den inställningen när du bläddrar till andra objekt.

Innan den här ändringen genomfördes var du tvungen att välja att filtrera bort systemuppdateringar för varje objekt när du surrade på Workfront webbplats.

Mer information finns i [Uppdatera arbete](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Visa data i användningsrapporten {#visualize-data-in-the-utilization-report}

 Nu kan du visa användningsinformation i en diagramvy. 

Mer information finns i [Översikt över resursanvändningsrapporten](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [Översikt över resursanvändningsrapporten](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Prestandaförbättring för användningsrapporten {#utilization-report-performance-improvement}

>[!NOTE]
>
>Den här funktionen släpptes i en patch efter betaversionen.

När du nu kör en användningsrapport uppmanas du att använda ett filter innan rapporten körs. Ändringen säkerställer att den mest relevanta informationen genereras i användningsrapporten så snabbt som möjligt.

Mer information om hur du kör en användningsrapport finns i [Översikt över resursanvändningsrapporten](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [Översikt över resursanvändningsrapporten](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Förbättrade dokument: Smidigt gränssnitt {#document-enhancements-streamlined-interface}

Användarupplevelsen när du lägger till dokument i Workfront är nu mer smidig och intuitiv. Nu kan du överföra ett dokument från filsystemet, begära ett dokument eller länka en fil från ett tredjepartsprogram (som Google eller Dropbox), allt från en enkel meny. 

Tidigare var dessa alternativ tillgängliga genom att öppna dialogrutan Lägg till dokument. 

Mer information finns i följande information:

* [Lägga till dokument i Adobe Workfront från filsystemet](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)
* [Begär ett dokument](../../../../documents/adding-documents-to-workfront/request-a-document.md)
* [Länka dokument från externa program](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md) 

>[!NOTE]
>
>Med den här ändringen är alternativet att klistra in en bild eller ett dokument från Urklipp inte längre tillgängligt.

## Förbättringar av korrektur i Workfront {#proofing-enhancements-within-workfront}

* [Förbättrad användarupplevelse och ytterligare funktioner](#improved-user-experience-and-additional-functionality)
* [Dela direkt från korrekturläsaren](#share-directly-from-the-proofing-viewer)
* [Konfigurera standardprofilroller](#configure-default-proof-roles)

### Förbättrad användarupplevelse och ytterligare funktioner {#improved-user-experience-and-additional-functionality}

Förutom en förbättrad användarupplevelse när du skapar korrektur i Workfront finns nu följande extrafunktioner:

* Sammanfoga flera bilder till ett enda korrektur.
* Korrektur för webbplatser i flera upplösningar (flera upplösningar kan skapas som enskilda korrektur eller kombineras till ett enda korrektur).
* Redigera filnamnet under överföringsprocessen.
* Inkludera anpassade fält i formuläret för att skapa korrektur.
* Lägg till ett anpassat meddelande till korrekturmeddelanden via e-post.
* Ytterligare korrekturinställningar 
* Validering av fel i realtid vid korrektur av en URL (tidigare behövde du vänta flera minuter innan ett fel visades)

Mer information finns i .

>[!NOTE]
>
> När du skapar ett nytt korrektur med ett automatiserat arbetsflöde stöds inte dra och släpp för användare som flyttar från en fas till en annan. Ta i stället bort användaren från ett steg och lägg till användaren i ett annat.

*Alternativet att flytta användare från ett steg till ett annat genom att dra och släppa återinförs i version 2018.1.*

### Dela direkt från korrekturläsaren {#share-directly-from-the-proofing-viewer}

Nu kan du dela materialet med specifika Workfront-användare direkt från korrekturläsaren.

>[!NOTE]
>
>Den här funktionen är endast tillgänglig för nya korrektur (korrektur som skapas efter version 2017.3) och endast för Workfront-instanser som är integrerade med ett Workfront Proof Premium-konto.

Före den här ändringen kan du bara dela genom att skapa en länk och sedan dela länken med en användare. 

Mer information finns i [Dela ett korrektur i Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Dela ett korrektur i Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

### Konfigurera standardprofilroller {#configure-default-proof-roles}

Nu kan du konfigurera de standardkorrekturroller som nya användare och gästanvändare har för att skapa nya korrektur i Workfront-systemet. 

Detta är standardrollen som användare tilldelas till ett korrektur när korrekturet delas med dem. 

## Förbättringar av korrektur i både Workfront och Workfront {#proofing-enhancements-within-both-workfront-proof-and-workfront}

* [Starta om och hoppa över videokorrektur i HTML5 (kortkommandon)](#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts)
* [Uppdateringar för korrekturläsaren för HTML 5](#html5-proofing-viewer-updates)

### Starta om och hoppa över videokorrektur i HTML5 (kortkommandon) {#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts}

Det finns nu kortkommandon i korrekturläsaren för HTML 5 som gör att du kan starta om videon från början och hoppa till slutet av videon.

Mer information om tillgängliga kortkommandon finns i [Kortkommandon i Workfront korrekturläsare](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/keyboard-shortcuts.md).

### Uppdateringar för korrekturläsaren för HTML 5 {#html5-proofing-viewer-updates}

HTML5-visningsprogrammet har nu stöd för statiska korrektur.

Före den här ändringen hade visningsprogrammet för HTML5 bara stöd för videoklipp. 

Visningsprogrammet för HTML innehåller följande nya funktioner för korrektur av statiskt innehåll:

* Gör en enda kommentar med markeringar på flera sidor i en enda vy

  Detta var tidigare endast möjligt i Kontinuerlig vy eller Tidskriftsvy

* Navigera i korrektur via miniatyrbilder

   * Identifiera enkelt den del av beviset som granskas. Detta är viktigt, särskilt när användare arbetar med korrektur i större format och långa webbsidor, eller när som helst behöver du en större zoomnivå för att kunna se detaljerna.
   * Ändra zoomnivån
   * Panorera innehållet

* Ange egna värden i mätningsverktyget
* När du kommenterar text i ett korrektur i korrekturläsaren i Workfront Proof kan du inkludera alternativ som anger att texten ska vara i fet stil, kursiv och understruken.

HTML5-visningsprogrammet stöder ännu inte alla funktioner som finns i det befintliga visningsprogrammet för Flashar. Följande funktioner är inte tillgängliga för närvarande, men kommer att ingå i en framtida version:

* Stöd för multimediefiler
* Jämförelseläge (video och statisk)
* Filtrera kommentarer (video och statisk)
* Granska hyperlänkar i dokument (statiska)
* Översättningar (video och statisk)
* Indikator som visar användare som arbetar med korrekturet
* Dela korrektur

Mer information om hur du korrekturläser statiska korrektur i HTML5-visningsprogrammet finns i .

Som Workfront-administratör i Workfront Proof kan du avgöra om användare i din organisation har tillgång till den nya korrekturläsaren för HTML 5 för videokorrektur.

## Ny Gantt-schemaomdesign {#new-gantt-chart-redesign}

Det nya Gantt-schemat innehåller följande förbättringar:

* Nya ikoner och markörer
* Nytt alternativ för att zooma in och ut i en viss tidsram
* Mindre aktivitetsceller i listdelen av diagrammet
* Omarbetade alternativ för inställningar, utskrift och växling till planerade datum.

Mer information om hur du konfigurerar alternativ i Gantt-schemat finns i [Konfigurera hur information visas i Gantt-schemat](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). 

## Inbyggda rapporter innehåller uppdaterade beskrivningar {#built-in-reports-contain-updated-descriptions}

Vi har uppdaterat beskrivningarna för våra systemrapporter i Workfront för att inkludera information om rapporttypen och de fält som ingår.  

Före denna förändring hade de flesta av våra inbyggda rapporter inga beskrivningar eller en mycket begränsad.

Mer information om inbyggda rapporter finns i [Använd inbyggda rapporter från Adobe Workfront](../../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

## Varumärkning i exporterade rapporter, listor och kontrollpaneler {#branding-in-exported-reports-lists-and-dashboards}

>[!NOTE]
>
>Den här funktionen är för närvarande inte tillgänglig för alla kluster i förhandsvisningsmiljön.

Om du använder varumärket i Workfront ingår nu logotypen som du använder i Global Navigation Bar i PDF-filerna som du exporterar från Workfront.

Följande PDF-filer innehåller organisationens logotyp på det exporterade dokumentet:

* Exporterade listor
* Exporterade och levererade rapporter
* Utskrivna instrumentpaneler

Mer information om att exportera data från Workfront finns i [Exportera data](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Förbättringar när du kopierar uppgifter och flyttar uppgifter eller problem {#improvements-when-copying-tasks-and-moving-tasks-or-issues}

Vi har förbättrat sättet att kopiera en uppgift eller flytta en uppgift eller ett problem på, så att det blir enklare att välja en överordnad för den kopierade eller flyttade uppgiften eller utgåvan. När du väljer en överordnad när du kopierar en uppgift kan du nu se en hierarki av uppgifter med deras överordnade - underordnade relation samt söka efter en överordnad i projekt med många uppgifter.

Det fanns inget sökfält i **Välj en överordnad** och aktivitetshierarkin var inte synlig i uppgiftslistan.

Mer information om att kopiera uppgifter finns i [Kopiera och duplicera uppgifter](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Mer information om hur du flyttar problem finns i [Flytta problem](../../../../manage-work/issues/manage-issues/move-issues.md).

## Ny konfiguration för återanrop av begäranden i området Godkännandeinställningar {#new-configuration-for-recalling-requests-in-the-approval-settings-area}

Vi har introducerat en ny inställning i området Godkännandeinställningar på systemnivå för att tillåta Workfront-administratörer att bestämma om de ska tillåta användare att återkalla ett problem eller en begäran vars första status väntar på godkännande. Om återkallande tillåts tas problemet bort. Om återkallandet inte tillåts kan användarna inte se knappen Återkalla när den första statusen för en utgåva väntar på godkännande.

Före den här ändringen tilläts alltid en återkallelse av problemet. När godkännandet återkallades förblev godkännandet fullständigt utan godkännande, vilket innebar att utfärdandet hade sin första status, utan något godkännande.

Mer information om inställningar för godkännande finns i [Konfigurera globala inställningar för godkännande](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md). 

>[!NOTE]
>
>Det här alternativet inaktiveras som standard när den här funktionen släpps. Återkommande problem är aktiverade som standard för alla organisationer. När den här funktionen släpps måste Workfront-administratören manuellt aktivera den här inställningen för att behålla funktionerna som de är i Workfront.

## Ny gruppering för resursbudgeterade timrapporter: allokeringsdatum {#new-grouping-for-resource-budgeted-hour-reports-allocation-date}

Vi har lagt till möjligheten att gruppera dina resultat efter tilldelningsdatum när du skapar en resursbudgeterad timrapport.

Före den här ändringen kunde du visa tilldelningsdatumet i rapportvyn och använda det i ett filter, men du kunde inte använda det här fältet i en gruppering.

Mer information om allokeringsdatumet finns i [Ordlista för Adobe Workfront-terminologi](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

Mer information om hur du skapar en rapport finns i [Skapa en anpassad rapport](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Förbättringar av resursplanering {#resource-planner-improvements}

* [Resursplanering: Visa data via FTE](#resource-planner-show-data-by-fte)
* [Resursplanering: Visa data per vecka och kvartal](#resource-planner-show-data-by-week-and-quarter)
* [Resursplanering: Visa efter användare](#resource-planner-view-by-user)
* [Resursplanering: Dra och släpp projekt för att ange prioritet](#resource-planner-drag-and-drop-projects-to-establish-priority)
* [Resursplanering: Exportera data i resursplaneraren till Excel](#resource-planner-export-the-data-in-the-resource-planner-to-excel)

### Resursplanering: Visa data via FTE {#resource-planner-show-data-by-fte}

Du kan nu visa allokeringen och tillgängligheten för dina resurser via FTE i resursplaneraren. Före den här ändringen kunde du bara visa värdena i timmar.

Mer information om hur du använder resursplaneraren finns i [Översikt över resursplanering](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Resursplanering: Visa data per vecka och kvartal {#resource-planner-show-data-by-week-and-quarter}

Du kan nu ändra tidsbildruteintervallet för resursplaneraren så att det visas per vecka eller kvartal. Före den här ändringen kunde du visa allokeringen och tillgängligheten för dina resurser och bara budgetera dem per månad.

Mer information om hur du använder resursplaneraren finns i [Översikt över resursplanering](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Resursplanering: Visa efter användare {#resource-planner-view-by-user}

Nu kan du visa informationen i resursplaneraren per användare, först och sedan efter projekt, roller och uppgifter. Du kan också visa en skillnad mellan Planerade och Tillgängliga timmar eller FTE för användare. Före den här ändringen kan du visa informationen i resursplaneraren efter projekt och roller.

Mer information om hur du använder resursplaneraren finns i [Översikt över resursplanering](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Resursplanering: Dra och släpp projekt för att ange prioritet {#resource-planner-drag-and-drop-projects-to-establish-priority}

Nu kan du dra och släppa projekt i önskad prioritetsordning. Före den här ändringen kan du bara ange projektens prioritet genom att manuellt tilldela dem ett nummer.

Mer information om hur du använder resursplaneraren finns i [Översikt över resursplanering](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Resursplanering: Exportera data i resursplaneraren till Excel {#resource-planner-export-the-data-in-the-resource-planner-to-excel}

Du kan nu exportera informationen i resursplaneraren till en Excel-fil.

Mer information om hur du använder resursplaneraren finns i [Översikt över resursplanering](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Mobilförbättringar {#mobile-improvements}

Vi har lagt till möjligheten att komma åt dina projekt och hantera dem från Workfront mobilapp. Nu kan du göra följande med Workfront mobilapp:

* Få tillgång till en lista över dina projekt
* Få åtkomst till en lista med aktiviteter och underaktiviteter i ett projekt
* Få åtkomst till en lista med problem i ett projekt
* Logga ett nytt problem i ett projekt

Du kan installera den här funktionen när du uppdaterar din Workfront-mobilapp. Uppdateringen kommer att finnas tillgänglig i både Apple- och Android-mobilbutikerna i november 2017.

## Workfront-integrering med Slack {#workfront-integration-with-slack}

>[!NOTE]
>
>Integreringen av Slack är för närvarande inte tillgänglig. Den kommer att vara tillgänglig i din produktionsmiljö i november 2017.

Vi lanserar en ny integrering mellan Workfront och Slack. Om ni redan har använt Slack för ert material kan ni nu integrera det med Workfront och genomföra Workfront gemensamma åtgärder utan att lämna kommunikationskanalerna i Slack. Nu kan du utföra följande åtgärder från ditt Slack-konto:

* Söka efter ett objekt i Workfront
* Få tillgång till dina arbeten och godkännandelistor
* Skapa en uppgift
* Skapa ett problem
* Prenumerera på alla objekt från en länk som delas med dig på det objektet
* Tilldela uppgifter och ärenden från en länk som delas med dig
* Godkänn ditt arbete
* Få åtkomst till dina favoriter och dina listor med senaste objekt

Mer information om hur du kommer åt Workfront från Slack finns i [Använda Workfront med Slack.](https://support.workfront.com/hc/en-us/sections/115000458033)

## Förbättringar i Outlook 365 {#outlook-365-improvements}

Vi har gjort följande förbättringar av Workfront-tillägget för Outlook 365:

* Lägg till en uppgift eller ett problem i ett projekt i Workfront: Du kan nu konvertera ett e-postmeddelande till en uppgift eller ett problem i Workfront med hjälp av tillägget Outlook 365. I den här processen kan du ange ett projekt som du vill att uppgiften eller utgåvan ska läggas till i, samt en tilldelad och ett förfallodatum. Före den här förbättringen kunde du bara skicka en begäran till en begärandekö eller lägga till en personlig uppgift i listan Arbeta på från Outlook 365. 
* Bevara en länk till Workfront-objekt i det ursprungliga e-postmeddelandet som konverterats till uppgifter, ärenden eller förfrågningar: När du konverterar ett e-postmeddelande från Outlook 365 till en uppgift, ett problem eller en förfrågan, bevaras en länk till uppgiften eller problemet som konverterades från det e-postmeddelandet i det ursprungliga e-postmeddelandet. Före den här ändringen fanns det ingen indikation i Outlook om ett e-postmeddelande har konverterats till en uppgift eller skickats som en begäran. 

  Mer information om hur du konverterar ett e-postmeddelande till en uppgift eller ett problem från Outlook 365 finns i [Lägg till ett Outlook-e-postmeddelande i ett projekt som en uppgift eller ett problem](../../../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

## API-ändringar {#api-changes}

* [API 8 ute nu](#api-8-now-available)
* [Borttagna och inaktuella versioner av API:t](#removed-and-deprecated-versions-of-the-api)
* [2017.3 Beta Final release activity](#updated-message-format-for-event-subscriptions)
* [Återförsök av händelseprenumerationer för olevererbara meddelanden](#event-subscription-retries-for-undeliverable-messages)

### API 8 ute nu {#api-8-now-available}

Workfront API version 8 finns nu och innehåller nya och uppdaterade resurser för Workfront-integreringar.

En lista över ändringar i Workfront API finns på [Uppdateringar av API-version 8](../../../../wf-api/api/new-api-version-8-updates.md).

### Borttagna och inaktuella versioner av API:t {#removed-and-deprecated-versions-of-the-api}

### Uppdaterat meddelandeformat för händelseprenumerationer

För att ge mer användbar information för dina integreringar som innehåller Workfront Event Subscriptions API har vi ändrat formatet för utgående meddelanden för resurser som stöds genom att ta med gamla och nya värden som är associerade med dessa resurser. För att undvika fel måste alla integreringar du har med Workfront Event Subscriptions API uppdateras i det nya formatet enligt beskrivningen i [API för händelseprenumeration](../../../../wf-api/general/event-subs-api.md).

### Återförsök av händelseprenumerationer för olevererbara meddelanden {#event-subscription-retries-for-undeliverable-messages}

Workfront ramverk för händelseprenumerationer innehåller nu en mekanism för hantering av händelseutlösta utgående meddelanden som inte kan leverera till kundslutpunkter. För att säkerställa kontinuerlig meddelandeleverans bör kunderna se till att slutpunkterna som förbrukar utgående meddelanden från händelseprenumerationer är korrekt konfigurerade. Mer information finns i [Återkommande prenumerationer på evenemang](../../../../wf-api/api/event-sub-retries.md).

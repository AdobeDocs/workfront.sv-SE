---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 Beta Final
description: Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i version 2017.2. Funktionerna på den här sidan gjordes tillgängliga i förhandsvisningsmiljön den 28 juni 2017. Det kommer att göras tillgängligt i produktionsmiljön den 26 juli 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 768e9aad-d7e7-4a3c-9f93-926cf588ddc7
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2314'
ht-degree: 0%

---

# 2017.2 Beta Final

Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i version 2017.2. Funktionerna på den här sidan gjordes tillgängliga i förhandsvisningsmiljön den 28 juni 2017. Det kommer att göras tillgängligt i produktionsmiljön den 26 juli 2017.

>[!IMPORTANT]
>
>Funktionerna som beskrivs på den här sidan kan ändras innan de är tillgängliga i produktionsmiljön.

En lista över alla ändringar som gjorts under 2017.2 finns i [Översikt över versionsaktivitet för 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

Beta Final-utgåvan 2017.2 innehåller förbättringar både för Workfront-administratörer och andra användare:

**För administratörer:**

* [Avgör tillgängligheten för HTML5-visningsprogrammet (ProofHQ och Workfront)](#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront)
* [Stöd för SHA-256-certifikat för SAML 2.0](#support-sha-256-certificates-for-saml-2-0)
* [Före-typ för mappningsattribut](#type-ahead-for-mapping-attributes)
* [API-förbättring: få åtkomst till användarallokeringar](#api-enhancement-access-user-allocations)

**För alla användare:**

* [Resursplanering](#resource-planner)
* [Nytt schemaläggningsområde i ett projekt (Team Builder)](#new-scheduling-area-in-a-project-team-builder)
* [Resursplanering: Visa färre objekt som standard](#resource-scheduling-show-fewer-items-by-default)
* [Resursschemaläggning: Visa släppindikator och överallokering när du drar aktiviteter och problem](#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues)
* [Resursschemaläggning: Användarallokeringar avrundas inte längre till närmaste halvtimme](#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour)
* [Exportera användningsrapporten i formaten TSV och PDF](#export-the-utilization-report-in-tsv-and-pdf-formats)
* [2017.2 Beta Final](#user-calendar-enhancements-in-the-my-work-area%22)
* [2017.2 Beta Final](#layout-template-determines-whether-the-new-or-legacy-calendar-displays-in-the-my-work-area)
* [Korrektur för beslut visas på arbetsytan (Workfront)](#proof-decision-displays-in-the-my-work-area-workfront)
* [Visa korrektur för multimedia i förinställda upplösningar (ProofHQ och Workfront)](#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront)
* [Visa URL till undersidor i kommentarer om mediekorrektur (ProofHQ och Workfront)](#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront)
* [Skapa anpassade vyer baserade på befintliga standardvyer (ProofHQ)](#create-custom-views-based-on-existing-standard-views-proofhq)
* [Filtrera rapportområdet (Korrektur)](#filter-the-reporting-area-proofhq)
* [Visa lägsta och högsta värden i rapporter (ProofHQ)](#display-minimum-and-maximum-values-in-reports-proofhq)
* [Meddelande i appen för godkännande av korrektur](#in-app-notification-for-proof-approval)
* [Mobila förbättringar](#mobile-improvements)
* [Snedstreck har lagts till i filtersatser för fältvärden som innehåller kommatecken](#slash-added-to-filter-statements-for-field-values-that-contain-commas)
* [Flera faktureringspriser](#multiple-billing-rates)
* [Nytt fält för resursbudgeterad timme](#new-resource-budgeted-hour-field)
* [Visa användarjobbroll i området Tilldelad till på informationssidan för uppgifter och problem](#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues)

>[!NOTE]
>
>Verktygen för resursschemaläggning har tagits bort från Workfront i version 23.1. Mer information om att schemalägga resurser med hjälp av belastningsutjämnaren finns i [Översikt över belastningsutjämnaren](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

## Nytt schemaläggningsområde i ett projekt (Team Builder) {#new-scheduling-area-in-a-project-team-builder}

Schemaläggningsområdet i ett projekt (tidigare Team Builder) har omarbetats med ett uppdaterat och mer intuitivt användargränssnitt. Den nya funktionen Schemaläggning är nu bättre anpassad till de funktioner för resursplanering som finns i andra delar av Workfront.

Bland förbättringarna finns:

* Visa aktuella resursallokeringar för medlemmar i projektteamet, så att du kan fatta mer välgrundade beslut när du gör tilldelningar
* Visuell representation av aktivitetens varaktighet på tidslinjen för tidsplanering
* Filtrera den information som visas på tidslinjen i schemat
* Lägg enkelt till och ta bort användare från projektteamet, direkt från tidslinjen för schemaläggning

Följande funktionalitet är tillgänglig i andra delar av verktyget när resurser schemaläggs, men är inte tillgänglig när resurser schemaläggs i teamschemaläggningsområdet:

* Konfigurera överordnade uppgifter som ska visas på tidslinjen för schemaläggning
* Konfigurera projektnamn som ska visas på tidslinjen för schemaläggning
* Ändra användartilldelningar med verktyget Växla
* Filtrera efter portfölj, program och projekt

Mer information om de funktioner som är tillgängliga i området Team Scheduling finns i&quot;Kom igång med Resource Scheduling&quot;.

## Resursschemaläggning: Visa färre objekt som standard {#resource-scheduling-show-fewer-items-by-default}

Som standard visas nu högst 10 arbetsuppgifter per dag på tidslinjen för schemaläggning för en viss användare. Du kan expandera listan för att visa alla uppgifter och ärenden som för närvarande är tilldelade till den användaren.

På så sätt kan du enklare bläddra på tidslinjen när användare tilldelas många uppgifter och problem.

Före den här ändringen visades alla uppgifter och problem alltid för alla användare.

Mer information om hur du tilldelar användare uppgifter och utgåvor på tidslinjen finns i &quot;Tilldela ej tilldelade uppgifter och utgåvor manuellt i tidsplaneringsområdena&quot;.

## Resursschemaläggning: Visa släppindikator och övertilldelning när du drar aktiviteter och ärenden {#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues}

När du tilldelar en uppgift eller ett problem till en användare på tidslinjen via dra-och-släpp visas nu följande information innan uppgiften eller utgåvan släpps och tilldelningen slutförs:

* En släppindikator visas på användarens rad. På så sätt kan du se var ett objekt tilldelas innan du gör tilldelningen.
* Om användarallokeringar är aktiverade på tidslinjen för tidsplanering visas indikatorerna för röd överallokering om tilldelningen slutförs, vilket resulterar i att användaren blir överallokerad.

Före dessa ändringar visades ingen information innan uppgiften eller problemet släpptes.

Mer information om hur du tilldelar användare uppgifter och utgåvor på tidslinjen finns i &quot;Tilldela ej tilldelade uppgifter och utgåvor manuellt i tidsplaneringsområdena&quot;.

## Resursschemaläggning: Användarallokeringar avrundas inte längre till närmaste halvtimme {#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour}

När flera användare tilldelas till en uppgift eller ett ärende, eller när en uppgift eller ett ärende sträcker sig över flera dagar, försöker Workfront distribuera planerade timmar jämnt mellan de tilldelade användarna och dagarna. Timmar avrundas som standard till närmaste hundradel (till exempel 1,33).

När du tidigare ändrat fördelade timmar manuellt justeras timmarna och avrundas till närmaste halvtimme (t.ex. avrundas 1,33 till 1,5).

Nu justeras inte timmarna längre och avrundas till närmaste halvtimme (1,33 är till exempel 1,33).

## API-förbättring: få åtkomst till användarallokeringar {#api-enhancement-access-user-allocations}

Nu kan du få åtkomst till skuggning av användarallokering via Workfront API.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../../../wf-api/api/access-proj-allocation-info-api.md" class="MCXref xref" xrefformat="{para}">Access Project Allocation Information via the API</a>.</p>
-->

## Exportera användningsrapporten i formaten TSV och PDF {#export-the-utilization-report-in-tsv-and-pdf-formats}

Nu kan du exportera användningsrapporten för ett projekt i formaten TSV och PDF, förutom XLSX-formatet.

Före den här ändringen kunde du bara exportera användningsrapporten i XLSX-format.

Mer information om hur du exporterar användningsrapporten finns i [Översikt över resursanvändningsrapporten](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) i [Översikt över resursanvändningsrapporten](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Skärmar för korrekturbeslut på arbetsytan (Workfront) {#proof-decision-displays-in-the-my-work-area-workfront}

När du nu visar korrekturgodkännanden på fliken Mina godkännanden på arbetsytan Mitt arbete visas korrekturbeslutet på arbetsytan i Mitt arbete tills du klickar på den nya uppdateringsknappen i Workfront eller tills nästa gång du uppdaterar webbläsarsidan.

Före den här ändringen fanns det inget som tydde på att ett beslut redan hade fattats om beviset, och beviset fanns kvar på fliken Mina godkännanden tills du uppdaterade webbläsaren.

Mer information finns i [Godkänna arbete](../../../../review-and-approve-work/manage-approvals/approving-work.md) i [Godkänna arbete](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Visa korrektur för multimedia i förinställda upplösningar (ProofHQ och Workfront) {#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront}

I en tidigare version av förhandsvisningsmiljön introducerades möjligheten att justera upplösningen för korrektur för multimedia antingen genom att ange en anpassad upplösning eller genom att dra bilden till önskad upplösning.

Du kan nu välja bland förinställda upplösningsalternativ för olika telefoner, surfplattor, bärbara och stationära datorer.

Mer information finns i&quot;Visa en förinställd upplösning&quot; i [Ändra interaktiv korrekturupplösning i korrekturläsaren](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

## Visa URL till delsidor i kommentarer om korrektur av multimedia (ProofHQ och Workfront) {#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront}

>[!NOTE]
>
>Den här funktionen är för närvarande tillgänglig i produktionsmiljön.

När du nu kommenterar en undersida i ett Rich Media-korrektur visas URL:en till undersidan i kommentaren.

Före den här ändringen stod det inte klart vilken undersida kommentaren avsåg.

Mer information finns i

## Avgör tillgängligheten för HTML5-visningsprogrammet för videokorrektur (ProofHQ och Workfront) {#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront}

Som Workfront-administratör i ProofHQ kan du avgöra om användare i din organisation har tillgång till den nya korrekturläsaren för HTML 5 för videokorrektur.

Mer information om hur du konfigurerar det här alternativet i Workfront finns i .

## Skapa anpassade vyer baserade på befintliga standardvyer (ProofHQ) {#create-custom-views-based-on-existing-standard-views-proofhq}

Nu kan du skapa en anpassad vy baserat på en standardvy. Alternativen Kolumner, Sortering och Filter från standardvyn inkluderas som standard i den nya vyn.

Innan den här ändringen utfördes var du tvungen att skapa en helt ny vy för att kunna skapa en anpassad vy. 

Mer information finns i [Skapa en anpassad vy](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md#creating) i [Skapa och hantera anpassade vyer i Workfront Proof-korrektur](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## Filtrera rapportområdet (ProofHQ) {#filter-the-reporting-area-proofhq}

Som standard innehåller data som visas på fliken Rapporter all information från ditt Korrektur-HQ-system. Nu kan du använda filter för att endast visa information som är relevant för dina behov. 

Mer information finns i [Filtrera rapporter](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#filtering-reports) i  [Kör rapporter i Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## Visa minimi- och maximivärden i rapporter (ProofHQ) {#display-minimum-and-maximum-values-in-reports-proofhq}

Du kan nu konfigurera om lägsta och högsta värden ska visas i diagrammet när du visar rapporter.

Mer information finns i [Visa rapporter](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#viewing-reports) i  [Kör rapporter i Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## Stöd för SHA-256-certifikat för SAML 2.0 {#support-sha-256-certificates-for-saml-2-0}

Nu har vi stöd för Secure Hash Algorithm 256 (SHA-256) när vi konfigurerar Workfront för enkel inloggning med SAML 2.0. Före den här versionen hade vi bara stöd för SHA-1 (Secure Hash Algorithm 1).

Mer information om att konfigurera Workfront med SAML 2.0 finns i [Konfigurera Adobe Workfront med SAML 2.0](../../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)

## Type-Ahead för mappningsattribut {#type-ahead-for-mapping-attributes}

Fälttypen Standardvärde i dialogrutan Attributmappning har uppdaterats till ett type-ahead-fält. Före den här ändringen var typen av standardvärdesfält en listruta.

Den här ändringen gäller för följande SSO-protokoll:

* Active Directory
* LDAP
* SAML 2.0

SAML 1.1 stöder inte attributmappning.

## Mobilförbättringar {#mobile-improvements}

>[!NOTE]
>
> Mobilappen släpps oberoende av Workfront huvudprogram. Funktionerna som beskrivs i det här avsnittet lanseras i början av augusti.

Följande nya funktioner visas i mobilapparna, både för Android och iOS:

* Skicka förfrågningar från mobilappen
* Tidrapport Nytt inlägg i mobilappen
* Anpassad formulärredigering från mobilappen
* Begäranden om godkännande av korrektur i mobilappen

Det kommer att finnas ett offentligt betaprogram för vissa av dessa funktioner för Android.

Mer information om det kommande betaprogrammet för mobilen finns i  Sidan [&quot;Betas&quot;](https://support.workfront.com/hc/en-us/sections/115000743248).

Mer information om hur du använder mobilappen Workfront finns i .  

## Snedstreck har lagts till i filtersatser för fältvärden som innehåller kommatecken {#slash-added-to-filter-statements-for-field-values-that-contain-commas}

När du skapar ett filter i textläge och filtrerar efter fältvärden som innehåller kommatecken måste du lägga till ett snedstreck (&quot;/&quot;) före kommatecknen som avgränsar värdena, för att se till att värdet läses som ett filteralternativ. Detta gäller endast för följande fälttyper:

* Listrutor
* Alternativknappar
* Kryssrutor

Före den här ändringen kunde du inte filtrera efter fält som hade alternativ som innehöll kommatecken.

Mer information om den här ändringen finns i [Översikt över filter](../../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Flera faktureringspriser {#multiple-billing-rates}

Nu kan du lägga till flera åsidosättningar av faktureringsfrekvens för samma jobbroll på projektnivå. Med den här nya funktionen kan du definiera datumintervall för varje åsidosättning av faktureringsfrekvens. Under det angivna datumintervallet används en annan faktureringsfrekvens för jobbrollen som tilldelats aktiviteter i ett projekt. Faktureringstarifferna multipliceras med timmarna i projektet för att beräkna intäkterna. Intäkter som beräknas inom datumintervallet för en faktureringsfrekvens förblir låsta till den taxan och uppdateras inte som frekvenserna för jobbrollerna i projektuppdateringen. När det gäller Faktisk intäkt kommer inga timmar som loggats innan faktureringstakten åsidosatts att beräknas om för att återspegla den aktuella faktureringstakten. De timmar som loggats innan åsidosättningen av faktureringssatsen lades till i projektet kommer att associeras med faktureringsfrekvensen för jobbrollen vid den tidpunkten.

Före den här ändringen kunde du bara åsidosätta faktureringssatsen för en jobbroll en gång, och Faktisk intäkt beräknas om för att återspegla den aktuella faktureringssatsen för alla timmar som loggats innan faktureringssatsen ändrades.

Mer information om debitering och intäkt finns i [Översikt över fakturering och intäkt](../../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Mer information om att åsidosätta faktureringssatser för jobbroller på projektnivå finns i [Översikt över åsidosättande av faktureringssatser för jobbroller och beräkning av intäkter för ett projekt](../../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Resursplanering {#resource-planner}

I den här versionen introducerar vi den första fasen av resursplaneraren, som ingår i den nya designen av den nya planeringsfliken i personområdet. Med Resursplaneraren kan du budgetera antalet timmar som användarna i dina resurspooler har tilldelats i alla aktuella projekt som du är resurshanterare för. I resursplaneraren kan du se följande allokeringsnummer per projekt, jobbroll och användare:

* Tillgängliga timmar
* Planerade timmar
* Budgeterade timmar
* Timavvikelse (mellan budgeterade och planerade timmar)
* Skillnad i nettotimma (mellan tillgängliga och budgeterade timmar)

Mer information om hur du använder resursplaneraren finns i [Resursplaneringsöversikt](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Nytt resursbudgeterat timfält {#new-resource-budgeted-hour-field}

Ett nytt fält har lagts till i Report Builder, som gör att du kan rapportera om resursbudgeterade timmar, som stöd för den nya planeringsfunktionen och resursplaneringen. Det här fältet visar hur många timmar en resurs har budgeterats för i ett projekt. Det här fältet är inte tillgängligt när resurser budgeteras med funktionen för äldre resursplanering.

Mer information om hur du använder budgeterade timmar i resursplaneraren finns i [Resursplaneringsöversikt](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Meddelande i appen för korrekturgodkännande {#in-app-notification-for-proof-approval}

När du har utsetts till godkännare för ett korrektur får du ett meddelande i appen om att korrekturgodkännandet väntar på ditt beslut. Meddelandet visar följande text: `<User name>` vill att du ska godkänna det här beviset&quot;. Om användarinformationen inte är tillgänglig ändras meddelandet till&quot;Detta bevis kräver ditt godkännande&quot;.

Före den här förbättringen var den enda visuella indikationen på att du har utsetts till godkännare på ett korrektur en ny begäran om bevis på arbetsytan Mitt arbete.

Mer information om meddelanden i appen finns i [Visa och hantera meddelanden i appen](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## Visa användarjobbroll i området Tilldelad till på informationssidan för uppgifter och problem {#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues}

När du nu visar informationssidan för en uppgift eller ett problem visas en jobbroll under den tilldelades namn i området Tilldelad till. Den här jobbrollen representerar jobbrollen för användaren som matchar jobbrolltilldelningen för uppgiften eller utgåvan. Om uppgiften eller utgåvan inte har tilldelats en jobbroll visas den primära jobbrollen för den tilldelade användaren.

Före den här ändringen visades bara användarens titel under användarens namn i området Tilldelad till. 

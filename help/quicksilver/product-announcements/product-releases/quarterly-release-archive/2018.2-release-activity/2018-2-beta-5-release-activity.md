---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 Beta 5 - versionsaktivitet
description: Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i 2018.2 Beta 5. Funktionerna kommer att vara tillgängliga i förhandsvisningsmiljön den 1 juni 2018. Förbättringar av korrektur som släpps med Beta 5 kommer att finnas tillgängliga i förhandsvisningsmiljön måndagen den 4 juni. Den kommer att göras tillgänglig i produktionsmiljön i juli 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0a8602aa-34c8-44d0-a102-9497d106f806
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '3158'
ht-degree: 0%

---

# 2018.2 Beta 5 - versionsaktivitet

Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i 2018.2 Beta 5. Funktionerna kommer att vara tillgängliga i förhandsvisningsmiljön den 1 juni 2018. Förbättringar av korrektur som släpps med Beta 5 kommer att finnas tillgängliga i förhandsvisningsmiljön måndagen den 4 juni. Den kommer att göras tillgänglig i produktionsmiljön i juli 2018.

>[!IMPORTANT]
>
> Funktionerna som beskrivs på den här sidan kan ändras innan de är tillgängliga i produktionsmiljön.

En lista över alla ändringar som gjorts under 2018.2 finns på  [Aktivitetsöversikt för version 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

2018.2 Beta 5 innehåller förbättringar för Workfront-administratörer och andra användare:

**För administratörer**

* [Visa ändringar som utlösts av användaren med granskningsloggar](#view-user-triggered-changes-with-audit-logs)
* [Visa licensinformation som gruppadministratör](#view-license-information-as-a-group-administrator)

**För alla användare**

* [Kalendervy i hemområdet](#calendar-view-in-the-home-area)
* [Ytterligare uppdateringar i arbetslistan (vänster panel) i Hem](#additional-updates-to-the-work-list-left-panel-in-home)
* [Konfigurera jobbrollsgränser för automatisk resursplanering](#configure-job-role-limits-for-automated-resource-scheduling)
* [Förbättringar av projekt- och rollvyn i resursplaneraren](#project-and-role-view-improvements-in-the-resource-planner)
* [Ändra storlek på kolumnbredder för projektlistor](#resize-column-widths-for-project-lists)
* [Ikonstöd för nya projektlistor](#icon-support-for-the-new-project-lists)
* [Lägg till fältet&quot;Stora miniatyrbilder&quot; i dokumentvyer](#add-large-thumbnail-field-in-document-views)
* [Öka exportgränsen för Excel](#increase-excel-export-limit)
* [Snabbfilter för projektlistor](#quick-filters-for-project-lists)
* [Referensutgåvsamlingar i projekt- och aktivitetsrapporter](#reference-issue-collections-in-project-and-task-reports)
* [Ny, mer robust version-meny när nya dokumentversioner läggs till i Workfront](#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront)
* [Mobilförbättringar i Android Beta-mobilappen](#mobile-improvements-in-the-android-beta-mobile-app)
* [Förbättringar av korrekturläsare (Workfront och Workfront Proof)](#proofing-viewer-enhancements-workfront-and-workfront-proof)
* [Språkförbättringar i Workfront](#proofing-enhancements-in-workfront)
* [Förbättringar av korrektur i Workfront Proof](#proofing-enhancements-in-workfront-proof)

## Kalendervy i hemområdet {#calendar-view-in-the-home-area}

Nu kan du hantera dina arbetsuppgifter och scheman i Workfront hemkalender. I vyn Hemkalender kan du göra följande:

* Ange ett eget schema för att utföra Workfront-uppgifter som du har tilldelats
* Se snabbt vilka uppgifter som förfaller eller har förfallit
* Visa totalt antal tilldelade timmar för en vecka
* Uppdatera uppgifter som du har tilldelats

Om du använder en kalender i Outlook kan du integrera kalendern för att visa Outlook-händelser i hemkalendervyn.

## Ytterligare uppdateringar av arbetslistan (vänster panel) i hemmet {#additional-updates-to-the-work-list-left-panel-in-home}

Följande förbättringar är nu tillgängliga för arbetslista i hemområdet:

* Antalet slutförda objekt visas nu inom parentes bredvid alternativet Slutfört på den nedrullningsbara menyn Filter.

  Tidigare visades inte antalet slutförda objekt på menyn Filter. 

* Slutförda objekt visas för de senaste två veckorna.

  Tidigare visades slutförda poster för de senaste tre månaderna.

  Mer information om hur du visar det färdiga arbetet i Hem-området finns i [Visa objekt i Arbetslista i Hem](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md) i artikeln [Visa objekt i Arbetslista i Hem](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Lägg till fältet Varaktighet och fältet Uppdrag som ska visas när objekt markeras i området Hem.

  Tidigare var uppdragsfältet tillgängligt som standard, men om det togs bort kunde det inte läggas till igen. Fältet Varaktighet var inte tidigare tillgängligt att lägga till.

  Mer information om hur du lägger till fält i området Hem finns i&quot;Skapa och hantera layoutmallar&quot;.

Mer information om hur du använder Hem-området finns i [Använda Hem-området](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Visa ändringar som utlösts av användaren med granskningsloggar {#view-user-triggered-changes-with-audit-logs}

Vi har skapat följande granskningsloggar för Workfront-administratörer för att spåra ändringar som utlösts av användare:

* Användargranskningslogg
* Granskningslogg på åtkomstnivå
* Gruppgranskningsloggar
* Inloggningsförsöksgranskningsloggar

Tidigare fanns det inget sätt att spåra ändringar i systemet.

Mer information finns i [Visa och exportera granskningsloggar](../../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Visa licensinformation som gruppadministratör {#view-license-information-as-a-group-administrator}

Vi har skapat en skrivskyddad licenssida där gruppadministratörer kan visa antalet licenser för de grupper de administrerar.

Före den här ändringen kunde gruppadministratörer inte visa licensinformation.

Mer information finns i [Gruppadministratörer](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

## Konfigurera begränsningar för jobbroller för automatisk resursschemaläggning {#configure-job-role-limits-for-automated-resource-scheduling}

>[!NOTE]
>
>Verktygen för resursschemaläggning har tagits bort från Workfront i version 23.1. Mer information om att schemalägga resurser med hjälp av belastningsutjämnaren finns i [Översikt över belastningsutjämnaren](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

I inställningarna för automatiserad resursschemaläggning kan du nu tilldela en gräns till en jobbroll. På så sätt kan du styra antalet resurser som tilldelas arbete, med samma roll.

Tidigare kunde du inte ange hur många användare i en viss jobbroll som kunde tilldelas arbete.

Mer information finns i &quot;Tilldela ej tilldelade uppgifter och ärenden manuellt i schemaläggningsområden&quot;.

## Förbättringar av projekt- och rollvyn i resursplaneraren {#project-and-role-view-improvements-in-the-resource-planner}

Resursplaneringens projekt- och rollvyer innehåller nu följande förbättringar:

* Förbättrade filter som hämtar information från hela databasen i stället för bara informationen på skärmen.
* Helskärmsläge.
* Prestanda är nu snabbare och effektivare.

   * Nya gränser för antalet projekt, roller och användare som du kan visa.
   * Lazy loading, vilket ger snabbare inläsning av projekt och roller.

* Snabb åtkomst till projekt och användare direkt från resursplaneraren.
* Snabbare dra-och-släpp-funktioner i projektvyn för att prioritera dina projekt.

Före dessa förbättringar har du rapporterat att resursplaneraren var långsam att läsa in och att du har upptäckt inkonsekvenser i de data som visas. Dessa förbättringar bör nu tas bort.

Mer information och information om de nya gränserna för resursplaneraren finns i [Resursplaneringsbegränsningar](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref" xrefformat="{para}">Resource Planner performance beta </a></p>
-->

## Ändra storlek på kolumnbredder för projektlistor {#resize-column-widths-for-project-lists}

När vi har arbetat med att förbättra funktionerna i våra listor hade vi tillfälligt inaktiverat möjligheten att ändra storlek på kolumnbredderna i följande projektlistor:

* Projekt jag äger
* Projekt som jag är på
* Alla projekt

I den här versionen kan vi nu ändra storlek på kolumnerna i alla projektlistor.

Vi har lagt till ytterligare förbättringar av den här funktionen.

När du nu drar den högra kanten på en kolumn för att ändra storlek på den behåller den angränsande kolumnen till höger sin storlek och gör listan bredare, i stället för att ändras. Du kan också dra en kolumns kant till höger förbi kanterna på de intilliggande kolumnerna.

Före den här förbättringen ändras storleken på den intilliggande kolumnen till höger om den storleksändrade kolumnen proportionellt så att den får plats på skärmen. Du kan inte dra kanten på en kolumn förbi den intilliggande kolumnens högra kant.  

Mer information om hur du ändrar ordning på kolumnerna i listor finns i [Ändra kolumnbredd och ordning](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Om du vill delta i vårt betatestningsprogram och se de aktuella förbättringarna i listan kan du läsa [New Lists Study.](https://experienceleaguecommunities.adobe.com/t5/workfront/ct-p/workfront?profile.language=sv) (Inloggning krävs)

## Ikonstöd för nya projektlistor {#icon-support-for-the-new-project-lists}

Eftersom vi har arbetat med att förbättra funktionerna i våra listor har vi tillfälligt inaktiverat visning av statusikoner i följande projektlistor:

* Projekt jag äger
* Projekt som jag är på
* Alla projekt

I den här versionen kan statusikoner visas igen i dina projektlistor för projekt eller andra objekt i en projektlista.

Mer information om hur du arbetar i listor finns i [Kom igång med listor i Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Lägg till fältet&quot;Stora miniatyrbilder&quot; i dokumentvyer {#add-large-thumbnail-field-in-document-views}

Vi lägger till ett nytt fält med namnet Stora miniatyrbilder i en dokumentvy i en lista eller rapport. När du väljer det här fältet i en dokumentvy visas en 400 pixlar bred miniatyrbild av dokumentet i en lista eller rapport.

Före den här ändringen kunde du bara lägga till fältet Miniatyrbild i en dokumentvy, som visar en 33-66 pixlar bred miniatyrbild av dokumentet.

Mer information om fält i listor och rapporter finns i [Ordlista för Adobe Workfront-terminologi](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Öka exportgränsen för Excel {#increase-excel-export-limit}

Vi har ökat gränsen för hur många rader du kan exportera i en Excel-fil. Du kan nu exportera följande:

* 65 000 rader i en Excel .xls-fil
* 100 000 rader i en Excel .xlsx-fil

De nya gränserna gäller när du exporterar följande från Workfront:

* En lista eller rapport från webbgränssnittet
* En lista eller rapport med API:t
* En schemalagd och levererad rapport

Före den här förbättringen kunde du bara exportera 50 000 rader i en Excel-fil.

Mer information om att exportera data från Workfront finns i [Exportera data](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Snabbfilter för projektlistor {#quick-filters-for-project-lists}

Du kan nu använda ett snabbfilter på listor.

Syftet med ett snabbfilter är att hjälpa dig att navigera direkt till de objekt i dina stora listor som är viktiga för dig, så att du snabbt kan granska, uppdatera eller dela dem med andra.

För närvarande är snabbfilter bara tillgängliga för projektlistorna på följande underflikar:

* Projekt som jag är på
* Projekt jag äger
* Alla projekt

Mer information om snabbfilter finns i avsnittet Använda snabbfilter i listor i [Kom igång med listor i Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## ReferensÄrendesamlingar i projekt- och uppgiftsrapporter {#reference-issue-collections-in-project-and-task-reports}

Nu kan du referera till en samling med problem i ett projekt eller i en uppgiftsvy och filtrera. Det kan du bara göra med textläget när du skapar en rapport.

Före den här förbättringen kunde du bara referera till en samling uppgifter i en projektvy eller ett filter.

Mer information om hur du refererar till en samling i en rapport finns i [Referenssamlingar i en rapport](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

Mer information om hur du använder textläge finns i  [Översikt över vanliga användningsområden för textläge](../../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

>[!NOTE]
>
>I följande video var exempeltextläget för utskickssamlingar felaktigt. Det korrekta exempeltextläget är tillgängligt i [referenssamlingar i en rapport](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

## Ny mer robust versionsmeny när nya dokumentversioner läggs till i Workfront {#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront}

När du nu lägger till nya versioner i dokument i Workfront innehåller menyn Ny version ytterligare alternativ och är nu konsekvent i alla delar av Workfront där du kan lägga till en ny version.

Du kan lägga till en ny dokumentversion från följande områden i Workfront:

* Från menyn Mer på fliken Dokument.
* Från menyn Dokumentåtgärder på dokumentinformationssidan.
* På fliken Alla versioner på dokumentinformationssidan.

Före den här ändringen var det bara listrutan Mer på fliken Dokument som innehöll alla alternativ för att lägga till en ny version.

Följande alternativ är nu tillgängliga på menyn Ny version för alla områden där du kan lägga till en ny version:

* Korrektur
* Endast dokument
* Länkade alternativ (från Dropbox, Från Google Drive och så vidare)
* Klistra in från Urklipp (detta är ett nytt alternativ när du lägger till versioner)

Mer information finns i [Lägga till dokument i Adobe Workfront från ditt filsystem](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md) i artikeln [Lägga till dokument i Adobe Workfront från ditt filsystem](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

## Mobilförbättringar i Android Beta mobilapp {#mobile-improvements-in-the-android-beta-mobile-app}

Följande förbättringar kommer att vara tillgängliga i Android Beta-versionen av mobilappen kort efter den här versionen:

* Svepningsåtgärder

  Du kan utföra aktiviteter som frivilliga för att arbeta med en uppgift, slutföra en uppgift, markera ett meddelande som det visas eller nytt, eller ringa en kontakt genom att svepa olika objekt i Workfront mobilapp.

  Följande områden har förbättrats med den här funktionen:

   * Mitt arbete och min startsida
   * Meddelanden
   * Kontakter
   * Godkännanden

* Nytt utseende när du visar fliken Detaljer för ett objekt

  Gränssnittet har ändrats när du visar ett objekt i Android Beta-versionen av mobilappen för att göra det enklare att redigera, slutföra eller bifoga ett dokument till det.

* Ny upplevelse vid loggning

  Loggningstiden är snabbare och enklare än tidigare, med en enklare knapp för loggningstid och ett smidigare gränssnitt för loggningstid.

I den här versionen är dessa förbättringar bara tillgängliga för Android Beta-versionen av Workfront-mobilappen. De är för närvarande inte tillgängliga för iOS.

Mer information om hur du registrerar dig som betatestare och laddar ned Android Beta-versionen av Workfront mobilapp finns i .

## Förbättringar av korrekturläsare (Workfront och Workfront Proof) {#proofing-viewer-enhancements-workfront-and-workfront-proof}

* [Uppdaterad utskriftssammanfattning](#updated-print-summary-page)
* [Lägg till användare i ett korrektur direkt från korrekturläsaren](#add-users-to-a-proof-directly-from-the-proofing-viewer)
* [Visa alla markeringsverktyg i korrekturläsaren](#display-all-markup-tools-in-the-proofing-viewer)
* [Konfigurera standardalternativ för sortering i korrekturläsaren](#configure-default-sorting-options-in-the-proofing-viewer)
* [Visa Workfront-dokumentgodkännanden i Desktop Proofing Viewer](#view-workfront-document-approvals-in-the-desktop-proofing-viewer)
* [Konfigurera länkar som öppnar nya flikar och fönster för att öppnas i Desktop Proofing Viewer](#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer)
* [Visningsindikator i korrekturläsaren](#presence-indicator-in-the-proofing-viewer)
* [Filtrera kommentarer för att visa en sida för interaktiva URL-korrektur i korrekturläsaren för skrivbordet](#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer)
* [Desktop Proofing Viewer for Static and Video Content](#desktop-proofing-viewer-for-static-and-video-content)
* [Lägg till anpassade enheter i systemet](#add-custom-devices-to-your-system)

### Uppdaterad sida för utskriftssammanfattning {#updated-print-summary-page}

Sidan Skriv ut sammanfattning har uppdaterats med ett nytt utseende och en ny känsla samt förbättrad funktionalitet.

Mer information finns i [Skriva ut en korrektursammanfattning i Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md).

### Lägg till användare i ett korrektur direkt från korrekturläsaren {#add-users-to-a-proof-directly-from-the-proofing-viewer}

Nu kan du lägga till användare i ett korrektur direkt från Web Proofing Viewer och Desktop Proofing Viewer. 

Tidigare kunde du inte lägga till enskilda användare i ett korrektur. I stället kan du bara kopiera den offentliga URL:en eller inbäddningskoden.

Mer information finns i [Dela ett korrektur genom att lägga till användare](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) i artikeln  [Dela ett korrektur från korrekturläsaren](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

### Visa alla markeringsverktyg i korrekturläsaren {#display-all-markup-tools-in-the-proofing-viewer}

Nu kan du konfigurera markeringsverktyget så att det visas hela tiden i stället för i en meny som du måste öppna. Detta gör det snabbare att växla mellan verktyg. När markeringsverktygen är konfigurerade på det här sättet visas de vågrätt högst upp i Web Proofing Viewer och Desktop Proofing Viewer.

Tidigare var markeringsverktygen bara tillgängliga i en nedrullningsbar meny.

Mer information om hur du konfigurerar den här kodinställningen finns i [Konfigurera inställningar för korrekturläsare](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

Mer information om hur du använder markeringsalternativ när du granskar ett korrektur finns i artikeln.

### Konfigurera standardalternativ för sortering i korrekturläsaren {#configure-default-sorting-options-in-the-proofing-viewer}

När du nu ändrar sorteringsalternativet i kommentarlistan i ett korrektur blir det alternativet standardsorteringsalternativet nästa gång du öppnar ett korrektur i Web Proofing Viewer eller Desktop Proofing Viewer. 

Mer information finns i artikeln.

### Visa Workfront-dokumentgodkännanden i korrekturläsaren för skrivbordet {#view-workfront-document-approvals-in-the-desktop-proofing-viewer}

Nu kan du fatta ett beslut om godkännande av Workfront-dokument i Desktop Proofing Viewer.

Tidigare var det bara i Web Proofing Viewer som du kunde godkänna Workfront-dokument. 

Mer information finns i  [Välj ett korrektur i korrekturläsaren](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) i artikeln  [Fatta ett beslut om ett korrektur i korrekturläsaren](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

### Konfigurera länkar som öppnar nya flikar och fönster för att öppnas i Desktop Proofing Viewer {#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer}

När du korrekturläser interaktivt innehåll i Desktop Proofing Viewer kan du nu konfigurera länkar som öppnas på en ny flik eller i ett nytt fönster så att de öppnas i Desktop Proofing Viewer så att du kan fortsätta korrekturgranska.

I det äldre korrekturläsaren gick det inte att granska länkar som öppnats i en ny flik eller i ett nytt fönster i korrekturläsaren.

Mer information finns i [Konfigurera inställningar för korrekturläsare](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

### Visningsindikator i korrekturläsaren {#presence-indicator-in-the-proofing-viewer}

När du nu granskar ett korrektur i Web Proofing Viewer eller Desktop Proofing Viewer kan du visa avataren för varje användare som för tillfället tittar på korrekturet visas i det övre högra hörnet av korrekturläsaren.

Mer information finns i [Granska ett korrektur samtidigt med flera granskare](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proof-with-multiple-reviewers.md).

### Filtrera kommentarer för att visa en sida för interaktiva URL-korrektur i korrekturläsaren för skrivbordet {#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer}

När du granskar en URL-adress i ett interaktivt korrektur i Desktop Proofing Viewer kan du nu filtrera kommentarer så att kommentarer bara visas på den aktuella sidan. 

Före den här ändringen var det här alternativet endast tillgängligt för statiska korrektur.

Mer information finns i artikeln.

### Desktop Proofing Viewer for Static and Video Content {#desktop-proofing-viewer-for-static-and-video-content}

Desktop Proofing Viewer har nu stöd för statiskt innehåll och videomaterial.

Tidigare hade det bara stöd för interaktivt innehåll.

Mer information om hur du konfigurerar statiska korrektur och videoklipp att öppnas i Desktop Proofing Viewer finns i [Konfigurera inställningar för korrekturläsare](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

Mer information om Desktop Proofing Viewer finns i [Granska korrektur i Desktop Proofing Viewer.](https://support.workfront.com/hc/en-us/sections/360000686434)

### Lägg till anpassade enheter i systemet {#add-custom-devices-to-your-system}

Nu kan du lägga till anpassade enheter i systemet, så att användarna kan granska interaktivt innehåll och simulera hur det visas på en viss enhet när de granskar ett korrektur i Desktop Proofing Viewer.

Före den här ändringen kunde användarna bara välja från en lista med förkonfigurerade standardenheter.

Mer information om hur du lägger till anpassade enheter finns i

Information om hur användare kan välja enheter när de granskar interaktivt innehåll finns i [Ändra interaktiv korrekturupplösning i korrekturläsaren](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

## Förbättringar av korrektur i Workfront {#proofing-enhancements-in-workfront}

* [Dela korrekturlänken direkt från Workfront](#share-the-proof-link-directly-from-workfront)
* [Rapport om ytterligare korrekturdata i Workfront](#report-on-additional-proofing-data-in-workfront)
* [Visa historiska data för korrekturgodkännanden i Workfront](#view-historical-data-for-proof-approvals-in-workfront)

### Dela korrekturlänken direkt från Workfront {#share-the-proof-link-directly-from-workfront}

Nu kan du skapa en länk för ett korrektur i Workfront och dela den direkt från Workfront. Du kan också kopiera URL-adressen och distribuera den med en alternativ metod.

Före den här ändringen kunde du bara kopiera korrekturlänken inom Workfront och distribuera den med en alternativ metod.

Mer information finns i [Dela ett korrektur i Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) i artikeln [Dela ett korrektur i Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

>[!NOTE]
>
>Den inbäddningslänk som är tillgänglig för tillfället kommer att tas bort i en framtida version. Inbäddningslänken är fortfarande tillgänglig via Workfront API.

### Rapport om ytterligare korrekturdata i Workfront {#report-on-additional-proofing-data-in-workfront}

I rapporter som innehåller dokumentversionsobjektet (t.ex. en dokumentversionsrapport och en korrekturgodkännanderapport) finns nu flera fält tillgängliga där du kan visa ytterligare korrekturinformation.

* Deadline för korrektur

  Visar veckodag, datum, tid på dagen och år för korrekturdeadline.

* Bekräftelsebeslut

  Visar korrekturens beslutsstatus (väntande, ändringar krävs eller godkänt).

* Korrekturnamn

  Visar korrekturnamnet.

* Korrektur för sidor

  Visar antalet sidor som ingår i korrekturet.

* Bevis förlopp

  Visar förloppsstatus för beviset (Skickat, Öppnat, Kommenterat, Beslutsgjort).

Mer information om dessa fält finns i  [Ordlista för Adobe Workfront-termer](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

### Visa historiska data för korrekturgodkännanden i Workfront {#view-historical-data-for-proof-approvals-in-workfront}

I rapporten Korrektur för godkännande kan du lägga till ett fält där du kan visa korrektur för godkännandebeslut för korrektur som inte längre är aktiva. Du kan göra detta genom att lägga till fältet Godkännarbeslut i din rapport.

Före den här ändringen kunde beslutet inte längre visas i en Workfront-rapport efter att ett beslut fattats om ett bevis.

Mer information finns i  [Ordlista för Adobe Workfront-termer](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Förbättringar av korrektur i Workfront Proof {#proofing-enhancements-in-workfront-proof}

* [Skapa en ny version av ett korrektur direkt från korrekturläsaren (Workfront Proof)](#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof)
* [Länk till ny korrekturinformation i korrekturläsaren och korrekturläsaren för skrivbordet (Workfront Proof)](#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof)

### Skapa en ny version av ett korrektur direkt från korrekturläsaren (Workfront Proof) {#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof}

Du kan nu skapa en ny version av ett korrektur direkt från det nya korrekturläsaren och korrekturläsaren för skrivbordet när du korrekturläser i Workfront Proof.

Tidigare var det här alternativet bara tillgängligt i den äldre Flash Viewer-versionen.

Mer information finns i [Kopiera korrektur i Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md) i artikeln  [Kopiera korrektur i Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md).

### Länk till ny korrekturinformation i korrekturläsaren och korrekturläsaren för skrivbordet (Workfront Proof) {#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof}

När du visar ett korrektur i korrekturläsaren kan Workfront Proof-användare nu snabbt gå till sidan med korrekturinformation i Workfront Proof.

Mer information finns i&quot;Visa korrekturinformation&quot;.

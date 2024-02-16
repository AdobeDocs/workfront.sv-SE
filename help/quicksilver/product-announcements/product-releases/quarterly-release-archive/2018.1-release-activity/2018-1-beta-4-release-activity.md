---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta 4 - versionsaktivitet
description: Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i 2018.1 Beta 4-versionen. Funktionen gjordes tillgänglig i förhandsvisningsmiljön den 24 januari 2018. Den kommer att göras tillgänglig i produktionsmiljön i mars 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 8e016f12-bc72-475c-a8cc-38ded4351f88
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2435'
ht-degree: 0%

---

# 2018.1 Beta 4 - versionsaktivitet

Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i 2018.1 Beta 4-versionen. Funktionen gjordes tillgänglig i förhandsvisningsmiljön den 24 januari 2018. Den kommer att göras tillgänglig i produktionsmiljön i mars 2018.

>[!IMPORTANT]
>
> Funktionerna som beskrivs på den här sidan kan ändras innan de är tillgängliga i produktionsmiljön.

En lista över alla ändringar som gjorts under 2018.1 finns på  [Aktivitetsöversikt för 2018.1-utgåvan](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

Beta 4-versionen från 2018.1 innehåller förbättringar för både Workfront-administratörer och andra användare:

**För administratörer**

* [Scheman som hanteras av gruppadministratörer](#schedules-managed-by-group-administrators)

**För alla användare**

* [Förbättringar av korrektur i Workfront](#proofing-improvements-within-workfront)
* [Korrektur för Workfront-korrektur - Förbättrad användarupplevelse och ytterligare funktioner](#proof-creation-in-workfront-proof-improved-user-experience-and-additional-functionality)
* [Korrekturförbättringar i Workfront och Workfront](#proofing-improvements-within-workfront-and-workfront-proof)
* [Uppdaterat utseende och känsla med integreringen av basecamp i Workfront Proof](#updated-look-and-feel-with-basecamp-integration-in-workfront-proof)
* [Klistra in bilder i Workfront från Urklipp](#paste-images-to-workfront-from-the-clipboard)
* [Förbättringar av användningsrapporten](#utilization-report-improvements)
* [Ta bort resursbudgeterat timobjekt från Workfront](#remove-the-resource-budgeted-hour-object-from-workfront)
* [Rapportanvändningsstatistik](#report-usage-statistics)
* [Gantt-schemauppdateringar](#gantt-chart-updates)
* [Optimering för nya Portfolio](#new-portfolio-optimizer)
* [Alternativ för justering av budgetdatum i resursplaneraren](#budget-date-adjustment-option-in-the-resource-planner)
* [Resursplanering: Begränsa tilldelningar till användare baserat på gruppmedlemskap](#resource-scheduling-restrict-assignments-to-users-based-on-group-membership)
* [Resursschemaläggning: Tillåt tilldelningar till användare oavsett roll](#resource-scheduling-allow-assignments-to-users-regardless-of-role)
* [Stöd för Emoji](#emoji-support)

## Förbättringar av korrektur i Workfront {#proofing-improvements-within-workfront}

Följande förbättringar har gjorts runt dokumentlistan i Workfront: 

* [Visa korrekturstatus från dokumentlistan](#view-proof-progress-from-the-document-list)
* [Nytt alternativ för att visa utskriftssammanfattningen från dokumentlistan](#new-option-to-view-the-print-summary-from-the-document-list)
* [Uppdaterad Look och känsla för att generera eller öppna korrektur från dokumentlistan](#updated-look-and-feel-for-generating-or-opening-the-proof-from-the-document-list)
* [Olika länkar borttagna från dokument i dokumentlistan](#various-links-removed-from-documents-on-the-document-list)
* [Visa filnamn på kombinerade korrektur](#view-file-names-on-combined-proofs)
* [Visa det aktuella aktiva steget i ett korrektur från dokumentlistan](#view-the-current-active-stage-of-a-proof-from-the-document-list)

### Visa korrekturstatus från dokumentlistan {#view-proof-progress-from-the-document-list}

Nu visas korrekturförloppsindikatorer för alla korrektur när du visar dokumentlistan. (Detta omfattar Skickat, Öppnat, Kommentarer gjorda och Beslut.)

Före den här ändringen var du tvungen att välja ett korrektur i dokumentlistan för att visa korrekturförloppet i den högra panelen. 

Mer information finns i [Översikt över korrektur och status](../../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md).

### Nytt alternativ för att visa utskriftssammanfattningen från dokumentlistan {#new-option-to-view-the-print-summary-from-the-document-list}

Nu kan du visa utskriftssammanfattningen för ett korrektur direkt från dokumentlistan.

Före den här ändringen kunde du bara visa utskriftssammanfattningen från korrekturläsaren. 

Mer information om hur du visar utskriftssammanfattningen från dokumentlistan finns i [Skriva ut en korrektursammanfattning i Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md).

### Uppdaterad Look och känsla för att generera eller öppna korrektur från dokumentlistan {#updated-look-and-feel-for-generating-or-opening-the-proof-from-the-document-list}

När du för muspekaren över ett dokument i dokumentlistan har nu alternativen för att generera korrekturet eller öppna korrekturet uppdaterats. Dessa alternativ är nu mer framträdande och visas som knappar.

Före den här ändringen var alternativen tillgängliga som länkar under dokumentnamnet.

Mer information finns i följande avsnitt:

* .
* in .

### Olika länkar borttagna från dokument i dokumentlistan {#various-links-removed-from-documents-on-the-document-list}

Följande åtgärder är inte längre tillgängliga som länkar för enskilda dokument i dokumentlistan:

* Generera korrektur
* Korrektur
* Information
* Dela
* Checka ut/Checka in

Följande åtgärder är nu tillgängliga som en knapp i dokumentet i dokumentlistan:

* Öppna korrektur (tillgängligt när korrekturet har skapats) 
* Generera korrektur (tillgängligt när korrekturet ännu inte har genererats)

Följande åtgärder är nu tillgängliga i listrutan bredvid knappen Öppna korrektur eller Generera korrektur:

* Korrekturinformation
* Dokumentinformation
* Skriv ut sammanfattning

Mer information finns i följande avsnitt:

* .
* in .

### Visa filnamn på kombinerade korrektur {#view-file-names-on-combined-proofs}

Nu kan du visa de enskilda filnamnen som utgör ett kombinerat korrektur. Den här informationen visas på fliken Detaljer när korrekturet är markerat i dokumentlistan.

Mer information finns i Visa alla filer i ett kombinerat korrektur. 

### Visa det aktuella aktiva steget i ett korrektur från dokumentlistan {#view-the-current-active-stage-of-a-proof-from-the-document-list}

När du väljer ett korrektur i dokumentlistan visas de aktuella aktiva stegen i den högra kolumnen på fliken Information. 

Mer information finns i [Visa aktiva faser i ett korrektur](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/view-active-stages-proof.md).  

## Korrektur för Workfront-korrektur - Förbättrad användarupplevelse och ytterligare funktioner {#proof-creation-in-workfront-proof-improved-user-experience-and-additional-functionality}

Förutom en förbättrad användarupplevelse när du skapar korrektur i Workfront Proof finns nu följande extrafunktioner:

* Sammanfoga flera bilder till ett enda korrektur.
* Korrektur för webbplatser i flera upplösningar (flera upplösningar kan skapas som enskilda korrektur eller kombineras till ett enda korrektur).
* Redigera filnamnet under överföringsprocessen.
* Inkludera anpassade fält i formuläret för att skapa korrektur.
* Lägg till ett anpassat meddelande till korrekturmeddelanden via e-post.
* Ytterligare korrekturinställningar 
* Validering av fel i realtid vid korrektur av en URL (tidigare behövde du vänta flera minuter innan ett fel visades)

>[!NOTE]
>
>Den nya korrektursidan i Workfront Proof matchar nu korrektursidan som nyligen blev tillgänglig när du skapade korrektur i Workfront. 

Mer information finns i  [Skapa korrektur i Workfront-korrektur](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Korrekturförbättringar i Workfront och Workfront {#proofing-improvements-within-workfront-and-workfront-proof}

Följande ändringar gäller när du lägger till dokument i Workfront och i Workfront Proof:

* [Ändra storlek på kommentarlistan vid granskning av korrektur](#resize-the-comment-list-when-reviewing-proofs)
* [Hyperlänkar är aktiva vid granskning av statiska korrektur](#hyperlinks-are-active-when-reviewing-static-proofs)
* [Förbättringar när korrektur läggs till](#improvements-when-adding-proofs)

### Ändra storlek på kommentarlistan vid granskning av korrektur {#resize-the-comment-list-when-reviewing-proofs}

Nu kan du ändra storlek på kommentarlistan när du granskar korrektur i korrekturläsaren.

Mer information finns i .

### Hyperlänkar är aktiva vid granskning av statiska korrektur {#hyperlinks-are-active-when-reviewing-static-proofs}

Hyperlänkar är nu aktiva när du granskar ett statiskt korrektur i korrekturläsaren. Klicka på en hyperlänk för att gå till den länkade sidan.

Den här funktionen stöds i alla filtyper som innehåller text, t.ex. PDF, DOC och så vidare. Bildfiler stöds inte.

### Förbättringar när korrektur läggs till {#improvements-when-adding-proofs}

Följande förbättringar är tillgängliga när du lägger till dokument som ska korrektur. 

* Informationen i mottagarlistan är nu tillgänglig i en vy med tre kolumner, vilket gör informationen enklare att visa och ändra. 

  Tidigare visades informationen i en vy med en kolumn, vilket krävde fler klick när ändringar behövdes. 

  Mer information finns i .

* Dra en eller flera mottagare från en arbetsflödesfas till en annan när du använder Automatiserat arbetsflöde. Du kan dra direkt till en scen eller dra till en scen i diagrammet, som finns högst upp på sidan.

  Mer information finns i .

* Arbetsflödesdiagrammet förblir synligt längst upp på sidan även när du bläddrar. Diagrammet är komprimerat som standard. Expandera diagrammet om du vill visa hela diagrammet.

  Mer information finns i .

* När du lägger till en mall i ett automatiserat arbetsflöde i ett korrektur visas en inläsande animering som anger att mallen läses in.

  Mer information finns i .

* Följande inställningar har flyttats från avsnittet Korrekturinställningar till avsnittet Arbetsflöde på sidan Nytt korrektur:

   * Primär beslutsfattare
   * Kräv endast ett beslut

## Uppdaterat utseende och känsla med integreringen av basecamp i Workfront Proof {#updated-look-and-feel-with-basecamp-integration-in-workfront-proof}

Utseendet och känslan i integreringen av Basecamp med Workfront Proof har uppdaterats. Funktionaliteten är densamma.

## Klistra in bilder i Workfront från Urklipp {#paste-images-to-workfront-from-the-clipboard}

Nu kan du lägga till bildfiler i Workfront genom att klistra in en bild från systemets Urklipp.

Möjligheten att klistra in från Urklipp togs bort från Workfront i en tidigare version. Den återinförs nu i den här versionen. Den nya metoden är effektivare och mer intuitiv.

Mer information finns i [Klistra in bilder från Urklipp](../../../../documents/managing-documents/paste-image-clipboard.md). 

## Förbättringar av användningsrapporten {#utilization-report-improvements}

Användningsrapporten innehåller följande förbättringar:

* Visa intäkter i användningsrapporten för ett projekt

  Gör att du kan visa Budgeterad intäkt, Planerad intäkt, Faktisk intäkt, Budgeterad avvikelse och Planerad avvikelse.

* Jämför intäkter med planerade och faktiska kostnader

  Här kan du visa planerad eller faktisk kostnad tillsammans med planerad intäkt. Marginalen (%) visas också (marginalen beräknas som Intäkter - Kostnad / Intäkter).

* Intäkter visas när du visar diagrammet.
* Sidhuvuden förblir synliga vid rullning.

  När du bläddrar igenom informationen i användningsrapporten visas alltid rubriken längst upp i användningsrapporten, vilket gör att du lättare kan förstå informationen i rapporten.

  Tidigare var rubriken högst upp i användningsrapporten inte synlig när användaren bläddrar.

* Användningsrapport för ett enskilt projekt läses in automatiskt

  När du visar användningsrapporten för ett projekt läses rapporten in automatiskt.

  Innan den här ändringen utfördes var du tvungen att klicka på Kör innan rapporten kördes.

* Förbättrade prestanda

Mer information om användningsrapporten finns i [Översikt över resursanvändningsrapporten](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Ta bort resursbudgeterat timobjekt från Workfront {#remove-the-resource-budgeted-hour-object-from-workfront}

För att åtgärda prestandaproblem har fältet Resursbudgeterad timme tillfälligt tagits bort från Workfront.

Resursbudgeterade timmar är de timmar som du budgeterar för dina resurser eller dina projekt i resursplaneraren. Du kan för närvarande inte längre rapportera om det här fältet i webbprogrammet eller via API:t. Fältet återställs i en framtida version när prestandaproblemen har lösts.

Mer information om budgeteringstimmar i Resursplanering finns i [Översikt över resursplanering](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md). 

## Rapportanvändningsstatistik {#report-usage-statistics}

Nu kan du visa följande användningsinformation för dina Workfront-rapporter i en lista över rapporter:

* Senast visad av
* Senaste visningsdatum
* De senaste 10 visningsprogrammen
* Vyer denna månad/kvartal/år
* Vyer förra månaden/kvartal/år
* Alla vyer

Före den här uppdateringen var du begränsad till vilken användningsinformation du kunde se på dina rapporter.

Mer information om rapportanvändning finns i [Visa rapportanvändning](../../../../reports-and-dashboards/reports/report-usage/view-report-usage.md)

## Scheman som hanteras av gruppadministratörer {#schedules-managed-by-group-administrators}

Som gruppadministratör kan du skapa och redigera scheman som är kopplade till de grupper som du administrerar samt deras undergrupper. Före den här ändringen kunde endast Workfront-administratörer skapa och redigera scheman.

Mer information om hur du hanterar scheman finns i [Skapa ett schema](../../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

## Gantt-schemauppdateringar {#gantt-chart-updates}

Gantt-schemat kan nu redigeras. Med Gantt-schemat kan du göra följande uppdateringar för dina uppgifter:

* Skapa tidigare relationer
* Redigera aktivitetens varaktighet
* Uppdatera aktivitetsprocenten slutförd
* Använd resursutjämning

Före den här ändringen kunde du bara ta bort tidigare relationer i Gantt-diagrammet och du kan bara redigera uppgifter i uppgiftslistan.

Mer information om Gantt-schemat finns i [Uppdatera information i Gantt-schema för uppgiftslista](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md)

## Optimering för nya Portfolio {#new-portfolio-optimizer}

Området Portfolio Optimizer i Workfront har nu uppdaterats med ett nytt utseende och en ny känsla. Funktionen har inte ändrats.

Mer information om Portfolio Optimizer finns i [Portfolio Optimizer - översikt](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)

## Alternativ för justering av budgetdatum i resursplaneraren {#budget-date-adjustment-option-in-the-resource-planner}

Vi har lagt till ett alternativ som ger dig snabb insyn i tidsramar utan budgeteringskonflikter. När du har visat när tidsramarna utan budgeteringskonflikter inträffar kan du flytta dina budgeterade timmar manuellt till dessa tider. Detta kommer även att justera timernas budgeterade datum. Före den här uppdateringen var det inte möjligt att visa budgeteringskonflikter för ett projekt i en överblick.

Mer information om hur du justerar budgeterade datum i resursplaneraren finns i avsnittet Justera budgetdatum i [Översikt över resursplanering](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)

## Resursplanering: Begränsa tilldelningar till användare baserat på gruppmedlemskap {#resource-scheduling-restrict-assignments-to-users-based-on-group-membership}

>[!NOTE]
>
>Verktygen för resursschemaläggning har tagits bort från Workfront i version 23.1. Mer information om att schemalägga resurser med hjälp av belastningsutjämnaren finns i [Översikt över belastningsutjämnaren](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

När du gör användartilldelningar i schemaläggningsområdet (enligt beskrivningen i Tilldela ej tilldelade uppgifter och utgåvor manuellt i schemaläggningsområdena) kan du nu konfigurera Workfront så att tilldelningar av aktiviteter och utgåvor begränsas endast till de användare som är medlemmar i den grupp som är definierad i det projekt där aktiviteten eller utgåvan har sitt ursprung. 

Detta gäller för tilldelningar på följande sätt:

* När du tilldelar en användare till alla uppgifter och ärenden för en viss roll, enligt beskrivningen i Tilldela ej tilldelade uppgifter och ärenden manuellt i schemaläggningsområdena.

  Före den här ändringen kan en uppgift eller ett problem alltid tilldelas till vilken användare som helst, oavsett användarens gruppmedlemskap. 

* När du byter tilldelningar med en annan användare, vilket beskrivs i Tilldela ej tilldelade uppgifter och utgåvor manuellt i schemaläggningsområdena.

  Före den här ändringen kan en uppgift eller ett problem alltid tilldelas till vilken användare som helst, oavsett användarens gruppmedlemskap. 

* När du tilldelar en aktivitet eller ett problem manuellt från tidslinjen för schemaläggning, enligt beskrivningen i Tilldela ej tilldelade uppgifter och ärenden manuellt i schemaläggningsområdena.

  Före den här ändringen kan en uppgift eller ett problem alltid tilldelas till vilken användare som helst, oavsett användarens gruppmedlemskap. 

* När du tillåter att Workfront automatiskt tilldelar användare, enligt beskrivningen i Tilldela ej tilldelade uppgifter och ärenden manuellt i schemaläggningsområdena.

  Före den här ändringen skulle Workfront tilldela användare uppgifter och utgåvor oavsett gruppmedlemskap.

Mer information om hur du konfigurerar det här alternativet finns i&quot;Kom igång med resursschemaläggning&quot;.

## Resursschemaläggning: Tillåt tilldelningar till användare oavsett roll {#resource-scheduling-allow-assignments-to-users-regardless-of-role}

När du gör användartilldelningar i området Schemaläggning (enligt beskrivningen i Tilldela ej tilldelade uppgifter och utgåvor manuellt i schemaläggningsområdena), kan du nu konfigurera Workfront så att aktiviteter och utgåvor kan tilldelas alla användare, oavsett om användaren har en roll definierad i användarprofilen som matchar rolltilldelningen för den uppgift eller det problem som tilldelas dem.

Detta gäller för tilldelningar på följande sätt:

* När du tilldelar en användare till alla aktiviteter och utgåvor för en viss roll, enligt beskrivningen i Tilldela ej tilldelade uppgifter och utgåvor manuellt i schemaläggningsområdena i Tilldela ej tilldelade uppgifter och utgåvor manuellt i schemaläggningsområdena.

  Före den här ändringen måste den primära rollen för användaren som du tilldelar matcha rollen som redan definierats i fältet Välj roll.

* När du byter tilldelningar med en annan användare, vilket beskrivs i Tilldela ej tilldelade uppgifter och utgåvor manuellt i schemaläggningsområdena.

  Före den här ändringen måste den primära rollen för användaren som du tilldelar matcha rollen som redan definierats i fältet Välj roll.

* När du tilldelar en aktivitet eller ett problem manuellt från tidslinjen för schemaläggning, enligt beskrivningen i Tilldela ej tilldelade uppgifter och ärenden manuellt i schemaläggningsområdena.

  Före den här ändringen visades endast användare vars roll matchade rollen för den uppgift eller det problem som du tilldelade på tidslinjen för schemaläggningen.

>[!NOTE]
>
>Detta gäller inte när Workfront automatiskt tilldelar användare, vilket beskrivs i Tilldela ej tilldelade uppgifter och ärenden manuellt i schemaläggningsområdena. När användare tilldelas automatiskt kan uppgifter och utgåvor endast tilldelas användare med en matchande roll.

Mer information om hur du konfigurerar det här alternativet finns i&quot;Kom igång med resursschemaläggning&quot;.

## Stöd för Emoji {#emoji-support}

Nu kan du ange tonen för kommentarer och uppdateringar som du gör i Workfront genom att infoga känslolägesikoner. Alla meddelanden som läggs till i kommentarer som görs på fliken Uppdateringar visas också i uppdateringens e-postmeddelande. 

Mer information finns i [Uppdatera arbete](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Preview 3
description: Den här sidan beskriver alla ändringar som är tillgängliga i förhandsvisningsmiljön i R1.3-versionen. Funktionerna på den här sidan gjordes tillgängliga i förhandsvisningsmiljön den 1 februari 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d1502a17-b131-4d29-9b0c-03ad44be4ba6
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1347'
ht-degree: 0%

---

# R1 Preview 3

Den här sidan beskriver alla ändringar som är tillgängliga i förhandsvisningsmiljön i R1.3-versionen. Funktionerna på den här sidan gjordes tillgängliga i förhandsvisningsmiljön den 1 februari 2017.

En lista över alla ändringar som gjorts i R1 finns i [Aktivitetsöversikt för R1-utgåvan](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## Förbättrad metod för länkning av externa filer

Alternativet för att länka dokument från en extern källa (som Google Drive, Box, Dropbox och så vidare) finns nu på en mer framträdande plats i dokumentområdet. 

Dessutom är det nu mer intuitivt att auktorisera en dokumentleverantör innan den länkar filer från den leverantören för första gången (det är helt enkelt ett extra steg när du länkar filer från en extern leverantör).

Före dessa ändringar fanns alternativet att länka filer från en extern källa i dialogrutan Lägg till dokument i området Dokument. Innan ett dokument länkas från en extern källa för första gången måste användaren som länkar dokumentet auktorisera dokumentprovidern under Konfigurera.

Mer information finns i  [Länka dokument från externa program](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Uppdaterat team som arbetar med kalender

>[!NOTE]
>
>Verktygen för resursschemaläggning har tagits bort från Workfront i version 23.1. Mer information om att schemalägga resurser med hjälp av belastningsutjämnaren finns i [Översikt över belastningsutjämnaren](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Arbetskalendern som är tillgänglig för team innehåller nu ytterligare funktioner och en uppdaterad stil och känsla. Teamet som arbetar med kalendern fungerar nu på ungefär samma sätt som verktyget för resursplanering för projekt.

Det uppdaterade teamet som arbetar med kalendern innehåller följande förbättringar:

* Visa användare i bokstavsordning eller grupperade efter roll.
* Filtrera tidslinjen för schemaläggning efter projektprioriteringar, status och enskilda projekt. Du kan även filtrera tidslinjen för schemaläggning efter roller och användare. (Filterområdet innehåller färre alternativ än när resurser för projekt schemaläggs.)
* Inkludera ärenden på tidslinjen för tidsplanering.
* Visa användartilldelningar och ändra antalet timmar som användare tilldelas till vissa uppgifter och utgåvor för varje dag.
* Visa indikatorer som visar när användare är överallokerade en viss dag.
* Konfigurera om slutfört arbete ska visas på tidslinjen för schemaläggningen.

Skillnader från verktyget för resursplanering när resurser schemaläggs för projekt:

* Alla teammedlemmar visas i teamet som arbetar i kalendern.\
  När du schemalägger resurser för projekt visas endast användare som har en associerad roll som matchar en roll för en eller flera uppgifter i området Ej tilldelade.
* Växlingsverktyget är inte tillgängligt och ingår inte i teamet som arbetar med kalendern.
* Alla teammedlemmar kan göra ändringar i teamet som arbetar i kalendern.\
  När resurser schemaläggs för projekt kan bara resurshanterare fatta resursbeslut för projektet.
* Problem visas som standard i teamet som arbetar i kalendern.\
  När resurser för projekt schemaläggs visas inte ärenden som standard.

Mer information om hur du använder det uppdaterade teamet Arbeta med kalender finns i &quot;Resursschemaläggning&quot;.

## Förbättringar av resursplanering

Tidslinjen för schemaläggning innehåller följande förbättringar:

* &quot;Använd filtret för att styra vilka användare som visas på tidslinjen i schemat&quot;
* &quot;Användare finns kvar på tidslinjen efter att de tilldelats en uppgift&quot;

### Använd filtret för att styra vilka användare som ska visas på tidslinjen för schemaläggning {#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline}

>[!NOTE]
>
>Verktygen för resursschemaläggning har tagits bort från Workfront i version 23.1. Mer information om att schemalägga resurser med hjälp av belastningsutjämnaren finns i [Översikt över belastningsutjämnaren](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Filtret kan nu användas för att styra vilka användare som visas på tidslinjen för schemaläggning, utöver vilka uppgifter och ärenden som visas i området Ej tilldelade. När användare är markerade i filtret visas bara de användare som du väljer, oavsett om de har en rolltilldelning som matchar rolltilldelningen för uppgifter i området Ej tilldelade. Alla uppgifter som för närvarande är tilldelade den användaren visas också.

Före den här ändringen kontrollerade filtret bara vilka uppgifter och problem som visades i området Ej tilldelade. Användare visades på tidslinjen för schemaläggning endast om användaren matchade rolltilldelningen för en uppgift i området Ej tilldelad.

Mer information om hur du använder filtret för att styra vad som visas på tidslinjen finns i Filtrera information i området Schemaläggning och Tilldela ej tilldelade uppgifter och ärenden manuellt i områdena Schemaläggning.

### Användare finns kvar på tidslinjen efter att de tilldelats en uppgift {#users-remain-on-the-timeline-after-being-assigned-a-task}

Användarna finns kvar på tidslinjen när de har tilldelats en uppgift eller ett ärende, även om det inte finns några återstående uppgifter eller problem som har en matchande rolltilldelning. På så sätt kan du göra nödvändiga ändringar efter att användarna har tilldelats.

Före den här ändringen försvinner användare från tidslinjen för schemaläggning omedelbart efter att de har tilldelats en uppgift eller ett problem om det inte finns några återstående uppgifter eller utleveranser i området Ej tilldelade med en matchande rolltilldelning.

Mer information finns i &quot;Tilldela ej tilldelade uppgifter och ärenden manuellt i schemaläggningsområden&quot;.

## Anpassa Workfront Terminologi genom att ändra objektnamn

Nu kan du anpassa Workfront-terminologi genom att ändra namnen på vissa objekt.\
Med en layoutmall kan du nu ändra namnen på följande arbetsobjekt så att de passar organisationens behov:

* Portfolio
* Program
* Projekt
* Uppgift
* Problem

Om du till exempel arbetar med kampanjer i stället för med projekt i din organisation kan du ersätta namnet på objektet&quot;Projekt&quot; med&quot;Campaign&quot;.

När du gör den här ersättningen visas objektens uppdaterade namn i följande områden i programmet:

* Globalt navigeringsfält
* Alla flikar
* Alla menyer 
* Report builder och rapportelement (vyer, filter och grupperingar)
* Spara knappar
* Exporterade filer
* E-post

I följande områden visas inte objektens uppdaterade namn:

* Resursuppskattningar
* Resursbudgethanteraren
* Kapacitetsplanering
* Resursrutnät
* Team Builder
* Portfolio Optimizer 
* Mobilappar
* Outlook-tillägg

Mer information om hur du anpassar Workfront-terminologin med hjälp av en layoutmall finns i avsnittet&quot;Anpassa terminologi&quot; i&quot;Skapa och hantera layoutmallar&quot; och&quot;Förstå effekterna av att anpassa objektnamn&quot; i [Förstå objekt i Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Inkludera start- och slutdatum för godkännande i rapporter

Du kan nu inkludera följande fält när du skapar eller ändrar rapporter:

* Startdatum för godkännandesökväg
* Slutförandedatum för godkännandesökväg

Med dessa fält kan du få information om när den aktuella eller senaste godkännandesökvägen startades och när den markerades som fullständig.

Mer information om dessa fält finns i [Ordlista för Adobe Workfront-terminologi](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

Mer information om godkännandesökvägar, hur de skapas och aktiveras samt vilken funktion de har i godkännandeprocesser finns i [Skapa en godkännandeprocess för arbetsobjekt](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Följande fält har tagits bort från Workfront och kan inte längre inkluderas i rapporter (dessa fält innehåller information om projektet i stället för information om själva godkännandena och har ofta missbrukats):

* Startdatum för planerade godkännanden
* Planerat startdatum för godkännande
* Beräknat startdatum för godkännande

## Nya alternativ för e-postsammandrag av&quot;förfrågningar jag gjort&quot;

Leveransalternativet Daglig sammandrag har lagts till under Begäranden som jag har gjort i meddelandeinställningarna.

Mer information finns i [Ändra dina egna e-postmeddelanden](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Kom ihåg att uppdatera e-postadressen som är kopplad till ditt konto för att kunna testa den här funktionen. Detta är obligatoriskt eftersom förhandsvisningssandlådan rensar e-postadresserna för alla användare.

## Uppdaterat utseende och känsla för e-postmeddelanden om godkännande av dokument

Utseendet på och känslan av meddelandet för&quot;Dokumentgodkännande&quot; har uppdaterats med ett nytt användargränssnitt:

Mer information om e-postmeddelanden finns i [Adobe Workfront-meddelanden](../../../../workfront-basics/using-notifications/wf-notifications.md).

Kom ihåg att uppdatera e-postadressen som är kopplad till ditt konto för att kunna testa den här funktionen. Detta är obligatoriskt eftersom förhandsvisningssandlådan rensar e-postadresserna för alla användare.

## Förbättringar i milstolpevyn

Vyn Milstolpe som är tillgänglig när du visar en projektlista eller en projektrapport innehåller nu följande förbättringar:

* Planerade datum kan redigeras
* Procent färdigt för projekt och uppgifter visas

Innan den här ändringen utfördes var du tvungen att gå till den enskilda uppgiften för att kunna redigera datum eller visa procent färdigt.

Mer information finns i [Använd vyn Milstolpe](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

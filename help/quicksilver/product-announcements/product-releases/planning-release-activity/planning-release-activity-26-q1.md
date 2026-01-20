---
content-type: release-notes
title: Första utgåvan av kvartal 2026 för Adobe Workfront Planning
description: Detta är lanseringsaktiviteten för Adobe Workfront Planning-produkten för första kvartalet 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: d60123df6e18025a886809fa390137bdf9287e6e
workflow-type: tm+mt
source-wordcount: '2014'
ht-degree: 0%

---

# Första utgåvan av kvartal 2026 för Adobe Workfront Planning

I den här artikeln beskrivs funktionerna som lanseras för Workfront Planning i den första utgåvan av kvartal 2026.

<!--keep the sentence below for all future quarterly release pages-->

En lista över alla funktioner som släppts för Adobe Workfront Planning finns i [Versionsaktivitet för Adobe Workfront Planning: artikelindex](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).


## Globala posttyper kan delas från den sekundära arbetsytan

>[!NOTE]
>
>Förhandsgranska: 15 januari 2026
>Production fast release: 15 januari 2026
>Produktion för alla: 15 januari 2026
>[!BADGE Frånschemat &#x200B;]{type=Neutral}

Nu kan du dela globala posttyper som du har lagt till på en sekundär arbetsyta från den arbetsytan. Användarna får också samma behörigheter till alla poster på den sekundära arbetsytan som du delar.

>[!NOTE]
>
>Användare kan ha olika behörigheter för samma globala posttyp på den primära arbetsytan eller på andra sekundära arbetsytor där posttypen lades till. Workspace och posttypsbehörigheter överförs till posterna.

Före den här ändringen kan du bara dela den globala posttypen från den ursprungliga primära arbetsytan.

Mer information finns i [Posttypöversikt för arbetsytan över &#x200B;](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).


## Poster som lagts till i en global posttyp på en sekundär arbetsyta visas inte från andra sekundära arbetsytor

>[!NOTE]
>
>Förhandsgranska: 15 januari 2026
>Production fast release: 15 januari 2026
>Produktion för alla: 15 januari 2026
>[!BADGE Frånschemat &#x200B;]{type=Neutral}

Poster som läggs till i en global posttyp på en sekundär arbetsyta visas bara från den arbetsytan eller från posttypens ursprungliga primära arbetsyta. Före den här uppdateringen var poster som lagts till på en sekundär arbetsyta också synliga från andra sekundära arbetsytor där du kanske har behörighet att visa.

Mer information finns i [Posttypöversikt för arbetsytan över &#x200B;](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).

## Skapa posttypshierarkier i arbetsytor

>[!NOTE]
>
>Förhandsgranska: 23 december 2025
>Production fast release: 14 januari 2026
>Produktion för alla: 15 januari 2026

Du kan nu definiera flexibla men strukturerade hierarkier mellan post- och objekttyper.

Hierarkier är anslutningar mellan posttyper. Du kan ha upp till fyra post- och objekttyper anslutna i en hierarki, och du kan ha upp till fem hierarkier i en arbetsyta. Den första posttypen i hierarkin är den första överordnade posten.

Du kan använda hierarkier för att organisera arbetet och för att visualisera hur strategin leder till körning.

Tänk på följande när du skapar hierarkier:

* Du kan bara ansluta Planning-posttyper från en arbetsyta och Workfront-projekt i en hierarki.
* En posttyp eller ett projekt kan bara ha en överordnad i samma arbetsyta.
* En posttyp kan vara överordnad i flera hierarkier.
* Kopplingsbara posttyper kan inte användas i hierarkier i andra arbetsytor än sina egna.
* Globala posttyper kan bara användas i hierarkier i arbetsytor som de skapades i eller har lagts till i.

Mer information finns i [Översikt över hierarki och vägbeskrivningar](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

## Nya enhetliga vägbeskrivningar har lagts till på posternas sidor

>[!NOTE]
>
>Förhandsgranska: 23 december 2025
>Production fast release: 14 januari 2026
>Produktion för alla: 15 januari 2026

När du skapar hierarkier mellan posttyper genereras vägbeskrivningar för poster som tillhör de posttyperna.

Registrera vägbeskrivningar återspeglar deras plats i en hierarki. När du har skapat hierarkier kan du se en posts synliga spreadcrumb högst upp på sidan, vilket anger vilka andra överordnade eller underordnade objekt som är kopplade till den. Hierarkierna är desamma i Workfront och Planning.

Du kan till exempel visa ett projekts planeringshierarki när det är anslutet till posttyperna Planering i dess planeringsspåret och dess Workfront-hierarki när det är anslutet till Workfront-objekttyper, som portföljer eller Program, i Workfront.

Mer information finns i [Översikt över hierarki och vägbeskrivningar](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).


## Förbättringar av anslutna postsidor

>[!NOTE]
>
>Förhandsgranska: 19 december 2025
>Snabb produktion: 14 januari 2026
>Produktion för alla: 15 januari 2026

För att du ska få större flexibilitet när du arbetar med sammankopplade arkivsidor har vi förbättrat vyfunktionerna i det här området av Workfront Planning. Följande är förbättringar på sidorna för kopplade poster i en post:

* Nu kan du lägga till en tidslinje och en kalendervy på postens sida med kopplade poster.
* Nu kan du dela alla vyer från en ansluten postsida. De vyer som delas från dessa sidor är synliga i hela systemet av alla användare som du delar dem med i andra områden av Workfront Planning. Alla vyer som delas inom andra områden av Planning visas också på sidan för anslutna poster för samma användare som de delas med.
* Vi har lagt till en begränsning som endast tillåter en ansluten postsida per post eller objekttyp. Före den här förbättringen kan du lägga till flera sidor för samma post eller objekttyp. Nu kan du använda flera vyer för samma posttyp på en och samma postsida.
* Vi har lagt till en **ny rad**-länk längst ned i en tabellvy och en **Anslut poster**-knapp i den övre högra delen av sidan med anslutna poster. Före den här förbättringen fanns länken **Ny rad** och knappen **Anslut poster** bara på en projektansluten sida.

Mer information finns i [Lägga till en kopplad postsida i en post](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

## Dela vyer på sidan Projekt - kopplade poster

>[!NOTE]
>
>Förhandsgranska: 18 december 2025
>Production fast release: 14 januari 2026\
>Produktion för alla: 15 januari 2026

För att göra det enklare att se den information du behöver har vi lagt till möjligheten att dela vyer på sidan Projects Connected records. Nu kan du dela vyer med andra användare, team eller grupper.

Mer information finns i [Lägga till en kopplad postsida i en post](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

## Aktuellt jokertecken för användare är nu tillgängligt i projektanslutningsvisningsfilter

>[!NOTE]
>
>Förhandsgranska: 18 december 2025
>Production fast release: 14 januari 2026\
>Produktion för alla: 15 januari 2026

För att göra det enklare att filtrera efter projektanslutningar som gäller dig har vi skapat ett jokertecken för den aktuella användaren. När du filtrerar kan du nu välja &quot;Jag (inloggad användare)&quot;. Filtret gäller sedan den användare som visar listan med förfrågningar.

Det här kan vara praktiskt när du lägger till ett filter i en vy som flera användare kommer att använda. Varje användare ser filterresultat som gäller dem.

Jokertecknet är tillgängligt i fält där värdet är en användare.

Mer information om hur du konfigurerar projektanslutningsvyer, inklusive filter, finns i [Lägga till en ansluten postsida till en post](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).


## Förbättringar av Workspace huvudsida

>[!IMPORTANT]
>
>Detta har tillfälligt tagits bort från förhandsgransknings- och produktionsmiljöerna.

>[!NOTE]
>
>Förhandsgranska: 18 december 2025
>Snabb produktion: 14 januari 2026
>Produktion för alla: 15 januari 2026

Följande förbättringar har gjorts på startsidan för Workspaces i Workfront Planning:

* En snabbare och mer dynamisk rullningsupplevelse. Detta syns särskilt om organisationen har ett stort antal arbetsytor och för systemadministratörer.

* Vi har lagt till en sökruta där du nu kan söka efter en specifik arbetsyta efter namn.

* Fliken **Andra arbetsytor** har bytt namn till **Alla arbetsytor** och innehåller alla arbetsytor som du har minst behörighet att visa, inklusive de som du har skapat.

Mer information finns i [Redigera arbetsytor](/help/quicksilver/planning/architecture/edit-workspaces.md).


## Lägga till fältet för varumärkesanslutning till Produkter och profiler som standard på arbetsytan i GenStudio

>[!NOTE]
>
>Förhandsgranska: 11 december 2025
>Production fast release: 11 december 2025
>Produktion för alla: 11 december 2025
>[!BADGE Frånschemat &#x200B;]{type=Neutral}

Anslutningsfältet med GenStudio for Performance Marketing Brand läggs nu till som standard för posttyperna Produkter och Personas på arbetsytan GenStudio i Workfront Planning.

Organisationen måste ha både Workfront Planning och Adobe GenStudio for Performance Marketing.

Före den här förbättringen kunde du bara lägga till anslutningsfältet Varumärke manuellt till valfri posttyp, inklusive Produkter och Personas. Du kan fortfarande manuellt koppla posttypen Brand GenStudio till andra posttyper i Workfront Planning.

Mer information finns i [Kom igång med integreringen mellan Adobe Workfront Planning och Adobe GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).

## Begränsa borttagning av GenStudio for Performance Marketing-användares behörigheter från Planning

>[!NOTE]
>
>Förhandsgranska: 11 december 2025
>Production fast release: 11 december 2025
>Produktion för alla: 11 december 2025
>[!BADGE Frånschemat &#x200B;]{type=Neutral}

Vi har lagt till ett skyddsutkast som förhindrar dig från att ta bort behörigheter för GenStudio for Performance Marketing-användare från Workfront Planning-objekt. Med den här förbättringen kan du inte längre ta bort GenStudio-användare från GenStudio-arbetsytan i Planning, och du kan inte heller inaktivera ärvda behörigheter för posttyper i GenStudio-arbetsytan om dessa behörigheter omfattar GenStudio-användare. När du tog bort de här användarna från GenStudio-arbetsytan i Planning före den här förbättringen förlorar de även behörigheter för posttyper i GenStudio.

Organisationen måste ha både Workfront Planning och Adobe GenStudio for Performance Marketing.

Mer information finns i [Kom igång med integreringen mellan Adobe Workfront Planning och Adobe GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).


## Offentlig delning av vyer på en global posttyp på en sekundär arbetsyta har tagits bort


>[!NOTE]
>
>Förhandsgranska: 3 december 2025
>Production fast release: 4 december 2025
>Produktion för alla: 15 januari 2026


Fliken Offentlig delning har tagits bort vid delning av en vy för en global post på en sekundär arbetsyta. Du kan inte dela en vy offentligt från en global posttyp som lagts till på en annan arbetsyta från en befintlig global posttyp. Du kan dela en global posttypvy offentligt från den ursprungliga arbetsytan.

Mer information finns i [Dela vyer](/help/quicksilver/planning/access/share-views.md).


## Koppla samman GenStudio for Performance Marketing-varumärken med posttyperna Workfront Planning

>[!NOTE]
>
>Förhandsgranska: 13 november 2025
>Production fast release: 13 november 2025
>Produktion för alla: 13 november 2025

Nu kan du koppla posttyper för Workfront Planning till varumärken från Adobe GenStudio for Performance Marketing. Organisationen måste ha både Workfront Planning och Adobe GenStudio for Performance Marketing.

Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).


## Ny fältsökruta i ikonerna för filter, fält och radfärger i planeringsvyn

>[!NOTE]
>
>Förhandsgranska: 6 november 2025
>Production fast release: 11 december 2025
>Produktion för alla: 15 januari 2026

Du kan nu söka efter ett specifikt fält när du skapar ett vyelement i en posttypvy. Vi har lagt till sökrutor när du skapar ett filter, sorterar, grupperar eller när du konfigurerar fält eller radfärger. Före den här förbättringen kunde du bläddra igenom listan med tillgängliga fält.

Den här förbättringen är tillgänglig i alla posttypsvyer.

Mer information finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md).


## Globala posttyper och möjligheten att lägga till dem som befintliga posttyper på andra arbetsytor

>[!NOTE]
>
>Förhandsgranska: 16 oktober 2025
>Production fast release: 13 november 2025
>Produktion för alla: 15 januari 2026

När du implementerar Workfront Planning för en organisation med flera team och gemensamma arbetsflöden kan du behöva definiera en sammanhängande struktur och metadata för nyckelposttyper (som kampanjer och slutprodukter) som kan läggas till i varje teames arbetsytor för att fånga och hantera deras arbete.

Ni kan också behöva varje teames arbete för att komma upp på en central nivå.

I ett sådant arbetsflöde kan du se till att teamen hämtar sitt arbete på ett enhetligt sätt samtidigt som de låser upp teamets synlighet, utan att behöva lägga till alla i organisationen till varje arbetsyta. Du kan använda globala posttyper för att uppnå detta.

Nu kan du ange att en posttyp ska vara global och använda den på flera arbetsytor. Användare kan använda samma fältstruktur och anslutningar som redan har konfigurerats på en central arbetsyta.

Mer information finns i följande artiklar:

* [Posttyp för arbetsyta - översikt](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)

* [Konfigurera funktioner för korsarbetsyta för posttyper](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)

* [Lägga till befintliga posttyper från en annan arbetsyta](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)

## Ny gräns för anslutningsfält för en posttyp

>[!NOTE]
>
>Förhandsgranska: 16 oktober 2025
>Production fast release: 13 november 2025
>Produktion för alla: 15 januari 2026

Vi har infört en gräns på 30 anslutningsfält för varje posttyp.

Obs! Om din organisation har fler än 30 anslutningsfält för en posttyp kan du behålla de ytterligare fält som överskrider gränsen på 30. Du kan dock inte lägga till fler anslutningsfält till de posttyper som överskrider gränsen. Framöver kommer den nya gränsen på 30 anslutningsfält att gälla.

Mer information finns i [Översikt över anslutna posttyper](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Ange användarvänliga värden för val av urvalsfält

>[!NOTE]
>
>Förhandsgranska: 16 oktober 2025
>Production fast release: 13 november 2025
>Produktion för alla: 15 januari 2026

När du lägger till fältval till ett envalsfält eller flervalsfält kommer Workfront nu att tilldela unika användarvänliga värden till varje val. Före den här förbättringen genererade Workfront ett alfanumeriskt ID som var svårt att förstå och använda i API-anrop och andra integreringar.

Tänk på följande med den här förbättringen:

* De nya värdena läggs till i de nya fältalternativen. Befintliga fältalternativ behåller sina alfanumeriska ID:n.

* Alternativvärden är unika för ett fält men kan upprepas mellan olika fält.

* Om du ändrar namn på ett alternativ uppdateras inte dess ursprungliga värde.

* Alternativvärden visas med gemener och avgränsas med understreck när du väljer flera ord. Om du använder en etikett som redan används som ett annat alternativnamn för samma fält lägger Workfront till ett sekventiellt nummer till värdet.

Mer information finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).







---
content-type: release-notes
title: Första utgåvan av kvartal 2026 för Adobe Workfront Planning
description: Detta är lanseringsaktiviteten för Adobe Workfront Planning-produkten för första kvartalet 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: a58e7da96c43dd308a213c6d7ef74d5085a2e1ba
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 0%

---

# Första utgåvan av kvartal 2026 för Adobe Workfront Planning

I den här artikeln beskrivs funktionerna som lanseras för Workfront Planning i den första utgåvan av kvartal 2026.

<!--keep the sentence below for all future quarterly release pages-->

En lista över alla funktioner som släppts för Adobe Workfront Planning finns i [Versionsaktivitet för Adobe Workfront Planning: artikelindex](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Dela vyer på sidan Projekt - kopplade poster

>[!NOTE]
>
>Förhandsgranska: 18 december 2025
>Production fast release: 14 januari 2026\
>Produktion för alla: 15 januari 2026

För att göra det enklare att se den information du behöver har vi lagt till möjligheten att dela vyer på sidan Projects Connected records. Nu kan du dela vyer med andra användare, team eller grupper.

Mer information om begärandevyer, inklusive delning, finns i [Skapa och hantera vyer i området Förfrågningar](/help/quicksilver/manage-work/requests/create-requests/create-views-for-requests-list.md).

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

<!--

## Create record type hierarchies in workspaces

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast: January 14, 2026 
>Production all: January 15, 2026 

You can now define flexible but structured hierarchies between record or object types.  

Hierarchies are connections between record types. You can have up to 4 record and object types connected in one hierarchy, and you can have multiple hierarchies in one workspace. The first record type in the hierarchy is a parent, and all the other record or object types are its children objects.  

You can use hierarchies to organize work in a way that reflects how your teams actually plan, operate, and deliver and to visualize how strategy flows into execution. 

Consider the following when building hierarchies: 

* You can have multiple hierarchies in a workspace 
* You can connect only Planning record types from one workspace and Workfront projects in a hierarchy.  
* A record type or a project can only have one parent in the same workspace. 
* A record type can be the parent in multiple hierarchies 
* Connectable record types cannot be used in hierarchies in other workspaces than their own. 
* Global record types can be used in hierarchies only in the workspaces that they were created in or have been added to.  

When you create hierarchies between record types, they generate breadcrumbs for records that belong to those record types. 

For more information, see [Hierarchy and breadcrumb overview](help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

-->

<!--

## New unified breadcrumbs added to records' pages

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast: January 14, 2026 
>Production for all: January 15, 2026 

We have added breadcrumbs to a record's page to reflect its spot in a hierarchy. After you create hierarchies, you can see a record's breadcrumb at the top of its page, indicating what other parent or children objects are connected to it. Hierarchies are consistent across Workfront and Planning.  

For example, you can view a project's Planning hierarchy when it's connected to Planning record types in its Planning breadcrumb, and its Workfront hierarchy when it's connected to Workfront object types, like Portfolios or Programs, in Workfront.  

For information, see [Hierarchy and breadcrumb overview](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

-->

## Förbättringar av Workspace huvudsida

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

<!--

## Improvements to connected records pages

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast: January 14, 2026 
>Production for all: January 15, 2026 

To give you more flexibility when working with connected records pages, we have enhanced the functionality of views in this area of Workfront Planning. The following are improvements in the connected records pages of a record that are coming with this release:

* You can now add a timeline and a calendar view to a record's connected records page.
* You can now share views from a connected records page. The views shared from these pages are visible system-wide by all users you share them with in any other area of Workfront Planning. All views shared in any other areas of Planning are also visible in the connected records page for the same users they are shared with.
* We have added a restriction to only allow one connected records page per each record or object type. Prior to this enhancement, you could add multiple pages for the same record or object type. Now, you can use multiple views for the same record type in one connected records page.
* We have added a **New row** link at the bottom of a table view and a **Connect records** button in the upper-right area of the connected records page. Prior to this enhancement, the **New row** link and the **Connect records** button existed only on a project connected page. 

For information, see [Add a Connected records page to a record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

-->

## Lägga till fältet för varumärkesanslutning till Produkter och profiler som standard på arbetsytan i GenStudio

>[!NOTE]
>
>Förhandsgranska: 11 december 2025
>Production fast release: 11 december 2025
>Produktion för alla: 11 december 2025

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







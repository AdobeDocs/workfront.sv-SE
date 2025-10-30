---
content-type: release-notes
title: Första utgåvan av kvartal 2026 för Adobe Workfront Planning
description: Detta är lanseringsaktiviteten för Adobe Workfront Planning-produkten för första kvartalet 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 7fb12a3fbdad661baf2d0ad472ce8017e178ddef
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Första utgåvan av kvartal 2026 för Adobe Workfront Planning

I den här artikeln beskrivs funktionerna som lanseras för Workfront Planning i den första utgåvan av kvartal 2026.

<!--keep the sentence below for all future quarterly release pages-->

En lista över alla funktioner som släppts för Adobe Workfront Planning finns i [Versionsaktivitet för Adobe Workfront Planning: artikelindex](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).


<!--## New field search box in the Filters, Fields, and Row colors icons in Planning views

>[!NOTE]
>
>Preview: October 30, 2025 
>Production fast release: November 13, 2025 
>Production for everyone:  January 15, 2026 


You can now search for a specific field when building a view element in record type view. The new search boxes have been added when you build a filter, sort, grouping, or when you configure your fields or row colors. Prior to this enhancement, you could simply scroll through the list of available fields.
This improvement is available in all views.

For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).-->


## Globala posttyper och möjligheten att lägga till dem som befintliga posttyper på andra arbetsytor

>[!NOTE]
>
>Förhandsgranska: 16 oktober 2025
>&#x200B;>Production fast release: 13 november 2025
>&#x200B;>Produktion för alla: 15 januari 2026

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
>&#x200B;>Production fast release: 13 november 2025
>&#x200B;>Produktion för alla: 15 januari 2026

Vi har infört en gräns på 30 anslutningsfält för varje posttyp.

Obs! Om din organisation har fler än 30 anslutningsfält för en posttyp kan du behålla de ytterligare fält som överskrider gränsen på 30. Du kan dock inte lägga till fler anslutningsfält till de posttyper som överskrider gränsen. Framöver kommer den nya gränsen på 30 anslutningsfält att gälla.

Mer information finns i [Översikt över anslutna posttyper](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Ange användarvänliga värden för val av urvalsfält

>[!NOTE]
>
>Förhandsgranska: 16 oktober 2025
>&#x200B;>Production fast release: 13 november 2025
>&#x200B;>Produktion för alla: 15 januari 2026

När du lägger till fältval till ett envalsfält eller flervalsfält kommer Workfront nu att tilldela unika användarvänliga värden till varje val. Före den här förbättringen genererade Workfront ett alfanumeriskt ID som var svårt att förstå och använda i API-anrop och andra integreringar.

Tänk på följande med den här förbättringen:

* De nya värdena läggs till i de nya fältalternativen. Befintliga fältalternativ behåller sina alfanumeriska ID:n.

* Alternativvärden är unika för ett fält men kan upprepas mellan olika fält.

* Om du ändrar namn på ett alternativ uppdateras inte dess ursprungliga värde.

* Alternativvärden visas med gemener och avgränsas med understreck när du väljer flera ord. Om du använder en etikett som redan används som ett annat alternativnamn för samma fält lägger Workfront till ett sekventiellt nummer till värdet.

Mer information finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).
---
content-type: release-notes
title: Tredje kvartersversionen 2025 för Adobe Workfront Planning
description: Detta är lanseringsaktiviteten för Adobe Workfront Planning-produkten för tredje kvartalet 2025.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 6761f5af-2501-4487-8114-2751f1e4fe69
source-git-commit: 870e4130daf9924bf85b59eb09f7d548b8152096
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 0%

---

# Tredje kvartersversionen 2025 för Adobe Workfront Planning

I den här artikeln beskrivs de funktioner som lanseras för Workfront Planning i utgåvan för tredje kvartalet 2025.

<!--keep the sentence below for all future quarterly release pages-->

En lista över alla funktioner som släppts för Adobe Workfront Planning finns i [Versionsaktivitet för Adobe Workfront Planning: artikelindex](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Ny upplevelse när du delar upp poster i kompakt läge i tidslinjevyn

>[!NOTE]
>
>* Förhandsgranska: 22 maj 2025
>* Production fast release: 12 juni 2025
>* Produktion för alla kunder: 17 juli 2025

Vi har ändrat upplevelsen när du delar upp poster i tidslinjevyn och du har använt vyn Kompakt.
Med den nya uppdateringen ombeds du, när du definierar dina brytningsobjekt medan du visar tidslinjen i kompakt läge, att växla till standardvyn när du har avslutat konfigurationen av brytningsvillkoren.

Före den här förbättringen var det inte möjligt att definiera brytningsvillkoren när tidslinjevyn visas i kompakt läge.

Med den här uppgraderingen är standardalternativet. Före detta var läget Kompakt som standard.

Mer information finns i [Hantera tidslinjevyn](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Uppdatera inställningarna för tidslinjevyn för att definiera utseendet och känslan för de kopplade posternas fält när du använder alternativet Brytning

>[!NOTE]
>
>* Förhandsgranska: 15 maj 2025
>* Production fast release: 12 juni 2025
>* Produktion för alla kunder: 17 juli 2025

Nu kan du formatera postfältens utseende och känsla i tidslinjevyn för posterna i detaljerna. Du kan uppdatera följande inställningar för fälten i dessa poster:

* Stapelformat
* Färg

Före den här förbättringen kunde du bara formatera staplarna för huvudposterna när de visas i tidslinjevyn, och du kunde inte formatera staplarna för de kopplade posterna.\
 
Mer information finns i [Hantera tidslinjevyn](/help/quicksilver/planning/views/manage-the-timeline-view.md).  

## Exportera tabellvyn till en CSV- eller Excel-fil 

>[!NOTE]
>
>* Förhandsgranska: 15 maj 2025
>* Production fast release: 12 juni 2025
>* Produktion för alla kunder: 17 juli 2025

Vi har lagt till en ny funktion i Workfront Planning där du kan exportera information som visas i tabellvyn till en CSV- eller Excel-fil.  

Tänk på följande när du exporterar information från tabellvyn:  

* Den exporterade informationen tar hänsyn till de filter, grupperingar och sorteringar som tillämpas på tabellvyn i Workfront Planning.
* Miniatyrbilder och anpassade radfärger stöds inte i den exporterade filen.  
* Endast fält som är synliga i Workfront-gränssnittet exporteras. Dolda fält exporteras inte.  

Mer information finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md). 

## Workfront Planning-anslutna fält stöds nu när du importerar poster med en CSV- eller Excel-fil

>[!NOTE]
>
>* Förhandsgranska: 15 maj 2025
>* Production fast release: 12 juni 2025
>* Produktion för alla kunder: 17 juli 2025

Du kan nu fylla i värdena för anslutna fält när du lägger till poster till en posttyp med hjälp av en CSV- eller Excel-fil.  Endast anslutna planeringspostfält stöds. Fält som visar anslutningar till andra program stöds inte.

Den här ändringen stöds när du importerar en CSV- och Excel-fil för att skapa både en posttyp och poster för en befintlig posttyp.

Före den här förbättringen gick det inte att fylla i anslutningsfält när du importerade poster.

Mer information finns i följande artiklar:

* [Skapa poster genom att importera information från en CSV- eller Excel-fil](/help/quicksilver/planning/records/import-file-to-create-records.md).

* [Skapa posttyper genom att importera information från en CSV- eller Excel-fil](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md).

## Inline-redigering på sidan Anslutna poster i en post

>[!NOTE]
>
>* Förhandsgranska: 30 april 2025
>* Production fast release: 15 maj 2025
>* Produktion för alla kunder: 17 juli 2025

Nu kan du redigera poster på sidan Anslutna poster i en post. Med den här uppdateringen har vi infört följande:

* Sidans namn har ändrats från &quot;Anslutningsvy&quot; till &quot;Anslutna poster&quot;.
* Kopplade poster som visas på den här sidan går att redigera i tabellvyn. Anslutna Workfront-objekt fortsätter att visas i en skrivskyddad tabell.

Före den här förbättringen var tabellen på sidan Anslutningsvy skrivskyddad för postanslutningar.

Mer information finns i [Hantera postsidans layout](/help/quicksilver/planning/records/manage-the-record-page.md).

## Planeringsområdet visas som standard på huvudmenyn för standardlicensanvändare

>[!NOTE]
>
>* Förhandsgranska: 30 april 2025
>* Production fast release: 15 maj 2025
>* Produktion för alla kunder: 17 juli 2025

Standard- och systemadministratörsanvändare kan nu som standard hitta planeringsområdet på huvudmenyn, utan att tilldelas en layoutmall som innehåller den. Alla andra användare måste ha en layoutmall som innehåller planeringsområdet som de har tilldelats för att kunna komma åt den.

Före den här förbättringen måste användare med alla licensnivåer tilldelas layoutmallar som ändrats så att de fick med Planning-området på Huvudmenyn för att komma åt det här området.

>[!NOTE]
>
>Den här ändringen är synlig för alla nya och befintliga användare med en systemadministratör och en standardlicens.
>Befintliga användare som tilldelats en layoutmall kommer även fortsättningsvis att se allt enligt inställningarna som definierats i layoutmallen.

Mer information finns i [Översikt över Adobe Workfront-planering](/help/quicksilver/planning/access/access-overview.md).

## Färgformatering på radnivå i tabellvyn

>[!NOTE]
>
>* Förhandsgranska: 30 april 2025
>* Production fast release: 15 maj 2025
>* Produktion för alla kunder: 17 juli 2025

För att synliggöra viktig information i dina poster har vi infört färgformatering på radnivå för tabellvyn. Nu kan du välja en färg för varje rad när du har definierat villkor för varje alternativ.  Detta är en ny funktion som inte fanns före den här uppdateringen.

Mer information finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md).

## Ny inställning för att korta av långa postnamn i vyn Standardtidslinje

>[!NOTE]
>
>* Förhandsgranska: 23 april 2025
>* Production fast release: 15 maj 2025
>* Produktion för alla kunder: 17 juli 2025

Du kan nu aktivera en inställning på fliken Stapelformat i rutan Inställningar i en tidslinjevy för att korta av längre postnamn när du visar dem i standardvyn. Inställningen är inaktiverad som standard och kan bara aktiveras när du visar tidslinjevyn i standardläge. Eftersom den här inställningen är inaktiverad visas information på postfälten som standard utökad. Före den här förbättringen trunkerades informationen på postfälten som standard.

Mer information finns i [Hantera tidslinjevyn](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Delningsbehörigheter för posttyper


>[!NOTE]
>
>* Förhandsgranska: 17 april 2025
>* Production fast release: 12 juni 2025
>* Produktion för alla kunder: 17 juli 2025

För att få bättre kontroll över vilka som kan visa eller hantera poster i varje posttyp och säkerställa att endast behöriga personer kan hantera informationen för varje posttyp baserat på deras roller och ansvarsområden, har vi infört behörigheter på posttypsnivå.

Före den här förbättringen kunde du bara dela arbetsytor med andra och den behörighet som de tilldelats till en arbetsyta som tillämpas på alla posttyper i arbetsytan.

Vi har infört följande uppdateringar:

* Workspace-behörigheter delas automatiskt med alla posttyper på arbetsytan.
* Nivån för behörigheter som beviljas för arbetsytan visas som ärvda behörigheter för posttypen.
* Du kan inte dela en posttyp med en högre behörighetsnivå än användarna har på arbetsytan.
* Du kan inaktivera de ärvda behörigheterna för posttypen för att göra den skrivskyddad för alla personer på arbetsytan. Efter det kan du lägga till enskilda personer, team, grupper, företag eller roller och ge dem Contribute-behörighet för posttypen.

Mer information finns i [Dela posttyper](/help/quicksilver/planning/access/share-record-types.md).



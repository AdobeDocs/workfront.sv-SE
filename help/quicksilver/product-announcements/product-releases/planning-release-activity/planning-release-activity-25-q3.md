---
content-type: release-notes
title: Tredje kvartersversionen 2025 för Adobe Workfront Planning
description: Detta är lanseringsaktiviteten för Adobe Workfront Planning-produkten för tredje kvartalet 2025.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 6761f5af-2501-4487-8114-2751f1e4fe69
source-git-commit: eaba54ebfef15c5f823c7086b809165b5cfb181b
workflow-type: tm+mt
source-wordcount: '1908'
ht-degree: 0%

---

# Tredje kvartersversionen 2025 för Adobe Workfront Planning

I den här artikeln beskrivs de funktioner som lanseras för Workfront Planning i utgåvan för tredje kvartalet 2025.

<!--keep the sentence below for all future quarterly release pages-->

En lista över alla funktioner som släppts för Adobe Workfront Planning finns i [Versionsaktivitet för Adobe Workfront Planning: artikelindex](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

<!--## Auto-populate fields based on applied groupings

Preview: July 10, 2025 
Production fast release: August 14, 2025 
Production for everyone: October 16, 2025 

Now, when you have  groupings applied to a table view, adding a record to the table will auto-populate the fields associated with the groupings you add the record to.  

If you have multiple groupings applied, the system auto-populates the fields associated with all groupings only when you add the record at the end of the list inside the last grouping criteria.  

Prior to this enhancement, you had to manually update the fields associated with groupings.  

For information, see [Create records](/help/quicksilver/planning/records/create-records.md).-->

<!--## Common sharing button for views and record types

>[!NOTE]
>
>* Preview: July 9, 2025 
>* Production for everyone: July 17, 2025 

You can now share a view as well as a record type from the same button on the record type's page. Prior to this enhancement, you could only share the record type from the Share button on the record type page and a view from the view's tab.  

For more information, see the following articles: 

* [Share views](/help/quicksilver/planning/access/share-views.md)  

* [Share record types](/help/quicksilver/planning/access/share-record-types.md)
-->

<!--## Add teams as approvers on Planning request forms

>[!NOTE]
>
>* Preview: July 9, 2025 
>* Production for everyone: October 16, 20025 

To make the approval process more flexible, we've added the ability to add teams as approvers on Planning request forms. Now, you can enter and select team names when setting approvers. Any of the team members can make a decision, which counts as the approval decision for the entire team.

Previously, only individual users could be assigned as approvers. 

For more information, see [Add an approval to a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/add-approval-to-request-form.md).-->

## Uppdaterad upplevelse vid delning av begärandeformulär

>[!NOTE]
>
>* Förhandsgranska: 9 juli 2025
>* Produktion för alla: 17 juli 2025

För att göra upplevelsen av att dela ett begärandeformulär i Workfront Planning säkrare och enklare har vi gjort följande ändringar:

* Vi har tagit bort ärvda behörigheter. Formuläret för begäran delas nu endast med de som du väljer.
* Vi har tagit bort alternativen för att hantera och bidra för användare som du delar frågeformuläret med. Nu kan tillagda användare bara skicka formuläret.
* Fliken för offentlig delning visar nu länken och utgångsdatumet först när alternativet Skapa offentlig länk har aktiverats.

Mer information finns i [Skapa och hantera ett begärandeformulär i Adobe Workfront Planning](https://experienceleague.adobe.com/sv/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-requests/create-request-form).

## Expandera och komprimera alla grupperingar i tabellvyn

>[!NOTE]
>
>* Förhandsgranska: 26 juni 2025
>* Produktion för alla: 17 juli 2025

Nu kan du komprimera och utöka grupperingarna i en tabellvy med följande områden:

* Grupperingsrutan, som du kommer åt från tabellvyns verktygsfält

* En grupperings sidhuvud genom att högerklicka på den

Du kan komprimera eller expandera en eller alla grupperingar samtidigt.

Före den här förbättringen kunde du bara komprimera eller expandera en gruppering åt gången från varje grupperingsrubrik.

Mer information finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md).

## Ny sammanställningsfunktion för formelfält

>[!NOTE]
>
>* Förhandsgranska: 26 juni 2025
>* Produktion för alla: 26 juni 2025

När du kopplar posttyper och infogar ett formelfält som en sökning kan du nu använda sammanställningsfunktionerna (SUM, AVERAGE, MIN, MAX osv.) beroende på formelfältets format. Om t.ex. formelfältet är numeriskt kan du använda funktioner som SUM eller AVG. Om formelfältet är formaterat som text används inte sammanställningsfunktioner som SUM.

Tidigare kunde du bara tillämpa sammanställningsfunktioner på vanliga fält, men inte på formelfält, när du kopplar posttyper och hämtar in sökfält från de anslutna posterna.

Mer information finns i [Översikt över formelfält](/help/quicksilver/planning/fields/formula-fields.md).

## Tillgänglighet för anpassade kvartal för tidslinjen i Workfront Planning

>[!NOTE]
>
>* Förhandsgranska: 12 juni 2025
>* Production fast release: 17 juli 2025
>* Produktion för alla kunder: 17 juli 2025

När du konfigurerar anpassade kvartal i området Projektinställningar i installationsprogrammet är de anpassade kvartalen tillgängliga för tidslinjevyn i Workfront Planning.

Före den här uppdateringen var de anpassade kvartalen endast tillgängliga för Workfront rapporteringsfunktioner.

Med den här förbättringen kan kunder som köpt Workfront Planning se en uppdaterad upplevelse för att definiera anpassade kvartal. Uppdateringen innehåller följande förbättringar:

Mellanrum och överlappningar mellan kvartalen godtas inte längre.

Du kan ställa in upp till 100 anpassade kvartal. Före den här uppdateringen kunde du bara konfigurera 8 anpassade kvartal

Kunder som inte har köpt Workfront Planning kan nu använda anpassade kvartalsupplevelser utan förändringar.

Mer information finns i [Aktivera anpassade kvartal för projekt](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md).

## Beräkna alla beroende formler samtidigt

>[!NOTE]
>
>* Förhandsgranska: 12 juni 2025
>* Production fast release: 12 juni 2025
>* Produktion för alla kunder: 12 juni 2025

Vi har infört en förbättring som uppdaterar alla formelfält som är beroende av varandra samtidigt efter att ett refererat fält har uppdaterats manuellt. Formelfält som är 2, 3 eller 4 fält från fältet vars värde ändras manuellt och som refererar till varandra uppdateras nu automatiskt samtidigt.

Före den här förbättringen uppdaterades endast direkt beroende formelfält när värdet för ett referensfält uppdaterades manuellt.

Mer information finns i [Översikt över formelfält](/help/quicksilver/planning/fields/formula-fields.md).

## Nya uttryck har lagts till i formelfält

>[!NOTE]
>
>* Förhandsgranskning: 6 juni 2025
>* Production fast release: 6 juni 2025
>* Produktion för alla kunder: 6 juni 2025

Vi har lagt till följande uttryck i formelfält:

* ARRAYCONTAINS

* SORTASCARRAY

* SORTDESCARRAY

Före den här förbättringen hade dessa uttryck bara stöd i anpassade fält som beräknats av Workfront.

Mer information finns i [Översikt över formelfält](/help/quicksilver/planning/fields/formula-fields.md).

## Filter, kolumner och ytterligare fält som lagts till på fliken Planering i området Begäranden

>[!NOTE]
>
>* Förhandsgranska: 29 maj 2025
>* Production fast release: 12 juni 2025
>* Produktion för alla kunder: 17 juli 2025

Vi har lagt till följande funktioner i en lista över begäranden på fliken Planering i området Begäranden:

* Anges efter kolumn för att ange den person som lade till en begäran
* Filter som begränsar antalet begäranden som du kan visa på fliken Planering. Du kan filtrera listan efter följande objekt:

   * Workspace som förfrågningsformuläret kommer från
   * posttypen som är associerad med begärandeformuläret
   * Ange anmälningsdatum för begäran
   * begärandeformulärets namn
   * status för förfrågningarna
   * namnet på den person som ingav begäran.

* Kolumnkontroll om du vill visa eller dölja fält (eller kolumner) i listan Planeringsbegäranden.

Mer information finns i [Skicka Adobe Workfront Planning-begäranden för att skapa poster](/help/quicksilver/planning/requests/submit-requests.md).

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
>&#x200B;>Befintliga användare som tilldelats en layoutmall kommer även fortsättningsvis att se allt enligt inställningarna som definierats i layoutmallen.

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
>* Production fast release: 17 juli 2025
>* Produktion för alla kunder: 17 juli 2025

För att få bättre kontroll över vilka som kan visa eller hantera poster i varje posttyp och säkerställa att endast behöriga personer kan hantera informationen för varje posttyp baserat på deras roller och ansvarsområden, har vi infört behörigheter på posttypsnivå.

Före den här förbättringen kunde du bara dela arbetsytor med andra och den behörighet som de tilldelats till en arbetsyta som tillämpas på alla posttyper i arbetsytan.

Vi har infört följande uppdateringar:

* Workspace-behörigheter delas automatiskt med alla posttyper på arbetsytan.
* Nivån för behörigheter som beviljas för arbetsytan visas som ärvda behörigheter för posttypen.
* Du kan inte dela en posttyp med en högre behörighetsnivå än användarna har på arbetsytan.
* Du kan inaktivera de ärvda behörigheterna för posttypen för att göra den skrivskyddad för alla personer på arbetsytan. Efter det kan du lägga till enskilda personer, team, grupper, företag eller roller och ge dem Contribute-behörighet för posttypen.

Mer information finns i [Dela posttyper](/help/quicksilver/planning/access/share-record-types.md).



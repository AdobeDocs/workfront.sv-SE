---
title: Rapportförbättringar för första kvartalet 2026
description: Rapportförbättringar för första kvartalet 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: f8c41105607e972d3395cf8d89fb1fdf29f0da85
workflow-type: tm+mt
source-wordcount: '934'
ht-degree: 0%

---

# Rapportförbättringar för första kvartalet 2026

Den här sidan beskriver rapportförbättringar som gjorts i första utgåvan av kvartalet 2026 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön enligt vad som anges.

En lista över alla ändringar som är tillgängliga vid den här tidpunkten i den första utgåvan av kvartal 2026 finns i [Översikt över utgåvan första kvartalet 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).



## Valutauppdateringar på arbetsytans kontrollpaneler

>[!NOTE]
>
>Förhandsgranska: 18 december 2025
>Production fast release: 14 januari 2026
>Produktion för alla: 15 januari 2026

Vi har gjort följande uppdateringar för fält för inbyggd valuta:

* När flera valutor definieras i Workfront kan du nu välja en standardvaluta för instrumentpanelen när du skapar den.

* När du skapar en rapport kan du låsa ett valutafält. Detta garanterar att valutainställningen på kontrollpanelsnivå inte påverkar visningen av dessa värden.

* När du visar en kontrollpanel kan användare växla mellan olika definierade valutor i Workfront. Dessa ändringar gäller för hela instrumentpanelen med undantag för låsta valutafält.



## Snabbsökningstabellresultat i Canvas Dashboards

>[!NOTE]
>
>Förhandsgranska: 18 december 2025
>Production fast release: 14 januari 2026
>Produktion för alla: 15 januari 2026

Vi har lagt till en snabbsökning i tabellrapporter. Den här sökningen fungerar på alla sidor, så du kan söka efter data även om de inte är synliga just nu.


## Nytt alternativ för Visa summa för cirkeldiagram

>[!NOTE]
>
>Förhandsgranska: 18 december 2025
>Production fast release: 14 januari 2026
>Produktion för alla: 15 januari 2026

Vi har introducerat ett nytt alternativ för Visa totalt som konverterar cirkeldiagram till matrisdiagram. Med den här funktionen kan användare visa ett centralt värde som representerar summan av alla segment i diagrammet.

* För aggregeringstyper för antal är det visade mittvärdet ett antal av alla segment i diagrammet.
* För summeringstyper är det visade mittvärdet den aggregerade summan av det numeriska värdet eller valutavärdet.
* För aggregeringstyperna medelvärde, max och min visas medelvärdet, maximivärdet eller minimivärdet i mitten.

Användarna kan också välja att visa eller dölja en etikett för summan och ange ett anpassat etikettvärde.

Mer information finns i [Skapa en diagramrapport på en arbetsytekontrollpanel](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md).

## Nya konfigurationsalternativ för cirkeldiagram på arbetsytans kontrollpaneler

>[!NOTE]
>
>Förhandsgranska: 18 december 2025
>Production fast release: 14 januari 2026
>Produktion för alla: 15 januari 2026

Vi har introducerat två nya konfigurationsalternativ för cirkeldiagram:

* Dölj segmentetiketter: Du kan nu välja att dölja segmentetiketter i ett cirkeldiagram om de är för långa och påverkar diagrammets läsbarhet.
* Dölj och flytta diagramförklaringen: Du kan nu välja att dölja cirkeldiagramförklaringen. Du kan också ange teckenförklaringens placering till höger (standard), vänster, överst eller nederst i diagrammet.

Mer information finns i [Skapa en diagramrapport på en arbetsytekontrollpanel](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md).

## Förbättrat grupperingsantal på arbetsytans kontrollpaneler

>[!NOTE]
>
>Förhandsgranska: 18 december 2025
>Production fast release: 14 januari 2026
>Produktion för alla: 15 januari 2026

Vi har uppdaterat grupperingsfältet på arbetsytans kontrollpaneler för att visa antalet poster för den aktuella sidan och det totala antalet poster för grupperingen på alla sidor.

Grupperingsfältet visar till exempel &quot;3 av 7&quot; eller &quot;83 av 21032&quot; för att ge en tydlig bild av datafördelningen inom grupperingen.

Tidigare fanns det ingen detaljerad räkningsinformation i grupperingsfältet, vilket gjorde det svårt att förstå det totala antalet poster i en gruppering när man navigerar mellan flera sidor.

## Ny funktion för referensrader i rapporter på arbetsytans kontrollpaneler

>[!NOTE]
>
>Förhandsgranska: 18 december 2025
>Production fast release: 14 januari 2026
>Produktion för alla: 15 januari 2026

Nu kan du definiera en referensrad i Bar-, Column- och Line-diagram för att ange ett mål eller tröskelvärde för fyra dina seriebaserade rapporter.

Obs! Referensraden är inte dynamisk och det går inte att använda flera referensrader. Vi utforskar framtida förbättringar, men det finns inga omedelbara planer.

Mer information finns i [Skapa en diagramrapport på en arbetsytekontrollpanel](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md).

## Anpassa axeletiketter i diagramrapporter på arbetsytans kontrollpaneler

>[!NOTE]
>
>Förhandsgranska: 18 december 2025
>Production fast release: 14 januari 2026
>Produktion för alla: 15 januari 2026

Nu kan du anpassa axeletiketterna i diagramrapporter. Med den här nya funktionen kan du ange en ersättningsaxeletikett som ska visas i stället för standardobjektet och fältsökvägen. Dessutom kan du välja att helt dölja axeletiketterna.

Mer information finns i [Skapa en diagramrapport på en arbetsytekontrollpanel](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md).

## Duplicera en rapport på en arbetsytans kontrollpanel

>[!NOTE]
>
>Förhandsversion: 23 oktober 2025
>Produktion för alla kunder: 23 oktober 2025
>[!BADGE Frånschemat ]{type=Neutral}

Du kan nu duplicera en KPI-, tabell- eller diagramrapport på en Canvas Dashboard när den har skapats. När du har duplicerat rapporten kan du redigera den efter behov innan du sparar den.

## Tar bort fältalternativ från rapportfilter

>[!NOTE]
>
>Förhandsgranska: 6 november 2025
>Production fast release: 13 november 2025
>Produktion för alla: 15 januari 2026

Vi har tagit bort följande fältalternativ som tidigare var tillgängliga när ett filter tillämpades på en rapport:

* Andra grupp-ID
* Andra roller-ID
* Andra team-ID

Dessa togs bort på grund av problem som är kopplade till operatorerna Inte lika och Är tom. Om du har ett befintligt filter som använder något av dessa fält fortsätter det att fungera som förväntat. Du kan också fortsätta använda dessa fält i textläget <code></code>men du bör undvika att använda operatorerna Inte lika eller Är tom när du gör det.

Följande fältalternativ är tillgängliga som alternativ:

* Andra grupper: ID
* Andra roller: ID
* Andra team: ID


## Nya skyddsritningar för att förbättra inläsningstiden på arbetsytans kontrollpaneler

>[!NOTE]
>
>Förhandsgranska: 6 november 2025
>Production fast release: 13 november 2025
>Produktion för alla: 15 januari 2026

För att undvika tidsfördröjningar vid inläsning och förbättra övergripande prestanda på arbetsytans kontrollpaneler har vi tillämpat begränsningar för hur många kontrollpanelskomponenter som kan läggas till på en kontrollpanel:

* Rapporter per kontrollpanel: 25 gräns
* Grupperingar i tabellvyer: 5 gräns
* Avstånd från rapportens basobjekt: 10-gräns
* Kolumner i en tabellvy: 25 gräns
* Filteruppmaningar på kontrollpanelnivå: 10 gräns





---
title: Rapportförbättringar för första kvartalet 2026
description: Rapportförbättringar för första kvartalet 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 00483638948941c933e5f8bc8cb3edaf8e43fea1
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Rapportförbättringar för första kvartalet 2026

Den här sidan beskriver rapportförbättringar som gjorts i första utgåvan av kvartalet 2026 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön enligt vad som anges.

En lista över alla ändringar som är tillgängliga vid den här tidpunkten i den första utgåvan av kvartal 2026 finns i [Översikt över utgåvan första kvartalet 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

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

## Förbättrad visning av grupperingsantal på arbetsytans kontrollpaneler

>[!NOTE]
>
>Förhandsgranska: 6 november 2025
>Production fast release: 13 november 2025
>Produktion för alla: 15 januari 2026

När en tabellrapport har flera resultatsidor och tabellen är konfigurerad med grupperingar, visar nu tabellen både postmängden för den aktuella sidan och det totala antalet poster för alla sidor. Om tabellrapporten till exempel har 7 grupperingar och den första sidan visar 3, visas 3 av 7.


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
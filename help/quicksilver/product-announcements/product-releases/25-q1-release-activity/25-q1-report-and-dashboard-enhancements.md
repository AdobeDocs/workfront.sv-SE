---
title: Förbättringar av rapporten och kontrollpanelen för första kvartalet 2025
description: Förbättringar av rapporten och kontrollpanelen för första kvartalet 2025
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 3c0b4797-594c-44d0-b3ad-a64384b6c4a8
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---

# Förbättringar av rapporten och kontrollpanelen för första kvartalet 2025

Den här sidan beskriver alla rapport- och kontrollpanelsförbättringar som gjorts i den första utgåvan av kvartal 2025 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön enligt vad som anges.

En lista över alla ändringar som är tillgängliga vid den här tidpunkten i den första utgåvan av kvartal 2025 finns i [Översikt över utgåvan första kvartalet 2025](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md).

## Nya entiteter tillgängliga i Data Connect

>[!NOTE]
>
>Förhandsversion: 15 januari 2025; Produktionsrelease för alla kunder: 15 januari 2025

Vi har lagt till stöd för följande enheter i Data Connect:

* Projektteamanvändare
* Användarroll för projektteam
* Rapporteringsskyldiga budgeterade timmar
* Rapportvy - statistikantal
* Resurshanteraren
* RTF-anteckning

Vi har också lagt till stöd för följande byråspecifika enheter:

* Affärsprofil
* Affärsregel
* Plats
* Resurskategori för icke-arbetsplats
* Användarplats

Mer information finns i [Workfront Data Connect-dataordlista](/help/quicksilver/reports-and-dashboards/data-lake/data-dictionary.md).

## Gräns för 25 rapporter, externa sidor eller kalendrar i kontrollpaneler

>[!NOTE]
>
>Förhandsversion: 16 december 2024; Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)

För att behålla kontrollpanelens prestanda har vi implementerat en gräns för det totala antalet rapporter, externa sidor eller kalendrar som kan placeras på en kontrollpanel. När du skapar en ny kontrollpanel kan högst 25 objekt läggas till.

Befintliga kontrollpaneler som överskrider den här gränsen visar en varning om att endast de översta 25 objekten visas och när de har redigerats kan kontrollpanelen inte sparas förrän antalet objekt som ingår har reducerats till 25 eller färre.

Mer information finns i [Skapa en instrumentpanel](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Knapp för att skapa konto för förstagångsläsare för dataanslutning

>[!NOTE]
>
>Produktionsrelease för alla kunder: 14 november 2024

Administratörer som använder Data Connect för första gången har nu möjlighet att skapa ett nytt läsarkonto för Snowflake genom att klicka på en enda knapp. Processen tar några minuter, men kräver ingen ytterligare åtgärd.

Mer information om konfiguration av Data Connect finns i [Skapa ett läsarkonto för Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

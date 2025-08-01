---
title: Förbättringar av korrektur- och dokumenthantering för tredje kvartalet 2025
description: Förbättringar av korrektur- och dokumenthantering för tredje kvartalet 2025
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4829d487-7041-447f-9a68-fb1acf467734
source-git-commit: 2ff08963018c83e8d4fe88446f26efc115111a5e
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# Förbättringar av korrektur- och dokumenthantering för tredje kvartalet 2025

Den här sidan beskriver alla förbättringar av dokumenthanteringen som gjorts i tredje kvartersversionen 2025 till förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön enligt vad som anges.

En lista över alla ändringar som är tillgängliga vid den här tidpunkten i den tredje utgåvan av kvartal 2025 finns i [Översikt över utgåvan tredje kvartalet 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).


## Enhetliga godkännanden stegvis utrullning

>[!NOTE]
>
>Produktionsrelease för kunder: fasad utrullning från 17 juli 2025


Vi aktiverar enhetliga godkännanden, som tidigare kallades för godkännande av nya dokument, i en stegvis utrullning. Den här funktionaliteten aktiveras automatiskt i din Workfront-instans under de kommande sex månaderna.

Enhetliga godkännanden ersätter godkännanden i äldre dokument och ger följande funktioner direkt i ett dokument:

* Utse ett helt Workfront-team som granskare eller godkännare
* Ange en tidsgräns för granskning eller godkännande
* Skapa och återanvänd godkännandemallar
* Använd nya versioner
* Visa flera viktiga resultatindikatorer för dina godkännanden i Workfront Home widgets
* Använd paneler på arbetsytan för att visa rapportinformation om enhetliga godkännanden

Mer information finns i [Översikt över enhetliga godkännanden](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

## Uppdatering för korrekturläsaren för skrivbordet

>[!NOTE]
>
>* Produktionsrelease för alla kunder: 16 juni 2025

Desktop Proofing Viewer har uppdaterats till version 2.1.50.

Den här uppdateringen innehåller interna verktygsuppdateringar och påverkar inte slutanvändarnas funktioner.

Uppdateringen gäller både Mac och Windows.

## Ny korrektur- och GenStudio for Performance Marketing-integrering

>[!NOTE]
>
>* Produktionsrelease för alla kunder: 12 juni 2025

Vi är glada över att kunna introducera en ny integrering mellan Proofing och GenStudio for Performance Marketing. Med den här integreringen kan du

* Använd Workfront godkännandemallar för att definiera godkännandearbetsflöden

* Granska utkast i Workfront korrekturläsare

* Se granskningsbeslut för slutligt godkännande och publicering i GenStudio for Performance Marketing

### Integrationskrav

Workfront och GenStudio for Performance Marketing måste distribueras till samma IMS-organisation.

Mer information finns i [Kom igång med integreringen mellan GenStudio for Performance Marketing och Workfront Proof](/help/quicksilver/workfront-integrations-and-apps/review-and-approval-integrations/wf-proof-and-genstudio.md).

## Uppdatering för korrekturläsaren för skrivbordet

Desktop Proofing Viewer har uppdaterats till version 2.1.48.

Uppdateringen är en felkorrigering som gör att Desktop Viewer är kompatibel med Mac operativsystem. Electron nedgraderades till 34.4.0 och Chromium nedgraderades till 132.

Uppdateringen gäller både Mac och Windows.


## Assets i en länkad Google-mapp måste läggas till separat för att kunna visas i Workfront

>[!NOTE]
>
>* Förhandsversion: 2 juni 2025; Produktionsrelease för alla kunder: 2 juni 2025

Google [förbättrar säkerhetskontrollerna](https://workspace.google.com/blog/product-announcements/enhancing-security-controls-for-google-drive-third-party-apps) för tredjepartsprogram som använder Google Drive, vilket kräver att program antar en modell för användargodkännande. Därför måste enskilda resurser länkas en i taget för att vara synliga i Workfront. Mer information finns i [Konfigurera dokumentintegreringar](/help/quicksilver/administration-and-setup/configure-integrations/configure-document-integrations.md).

Viktiga funktioner som förblir oförändrade:

* Söka efter och filtrera efter resurser och mappar inifrån Google Drive modal
* Länka resurser till Workfront-objekt från Google Drive
* Överför resurser till Google Drive via listrutan Skicka till på dokumentsidan
* Visa och få åtkomst till mappstrukturen i en användares My Drive-område
* Länka en ny version av en resurs från Google Drive till ett befintligt dokument i Workfront
* Länka mappar till Workfront-objekt från Google Drive
* Överför resurser till Google Drive genom att dra och släppa dokument till en länkad mapp
* Skapa ett nytt Google Drive-dokument inifrån Workfront


## Nya beslutsknappar för dokumentgodkännande finns i korrekturläsaren

>[!IMPORTANT]
>
>Den här funktionen ingår i en fasad version och är endast tillgänglig för vissa kunder.

>[!NOTE]
>
>* Förhandsversion: 10 april 2025; Produktionsrelease för alla kunder: 17 april 2025

De nya beslutsknapparna för dokumentgodkännande visas nu i korrekturläsaren. När du skapar ett enkelt korrektur och sedan lägger till godkännare och granskare från dokumentsammanfattningen kan de nu fatta sitt beslut direkt i korrekturläsaren.

Tidigare var du tvungen att avsluta korrekturläsaren för att kunna fatta ett beslut.

Godkännanden som skapats före den här versionen visar inte knapparna i korrekturläsaren.

Mer information finns i [Använd godkännanden av nya dokument och korrektur tillsammans](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md).

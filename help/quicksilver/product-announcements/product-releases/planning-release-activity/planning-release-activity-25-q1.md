---
content-type: release-notes
title: Adobe Workfront Planning Release Activity för version 25.1
description: Detta är lanseringsaktiviteten för Adobe Workfront Planning-produkten för första kvartalet 2025.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 0022892cabb9a44fb21e33d88148b098c937f388
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 0%

---

# Första utgåvan av kvartal 2025 för Adobe Workfront Planning

<!--remove this important intro after the 25.1 release-->

>[!IMPORTANT]
>
>Informationen i den här artikeln handlar om Adobe Workfront Planning, ett nytt erbjudande från Adobe Workfront.
>
>Du måste köpa en Workfront Planning-plan, förutom en Workfront-plan, för att kunna komma åt och använda Workfront Planning-funktioner.
>
>En fullständig lista över krav för åtkomst till Workfront Planning finns i [Åtkomstöversikt](/help/quicksilver/planning/access/access-overview.md).
>En översikt över Workfront Planning finns i [Översikt över Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

I den här artikeln beskrivs funktionerna som lanseras för Workfront Planning i utgåvan 2025 av första kvartalet.

<!--keep the sentence below for all future quarterly release pages-->
<!--remove the general activity mention after First Quarter 2025 is released-->

En lista över alla funktioner som släppts för Adobe Workfront Planning efter den allmänna tillgänglighetsutgåvan den 28 augusti 2024 finns i [Adobe Workfront Planning Release Activity: artikelindex](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Nya visningstyper för procenttypsfält i tabellvyn

>[!NOTE]
>
>Förhandsversion: 7 november 2024; Produktion för snabb release: Med version 24.12 (december 2024); Produktion för kvartalsvis version: Med version 25.1 (januari 2025)

Om du vill göra det enklare att läsa tal i tabellvyn kan du nu välja mellan följande alternativ för att ändra hur ett procenttypsfält visas i tabellvyn:

* Nummer
* Liggande
* Cirkel

Den här visningstypen stöds bara i tabellvyn.

Före den här förbättringen kunde du bara visa procentvärden som tal.

Mer information finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

## Anslutningsfält stöds nu i förfrågningsformulär

>[!NOTE]
>
>Förhandsversion: 31 oktober 2024; Produktion för snabb release: Med version 24.11 (14 november 2024); Produktion för kvartalsvis publicering: Med version 25.1 (januari 2025)

Nu kan du lägga till anslutna fält för Workfront Planning-poster i ett formulär för posttypsbegäran.

Du kan inte lägga till anslutningssökningsfält eller anslutna fält för Workfront-objekt i formuläret för begäran.

Före den här förbättringen kunde dessa typer av fält inte läggas till i förfrågningsformulär i Workfront Planning.

Mer information finns i [Skapa och hantera ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Anslutningsvarning vid anslutning av poster som redan är länkade till andra poster

>[!NOTE]
>
>Förhandsversion: 31 oktober 2024; Produktion för snabb release: Med version 24.11 (14 november 2024); Produktion för kvartalsvis publicering: Med version 25.1 (januari 2025)

När du försöker ansluta poster som redan är anslutna någon annanstans och som tillhör en posttyp som är ansluten via en anslutning av typen En till många eller En till en får du nu ett varningsmeddelande om att posterna redan är anslutna. Om du bekräftar att du vill gå vidare med anslutningen, tas de markerade posterna bort från den ursprungliga posten och läggs till i den post som du redigerar.

Mer information om anslutningstyper finns i [Översikt över anslutna posttyper](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Ny informationsikon med en beskrivning av fälten på postens informationssida

>[!NOTE]
>
>Förhandsversion: 30 oktober 2024; Produktion för snabb release: Med version 24.11 (14 november 2024); Produktion för kvartalsvis publicering: Med version 25.1 (januari 2025)

Vi har lagt till en informationsikon till höger om fältnamnen på en postsida. Om du klickar på informationsikonen visas beskrivningen av fältet, om det finns en beskrivning. Före den här förbättringen visas beskrivningen av fältet när du hovrade över fältnamnet.

Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

## Ny Workfront-fälttyp för planeringsanslutningar

>[!NOTE]
>
>Förhandsversion: 24 oktober 2024; Produktion för snabb release: Med version 24.11 (14 november 2024); Produktion för kvartalsvis publicering: Med version 25.1 (januari 2025)

För att fortsätta att brygga Workfront-objekt till Workfront Planning records har vi lagt till en ny fälttyp i Workfront anpassade formulär som kallas Planning Connection. Genom att lägga till den här fälttypen i ett anpassat Workfront-formulär, och slutligen i ett Workfront-objekt, kan du nu göra följande:

* Visa poster som är kopplade till ett Workfront-objekt i det anpassade formuläret.

* Koppla ihop och koppla från Workfront Planning-poster från ett Workfront-objekt.

Du kan lägga till det nya fältet i formulär för alla objekttyper. Du kan emellertid bara redigera informationen i fältet från formulär som är kopplade till följande Workfront-objekt som kan anslutas från posttyperna Workfront Planning: Portfolio, Program, Projekt, Företag, Grupp.

Det går ännu inte att redigera planeringsanslutningsfälten för flera Workfront-objekt.

Mer information finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

[Visa en videodemonstration av den här funktionen](https://video.tv.adobe.com/v/3435633/){target=_blank}

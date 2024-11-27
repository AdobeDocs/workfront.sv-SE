---
content-type: release-notes
title: Adobe Workfront Planning Release Activity för version 25.1
description: Detta är lanseringsaktiviteten för Adobe Workfront Planning-produkten för första kvartalet 2025.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: ef0b719c-6d2e-4d3e-9522-da6dbd71c248
source-git-commit: d27c25e4eedb6b4df67d23b997fdf1222b95da57
workflow-type: tm+mt
source-wordcount: '1747'
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


## Importera befintliga Workfront-fält till posttyper för Workfront Planning

>[!NOTE]
>
>Förhandsversion: 27 november 2024; Produktion för snabb release: Med version 24.12 (december 2024); Produktion för kvartalsvis publicering: Med version 25.1 (januari 2025)

När du lägger till fält i en posttyp kan du nu välja att importera befintliga anpassade eller inbyggda Workfront-fält och associera dem med den posttyp som du har valt.

Före den här förbättringen var du tvungen att skapa alla fält manuellt och associera dem med posttyper.

Beräknade fält stöds inte för närvarande.

Mer information finns i [Importera fält från Adobe Workfront](/help/quicksilver/planning/fields/import-fields-from-workfront.md)

## Skapa posttyper, poster och fält genom att importera en CSV- eller Excel-fil

>[!NOTE]
>
>Förhandsversion: 27 november 2024; Produktion för snabb release: Med version 24.12 (december 2024); Produktion för kvartalsvis publicering: Med version 25.1 (januari 2025)

Nu kan du importera nya posttyper genom att importera en CSV- eller Excel-fil.

Följande information importeras:

* Namnet på bladet eller filen importeras som posttypsnamn.

* Den första raden i varje kolumn importeras som ett nytt fält. Du kan ha upp till 500 fält i varje importerat blad.

* Varje rad importeras som en ny post. Du kan ha upp till 10 000 poster i varje ark.

Mer information finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

## Undvik cirkelreferenser i formler

>[!NOTE]
>
>Förhandsversion: 27 november 2024; Produktion för snabb release: Med version 24.12 (december 2024); Produktion för kvartalsvis publicering: Med version 25.1 (januari 2025)

Vi har introducerat ett varningsmeddelande när vi redigerar eller skapar ett formelfält som kan skapa en cirkelreferens till sig själv eller delade fält. Du kan inte spara ett formelfält som antingen refererar till sig själv eller till artiklar som refereras i beräkningen.

Mer information finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

## Lägga till sidor i en kopplad vy på en postsida för att visa kopplade poster i en tabellvy

>[!NOTE]
>
>Förhandsversion: 27 november 2024; Produktion för snabb release: Med version 24.12 (december 2024); Produktion för kvartalsvis publicering: Med version 25.1 (januari 2025)

Du kan lägga till sidor i en posts informationsområde för att visa kopplade poster i en tabellvy. Du kan lägga till en sida per ansluten post.

De tillagda sidorna är skrivskyddade.

Mer information finns i [Hantera postsidans layout](/help/quicksilver/planning/records/manage-the-record-page.md).

## Fliken Ny planering i avsnittet Skickat i området Begäranden

>[!NOTE]
>
>Förhandsversion: 27 november 2024; Produktion för snabb release: Med version 24.12 (december 2024); Produktion för kvartalsvis publicering: Med version 25.1 (januari 2025)

Nu finns Workfront Planning-begäranden under Skickat i området Begäranden i Workfront. I avsnittet Skickat visas nu två flikar: förfrågningar som skickats in i Workfront på fliken Workfront och förfrågningar som skickats in med ett Workfront Planning-begärandeformulär på fliken Planning.

Du måste använda en länk till förfrågningsformuläret för att kunna lägga till förfrågningar till en posttyp i Workfront Planning. En Workfront Planning-begäran från Workfront Request-området kommer att skickas in senare.

Din organisation måste köpa ett Workfront Planning-paket innan du kan använda fliken Planering i området Begäranden.

Mer information finns i [Skicka Adobe Workfront Planning-begäranden för att skapa poster](/help/quicksilver/planning/requests/submit-requests.md).

## Ytterligare fälttyper stöds nu i förfrågningsformulär

>[!NOTE]
>
>Förhandsversion: 27 november 2024; Produktion för snabb release: Med version 24.12 (december 2024); Produktion för kvartalsvis publicering: Med version 25.1 (januari 2025)

Du kan nu lägga till följande fälttyper i ett formulär för posttypsbegäran i Workfront Planning:

* Folk
* Workfront-anslutningar

Före den här förbättringen kunde dessa typer av fält inte läggas till i förfrågningsformulär i Workfront Planning.

Mer information finns i Skapa och hantera ett begärandeformulär i Adobe Workfront Planning (/help/quicksilver/planning/requests/create-request-form.md).

## Begränsa offentlig delning av begärandeformulär som innehåller vissa fälttyper

>[!NOTE]
>
>Förhandsversion: 27 november 2024; Produktion för snabb release: Med version 24.12 (december 2024); Produktion för kvartalsvis release: Med version 25.1 (januari 2025)

Du kan inte längre dela ett begärandeformulär offentligt om formuläret innehåller någon av följande fälttyper:

* Formel
* Anslutningar
* Sökfält
* Folk

Mer information finns i [Skapa och hantera ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).


## Visa poster i kalendervyn efter vecka

>[!NOTE]
>
>Förhandsversion: 26 november 2024; Produktion för snabb release: Med version 24.12 (december 2024); Produktion för kvartalsvis release: Med version 25.1 (januari 2025)

Nu kan du visa poster i kalendervyn efter vecka. Före den här förbättringen kunde du bara visa kalendervyn per månad.

Mer information finns i [Hantera kalendervyn](/help/quicksilver/planning/views/manage-the-calendar-view.md).

## Återställ borttagna poster

>[!NOTE]
>
>Förhandsversion: 22 november 2024; Produktion för snabb release: Med version 24.12 (december 2024); Produktion för kvartalsvis release: Med version 25.1 (januari 2025)

När poster har tagits bort flyttas de nu tillfälligt till en nyligen borttagen behållare i 30 dagar. Du kan komma åt den nyligen borttagna behållaren från posttypens sida och den innehåller bara poster av en viss typ.

Workspace-hanterare kan återställa poster från papperskorgen i upp till 30 dagar efter att de tagits bort. Anslutna poster och deras fältinformation återställs också.

Det gick inte att återställa borttagna poster innan den här förbättringen utfördes.

Mer information finns i [Återställ borttagna poster](/help/quicksilver/planning/records/records-information.md).

## Adobe AI Assistant finns i informationsområdet

>[!NOTE]
>
>Förhandsversion: 21 november 2024; Produktion för snabb release: Med version 24.12 (december 2024); Produktion för kvartalsvis release: Med version 25.1 (januari 2025)

För att göra det enklare för dig att utföra arbetet har vi lagt till Adobe AI Assistant på en posts förhandsgranskning av information eller postens sida. Du kan använda AI-assistenten i en postsida för att uppdatera information om posten.

Mer information finns i [Översikt över Adobe Workfront Planning AI Assistant](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).

## Ny upplevelse när du lägger till en miniatyrbild och en omslagsbild på en postsida

>[!NOTE]
>
>Förhandsversion: 20 november 2024; Produktion för snabb release: Med version 24.12 (december 2024); Produktion för kvartalsvis release: Med version 25.1 (januari 2025)

När du öppnar en posts förhandsgranskning eller sida och posten inte har någon miniatyrbild eller omslagsbild, måste du nu hålla markören över området ovanför postens namn i rubriken för att se alternativen för att lägga till ett omslag och en miniatyrbild till posten. Före den här förbättringen visas de tomma platshållarbilderna för miniatyrbilden och omslaget ovanför postens namn.

Mer information finns i följande artiklar:

* [Lägga till en omslagsbild till en post](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
* [Lägga till en miniatyrbild i en post](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

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

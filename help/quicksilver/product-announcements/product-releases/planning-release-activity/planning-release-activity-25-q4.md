---
content-type: release-notes
title: Versionsaktivitet fjärde kvartalet 2025 för Adobe Workfront Planning
description: Detta är lanseringsaktiviteten för Adobe Workfront Planning-produkten för fjärde kvartalet 2025.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 4e1761f9-bf73-4355-925a-9136f2787a3f
source-git-commit: f7dcae5e6bcc8674ef37ef94282c50dc9ffe951d
workflow-type: tm+mt
source-wordcount: '900'
ht-degree: 0%

---

# Versionsaktivitet fjärde kvartalet 2025 för Adobe Workfront Planning

I den här artikeln beskrivs funktionerna som lanseras för Workfront Planning i den fjärde utgåvan av kvartal 2025.

<!--keep the sentence below for all future quarterly release pages-->

En lista över alla funktioner som släppts för Adobe Workfront Planning finns i [Versionsaktivitet för Adobe Workfront Planning: artikelindex](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Nya gränser för formelfält

>[!NOTE]
>
>* Förhandsgranska: 28 augusti 2025
>* Production fast release: 11 september 2025
>* Produktion för alla kunder: 16 oktober 2025

Vi har satt följande gränser för formelfält:

* Det finns en gräns på 20 formelfält per posttyp
* Ett formeluttryck får innehålla högst 50 000 tecken

Mer information finns i [Översikt över formelfält](/help/quicksilver/planning/fields/formula-fields.md).

## Visa fel när formelvärden inte kan matchas

>[!NOTE]
>
>* Förhandsgranska: 28 augusti 2025
>* Production fast release: 11 september 2025
>* Produktion för alla kunder: 16 oktober 2025

Fältet visas nu som &quot;#ERROR!&quot; för att visa att det inte går att lösa ett formelfält i något av följande fall:

* När ett fält som används i en formel tas bort.

* När ett fält som används i ett aggregerat uppslagsfält visas som #ERROR!.

* När ett formelvärde inte kan visas i det valda formatet.

Mer information finns i [Översikt över formelfält](/help/quicksilver/planning/fields/formula-fields.md).

## Nya uttryck har lagts till i formelfält i Planning

>[!NOTE]
>
>Förhandsgranska: 7 augusti 2025
>&#x200B;>Produktion för alla kunder :August, 2025
>&#x200B;>[!BADGE Frånschemat &#x200B;]{type=Neutral}

Vi har lagt till nya uttryck med följande användning i formelfält i Workfront Planning och i beräknade anpassade fält i Workfront:

* **REMOVEACCENTS(string)**: Tar bort diakritiska tecken från alla tecken med accent i indatasträngen.
* **REPLACEPATTERN (sträng, mönster, ersättningssträng)**: Ersätter matchningarna för det angivna mönstret med ersättningssträngen.
* **PASCAL(string)**: Konverterar indatasträngen till PascalCase genom att ändra den första bokstaven i varje ord till versal och ta bort alla blanksteg.

Mer information finns i [Översikt över beräknade datauttryck](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

## Lägga till Maximera och Minimera-knappar i fönstret där formelfält skapas

>[!NOTE]
>
>Förhandsgranska: 31 juli 2025
>&#x200B;>Produktion för alla kunder: 31 juli 2025
>&#x200B;>[!BADGE Frånschemat &#x200B;]{type=Neutral}

Vi har lagt till knappen Maximera för att förstora formelfältet när du skapar eller redigerar fältet i en posttabellvy. Dessutom har vi lagt till en Minimera-knapp i det nya förstorade fönstret för att återgå till rutan för att skapa fält.

Mer information finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

## Sidan Anslutna poster är nu tillgänglig i en posts förhandsgranskningsområde

>[!NOTE]
>
>* Förhandsgranska: 31 juli 2025
>* Production fast release: 14 augusti 2025
>* Produktion för alla kunder: 16 oktober 2025

Vi har nu gjort så att upplevelsen på den anslutna postsidan i förhandsvisningsrutan matchar den på sidan på hela sidan i en posts informationsområde.

Före den här förbättringen var det endast möjligt att visa anslutna poster på en sida med anslutna poster på hela sidan i en posts informationsområde.

Mer information finns i [Hantera postsidans layout](/help/quicksilver/planning/records/manage-the-record-page.md).

<!--## Updates to Requesting experience 

>[!NOTE]
>
>* Preview: July 31, 2025
>* Production fast release: August 14, 2025
>* Production for all customers: October 16, 2025

To create a better user experience when making requests in Workfront and Workfront Planning, we've updated the requesting experience. Now you can:

* View Workfront and Workfront Planning requests in a single list.
* Filter submitted requests based on criteria you specify.
* Search for and select Workfront request queues and Workfront Planning forms in a consolidated experience.
* Hide and reorder columns in the submitted requests list.

This update also features changes to the look and feel of the page.

Previously, Workfront and Workfront Planning requests were on separate tabs, and filters were not customizable.

For more information on creating requests see:

* For Workfront: [Create and submit requests](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)
* For Workfront Planning: [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md) -->

## Skapa poster i tidslinjevyn

>[!NOTE]
>
>Förhandsgranska: 24 juli 2025
>&#x200B;>Production fast release: 14 augusti 2025
>&#x200B;>Produktion för alla kunder: 16 oktober 2025

Nu kan du skapa poster i tidslinjevyn för en posttyp genom att dubbelklicka någonstans på tidslinjen.

Du kan välja datumintervall för posten eller öppna postens sida för att redigera all information.

Före den här förbättringen kunde du bara lägga till nya poster med knappen Ny post eller textbunden i tabellvyn.

Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).

## Alternativet Lägg till delning på menyn Mer för ett posttypskort

>[!NOTE]
>
>Förhandsgranska: 24 juli 2025
>&#x200B;>Production fast release: 14 augusti 2025
>&#x200B;>Produktion för alla kunder: 16 oktober 2025

Du kan nu dela en posttyp på menyn Mer på posttypskortet på arbetsytesidan. Före den här förbättringen var alternativet Dela bara tillgängligt på posttypssidan.

Mer information finns i [Dela posttyper](/help/quicksilver/planning/access/share-record-types.md).

## Visa alla Workfront Planning-vyer i helskärmsläge

>[!NOTE]
>
>Förhandsgranska: 24 juli 2025
>&#x200B;>Production fast release: 14 augusti 2025
>&#x200B;>Produktion för alla kunder: 16 oktober 2025

Nu kan du visa alla Workfront Planning-vyer (tabell, tidslinje och kalender) i helskärmsläge. Visningsfunktionen bevaras och du kan även ändra vyn i helskärmsläge.

Före den här förbättringen fanns inte den här funktionen.

Mer information finns i [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).

## Lägg till team som godkännare i planeringsförfrågningsformulär

>[!NOTE]
>
>Förhandsgranska: 22 juli 2025
>&#x200B;>Production for fast release: 14 augusti 2025
>&#x200B;>Produktion för alla kunder: 16 oktober 2025

För att göra godkännandeprocessen mer flexibel har vi lagt till möjligheten att lägga till team som godkännare i planeringsförfrågningsformulär. Nu kan du ange och välja teamnamn när du ställer in godkännare. Alla teammedlemmar kan fatta ett beslut som räknas som ett godkännandebeslut för hela teamet.

Tidigare kunde bara enskilda användare tilldelas godkännare.

Mer information finns i [Lägga till ett godkännande i ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

## Nya fält för att visa information om postgodkännande

>[!NOTE]
>
>Förhandsgranska: 17 juli 2025
>&#x200B;>Production for fast release: 14 augusti 2025
>&#x200B;>Produktion för alla kunder: 16 oktober 2025

Vi introducerar följande fält för att samla in godkännandeinformation för poster som skapats genom att skicka en begäran med ett godkännande:

* Godkänd av
* Godkännandedatum

Mer information finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

## Fyll i fält automatiskt baserat på använda grupperingar

>[!NOTE]
>
>Förhandsgranska: 10 juli 2025
>&#x200B;>Production fast release: 14 augusti 2025
>&#x200B;>Produktion för alla kunder: 16 oktober 2025


När du har använt grupperingar i en tabellvy fylls de fält som är kopplade till de grupperingar du lägger till posten i automatiskt i när du lägger till en post i tabellen.

Om du har använt flera grupperingar fylls fälten som är kopplade till alla grupperingar i automatiskt när du lägger till posten i slutet av listan i det sista grupperingsvillkoret.

Före den här förbättringen behövde du uppdatera fälten som var kopplade till grupperingar manuellt.

Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).

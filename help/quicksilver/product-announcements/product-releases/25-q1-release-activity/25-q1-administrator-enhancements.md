---
title: Förbättringar av första kvartalet 2025 för administratörer
description: Förbättringar av första kvartalet 2025 för administratörer
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: fa24040d-0403-4799-b690-c3d172797115
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 0%

---

# Förbättringar av första kvartalet 2025 för administratörer

Den här sidan beskriver alla administratörsförbättringar som gjorts i den första utgåvan av kvartal 2025 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön enligt vad som anges.

En lista över alla ändringar som är tillgängliga vid den här tidpunkten i den första utgåvan av kvartal 2025 finns i [Översikt över utgåvan första kvartalet 2025](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md).

## Affärsregler stöds nu för fler objekt

>[!NOTE]
>
>Förhandsversion: 16 januari 2025; Produktionsrelease för alla kunder: Med version 25.1 (januari 2025)
>
>_Endast tillgängligt för organisationer i Ultimate-planen._

Nu kan du skapa affärsregler och tillämpa validering på ytterligare objekt: Företag, Iteration, Resurskategori som inte är arbetsplats, Jobbroll, Användare, Tilldelning, Resurspool, Tid av, Dokument och Timme.

Följande objekt stöddes redan för affärsregler: Projekt, Aktivitet, Begäran, Portfolio, Program, Utgift, Faktureringspost, Grupp, Risk och Klassificeringskort.

Mer information finns i [Skapa och redigera affärsregler](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md).

## Jämför objekt mellan miljöer för att förbättra miljön

>[!NOTE]
>
>Förhandsversion: 6 januari 2025; Produktionsrelease för alla kunder: Med version 25.1 (januari 2025)

För att det ska bli enklare att avgöra vilket objekt som ska ingå i ett miljöbefordringspaket har vi lagt till möjligheten att jämföra objekt i olika miljöer. Nu kan du välja objekttyper och miljöer. Workfront genererar en lista med objekt av den typen, oavsett om de finns i målmiljön eller inte och om det objektet skiljer sig åt mellan källmiljön och målmiljön. Du kan sedan lägga till objekt i ett paket direkt från den här listan.

Om en användare tidigare ville jämföra objekt mellan miljöer måste de kontrollera objekten manuellt.

Mer information finns i [Jämför objekt mellan miljöer](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-compare.md).

## Fler tillgängliga objekt för miljöbefordran

>[!NOTE]
>
>Förhandsversion: 6 januari 2025; Produktionsrelease för alla kunder: Med version 25.1 (januari 2025)

Vi har lagt till fler objekt för att utöka funktionerna för miljöbefordran. Nu kan du lägga till följande objekt i ett miljöhöjdspaket:

* Platser
* Klassificeringskort
* Uppdrag

Tidigare var dessa objekt inte tillgängliga för miljöbefordran.

Mer information om tillgängliga objekt för miljöbefordran finns i [Objekt som stöds för miljöbefordran](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion) i artikeln Översikt över miljöbefordran.

## Förhindra att uppgifter flyttas när det finns timmar loggade

>[!NOTE]
>
>Förhandsversion: 19 december 2024; Produktionsrelease för alla kunder: Med version 25.1 (16 januari 2025)

Eftersom flyttningar av uppgifter eller problem som har loggade timmar ibland kan orsaka problem med regelefterlevnad eller revision, har vi lagt till en inställning under Inställningar för Aktivitet och problem i installationsprogrammet som gör att du kan förhindra användare från att flytta uppgifter och problem om det finns timmar inloggade. Före den här förbättringen kunde användare flytta uppgifter och problem till andra projekt, även om timmar var inloggade.

Mer information finns i [Konfigurera uppgifter och utgåvinställningar för hela systemet](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Inställning för att använda projekt eller användarschema för uppgifter med enkel tilldelning

>[!NOTE]
>
>Förhandsversion: 21 november 2024; Produktion för snabb release: Med version 24.12 (12 december 2024); Produktion för kvartalsvis publicering: Med version 25.1 (16 januari 2025)

Som system- eller gruppadministratör har du nu en ny inställning som anger om Workfront ska använda projektets eller användarens schema för att beräkna tidslinjen för projektet när du tilldelar en användare till en aktivitet och både projektet och användaren är associerade med ett schema. Före den här förbättringen fanns den här inställningen för fleranvändartilldelningar. Inställningen är nu tillgänglig för enanvändartilldelningar av uppgifter.

Mer information finns i [Konfigurera systemomfattande projektinställningar](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Affärsreglerna stöder nu hyperlänkar

>[!NOTE]
>
>Förhandsversion: 21 november 2024; Produktion för snabb release: Med version 24.12 (12 december 2024); Produktion för kvartalsvis publicering: Med version 25.1 (16 januari 2025)

Nu kan du inkludera hyperlänkar i det anpassade felmeddelandet för en affärsregel, som vägleder användaren om hur de kan ändra sin åtgärd inom regelbegränsningen. Den statiska URL:en kan länka till dokumentation eller andra sidor som skulle vara till hjälp för användaren.

Mer information finns i [Skapa och redigera affärsregler](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md).

## Det finns nu möjlighet att filtrera på inbyggda typsnittsfält

>[!NOTE]
>
>Förhandsversion: 21 november 2024; Produktion för snabb release: Med version 24.12 (12 december 2024); Produktion för kvartalsvis publicering: Med version 25.1 (16 januari 2025)

När du lägger till en intern fältreferens i ett anpassat formulär och den refererar till ett typsnittsfält (till exempel Portfolio, Företag eller Ägare), är nu ett filteralternativ tillgängligt. Med filtret kan du begränsa vilka objekt som användare kan välja när de använder fältet. Det här anpassade filtret fungerar på samma sätt som ett filter i ett anpassat typsnittsfält, där textläget används för att definiera filtret.

Mer information finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Ikonen &quot;Flytta till&quot; har lagts till i anpassade fält

>[!NOTE]
>
>Förhandsversion: 29 oktober 2024; Produktion för snabb release: Med version 24.11 (14 november 2024); Produktion för kvartalsvis publicering: Med version 25.1 (16 januari 2025)

När ett anpassat formulär innehåller flera avsnitt med många fält kan det vara svårt att flytta ett fält från ett avsnitt till ett annat genom att dra och släppa. En&quot;flytta till&quot;-ikon har lagts till i varje fält, så att du kan markera det avsnitt som fältet placeras i.

Mer information finns i [Ordna och förhandsgranska ett formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).

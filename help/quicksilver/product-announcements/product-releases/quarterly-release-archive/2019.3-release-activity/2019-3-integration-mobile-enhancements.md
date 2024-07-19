---
product-previous: mobile
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: 2019.3-integrering och mobilförbättringar
description: Den här sidan beskriver alla ändringar av integrering och mobilförbättringar som gjorts i version 2019.3. Den gjordes tillgänglig i produktionsmiljön den 19 augusti 2019.
author: Luke
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 15e03405-63ff-48ea-b873-cf44f1f46282
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# 2019.3-integrering och mobilförbättringar

Den här sidan beskriver alla ändringar av integrering och mobilförbättringar som gjorts i version 2019.3. Den gjordes tillgänglig i produktionsmiljön den 19 augusti 2019.

En lista över alla ändringar som gjorts under 2019.3 finns i [Översikt över versionsaktiviteten för 2019.3 ](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md).

## Stöd för delade objekt i MS OneDrive-integreringen

Nu kan du länka dina delade OneDrive-filer och -mappar till Workfront-objekt. På samma sätt kan du överföra filer i Workfront till delade mappar i OneDrive.

Mer information finns i avsnitten [Länka ett externt dokument till Workfront](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents), [Länka en eller flera externa mappar](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-a-folder) och [Uppdatera och länka ett dokument från Workfront till en extern molnleverantör](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents) i artikeln [Länka dokument från externa program](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Mer information finns i avsnittet [Länka ett externt dokument till Workfront](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) i artikeln [Länka dokument från externa program](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Domänspecifikation krävs för alla Workfront-inloggningar

Alla Workfront-inloggningar kräver nu att användaren anger domänen om domänen inte redan har angetts i Workfront URL. Om du kräver den här informationen blir din Workfront-instans säkrare. Om implementeringen av Workfront har flera instanser kan du med den här förbättringen lägga till samma användare i varje instans av Workfront i implementeringen.

Den här ändringen kan påverka både användarinloggningar och API-integreringar:

* **Användarinloggningar**

  Om företagsdomänen inte ingår i Workfront URL:er visas nu ett nytt domänfält på inloggningsskärmen förutom fälten Användarnamn och Lösenord.

  För de flesta kunder krävs ingen ändring eftersom domäninformationen redan finns i Workfront URL. Exempel: *domän*.my.workfront.com.

* **API-integreringar**

  Om du har en API-kod som går till en adress som inte innehåller ditt domännamn, kommer den API-koden inte längre att fungera.

Mer information finns i [Logga in på Adobe Workfront](../../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/log-in-to-workfront.md).

## Konvertera uppgifter och ärenden till projekt med mobilappen på iOS

Nu kan du konvertera enskilda uppgifter och ärenden till projekt i Workfront mobilapp på iOS.

## Logga in på mobilappen med fingeravtryck eller ansikte-ID

Beroende på din enhet kan du välja att logga in på Workfront mobilapp med fingeravtryck eller ID-teknik för ansikte. När du loggar in på mobilappen tillfrågas du om du vill logga in med den autentiseringsmetod som telefonen stöder.

Mer information om hur du hanterar den här funktionen finns i [Adobe Workfront för iOS](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md) eller [Adobe Workfront för Android](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md).

## Ny inställning för automatisk utloggning av användare på mobilen

För att göra Workfront mobilapp säkrare för dig och ditt företag loggas användare ut automatiskt efter 15 dagars inaktivitet. Workfront-administratörer kan anpassa den här tidsgränsen i webbprogrammet under Konfigurera > System > Inställningar.

Mer information finns i [Konfigurera systemsäkerhetsinställningar](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Mobilappen kräver domän vid inloggning

Som en säkerhetsförbättring kräver nu Workfront Mobile App att du anger din domän om du inte loggar in med inloggningsuppgifter för enkel inloggning.

>[!NOTE]
>
>iOS: 12 juni 2019
>
>Produktionstillgänglighet: 17 juni 2019

## Ta bort objekt med mobilappen på iOS

>[!NOTE]
>
>Den här funktionen var tillgänglig i appbutikerna för iOS den 19 augusti 2019.

Nu kan du ta bort objekt som uppgifter, problem och tidrapporter i iOS mobilapp. Du måste ha rätt behörighet för objektet för att kunna ta bort det.

## Filtrera efter avancerade projekt i mobilappen

>[!NOTE]
>
>Den här funktionen kommer att vara tillgänglig i appbutikerna för både iOS och Android den 19 augusti 2019.

Vi har lagt till döda projekt som ett filteralternativ på fliken Projekt i mobilappen.

## Återställ lösenordet med mobilappen

Du kan använda appen Workfront Mobile för att återställa ditt lösenord om du har glömt det. Tryck på Har du glömt lösenordet? och följ anvisningarna på skärmen. Du kan inte återställa ditt SSO-lösenord i mobilappen.

## Nytt utseende och känsla för mobilen

Vi har lagt till följande förbättringar av utseende och känsla för att förbättra din upplevelse av Workfront mobilapp.

* Flyttade följande från det övre fältet på detaljsidan till mer framträdande områden på skärmen:

   * Plustecknet finns nu längst ned till vänster på skärmen
   * Den bockmarkering som används för att börja arbeta med ett objekt är nu en Work On It-knapp i skärmens övre mitt

* Nu kan du visa kopplade anpassade formulär genom att trycka på Visa mer längst ned på detaljsidan.
* Utseendet på sidorna som du använder för att skicka uppgifter, utgåvor och förfrågningar har ändrats.


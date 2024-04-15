---
title: Andra kvartalet 2024 - administratörsförbättringar
description: Andra kvartalet 2024 - administratörsförbättringar
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a297ee8d-d949-45ab-a219-437316fa8fa3
source-git-commit: a1386652f5181d4aa94ddab8e4f9714ef1c08b73
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 0%

---

# Andra kvartalet 2024 - administratörsförbättringar

Den här sidan beskriver alla administratörsförbättringar som gjorts i andra utgåvan av kvartalet 2024 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön enligt vad som anges.

En lista över alla ändringar som är tillgängliga vid den här tidpunkten i den andra utgåvan av kvartal 2024 finns på [Andra utgåvan, kvartal 2024, översikt](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).

## Visningslogik och hopplogik är nu tillgängliga i formulärdesignerns förhandsgranskningsläge

>[!NOTE]
>
>Förhandsversion: 28 mars 2024; Produktion för alla kunder: 24.4 (11 april 2024)

Med den anpassade betaversionen av formulär kan du nu testa visningslogiken och hoppa över logiken i förhandsgranskningsläget. Tidigare visades alla fält i förhandsgranskningen även när logiken tillämpades.

Mer information om hur du förhandsgranskar ett anpassat formulär i formulärdesignern finns i [Organisera och förhandsgranska ett formulär med formulärdesignern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).

## Företag och användare har nu stöd för avancerade anpassade formulärfält

>[!NOTE]
>
>Förhandsversion: 14 mars 2024; Produktion för alla kunder: 24.4 (11 april 2024)

Avancerade anpassade formulärfunktioner som externa sökningsfält och inbyggda Workfront-fält är nu tillgängliga när du bifogar ett anpassat formulär till ett företag eller en användare. De avancerade funktionerna finns på sidorna Företagsinformation och Användarinformation, inte i dialogrutorna Redigera företag och Redigera användare. Det anpassade formuläret måste skapas i den nya formulärdesignern för att du ska kunna utnyttja dessa fälttyper.

Mer information om anpassade formulärfält finns i [Designa ett formulär med formulärdesignern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Integrering med JumpSite är nu tillgängligt för nya pakettyper

>[!NOTE]
>
>Förhandsversion: 26 februari 2024; Produktion för snabb release: Med version 24.3 (14 mars 2024); Produktion för alla kunder: 24.4 (11 april 2024)

Den befintliga JumpSeat-integreringen är nu tillgänglig för konton med någon av de nya pakettyperna (dvs. Select, Prime eller Ultimate). Du måste fortfarande ha en aktiv JumpSite-prenumeration för att kunna aktivera integreringen.

Mer information om JumpSeat-integrering finns i [Konfigurera JumpSeat-integrering](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## Workfront inbyggda fält är tillgängliga i betaversionen av formulärdesignern

>[!NOTE]
>
>Förhandsversion: 29 februari 2024; Produktion för snabb release: Med version 24.3 (14 mars 2024); Produktion för alla kunder: 24.4 (11 april 2024)

Nu kan du lägga till fält som är inbyggda i Workfront i dina anpassade formulär. Med den här nya fälttypen kan du ordna och presentera data för användarna på ett logiskt sätt, utan att behöva återskapa befintliga data i anpassade fält.

När du har valt Inbyggt fält i listan med anpassade formulärfält för att lägga till fältet i formulärdesignern, kan du välja vilket inbyggt fält som helst för formulärets objekt. Om t.ex. listan Objekttyper längst upp i formulärdesignern visar Projekt, kan du välja inbyggda fält för projekt, men inte fält som är specifika för uppgifter.

När det anpassade formuläret bifogas till ett objekt fylls fältet i från objektdata. Fältet Beskrivning i ett anpassat formulär som är kopplat till ett projekt hämtas till exempel i projektbeskrivningen. (Fältet kan visa &quot;Ej tillämpligt&quot; om inga data är tillgängliga.)

Inbyggda fält som används i anpassade formulär blir tillgängliga i fältbiblioteket i designern för återanvändning. De visas också i området Inställningar > Anpassad Forms > Fält så att du kan se vilka formulär de används i.

Den här funktionen är bara tillgänglig i betaversionen av formulärdesignern, inte i det äldre formulärverktyget.

Mer information finns i [Designa ett formulär med formulärdesignern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

[Visa en videodemonstration av den här funktionen.](https://video.tv.adobe.com/v/3427702/){target=_blank}

## Attributmappning är nu tillgänglig för organisationer som har migrerat till Adobe IMS

>[!NOTE]
>
>Förhandsversion: 22 februari 2024; Produktion för alla kunder: 22 februari 2024

Workfront systemadministratörer kan nu konfigurera mappning av användarattribut för organisationer som har migrerat till Adobe IMS. Detta gör att användarinformation kan skickas till Workfront från organisationens SSO-leverantör (Single Sign-on), så att användarens data inte behöver anges i både Workfront och SSO-providern.

Tidigare var den här funktionen bara tillgänglig för organisationer som ännu inte börjat använda Adobe IMS.

Instruktioner om hur du konfigurerar attributmappning finns i [Mappa användarattribut i Adobe enhetliga upplevelse](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md#map-user-attributes-in-the-adobe-unified-experience) i artikeln **Mappa användarattribut och autodistribuera nya användare**.

## Hopplogik och visningslogik finns nu i betaversionen av formulärdesignern

>[!NOTE]
>
>Förhandsversion: 8 februari 2024; Produktion för snabb release: Med version 24.2 (15 februari 2024); Produktion för alla kunder: 24.4 (11 april 2024)

Nu kan du redigera befintlig visnings- och hopplogik och lägga till ny logik i anpassade formulär i betaversionen av formulärdesignern. Ett lättanvänt logiskt verktyg hjälper dig att definiera vilka fält som ska visas eller hoppas över baserat på val i formuläret.

Ikoner i ett fält på formulärdesignerns arbetsyta anger att logiken är konfigurerad i det fältet eller att fältet används i logikregler som är konfigurerade för andra fält.

Mer information finns i [Lägg till visningslogik och hoppa över logik med formulärdesignern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).

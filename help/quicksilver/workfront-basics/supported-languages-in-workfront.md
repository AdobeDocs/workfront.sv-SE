---
content-type: reference
navigation-topic: get-started-with-workfront
title: Språk som stöds i Adobe Workfront
description: Du kan ändra vilket språk som används för att visa Adobe Workfront och e-postmeddelanden från Workfront genom att justera språkinställningarna i webbläsaren och ditt standardspråk för e-post i Workfront.
feature: Get Started with Workfront
author: Becky
exl-id: 0b76175f-5fe2-49df-b605-68e6e66b4366
source-git-commit: 976cfce04c2dd4526265f9427007b97a768c8d6a
workflow-type: tm+mt
source-wordcount: '1137'
ht-degree: 0%

---

# Språk som stöds i Adobe Workfront

Du kan ändra vilket språk som används för att visa Adobe Workfront och e-postmeddelanden från Workfront genom att ändra språkinställningarna i webbläsaren (om din organisation inte har migrerats till Adobe Admin Console) eller språkinställningarna för din Adobe Experience Cloud-profil (om du använder Adobe Admin Console) och ditt standardspråk för e-postmeddelanden i Workfront.

Mer information om hur du ändrar vilket språk du visar arbetsytan på finns i [Ändra språket](#change-the-language) i den här artikeln.

Workfront terminologi uppdateras för de språk som stöds i varje Workfront-uppdatering.

Workfront har stöd för följande språk:

* Engelska (en-US)
* Franska (fr-FR)
* Tyska (de-DE)
* Japanska (ja-JP)
* Spanska (es-ES)
* Italienska (IT-IT)
* Portugisiska (pt-BR)
* Koreanska (ko-KR)
* Kinesiska - förenklad (zh-CN)
* Kinesiska - traditionell (zh-TW)

Det språk som används för att visa Workfront i din webbläsare styrs av språkinställningarna i webbläsaren om organisationen inte befinner sig i Adobe Admin Console, eller av ditt profilspråk i Adobe Experience Cloud om organisationen finns i Adobe Admin Console. I båda fallen måste du välja ett språk som visas i listan med språk som stöds.

Om du vill visa utgående e-post på något av de språk som stöds ändrar du inställningarna för e-postadress för användare eller kundinformation i Workfront.\
Du måste vara Workfront-administratör för att kunna ändra inställningarna för kundinformation.\
Mer information om hur du ändrar kundinformation och språkområde för e-post för användare finns i [Ändra språkområdet för e-post för Workfront och användare](#change-the-workfront-and-user-locales).

Du kan kontraktera en tredje part om du vill att Workfront gränssnitt och utgående e-post från Workfront ska översättas till andra språk. Dessa översättningar stöds inte av Workfront och alla andra språk än de som listas ovan stöds inte.

>[!NOTE]
>
>Delar av gränssnittet kan fortfarande vara oöversatta för följande:
>
>* När du använder ett språk som inte stöds visas gränssnittet på engelska
>* Hjälpmenyn, samt hjälpinnehållet som öppnas från den menyn, visas på engelska
>* Den text som användaren skriver behålls på det språk som angavs i originalet. Detta kan omfatta, men är inte begränsat till:
>
>   * Projektnamn
>   * Uppgiftsnamn
>   * Ärendenamn
>   * Portfolio names
>   * Programnamn
>   * Godkännandenamn
>   * Beskrivning
>   * Anpassade formulärnamn
>   * Namn på timtyper
>   * Utgiftstyper
>   * Milstolpar
>   * Egna flikar
>   * Status
>   * Rapportnamn
>

## Språkavvikelser som stöds vid korrektur

Web Proofing Viewer i Workfront stöder de flesta språk som stöds i Workfront.

Följande språk stöds inte i språkverktyget:

* Kinesiska - traditionell (zh-TW)
* Koreanska (ko-KR)

Ditt företag måste köpa en korrekturlicens för att du ska kunna använda Web Proofing Viewer.

Mer information om korrektur finns i [Korrektur](../review-and-approve-work/proofing/proofing.md).

När du visar Workfront på ett språk som inte stöds i korrekturverktyget visas Web Proofing Viewer på engelska.

Om du använder Workfront Proof (det fristående korrekturläsningsverktyget) på ett språk som inte stöds i Workfront visas Web Proofing Viewer i Workfront på engelska.\
Mer information om vilka språk som stöds i Workfront Proof finns i [Språkinställningar i Workfront Proof](../workfront-proof/wp-getstarted/system-information/language-settings.md).

## Språk som stöds i Adobe Workfront Fusion

För närvarande stöder Workfront Fusion endast engelska.

* Allt innehåll i Workfront Fusion, samt allt hjälpinnehåll som rör Workfront Fusion, visas på engelska.
* Workfront Fusion stöder inte användning av icke-engelska texttecken i fält som användaren anger.

Företaget måste köpa en Workfront Fusion-licens för att få tillgång till Workfront Fusion.\
Mer information om Workfront Fusion finns i [Adobe Workfront Fusion - översikt](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).

## Ändra språk

Du kan ändra det språk som används för att visa Workfront och det språk som används i utgående e-postmeddelanden genom att ändra följande inställningar:

* Språket i webbläsaren (för användare som inte befinner sig i Adobe Admin Console)
* Det primära och sekundära språket i din AEM-profil (för användare på Adobe Admin Console)
* Inställningarna för kundinformation och användarens e-postadress i ditt Workfront-konto.

För att se alla tillgängliga översättningar för ditt valda språk bör både Workfront nationella inställningar och webbläsarens nationella inställningar anges till samma språk.

Om du vill ta reda på om din organisation har migrerats till Adobe Admin Console kan du kontrollera den URL som du använder för att visa Workfront.

| URL | Adobe Experience | Språkkontroll |
|---|---|---|
| (CompanyName).my.workfront.com | Inte migrerad till Adobe Admin Console | [Ändra webbläsarspråk](#change-the-browser-language) |
| experience.adobe.com | Migrerad till Adobe Admin Console | [Ändra Adobe Experience Cloud-språk](#change-the-adobe-experience-cloud-language) |

* [Ändra webbläsarspråk](#change-the-browser-language)
* [Ändra Adobe Experience Cloud-språk](#change-the-adobe-experience-cloud-language)
* [Ändra e-postadresser för Workfront och användare](#change-the-workfront-and-user-locales)

### Ändra webbläsarspråk {#change-the-browser-language}

Om din organisation inte har migrerats till Adobe Admin Console visas ditt Workfront-gränssnitt på det språket när du byter webbläsarspråk.\
Mer information om vilka språk som stöds av Workfront finns i [Språk som stöds i Adobe Workfront](#supported-languages).

Webbläsarspråket måste ändras för enskilda användare.

Se hjälpmenyn för din webbläsare för mer information om hur du byter språk i din webbläsare.

### Ändra Adobe Experience Cloud-språk

Om din organisation har migrerats till Adobe Admin Console avgör ditt Adobe Experience Cloud-profilspråk vilket språk som visas i Workfront.

1. Klicka på din profilbild längst till höger i verktygsfältet i Adobe Experience Cloud och klicka sedan på **Inställningar**. Adobe Experience Cloud-verktygsfältet finns direkt ovanför Workfront huvudverktygsfält.

1. Klicka på namnet på det valda språket under **Profil** under ditt namn och din e-postadress.

1. Välj önskade språk i listrutorna **Första språket** och **Andra språket**. Det första språket är ditt standardspråk, medan det andra språket bara visas om det första språket inte stöds av ett visst program.

### Ändra e-postadresser för Workfront och användare {#change-the-workfront-and-user-locales}

* [Ändra standardspråk för e-post för Workfront](#change-the-workfront-locale)
* [Ändra användarens e-postspråk](#change-the-user-locale)

### Ändra standardspråk för e-post för Workfront {#change-the-workfront-locale}

När du ändrar Workfront standardspråk för e-post ändrar du det språk, datum och nummer som används i utgående meddelanden för alla Workfront-användare. Dessa inställningar blir standard för alla nya användare som du skapar.

Så här ändrar du Workfront standardspråk för e-post:

1. Logga in på Workfront som Workfront-administratör.

{{step-1-to-setup}}

1. Klicka på **System** > **Kundinformation.**

1. I avsnittet **Grundläggande information** klickar du på listrutan **Standardspråk för e-post** för att välja det språk som du vill att Workfront-e-postmeddelanden ska visas i.

1. Klicka på **Spara**.

### Ändra användarens e-postspråk {#change-the-user-locale}

När du ändrar ditt språkområde för e-post för användare ändrar du språk, datum och nummerformat som används i dina utgående meddelanden. De här inställningarna åsidosätter de systeminställningar som har valts under Kundinformation i installationsprogrammet.

>[!NOTE]
>
>När din organisation använder Adobe Unified Experience lagras språkinställningarna i din Adobe-profil och e-postspråkinställningen används inte. Se [Ändra Adobe Experience Cloud ](#change-the-adobe-experience-cloud-language) i den här artikeln.

Så här ändrar du din e-postadress för användare:

{{step1-click-main-menu}}

1. Klicka på din användarprofilbild.

1. Klicka på menyn Mer ![](assets/more-icon.png) och sedan på **Redigera**.

1. I avsnittet **Inställningar** klickar du på listrutan **Språk för e-post** för att välja det språk som du vill att Workfront-e-postmeddelanden ska visas i.

1. Klicka på **Spara ändringar**.

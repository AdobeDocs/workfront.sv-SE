---
product-area: documents
navigation-topic: proofing-overview
title: Granska interaktivt innehåll i tillägget för webbkorrektur
description: Adobe Workfront granskningsverktyg är ett webbläsartillägg som gör att du kan kontrollera interaktivt innehåll i en ZIP-fil eller med en URL.
author: Courtney
feature: Digital Content and Documents
exl-id: 4fea13cc-2d56-466e-8851-6134782e7e80
source-git-commit: 78d9e8e47f8f6777f9211d8f85a3dfbc9405d798
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# Granska interaktivt material med Adobe Workfront granskningsverktyg


>[!IMPORTANT]
>
> Vi rekommenderar att du använder Desktop Proofing Viewer för interaktivt innehåll som finns på en webbplats som kräver SSO-autentisering eller som förhindrar att webbplatsen öppnas i iFrames, till exempel Figma.

Adobe Workfront granskningsverktyg är ett webbaserat webbläsartillägg som gör att du kan markera interaktivt innehåll i en ZIP-fil eller med en URL. Adobe Workfront granskningsverktyg finns i följande webbläsare:

* Firefox
* Chrome
* Edge
* Safari

## Installera tillägget

### Förutsättningar

* Du måste ta bort det äldre tillägget för Web Viewer för att kunna använda verktyget Adobe Workfront Review.

### Installera tillägget

Granskare och godkännare måste installera Adobe Workfront granskningsverktyg. i någon av följande webbläsare:

* [Firefox-tillägg](https://addons.mozilla.org/en-US/firefox/addon/adobe-workfront-review-tool/)

* [Chrome-tillägg](https://chromewebstore.google.com/detail/adobe-workfront-review-to/lhdepbgeilldghlfnankdnponhljpgml)

* [Edge](https://microsoftedge.microsoft.com/addons/detail/adobe-workfront-review-to/llhapmaiiddmcamgeapaipjpagnoijen)

* [Safari-tillägg](https://apps.apple.com/us/app/adobe-workfront-review-tool/id6741517062?mt=12)



För att interaktiva korrektur ska kunna öppnas automatiskt i Adobe Workfront granskningsverktyg måste en Workfront-administratör uppdatera korrekturinställningarna på arbetsytan enligt beskrivningen i avsnitten nedan.

## Använda Adobe Workfront granskningsverktyg i GenStudio for Performance Marketing och Creative Cloud Express

Det här tillägget krävs för att granska innehåll i GenStudio for Performance Marketing och Creative Cloud Express. Assets öppnas automatiskt i Web Viewer. Du behöver inte uppdatera några kontoinställningar.


## Uppdatera standardvärden för Workfront-korrektur

Om du vill använda Workfront granskningsverktyg som standardvisningsprogram för interaktivt innehåll måste du uppdatera standardinställningarna för korrektur i Workfront.

>[!IMPORTANT]
>
>Vi rekommenderar att du använder Desktop Proofing Viewer om innehållet du behöver granska finns på en webbplats som
>
>* Kräver SSO-autentisering
>* Förhindrar att deras plats öppnas i iFrames, t.ex. Figma

### Använd Adobe Workfront granskningsverktyg som standardvisningsprogram för URL- och ZIP-korrektur

Om du vill använda webbgranskningsverktyget för URL- och ZIP-korrektur måste en Workfront-administratör justera standardinställningen för interaktiva korrektur.

1. Klicka på **Korrektur** på Workfront huvudmeny.
1. Klicka på **Kontoinställningar** och sedan på fliken **Inställningar** .
1. I avsnittet **Korrekturinställningar** letar du reda på **Desktop Proofing Viewer for Interactive proofing** och klickar på **Setup**.
1. Välj **Inaktiverad** i listrutan. Interaktiva korrektur som skapats från en URL- eller ZIP-fil öppnas nu automatiskt i Adobe Workfront Review-verktyget, som är en webbaserad webbläsare.
1. Klicka på **Spara**.

>[!NOTE]
>
>Den här ändringen gäller för alla interaktiva korrektur i din Workfront-instans. Vi rekommenderar att du testar den nya upplevelsen i förhandsvisningsmiljön innan du aktiverar den i Production. Du kan enkelt växla tillbaka till Desktop Viewer genom att ändra kontoinställningen **Desktop Proofing Viewer for Interactive proofing** tillbaka till **Aktiverad för alla interaktiva korrektur**.

### Använd Adobe Workfront granskningsverktyg som standardvisningsprogram endast för ZIP-korrektur

Om du bara vill använda webbgranskningsverktyget för ZIP-korrektur måste en Workfront-administratör justera standardinställningen för interaktiva korrektur.

1. Klicka på **Korrektur** på Workfront huvudmeny.
1. Klicka på **Kontoinställningar** och sedan på fliken **Inställningar** .
1. I avsnittet **Korrekturinställningar** letar du reda på **Desktop Proofing Viewer for Interactive proofing** och klickar på **Setup**.
1. Välj **Endast aktiverad för interaktiva korrektur som skapats från en URL** i listrutan. Interaktiva korrektur som skapats från en ZIP-fil öppnas nu automatiskt i Adobe Workfront Review-verktyget, som är en webbaserad webbläsare. Interaktiva korrektur som skapats från en URL-adress är fortfarande öppna i Desktop Proofing Viewer.
1. Klicka på **Spara**.

>[!NOTE]
>
>Den här ändringen gäller för alla ZIP-korrektur i din Workfront-instans. Vi rekommenderar att du testar den nya upplevelsen i förhandsvisningsmiljön innan du aktiverar den i Production. Du kan enkelt växla tillbaka till Desktop Viewer genom att ändra kontoinställningen **Desktop Proofing Viewer for Interactive proofing** tillbaka till **Aktiverad för alla interaktiva korrektur**.


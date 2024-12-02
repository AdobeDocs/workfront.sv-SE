---
product-area: documents
navigation-topic: proofing-overview
title: Granska interaktivt innehåll i tillägget för webbkorrektur
description: Adobe Workfront granskningsverktyg är ett webbläsartillägg som gör att du kan kontrollera interaktivt innehåll i en ZIP-fil eller med en URL.
author: Courtney
feature: Digital Content and Documents
exl-id: 4fea13cc-2d56-466e-8851-6134782e7e80
source-git-commit: 9bc1502149d99624d8494aef86e11e18a95f563b
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# Granska interaktivt material med Adobe Workfront granskningsverktyg

<span class="preview">Adobe Workfront Review Tool will be available on November 7, 2024. Det här tillägget är för närvarande i betaversion.</span>

Adobe Workfront granskningsverktyg är ett webbaserat webbläsartillägg som gör att du kan kontrollera interaktivt innehåll i en ZIP-fil eller med en URL. Adobe Workfront granskningsverktyg finns i följande webbläsare:

* Firefox
* Chrome
* Edge

Vi rekommenderar att du använder Desktop Proofing Viewer om innehållet du behöver granska finns på en webbplats som

* Kräver SSO-autentisering
* Förhindrar att deras webbplats öppnas i iFrames, t.ex. Figma



## Använd Adobe Workfront granskningsverktyg som standardvisningsprogram för URL- och ZIP-korrektur

Om du vill använda webbgranskningsverktyget för URL- och ZIP-korrektur måste en Workfront-administratör justera standardinställningen för interaktiva korrektur.

1. Klicka på **Korrektur** på Workfront huvudmeny.
1. Klicka på **Kontoinställningar** och sedan på fliken **Inställningar** .
1. I avsnittet **Korrekturinställningar** letar du reda på **Desktop Proofing Viewer for Interactive proofing** och klickar på **Setup**.
1. Välj **Inaktiverad** i listrutan. Interaktiva korrektur som skapats från en URL- eller ZIP-fil öppnas nu automatiskt i Adobe Workfront Review-verktyget, som är en webbaserad webbläsare.
1. Klicka på **Spara**.

>[!NOTE]
>
>Den här ändringen gäller för alla interaktiva korrektur i förhandsgransknings- och produktionsmiljöer. Vi rekommenderar att du testar den nya upplevelsen i förhandsvisningsmiljön innan du aktiverar den i Production. Du kan enkelt växla tillbaka till Desktop Viewer genom att ändra kontoinställningen till **Aktiverad för alla interaktiva korrektur**.

## Använd Adobe Workfront granskningsverktyg som standardvisningsprogram endast för ZIP-korrektur

Om du bara vill använda webbgranskningsverktyget för ZIP-korrektur måste en Workfront-administratör justera standardinställningen för interaktiva korrektur.

1. Klicka på **Korrektur** på Workfront huvudmeny.
1. Klicka på **Kontoinställningar** och sedan på fliken **Inställningar** .
1. I avsnittet **Korrekturinställningar** letar du reda på **Desktop Proofing Viewer for Interactive proofing** och klickar på **Setup**.
1. Välj **Endast aktiverad för interaktiva korrektur som skapats från en URL** i listrutan. Interaktiva korrektur som skapats från en ZIP-fil öppnas nu automatiskt i Adobe Workfront Review-verktyget, som är en webbaserad webbläsare. Interaktiva korrektur som skapats från en URL-adress är fortfarande öppna i Desktop Proofing Viewer.
1. Klicka på **Spara**.

>[!NOTE]
>
>Den här ändringen gäller för alla interaktiva korrektur i förhandsgransknings- och produktionsmiljöer. Vi rekommenderar att du testar den nya upplevelsen i förhandsvisningsmiljön innan du aktiverar den i Production. Du kan enkelt växla tillbaka till Desktop Viewer genom att ändra kontoinställningen till **Aktiverad för alla interaktiva korrektur**.

## Installera tillägget

Granskare och godkännare måste installera Adobe Workfront granskningsverktyg. i någon av följande webbläsare:

* [Firefox-tillägg](https://addons.mozilla.org/en-US/firefox/addon/adobe-workfront-review-tool/)

* [Chrome-tillägg](https://chromewebstore.google.com/detail/adobe-workfront-review-to/lhdepbgeilldghlfnankdnponhljpgml)

* [Edge](https://microsoftedge.microsoft.com/addons/detail/adobe-workfront-review-to/llhapmaiiddmcamgeapaipjpagnoijen)

När du har installerat tillägget öppnas interaktiva korrektur automatiskt i Adobe Workfront granskningsverktyg.

>[!IMPORTANT]
>
>Du måste ta bort det äldre tillägget för Web Viewer för att kunna använda verktyget Adobe Workfront Review.

---
title: Integreringsförbättringar för första kvartalet 2024
description: Integreringsförbättringar för första kvartalet 2024
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0d581f3c-2aaf-4ac1-97a5-df1b01627080
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Integreringsförbättringar för första kvartalet 2024

Den här sidan beskriver alla integreringsförbättringar som gjorts i den första utgåvan av kvartal 2024 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön i den första utgåvan av kvartal 2024.

En lista över alla ändringar som är tillgängliga vid den här tidpunkten i den första utgåvan av kvartal 2024 finns i [Översikt över utgåvan första kvartalet 2024](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).

## För att mappa metadata i Experience Manager Assets Essentials används nu `xcm:keywords` i stället för `dc:subject`

Vi har uppdaterat integreringen av Experience Manager Assets Essentials så att den matchar upplevelsen i Experience Manager Assets as a Cloud Service integrering. När du mappar flera enkelradiga textfält till ett enda fält i Experience Manager Assets använder båda tjänsterna nu fältet `xcm:keywords`.

Tidigare mappades dessa fält till fältet `dc:subject` i Experience Manager Assets Essentials. Experience Manager Assets as a Cloud Service funktioner är oförändrade.

Alla Experience Manager Assets Essentials-metadata som är mappade till `dc:subject` måste mappas om till `xcm:keywords`.

Mer information om att mappa metadata till Experience Manager Assets Essentials finns i [AEM nyckelord](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md#aem-keyword).

## Typsnittsfält är nu tillgängliga i Adobe Experience Manager Integration

För att göra det enklare att länka fält mellan Workfront och Adobe Experience Manager har vi lagt till stöd för typsnittsfält i metadatamappningen. Nu kan du mappa typsnittsfält till motsvarande fält i Adobe Experience Manager.

Om en användare väljer ett annat värde för ett fält i Workfront återspeglas ändringen direkt i Adobe Experience Manager. Om ett fältvärdesalternativ ändras (till exempel om ett team ändrar namnet till ett nytt namn) återspeglas dessutom ändringen i Adobe Experience Manager.

Mer information och instruktioner om metadatamappning i Adobe Experience Manager-integreringen finns i [Konfigurera metadata](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-metadata-optional).

## Publicera material automatiskt i Adobe Experience Manager

Vi har lagt till ytterligare ett arbetsflöde i Adobe Experience Manager-integreringen. Nu kan du ange att dina resurser ska publiceras automatiskt när de skickas till Adobe Experience Manager. Integrationen kan konfigureras för att publicera till Adobe Experience Manager publiceringstjänst eller till en Adobe Experience Manager varumärkesportal.

Det automatiska Publish-arbetsflödet kan aktiveras och konfigureras i Adobe Experience Manager-integreringen. När det här alternativet är aktiverat kan arbetsflödet redigeras på projektmallen eller projektnivån.

Mer information finns i [Publicera resurser](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md#publishing-assets) i [Använda arbetsflöden i Experience Manager Assets-integrering](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).

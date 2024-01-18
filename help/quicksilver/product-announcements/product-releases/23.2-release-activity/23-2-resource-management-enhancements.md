---
title: 23.2 Förbättrad resurshantering
description: 23.2 Förbättrad resurshantering
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: b225ae19-eee7-4329-a42d-2a2bf9adad01
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# 23.2 Förbättrad resurshantering

Den här sidan beskriver alla förbättringar av resurshanteringen som gjorts i version 23.2 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön med version 23.2.

En lista över alla ändringar som är tillgängliga i version 23.2 finns i [23.2 Versionsöversikt](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

## Introduktion till fältet Arbetstid för korrekt beräkning av användarkapacitet

>[!NOTE]
>
>Förhandsversion: 16 februari 2023; Planerad produktionsversion: 2 mars 2023

För att resursansvariga ska kunna beräkna tillgängligheten för sina användare och ta hänsyn till den tid som användarna lägger ner på faktiskt, projektrelaterat arbete introducerar vi arbetstidsbegreppet för Adobe Workfront.

Du kan definiera värdet för fältet Arbetstid för varje användare när du skapar eller redigerar deras profil. Mer information finns i [Redigera en användares profil](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Fältet Arbetstid representerar den procentandel av heltidsekvivalent (FTE) tid som användaren är tillgänglig för faktiskt arbete, exklusive extrakostnader. Arbetstiden måste vara ett decimaltal med ett värde mellan 0 och 1. Exempel: 20 % tillgänglighet för faktiskt arbete är 0,2.

Fältets standardvärde är 1, vilket anger att en användare tillbringar hela sitt heltidsanställda på faktiskt, projektrelaterat arbete.

Som ett resultat av den här uppdateringen beräknar Workfront användarens tillgänglighet med formlerna nedan, beroende på vad du har valt i området Resurshantering:

* Standardschema:
* Användarkapacitet = [(Schemalagda timmar - schemalagda undantag) * FTE - ledig tid] * Arbetstid
* Användarens schema:
* Användarkapacitet = (schemalagda timmar - schemalagda undantag - ledig tid) * Arbetstid.

Mer information finns i [Konfigurera [!UICONTROL Resource Management] inställningar](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

[Visa en videodemonstration av den här funktionen](https://video.tv.adobe.com/v/3415608/){target=_blank}

---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Exportera historikdata från Adobe Workfront: pros and Cons'
description: I den här artikeln förklaras för- och nackdelarna med fyra alternativ som du kan använda för att exportera historiska data från Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---

# Exportera historiska data från [!DNL Adobe Workfront]: för- och nackdelar

<!-- Audited: 5/2025 -->

I den här artikeln förklaras för- och nackdelarna med fyra alternativ som du kan använda för att exportera historiska data från Adobe Workfront.

## Använd en av våra partners

[!DNL AtAppStore] ([www.atappstore.com](https://www.atappstore.com)) har en lättanvänd app (deras [Workfront Snapshot](https://store.atappstore.com/product/workfront-snapshot/)-lösning) som gör att du kan hämta dina data själv. Med ett valfritt visningsprogram (deras [Workfront Snapshot Viewer](https://store.atappstore.com/product/workfront-snapshot-viewer/) -lösning) kan du enkelt visa dina data offline.

* **Pros:** Alla dina [!DNL Workfront] huvudobjekt exporteras, inklusive anpassade fält och anteckningar, och lagras i en lättillgänglig [!DNL MS Access]-databas. Visningsprogrammets gränssnitt är enkelt att använda och läsa. Extrahering av dokument är också tillgängligt separat som en tjänst, där utdata är ordnade i en logisk mappstruktur som mappar till varje dokument och dess tidigare versioner.

* **Kon:** Det finns en teknisk begränsning på 2 GB data, men med AtAppStore kan du endast köpa det du behöver.

* **Kostnader:** Mer information finns på [https://store.atappstore.com/product/workfront-snapshot/](https://store.atappstore.com/product/workfront-snapshot/).



## Exportera via [!UICONTROL Kick-Starts]

Oavsett om du har öppethållande på distans eller inte, kan du använda en av våra konsulter för att exportera data i form av rapporter eller [!UICONTROL kick-starts], eller så kan du själv köra dessa rapporter:

* **Pros**: Rapporterna är enkla att läsa och kan importeras i flera olika program. De kan anpassas så att de innehåller grupperingar och vyer som du vill ha.

* **Kon**: Dokument måste hämtas separat.

* **Kostnad**: Det är gratis om du kan köra rapporterna själv (allt du behöver är en systemadministratörsinloggning) eller om du kan använda återstående konsulttjänster på distans. Om du är intresserad av att köpa fjärrrådgivning för detta kan du tala med din AE/CAE.

  Mer information om hur du använder Quick-Starts för att exportera data finns i [Exportera data från [!DNL Adobe Workfront] via [!UICONTROL Kick-Starts]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## Använd vårt öppna API

Om ni har rätt resurser i er organisation kan de skapa ett anpassat API för att hämta alla era data från Workfront:

* **Pros**: Du har kontroll över vilka exporter som görs från systemet.

* **Kon**: Den tid du tillbringar läggs på dig, och du måste hitta resurser för att koda API:t och utföra exporten.

* **Kostnad**: Den är intern för din organisation.

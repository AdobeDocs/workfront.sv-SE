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
source-git-commit: 7f0aac7c8519b1e570e29fedf1492918e8120ad2
workflow-type: tm+mt
source-wordcount: '548'
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

## Begär en [!DNL Postgres]-datadumpfil från vårt databasteam

Du måste skicka en begäran till vårt kundsupportteam, som sedan skickar en begäran till vårt databasteam om att exportera en databasdumpfil (.dmp [!DNL Postgres] fil) med dina data. Ytterligare en begäran kommer att skickas till vårt NOC-team för att hämta alla dina lagrade dokument.

* **Pros**: Du får hela din datainläsning, inklusive anpassade fält och dokument som lagras i systemet.

* **Kon**: Det finns inget sätt att läsa den här filen om du inte överför den till en [!DNL Postgres]-databas och återupprättar relationerna mellan tabellerna. Dokumenten lagras på en separat filserver och måste extraheras separat med en separat process av NOC-teamet. Då finns det ingen organisation för dokumenten och de hänvisas alla till av deras GUID.

* **Kostnad**: Det är en kostnad kopplad till den här hämtningen, beroende på hur lång tid det tar för teamet att skapa filen. Kontakta en återförsäljare för mer information eller för att komma igång.

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

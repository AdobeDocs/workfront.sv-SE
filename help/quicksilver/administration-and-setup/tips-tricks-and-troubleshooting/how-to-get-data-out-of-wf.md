---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '''Exportera historiska data från Adobe Workfront: För- och nackdelar'
description: I den här artikeln förklaras för- och nackdelarna med fyra alternativ som du kan använda för att exportera historiska data från Workfront.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: f3af39e760b2b407cda5ab78497cdc775defdcf6
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 0%

---

# Exportera historiska data från [!DNL Adobe Workfron]t: För- och nackdelar

I den här artikeln förklaras för- och nackdelarna med fyra alternativ som du kan använda för att exportera historiska data från [!DNL Workfront].

## Använd en av våra partners

[!DNL AtAppStore], a [!DNL Workfront] certifierad partner har en lättanvänd app som gör att du kan hämta dina data. Den här appen innehåller även ett visningsprogram som gör att du enkelt kan visa dina data.

* **Pros:** Alla dina [!DNL Workfront] objekt exporteras, inklusive anpassade fält. Visningsprogrammets gränssnitt är enkelt att använda och läsa, och det är enkelt att importera i en [!DNL MS Access] Databas.

* **Kon:** Dokument exporteras inte. Du måste ladda ned dem separat. Mer information finns på [http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx.](http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx)

## Begär en [!DNL Postgres] datadumpfil från vårt databasteam

Din kontoansvarige kan skicka en begäran till vårt databasteam om att exportera en databasdumpfil (.dmp [!DNL Postgres] fil) med dina data. Ytterligare en begäran kommer att skickas till vårt AOS-team för att hämta alla dina lagrade dokument.

* **Proffs**: Du får hela datainläsningen inklusive anpassade fält och dokument som lagras i systemet.

* **Kon**: Databasfilen är svår att läsa: det finns inget sätt att läsa den här filen om du inte överför den till en [!DNL Postgres] och återupprätta relationerna mellan tabellerna. Dokumenten lagras på en separat filserver och måste extraheras separat med en separat process av AOS-teamet. Då finns det ingen organisation för dokumenten och de hänvisas alla till av deras GUID.
* **Kostnad**: Det är en kostnad kopplad till den här hämtningen, beroende på hur lång tid det tar för teamet att skapa filen. Kontakta en återförsäljare för mer information eller för att komma igång.

## Exportera via [!UICONTROL Kick-Starts]

Oavsett om du har öppethållande på distans eller inte kan du använda någon av våra konsulter för att exportera data i form av rapporter eller [!UICONTROL kick-starts]eller så kan du köra dessa rapporter själv:

* **Proffs**: Rapporterna är enkla att läsa och kan importeras i flera olika program. de kan anpassas så att de innehåller grupperingar och vyer som du vill ha med.

* **Kon**: Dokumenten måste laddas ned separat.

* **Kostnad**: Det är kostnadsfritt om du kan köra rapporterna själv (allt du behöver är en systemadministratörsinloggning) eller om du kan använda återstående fjärrådgivningstimmar. Om du är intresserad av att köpa fjärrrådgivning för detta kan du tala med din AE/CAE.

   Mer information om hur du använder Spark-Starts för att exportera data finns i [Exportera data från [!DNL Adobe Workfront] via [!UICONTROL Kick-Starts]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## Använd vårt öppna API

Om ni har rätt resurser i er organisation kan de skapa ett anpassat API för att hämta alla era data från Workfront:

* **Proffs**: Du styr vilka exporter som görs från systemet.

* **Kon**: Tiden spenderas åt dig och du måste hitta resurser för att koda API:t och utföra exporten.

* **Kostnad**: Inbyggt i er organisation.

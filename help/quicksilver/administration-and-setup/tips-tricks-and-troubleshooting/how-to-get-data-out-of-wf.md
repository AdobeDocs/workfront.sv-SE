---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Exportera historiska data från Adobe Workfront: pros and cons'
description: I den här artikeln förklaras för- och nackdelarna med fyra alternativ som du kan använda för att exportera historiska data från Workfront.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '501'
ht-degree: 0%

---

# Exportera historiska data från [!DNL Adobe Workfron]t: För och nackdelar

I den här artikeln förklaras för- och nackdelarna med fyra alternativ som du kan använda för att exportera historiska data från [!DNL Workfront].

## Använd en av våra partners

[!DNL AtAppStore], en [!DNL Workfront]-certifierad partner, har en lättanvänd app som gör att du kan hämta dina data. Den här appen innehåller även ett visningsprogram som gör att du enkelt kan visa dina data.

* **Fördelar:** Alla dina [!DNL Workfront]-objekt exporteras, inklusive anpassade fält. Visningsprogrammets gränssnitt är enkelt att använda och läsa och kan enkelt importeras i en [!DNL MS Access]-databas.

* **Kon:** Dokument exporteras inte. Du måste ladda ned dem separat. Mer information finns på [http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx.](https://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx)

## Begär en [!DNL Postgres]-datadumpfil från vårt databasteam

Din kontoansvarige kan skicka en begäran till vårt databasteam om att exportera en databasdumpfil (.dmp [!DNL Postgres]) med dina data. Ytterligare en begäran kommer att skickas till vårt AOS-team för att hämta alla dina lagrade dokument.

* **Pros**: Du får hela din datainläsning, inklusive anpassade fält och dokument som lagras i systemet.

* **Kon**: Databasfilen är svår att läsa: du kan inte läsa den här filen om du inte överför den till en [!DNL Postgres]-databas och återupprättar relationerna mellan tabellerna. Dokumenten lagras på en separat filserver och måste extraheras separat med en separat process av AOS-teamet. Då finns det ingen organisation för dokumenten och de hänvisas alla till av deras GUID.
* **Kostnad**: Det är en kostnad kopplad till den här hämtningen, beroende på hur lång tid det tar för teamet att skapa filen. Kontakta en återförsäljare för mer information eller för att komma igång.

## Exportera via [!UICONTROL Kick-Starts]

Oavsett om du har öppethållande på distans eller inte, kan du använda en av våra konsulter för att exportera data i form av rapporter eller [!UICONTROL kick-starts], eller så kan du själv köra dessa rapporter:

* **Pros**: Rapporterna är enkla att läsa och kan importeras i en mängd olika program. De kan anpassas så att de omfattar alla grupperingar och vyer som du vill ha.

* **Kon**: Dokument måste hämtas separat.

* **Kostnad**: Det är kostnadsfritt om du kan köra rapporterna själv (allt du behöver är en systemadministratörsinloggning) eller om du kan använda de återstående arbetstiderna för fjärrrådgivning. Om du är intresserad av att köpa fjärrrådgivning för detta kan du tala med din AE/CAE.

  Mer information om hur du använder Quick-Starts för att exportera data finns i [Exportera data från [!DNL Adobe Workfront] via [!UICONTROL Kick-Starts]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## Använd vårt öppna API

Om ni har rätt resurser i er organisation kan de skapa ett anpassat API för att hämta alla era data från Workfront:

* **Pros**: Du har kontroll över vilka exporter som görs från systemet.

* **Kon**: Den tid du tillbringar läggs på dig, och du måste hitta resurser för att koda API:t och utföra exporten.

* **Kostnad**: Inbyggt i din organisation.

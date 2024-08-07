---
content-type: release-notes
navigation-topic: 2019-2-release-activity
title: Förbättringar av korrektur för 2019.2
description: Den här sidan beskriver alla språkförbättringar som ingår i version 2019.2. Funktionen planeras bli tillgänglig i produktionsmiljön den 20 maj 2019.
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: e8b67a10-1c9a-427e-96d5-0bcee47333f3
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# Förbättringar av korrektur för 2019.2

Den här sidan beskriver alla språkförbättringar som ingår i version 2019.2. Funktionen planeras bli tillgänglig i produktionsmiljön den 20 maj 2019.

En lista över alla ändringar som gjorts under 2019.2 finns i [2019.2 Release Activity Overview](../../../../product-announcements/product-releases/quarterly-release-archive/2019.2-release-activity/2019-2-release-activity-overview.md).

## Tillåt användare utan korrekturlicens att använda åtgärder och lösa kommentarer

Nu kan användare som saknar korrekturlicens använda åtgärder på kommentarer och lösa kommentarer. Du kan ge behörighet för de här aktiviteterna när du lägger till en användare till ett korrektur.

Tidigare var det bara användare med en korrekturlicens och korrekturrollen som författare eller moderator som kunde vidta åtgärder och lösa kommentarer på ett korrektur.

## Tagga en användare när han eller hon kommenterar ett korrektur i korrekturläsaren

Om du har redigeringsbehörighet för korrekturet kan du nu tagga eller &quot;@mention&quot; för alla som har en e-postadress som känns igen av Workfront när du kommenterar ett korrektur. Detta omfattar följande:

* Alla som har lagts till i ett bevis på din organisations Workfront-konto med hjälp av e-postadressen.
* Alla som har använt e-postadressen för att prenumerera på ett bevis i din organisations Workfront-konto.

Tidigare kunde du bara tagga användare som hade lagts till i korrekturets arbetsflöde. Det är fortfarande så taggningen fungerar om du inte har redigerat rätt på korrekturet.

## Filtrera korrekturgodkännanderapport för att utelämna tidigare korrekturversioner

>[!NOTE]
>
>Den här funktionen släpptes direkt till produktionsmiljön under 2019.2-förhandsgranskningen.

På alla korrekturgranskningsrapporter kan du nu använda det nya filtret Är aktuell dokumentversion för att inkludera endast de aktuella versionerna av korrektur som väntar på ditt godkännande.

Detta är användbart om du till exempel har ombetts att godkänna korrektur som har flera versioner. När du kör rapporten Korrektur på godkännande med filtret Är aktuell dokumentversion visas endast den aktuella versionen av varje korrektur som väntar på ditt godkännande, utan tidigare versioner som du inte längre behöver arbeta med.

Mer information finns i [Filtrera: Rapport om godkännande av korrektur för att utesluta tidigare korrekturversioner](../../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-proof-approval-report.md).


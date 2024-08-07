---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: 2020.1 Andra förbättringar
description: Den här sidan beskriver alla förbättringar som gjorts i allmänna delar av Workfront med version 2020.1. Dessa förbättringar är för närvarande tillgängliga i förhandsvisningsmiljön och kommer att vara tillgängliga i produktionsmiljön i slutet av mars eller början av april 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a716590c-c833-458a-a138-9bc0723e5896
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# 2020.1 Andra förbättringar

Den här sidan beskriver alla förbättringar som gjorts i allmänna delar av Workfront med version 2020.1. Dessa förbättringar är för närvarande tillgängliga i förhandsvisningsmiljön och kommer att vara tillgängliga i produktionsmiljön i slutet av mars eller början av april 2020.

En lista över alla ändringar som är tillgängliga i version 2020.1 finns i [2020.1 versionsöversikt](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## Ändringar som krävs för att lägga till korrektur i tillåtelselista

>[!NOTE]
>
>Den här funktionen har tagits bort från version 2020.1. Den kommer att göras tillgänglig vid ett senare tillfälle.

Korrekturdomänen ändras from proofhq.com till workfront.com.

Om din brandvägg eller e-postserver är konfigurerad att endast tillåta åtkomst till vissa leverantörer, måste du lägga till följande extra URL-adress i din tillåtelselista för att se till att användare i din organisation kan visa korrektur i Workfront både i webbläsarvisningsprogrammet och i skrivbordsvisningsprogrammet:

&#42;.workfront.com

URL:en för &#42;proofhq.com krävs fortfarande.

Mer information om hur du uppdaterar tillåtelselista finns i [Konfigurera tillåtelselista för brandväggen](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

>[!NOTE]
>
>Den här uppdateringen gäller endast för korrektur i Workfront. Den gäller inte när du använder Workfront Proof fristående program.

## Workfront cookie-beteende har uppdaterats för att bibehålla kompatibilitet med Chrome

För att bibehålla kompatibiliteten med en kommande Google Chrome-uppdatering (Chrome v80) har vi uppdaterat Workfront-plattformen så att cookies skickas på rätt sätt med begäranden.

Den här Chrome-uppdateringen ändrar standardvärdet för cookie-attributet SameSite. Om du vill testa hur din Workfront-instans fungerar efter Google Chrome-uppdateringen justerar du flaggorna i Chrome och aktiverar följande alternativ:

* &quot;SameSite som standard cookies&quot;
* &quot;Cookies utan SameSite måste vara säkra&quot;

## Workfront kommentarer synkroniseras med Jira

Integreringen av Workfront för Jira synkroniserar nu dina Workfront-kommentarer till Jiras inbyggda kommentarström.

Tidigare kunde du synkronisera kommentarer från Jira till Workfront, men inte från Workfront till Jira.

Mer information finns i [Konfigurera Adobe Workfront för Jira](../../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Optimeraren för Flash Portfolio har tagits bort

Vi har tagit bort möjligheten att växla mellan den nya och den gamla (baserat på Flash) Portfolio Optimizer från Workfront Classic-miljön för alla kunder. Äldre Portfolio Optimizer är en föråldrad funktion och de nya verktygen har samma funktionalitet idag.

Mer information om portföljoptimeraren finns på https://experience.workfront.com/s/article/Understanding-the-Portfolio-Optimizer-356650079

Mer information om hur du ersätter Flash-baserade verktyg i Workfront finns i [Ersättning av Flash-baserade verktyg i Adobe Workfront](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).

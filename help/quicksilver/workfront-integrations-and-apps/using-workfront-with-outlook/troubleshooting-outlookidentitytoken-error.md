---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 'Felsökning: outlookIdentityToken-fel vid användning av Workfront för Outlook'
description: Om du får ett OutlookIdentityToken-fel när du använder Workfront för Outlook måste du aktivera Microsoft 365-token för din organisation.
author: Becky
feature: Workfront Integrations and Apps
source-git-commit: 571ed00f44322d73183323c4d4154284cd028301
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---

# Felsökning: outlookIdentityToken-fel vid användning av Workfront för Outlook

När du använder Workfront för Outlook kan följande fel uppstå:

```
Unexpected error
Unable to get the outlookIdentityToken
```

För att åtgärda det här felet måste du aktivera Microsoft 365-token för din organisation. Eftersom detta måste göras i Microsoft 365 kan Workfront inte aktivera dessa tokens för din organisation.

Instruktioner om hur du aktiverar tidigare Microsoft 365-token finns i [Aktivera eller inaktivera tidigare Exchange Online-token](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/turn-exchange-tokens-on-off) i Microsoft-dokumentationen.

Mer information om äldre token finns i [Kan jag aktivera gamla token i Exchange Online igen?](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on) i Microsoft-dokumentationen.

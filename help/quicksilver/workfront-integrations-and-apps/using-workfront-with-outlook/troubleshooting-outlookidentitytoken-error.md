---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 'Felsökning: outlookIdentityToken-fel vid användning av Workfront för Outlook'
description: Om du får ett OutlookIdentityToken-fel när du använder Workfront för Outlook måste du aktivera Microsoft 365-token för din organisation.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4a911760-e3fe-4e77-b7aa-b08f9ea59d6a
source-git-commit: 793c8c940c8cb7ac53169edf21ddf28af2554120
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Felsökning: outlookIdentityToken-fel vid användning av Workfront för Outlook

>[!IMPORTANT]
>
>[Microsoft har inaktiverat stöd för äldre Exchange-onlinetoken](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) som användes av Workfront Outlook-tillägget för autentisering. Denna ändring av Microsoft har stegvis genomförts och är klar den 1 oktober 2025.
>
>**Eftersom Microsoft har inaktiverat dessa token fungerar inte längre integreringen i Workfront för Microsoft Outlook.**

När du använder Workfront för Outlook kan följande fel uppstå:

```
Unexpected error
Unable to get the outlookIdentityToken
```

För att åtgärda det här felet måste du aktivera Microsoft 365-token för din organisation. Eftersom detta måste göras i Microsoft 365 kan Workfront inte aktivera dessa tokens för din organisation.

Instruktioner om hur du aktiverar tidigare Microsoft 365-token finns i [Aktivera eller inaktivera tidigare Exchange Online-token](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/turn-exchange-tokens-on-off) i Microsoft-dokumentationen.

Mer information om äldre token finns i [Kan jag aktivera gamla token i Exchange Online igen?](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on) i Microsoft-dokumentationen.

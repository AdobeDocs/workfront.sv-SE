---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 'Felsökning: outlookIdentityToken-fel vid användning av Workfront för Outlook'
description: Om du får ett OutlookIdentityToken-fel när du använder Workfront för Outlook måste du aktivera Microsoft 365-token för din organisation.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4a911760-e3fe-4e77-b7aa-b08f9ea59d6a
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# Felsökning: outlookIdentityToken-fel vid användning av Workfront för Outlook

>[!IMPORTANT]
>
>[Microsoft håller på att inaktivera stöd för äldre Exchange-onlinetoken](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), som för närvarande används av Workfront Outlook-tillägget för autentisering. Denna förändring från Microsoft har redan börjat påverka kunderna och kommer att fortsätta att gälla i faser fram till oktober 2025.
>
>* **När Microsoft har inaktiverat alla dessa variabler fungerar inte längre integreringen med Workfront för Microsoft Outlook.**
>
>Som en del av den här ändringen har Microsoft beslutat att ändra hur tokens återaktiveras. Efter den **30 juni 2025** kan administratörer inte längre återaktivera tokens själva. Det är bara Microsoft Support som kan bevilja undantag. **Den 1 oktober 2025 inaktiveras äldre token för alla innehavare. Undantag beviljas inte.**


När du använder Workfront för Outlook kan följande fel uppstå:

```
Unexpected error
Unable to get the outlookIdentityToken
```

För att åtgärda det här felet måste du aktivera Microsoft 365-token för din organisation. Eftersom detta måste göras i Microsoft 365 kan Workfront inte aktivera dessa tokens för din organisation.

Instruktioner om hur du aktiverar tidigare Microsoft 365-token finns i [Aktivera eller inaktivera tidigare Exchange Online-token](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/turn-exchange-tokens-on-off) i Microsoft-dokumentationen.

Mer information om äldre token finns i [Kan jag aktivera gamla token i Exchange Online igen?](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on) i Microsoft-dokumentationen.

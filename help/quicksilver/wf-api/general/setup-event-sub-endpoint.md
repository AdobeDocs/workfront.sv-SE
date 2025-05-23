---
content-type: api
navigation-topic: general-api
title: Leveranskrav för evenemangsprenumeration
description: Leveranskrav för evenemangsprenumeration
author: Becky
feature: Workfront API
role: Developer
exl-id: 1b621b35-6c8b-4f6a-bcba-ed6cbfe83a8c
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---


# Leveranskrav för evenemangsprenumeration

Händelseprenumerationsmeddelanden är meddelanden som kan konfigureras för att meddela användare när vissa händelser inträffar. Mer information om vilka Event-prenumerationer som finns finns i [Vanliga frågor och svar - Händelseprenumerationer](../../wf-api/general/event-subs-faq.md).

## Standarder för leverans av händelseprenumerationsmeddelanden

Slutpunkter för tjänsten som använder Adobe Workfront händelseteckningsmeddelanden måste uppfylla följande grundläggande krav för att meddelanden ska kunna skickas och tas emot korrekt:

* Tjänstens slutpunkt måste acceptera HTTP POST-begäranden. HTTP POST är den förfrågningsmetod som används i alla leveranser av händelseprenumerationsmeddelanden, inklusive valideringsmeddelanden.

* För att leveranssystemet för händelseprenumerationer ska kunna bekräfta att meddelandet togs emot måste slutpunkten returnera en HTTP-status på 200 nivåer (till exempel 200 OK eller 202) för alla inkommande meddelanden.

* Om en status på 200 nivåer inte returneras antar systemet för händelseprenumerationer att meddelandet inte kunde levereras och börjar tillämpa rätt princip för återförsök. Mer information om Workfront återförsöksprincip finns i [Återförsök med händelseprenumerationer](../../wf-api/api/event-sub-retries.md).

* I samband med att en 200-nivåstatus returneras som svarsstatus måste HTTP-svaret tas emot inom fem sekunder efter att leveransförsöket har startats. Detta villkor säkerställer att konsumentaffärsprocesser eller infrastrukturbegränsningar inte försenar leveransen av andra meddelanden som väntar på leverans.

* Om en långvarig affärsprocess utlöses av ett händelseteckningsmeddelande rekommenderar Workfront  att

   1. Slutpunkten sparar meddelandeinformationen vid mottagandet och svarar omedelbart med statusen 200 nivåer.
   1. När en slutpunkt har svarat på en begäran om leverans av en händelseprenumeration kan de sparade meddelandena behandlas.

* Evenemangsprenumerationsmeddelanden eller -objekt får inte vara större än 1 MB.

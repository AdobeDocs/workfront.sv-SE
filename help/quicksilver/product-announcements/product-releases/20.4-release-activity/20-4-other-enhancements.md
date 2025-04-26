---
title: 20.4 Andra förbättringar
description: 20.4 Andra förbättringar
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: bd8fcafc-00cc-4025-b2d3-e3a6f12e40fc
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# 20.4 Andra förbättringar

Den här sidan beskriver alla andra förbättringar som gjorts i version 20.4 till förhandsvisningsmiljön. Dessa förbättringar kommer att bli tillgängliga i produktionsmiljön den 9 november 2020.

En lista över alla ändringar som är tillgängliga i version 20.4 finns i [20.4 versionsöversikt](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Nytt för administratörer: Byt alternativ för Workfront-miljö tillgängligt

För en effektivare och smidigare upplevelse kan gruppadministratörer och Workfront-administratörer nu snabbt växla mellan olika Workfront-miljöer från vilken sida som helst i Workfront utan att behöva logga ut.

I den nya Workfront-versionen visas alternativet Växla till klassisk på huvudmenyn.

I Workfront Classic visas alternativet Växla till den nya upplevelsen på den meny som visas när du klickar på profilbilden i det övre högra hörnet av det globala navigeringsfältet.

Den här funktionen ingår nu i [Administratörsgrunderna, del 1 utbildningsväg](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home) på Workfront One.

## Förbättrad kryptering för Workfront Proof

Vi gör några ändringar för att förbättra styrkan på kryptering av data-i-rörelse i Workfront korrekturprogram. De svaga TLS-lärarna kommer att bli inaktuella den 11 november 2020.

Kontrollera att du använder en webbläsare som stöds när du använder Workfront. Mer information om vilka webbläsare som stöds finns i [Adobe Workfront webbläsarkrav](../../../workfront-basics/workfront-browser-requirements.md).

## Nytt utseende och känsla för 3 e-postmallar

För att förbättra läsbarheten och den övergripande upplevelsen har följande e-postmallar ett nytt utseende och en ny känsla:

* Ny arbetsbegäran
* En beroende uppgift som du är tilldelad till är nu klar att starta
* E-postmeddelande för team med föregående slutförd

Om du vill aktivera e-post för testning i förhandsvisningsmiljön läser du avsnittet Hantera e-postmeddelanden i förhandsgranskningsavsnittet i [Ändra dina egna e-postmeddelanden](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Nya e-postmeddelanden för team

Vi har lagt till följande e-postmeddelanden för team:

* En föregångare till en uppgift som har tilldelats mitt team har slutförts: Det tilldelade teamet får ett e-postmeddelande när en föregångare till en av deras uppgifter har markerats som slutförd.
* Alla föregångare för en uppgift som har tilldelats mitt team är slutförda: Det tilldelade teamet får ett e-postmeddelande för varje föregångare som har markerats som slutförd.

Mer information finns i [Meddelanden: Information om arbete som tilldelats mig](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

## Nytt för administratörer: Förbättringar av e-postmeddelanden

Med ett enda klick kan du nu aktivera eller inaktivera ett e-postmeddelande för en händelse i installationsprogrammet. Klicka bara på På/Av bredvid meddelandets namn.

Observera också att vår moderna formatering nu förbättrar upplevelsen av att konfigurera händelsemeddelanden i området E-postmeddelanden.

Mer information om hur du konfigurerar e-postmeddelanden finns i [Konfigurera händelsemeddelanden för alla i systemet](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Den här funktionen finns nu med i utbildningssökvägen [E-post och i programmet ](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home) på Workfront One.

## Nya API-objekt som utlöser händelseprenumerationsuppdateringar

Två nya API-objekt, documentVersion och proofApproval, skapades och har konfigurerats för att utlösa uppdateringar av händelseprenumerationer när ett dokument versionsindelas eller godkänns.

En fullständig lista över fält som är associerade med varje objekt finns i [Resursfält för händelseprenumerationer](../../../wf-api/api/event-sub-resource-fields.md).

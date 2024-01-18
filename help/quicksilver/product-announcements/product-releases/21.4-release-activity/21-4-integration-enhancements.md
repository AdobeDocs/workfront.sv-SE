---
title: 21.4 Integration enhancements
description: 21.4 Integration enhancements
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: d3e2342e-1c44-49c2-90bc-9fd77fbb2db8
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# 21.4 Integration enhancements

Den här sidan beskriver alla integreringsförbättringar som gjorts i version 21.4 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön den 4 oktober 2021.

En lista över alla ändringar som är tillgängliga i version 21.4 finns i [21.4 Versionsöversikt](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## Länka dokument från Dropbox Business

Vi har lagt till Dropbox Business som en tillgänglig dokumentintegrering. Nu kan du komma åt dokument som du har sparat i Dropbox Business direkt inifrån Workfront.

Med Dropbox Business kan du länka delade dokument och överföra dokument till delade mappar. Dropbox (inte Dropbox Business) tillåter endast dokumentägaren att visa dokumentet i Workfront.

Din Workfront-administratör kan aktivera integreringen för din organisation.

Mer information finns i [Länka dokument från externa program](../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Information om hur en Workfront-administratör kan aktivera det här alternativet finns i [Konfigurera dokumentintegreringar](../../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Uppdateringar av Workfront för Slack

Följande uppdateringar visas nu i Workfront för integrering med Slack:

* Workfront för Slack har ett nytt utseende och en ny känsla.
* Nu får du meddelanden från Workfront för Slack i realtid.

  Om du till exempel har tilldelats en uppgift får du det meddelandet så snart du har tilldelats. Tidigare kunde det dröja innan anmälan gjordes i Slack.

Den här uppdateringen kräver att du auktoriserar om Workfront för integrering med Slack. Information om hur du godkänner integreringen finns i [Konfigurera Adobe Workfront för Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Mer information om Workfront för Slack-meddelanden finns i [Få Adobe Workfront-meddelanden i Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Mer tydlig information om kontoåtkomst när du godkänner Adobe Workfront-integreringar

Medgivandeskärmarna för Adobe Workfront-integreringar har nu uppdaterats. Nu kan du se de specifika åtgärder och områden som integreringarna har tillgång till, så att du bättre kan förstå vad du tillåter integreringen eller programmet att komma åt.

Den här nya godkännandeskärmen gäller för alla Adobe Workfront-integreringar som använder OAuth 2.0.

Mer information om specifika integreringar finns i integreringens dokumentation.

## API-nyckelautentisering behövs inte längre för integreringar

Workfront integreringar har nyligen börjat använda OAuth2 för bättre säkerhet och användbarhet. Som en del av detta kräver Workfront inte längre API-nycklar för integreringsautentisering.

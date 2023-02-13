---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: När ett autentiserat e-postmeddelande inte accepteras på grund av domänens DMARC-princip
description: Om ett e-postmeddelande skickas från [!DNL Workfront] systemet inte accepteras på grund av domänens DMARC-princip kan e-postadministratören åtgärda problemet genom att konfigurera ditt e-postsystem så att alla e-postmeddelanden från workfront.com tillåts.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2443267a-dcc0-485b-be29-17539fb54188
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# Oautentiserad e-post accepteras inte på grund av domänens DMARC-princip

## Problem

[Testa] Jag fick följande studsmeddelande via e-post:

550-5.7.1 Oautentiserad e-post från &quot;customer domain.com&quot; accepteras inte på grund av\
550-5.7.1 domänens DMARC-policy. Kontakta administratören för &quot;customer domain.com&quot;\
550-5.7.1-domän om detta var en giltig post. Besök\
550-5.7.1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690) om du vill veta mer om DMARC\
550 5.7.1-initiativ.

## Lösning

DMARC är konfigurerat i företagets e-postsystem och ingår inte i [!DNL Adobe Workfront]. Om du får det här e-postmeddelandet måste du kontakta e-postadministratören.

E-postadministratören bör konfigurera ditt e-postsystem så att e-post från noreply@workfront.com tillåts/betros, eller helst alla e-postmeddelanden från workfront.com.

Mer information om DMARC finns i [https://support.google.com/mail/answer/2451690.](https://support.google.com/mail/answer/2451690)

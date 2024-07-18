---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Inloggningsfel: Följande fält är ogiltiga: emailAddr får inte vara null'
description: När jag försöker logga in på  [!DNL Adobe Workfront] URL:en för min domän omdirigeras jag till SAML-inloggningsportalen och omdirigeras sedan tillbaka till  [!DNL Workfront] med ett fel som anger att fältet emailAddr inte kan vara null.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 0%

---

# Inloggningsfel: Följande fält är ogiltiga: emailAddr får inte vara null

## Problem

När jag försöker logga in på [!DNL Adobe Workfront] med min URL (https://customerdomain.my.workfront.com) omdirigeras jag till SAML-inloggningsportalen och omdirigeras sedan tillbaka till [!DNL Workfront] med följande fel:

&quot;Vi provar det igen. Följande fält är ogiltiga: emailAddr får inte vara null.&quot;

## Orsak

Felet orsakas av ett felaktigt objekt i området Mappa användarattribut i SAML 2.0-konfigurationen. Mer information om mappning av användarattribut för SAML 2.0 finns i [Konfigurera Adobe Workfront med SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## Lösning

Uppdatera attributmappningen för e-postadressen och klicka på **[!UICONTROL Save]**.

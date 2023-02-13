---
content-type: reference
navigation-topic: announcements
title: TLS 1.2 krävs i Adobe Workfront
description: För att ge optimal säkerhet kräver Adobe Workfront att alla webbläsaranslutningar och API-integreringar som är beroende av TLS 1.0 eller tidigare uppgraderas för att använda TLS 1.2. I förhandsvisningsmiljön är TLS 1.0 redan inaktiverat.
author: Luke
feature: Product Announcements
exl-id: 153668ae-0647-47fd-9153-ce45cd8c54ee
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# TLS 1.2 krävs i Adobe Workfront

För att ge optimal säkerhet kräver Adobe Workfront att alla webbläsaranslutningar och API-integreringar som är beroende av TLS 1.0 eller tidigare uppgraderas för att använda TLS 1.2. I förhandsvisningsmiljön är TLS 1.0 redan inaktiverat.

Workfront upphörde officiellt med stödet för TLS 1.0 i mars 2018. Alla integreringar som utnyttjar TLS 1.0 slutade fungera från och med 9 januari 2019.  TLS 1.1 kommer att inaktiveras fjärde kvartalet 2019.

I följande avsnitt finns mer information om dessa viktiga milstolpar samt hur du kan förbereda dig för uppgraderingen i din organisation:

## Workfront upphör med det officiella stödet för TLS 1.0 (5 mars 2018)

Workfront upphörde med det officiella stödet för TLS 1.0 i mars 2018.

Webbläsaranslutningar och API-integreringar som utnyttjar TLS 1.0 fungerar fortfarande, men Workfront löser inga problem i Workfront-programmet som är relaterade till TLS 1.0.

## Workfront-integreringar som använder TLS 1.0 är inaktiverade (9 januari 2019)

Den 9 januari 2019 måste alla webbläsaranslutningar och API-integrationer som använder TLS 1.0 uppgraderas för att använda TLS 1.1 eller senare. Webbläsaranslutningar och API-integreringar som fortsätter att utnyttja TLS 1.0 (både inkommande och utgående anslutningar) kommer inte längre att kunna kommunicera med Workfront-programmet efter denna tid. 

## TLS 1.1 kommer att inaktiveras fjärde kvartalet 2019

I produktionsmiljön inaktiverades TLS 1.1 den 21 oktober 2019. Därefter kommer alla integreringar som använder TLS 1.1 inte längre att fungera.

Den här förändringen kommer att träda i kraft i förhandsgransknings- och sandlådemiljöerna den 7 augusti för att hjälpa organisationer att förbereda sig för avstängningen.

## Förbereder TLS-uppgraderingen

* [Vid åtkomst till Workfront via webbläsaren](#when-accessing-workfront-via-the-browser)
* [Vid anslutning till Workfront via API](#when-connecting-to-workfront-via-the-api)

### Vid åtkomst till Workfront via webbläsaren {#when-accessing-workfront-via-the-browser}

Se till att användare i organisationen använder Workfront via en webbläsare som stöds. (Information om vilka webbläsare som stöds finns i [Krav för Adobe Workfront webbläsare](../../../workfront-basics/workfront-browser-requirements.md).)

Alla webbläsare som stöds av Workfront är kompatibla med TLS 1.2.

### Vid anslutning till Workfront via API {#when-connecting-to-workfront-via-the-api}

Om du integrerar tredjepartsprogram med Workfront via API:t (både inkommande och utgående) måste du se till att TLS 1.2 (och TLS 1.2-krypteringsprotokoll) är aktiverade i integreringarna.

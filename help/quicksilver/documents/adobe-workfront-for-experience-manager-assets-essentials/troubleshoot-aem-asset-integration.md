---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Felsöka integreringen med Adobe Experience Manager
description: Koppla samman ditt material med ditt i Experience Manager Assets Essentials - EDIT ME.
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: e4bf79b8c5d53870aec6d415510acccb53a5c7f6
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Felsöka Adobe Experience Manager-integreringen

## Problem: Resurser sparas inte i Adobe Experience Manager

När en användare väljer en resurs eller mapp att exportera till Experience Manager Assets och klickar på Välj stängs väljarfönstret men resurserna sparas inte i Experience Manager Assets. Det finns inget i Workfront som tyder på att resurserna inte sparades till Experience Manager Assets.

### Orsak

Detta kan inträffa på grund av tillåtelselista i Adobe Cloud Manager. Om tillåtelselista för en organisation i Adobe Cloud Manager är tom begränsas inte IP-adresserna och Workfront har åtkomst till organisationens mappar och resurser i Adobe Experience Manager. Men om bara en enda IP-adress läggs till i Cloud Manager-tillåtelselista antar tillåtelselista att ingen IP-adress tillåts i listan. Om Cloud Manager-tillåtelselista innehåller IP-adresser måste därför Workfront IP-adresser läggas till i tillåtelselista för att Workfront ska kunna skicka resurser till Experience Manager Assets.

### Lösning:

Lägg till Workfront IP-adresser i tillåtelselista för Adobe Cloud Manager.

* Instruktioner om hur du lägger till IP-adresser i Adobe Cloud Manager finns i [Introduktion till IP Tillåtelselista](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction.html?lang=en) i Adobe Experience Manager-dokumentationen.
* En lista över Workfront IP-adresser som ska läggas till i tillåtelselista finns på [Konfigurera brandväggen](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md).



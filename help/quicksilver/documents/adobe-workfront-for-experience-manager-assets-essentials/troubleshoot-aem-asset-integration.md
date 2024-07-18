---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Felsöka integreringen med Adobe Experience Manager
description: 'Problem: Assets sparas inte i Adobe Experience Manager'
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: f7e31e20-01e3-462d-9020-005e155f0259
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Felsöka Adobe Experience Manager-integreringen

## Problem: Assets sparas inte i Adobe Experience Manager

När en användare väljer en resurs eller mapp att exportera till Experience Manager Assets och klickar på Välj stängs väljarfönstret men resurserna sparas inte i Experience Manager Assets. Det finns inget i Workfront som tyder på att resurserna inte sparades till Experience Manager Assets.

### Orsak

Detta kan inträffa på grund av tillåtelselista i Adobe Cloud Manager. Om Adobe Cloud Manager-tillåtelselista för en organisation är tom är IP-adresserna inte begränsade och Workfront har åtkomst till organisationens mappar och resurser i Adobe Experience Manager. Om en enda IP-adress läggs till i Cloud Manager tillåtelselista antar dock tillåtelselista att en IP-adress som inte finns med i listan inte tillåts. Om Cloud Manager tillåtelselista innehåller IP-adresser måste därför Workfront IP-adresser också läggas till i tillåtelselista för att Workfront ska kunna skicka resurser till Experience Manager Assets.

### Lösning:

Lägg till Workfront IP-adresser i Adobe Cloud Manager-tillåtelselista.

* Instruktioner om hur du lägger till IP-adresser i Adobe Cloud Manager finns i [Introduktion till IP Tillåtelselista](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction.html?lang=en) i Adobe Experience Manager-dokumentationen.
* En lista över Workfront IP-adresser som ska läggas till i tillåtelselista finns i [Konfigurera brandväggen](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

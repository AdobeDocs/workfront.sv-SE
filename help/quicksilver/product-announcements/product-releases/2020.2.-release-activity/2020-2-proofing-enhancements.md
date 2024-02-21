---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: Förbättringar av 2020.2-korrektur
description: På den här sidan beskrivs alla korrekturförbättringar som gjorts i 2020.2-versionen av produktionsmiljön. Dessa förbättringar gjordes tillgängliga i produktionsmiljön den 11 maj 2020.
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 021c6e0c-3593-40f7-8eeb-7e016001893e
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 0%

---

# Förbättringar av 2020.2-korrektur

På den här sidan beskrivs alla korrekturförbättringar som gjorts i 2020.2-versionen av produktionsmiljön. Dessa förbättringar gjordes tillgängliga i produktionsmiljön den 11 maj 2020.

En lista över alla ändringar som är tillgängliga i version 2020.2 finns på [Översikt över version 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Korrekturdomänen ändras från proofhq.com till workfront.com.

>[!NOTE]
>
>Den här funktionen kommunicerades ursprungligen som en del av 2020.1-utgåvan, men togs bort från utgåvan innan den lanserades till Production.

Om din brandvägg eller e-postserver är konfigurerad att endast tillåta åtkomst till vissa leverantörer, måste du lägga till följande extra URL-adress i din tillåtelselista för att se till att användare i din organisation kan visa korrektur i Workfront både i webbläsarvisningsprogrammet och i skrivbordsvisningsprogrammet:

&#42;.workfront.com

The &#42;proofhq.com URL krävs fortfarande.

Mer information om hur du uppdaterar tillåtelselista finns i [Konfigurera brandväggens tillåtelselista](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Den här uppdateringen gäller endast för korrektur i Workfront. Den gäller inte om du använder det fristående programmet Workfront Proof.

## Granska korrekturkommentarer från gäster visas i uppdateringsområdet

För att effektivisera samarbetet vid korrektur visas gästkommentarer i uppdateringsområdet.

Tidigare fanns endast korrekturkommentarer från gäster tillgängliga i beviset.

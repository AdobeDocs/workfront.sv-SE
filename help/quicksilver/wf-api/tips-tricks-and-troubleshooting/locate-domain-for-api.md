---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Domänformat för Adobe Workfront API-anrop
description: Hitta din domän för användning i Adobe Workfront API
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
source-git-commit: c2ce6776ceebe3c1d3915e3791fc84eb0245ba4d
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---

# Domänformat för Adobe Workfront API-anrop

När du gör ett API-anrop till Workfront API använder du organisationens domän i anropet. Formatet för den här domän-URL:en skiljer sig åt beroende på om din organisation har anslutit till det enhetliga Adobe-gränssnittet.

Om du vill veta om din organisation finns på Adobe Unified Shell kan du kontrollera den URL som visas när du visar en Workfront-sida.

| Workfront URL börjar med: | URL för API-anrop: |
|---|---|
| `<yourdomain>.my.workfront.com` | `<yourdomain>.my.workfront.com` |
| `experience.adobe.com` | `<yourdomain>.my.workfront.adobe.com` |

Så här hittar du din domän:

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Setup]** ![ikonen Konfigurera](/help/_includes/assets/gear-icon-setup.png).
1. Välj **System** och sedan **Kundinformation**.

   Domänen visas till höger på skärmen.

   ![Domän](assets/domain.png)


---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Flera webbläsarflikar gör att Workfront loggar ut
description: När en användare har flera webbläsarflikar öppna kan Workfront automatiskt logga ut.
feature: Get Started with Workfront
source-git-commit: ef85b267b3417dddd0c9cc4a2b916b83dc416e14
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Flera webbläsarflikar gör att Workfront loggar ut

>[!IMPORTANT]
>
>Problemet gäller endast organisationer som har anslutit sig till Adobe IMS.

## Problem

När en användare har flera webbläsarflikar öppna och klickar på en flik som har varit inaktiv under en tid, har tabbsessionen gått ut. Användaren kan inte se sidan som han/hon hade öppnat, utan ser i stället följande meddelande:

```
Tab session expired
This tab session has been halted due to inactivity. Refresh the tab to continue where you left off.
```

## Orsak

Det här beteendet beror på PBA (Policy-Based Authentication), en säkerhetsåtgärd som konfigurerats av din organisation. När en flik har varit inaktiv i mer än den tidsgräns som har angetts i organisationens PBA-konfiguration, förfaller tabbsessionen.

## Lösning

Lösningen beror på om du har varit aktiv på en annan flik som är inloggad på Workfront.

* Om du har en aktiv Workfront-flik öppen läser du in den förfallna fliken igen. Den återgår till sidan som du hade öppnat innan den gick ut.

* Om du inte har en aktiv Workfront-flik öppen loggar du in i Workfront igen.
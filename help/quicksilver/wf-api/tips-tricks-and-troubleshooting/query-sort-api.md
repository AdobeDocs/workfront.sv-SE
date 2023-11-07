---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Sortera frågeresultat i API
description: Sortera frågeresultat i API
author: Becky
feature: Workfront API
role: Developer
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '60'
ht-degree: 0%

---


# Sortera frågeresultat i API

Du kan sortera resultatet efter vilket fält som helst om du lägger till följande i ditt API-anrop:

```
&entryDate_Sort=asc
```

Om du t.ex. vill sortera efter planerat startdatum för aktiviteten tar du bort `entryDate` och ersätta den med `plannedCompletionDate`.

Detta fungerar för de flesta fält i Adobe Workfront.

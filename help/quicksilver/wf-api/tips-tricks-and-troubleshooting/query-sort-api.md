---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Sortera frågeresultat i API
description: Sortera frågeresultat i API
author: Becky
feature: Workfront API
role: Developer
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: 5936982217adc6cfcaf9e400bfff67a1496d3a78
workflow-type: tm+mt
source-wordcount: '60'
ht-degree: 0%

---


# Sortera frågeresultat i API

Du kan sortera resultatet efter vilket fält som helst om du lägger till följande i ditt API-anrop:

```
&entryDate_Sort=asc
```

Om du till exempel vill sortera efter aktivitet på Planerat slutdatum tar du bort `entryDate` och ersätter den med `plannedCompletionDate`.

```
&plannedCompletionDate_Sort=asc
```

Detta fungerar för de flesta fält i Adobe Workfront.

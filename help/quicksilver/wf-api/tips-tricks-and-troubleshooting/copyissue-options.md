---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Alternativkonfiguration för OPTASK copyIssue
description: En förklaring av de heltalsvärden som förväntas av copyIssue-slutpunkten.
author: Becky
feature: Workfront API
role: Developer
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 4%

---

# Alternativkonfiguration för OPTASK copyIssue


En av egenskaperna för ett copyIssue API-anrop är ett fält med namnet `options`. Fältet förväntar ett heltal.

Om du vill inkludera ett av följande alternativ anger du det matchande heltalet. Om du vill inkludera mer än ett alternativ anger du summan av de matchande heltalen.

| option | värde* |
|---|---|
| Rensa tilldelningar | 2 |
| Rensa förlopp | 4 |
| Rensa dokument | 128 |
| Rensa uppdateringar | 65536 |
| Rensa behörigheter | 524288 |
| Rensa anpassade data | 1048576 |

*Alla värden är tvåpotenser.

Exempel:

* Om du vill rensa förloppet när du kopierar utgåvan anger du värdet `options` för `4`.

* Om du vill rensa både förlopp och dokument anger du `options`-värdet `132`.

  Rensa förlopp = 4

  Rensa dokument = 128

  4 + 128 = 132

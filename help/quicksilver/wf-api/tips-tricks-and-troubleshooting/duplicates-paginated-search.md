---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Dubbletter returneras under en stor sidnumrerad sökning
description: Dubbletter returneras under en stor sidnumrerad sökning
author: Becky
feature: Workfront API
role: Developer
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 0%

---


# Dubbletter returneras under en stor sidnumrerad sökning

## Problem

När en stor sidnumrerad sökning utförs i API:t för ett objekt, får kunden dubblettposter och poster som saknas.

## Lösning

När ordern inte är formellt definierad, förlitar vi oss på ordningen på raderna som returneras av Oraclets databas, vilket inte garanterar någon deterministisk ordning. Två anrop i följd med samma fråga kan till exempel returnera rader i en annan ordning. På samma sätt kan raderna slumpmässigt tilldelas till olika&quot;sidor&quot; vid sidindelning, vilket leder till dubbletter. Den enklaste lösningen är att lägga till sortering efter ID:

```
&ID_Sort=asc
```


---
content-type: api
navigation-topic: wf-api
title: Hämta användarens tids-API
description: Hämta användarens tids-API
author: Becky
feature: Workfront API
role: Developer
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '94'
ht-degree: 0%

---

# Användare har tillgänglig tid-API

**URI: attask/api/v15.0/user/getUsersAvailableTime**

Användarnas tillgängliga tidsslutpunkt hämtar data om användarens tillgängliga tid. Detta möjliggör integreringar för sammanställning av data utifrån användarattribut och tidsintervall.

## Exempelbegäran

`curl -XPUT /attask/api/v15.0/user/getUsersAvailableTime`

## Begär parametrar

* **userID**: array med strängar. Obligatoriskt. Exempel: `"61a9cc0500002f9fdaa7a6f824f557e1"`.

* **fromDate**: datetime. sträng. Obligatoriskt. Exempel:  `"2022-07-10T00:00:00"`.

* **toDate**: datetime. sträng. Obligatoriskt. Exempel `"2022-07-20T23:59:59"`.

## Exempelsvar:

```
{
    "data": {
        "result": {
            "PAVL": {
                "61a9cc0500002f9fdaa7a6f824f557e1": [
                    0.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    0.0,
                    0.0,
                    480.0,
                    480.0,
                    480.0
                ]
            },
            "AVL": {
                "61a9cc0500002f9fdaa7a6f824f557e1": [
                    0.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    0.0,
                    480.0,
                    0.0,
                    480.0,
                    480.0,
                    480.0
                ]
            }
        }
    }
}
```

## Svarsparametrar

* **AVL**: Faktiskt antal tillgängliga timmar. Array med tal.
* **PAVL**: Rena tillgängliga timmar för schemaläggning som inte inkluderar lediga dagar eller ledig tid. Sträng.

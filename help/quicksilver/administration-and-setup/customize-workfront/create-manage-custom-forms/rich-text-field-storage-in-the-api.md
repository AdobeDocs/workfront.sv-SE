---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Lagring av RTF-fält i API
description: Om ett objekt, t.ex. ett projekt, en utgåva eller en uppgift innehåller RTF-text, lagras det och är tillgängligt som ett parametervärde via Workfront API.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2e4b18be-14bb-4d47-8e63-e2f4a5dc376f
source-git-commit: 3f7f4557c18bbb91ece850f910350d926a9e84bf
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---

# RTF-fältslagring i API

Om ett objekt, t.ex. ett projekt, en utgåva eller en uppgift innehåller RTF-text, lagras det och är tillgängligt som ett parametervärde via Workfront API.

Du kan begära textinformation från ett projektobjekt som innehåller RTF-text med fältet **parameterValues**.

En enkel HTTP-begäran kan till exempel likna följande:

`https://your-company.workfront.com/attask/api/v11.0/project?ID=your-project-ID&fields=parameterValues:*`

Om det här exempelprojektet innehåller ett anpassat formulär med 3 anpassade fält: beräkningsfält, stycketext och 1. Då returnerar begäran ovan ett svar som liknar följande, där fältet &quot;rich 1&quot; är ett RTF-parameterfält och textvärdet är &quot;**Hello** *World!*&quot;:

```
{
    Data: {
        ID: "xxxxxxxxxxxxxxxxxxxxxxx",
        name: "new project with rich text",
        objCode: "PROJ",
        - parameterValues: {
            DE:rich 1: "{
                "blocks":[
                {
                    "key":"7eibh",
                    "text":"Hello Word!",
                    "type":"unstyled",
                    "depth":0,
                    "inlineStyleRanges":[
                    {
                        "offset":0,
                        "length":6,
                        "style":"BOLD"
                    },
                    {
                        "offset":6,
                        "length":5,
                        "style":"ITALIC"
                    }
                    ],
                    "entityRanges":[
                    ],
                "data":{
                }
                }
                ],
            "entityMap":{
            }
        }",
        DE: paragraph text: "here is some paragraph text",
        DE: calc field: "here is a calc field entry",
        }
    }
}
```

Mer information om hur RTF-information lagras och kan hämtas via Adobe Workfront API finns i [RTF-fält i Adobe Workfront API](../../../wf-api/general/rich-text-field-api.md).

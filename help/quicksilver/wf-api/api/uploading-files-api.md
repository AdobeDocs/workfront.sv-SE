---
content-type: api
navigation-topic: api-navigation-topic
title: Överföra filer via API
description: Överföra filer via API
author: John
feature: Workfront API
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
source-git-commit: 03df0ad329255e86780c03bbb4541e0a0a526381
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Överföra filer via API

Du kan överföra filer med Workfront API:er med API-verktyg som Postman eller med enkla cURL-kommandon.

Information om hur du överför dokument finns i instruktionerna för **Överför dokument** i Workfront [Bokför beteende](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FWF_API%2FGeneral%2Fapi-basics.html). Du kan också använda samma instruktioner för cURL-begäranden.

**Följ dessa riktlinjer när du använder API-verktyg för att överföra filer:**

* Använd API-verktygsalternativet för att överföra filen. Dessa är ofta **Välj fil** på begärandeskärmen.

* Använd POSTENS HTTP-metod för att göra en begäran om att överföra filen.

* Din begäran bör resultera i ett svar som innehåller ett värde för dess referens.

* Använd handtagsvärdet, objekttypen och GUID-värdet för objID i en JSON-nyttolast för att göra ett efterföljande anrop. Detta är till för att skapa objektet för filen, som i följande exempel:

```
}
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "v1.0", "fileName" : "TestPDF"},
}
```

Du bör få ett ID för objektet i svaret.

Mer information finns i hjälpen för det API-verktyg du använder.

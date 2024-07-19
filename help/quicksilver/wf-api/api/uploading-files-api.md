---
content-type: api
navigation-topic: api-navigation-topic
title: Överföra filer via API
description: Överföra filer via API
author: Becky
feature: Workfront API
role: Developer
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# Överföra filer via API

Du kan överföra filer med Workfront API:er med API-verktyg som Postman eller med enkla cURL-kommandon.

Information om hur du överför dokument finns i instruktionerna för **överföring av dokument** i Workfront [Efterarbete](/help/quicksilver/wf-api/general/api-basics.md#post-behavior). Du kan också använda samma instruktioner för cURL-begäranden.

**Följ de här riktlinjerna när du använder API-verktyg för att överföra filer:**

* Använd API-verktygsalternativet för att överföra filen. Detta är ofta en **Välj fil**-knapp på begärandeskärmen.

* Använd POSTENS HTTP-metod för att göra en begäran om att överföra filen.

* Din begäran bör resultera i ett svar som innehåller ett värde för dess referens.

* Använd referensvärdet, objekttypen och GUID-värdet för objID i en JSON-nyttolast för att göra ett efterföljande anrop. Detta är till för att skapa objektet för filen, som i följande exempel:

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

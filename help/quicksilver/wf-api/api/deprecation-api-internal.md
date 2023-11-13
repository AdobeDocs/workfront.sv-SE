---
content-type: api
navigation-topic: api-navigation-topic
title: Borttagning av API-intern
description: Borttagning av API-intern
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
source-git-commit: acc7414a9c6eef838147aee675603b6cc2566fb9
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---

# Borttagning av API-intern

API-Internal är en version av Adobe Workfront API som inte stöds på grund av dess design och syfte. Även om den innehåller de senaste uppdateringarna av Workfront API kan den ändras utan föregående meddelande och bör därför användas med försiktighet i produktionsintegreringar. Workfront rekommenderar att du uppdaterar alla API-interna integreringar till ett versionshanterat API.

Mer information om vilka versioner av Workfront-API som stöds finns i [API-versionshantering och supportschema](../../wf-api/api/api-version-support-schedule.md).

**Använda API:t stöds inte**

Om dina integreringar kräver funktioner som inte är tillgängliga i ett versionshanterat API rekommenderar Workfront att du använder API-stöd som inte stöds. API-Intern fungerar inte på samma sätt som API-Intern. API:t stöds inte och innehåller även de senaste ändringarna av Workfront API. Reservation för ändringar. Workfront rekommenderar att du använder API:er som inte stöds i testmiljön där du kan utforska nya funktioner och se till att API:t är felfritt.

**Bestämma API-versionen som du använder**

Du kan bestämma vilken version av API som dina integreringar använder genom att använda REST för att skapa en URI som skickar ett anrop via HTTPS till Workfront och sedan returnerar ett JSON-svar.

I följande exempel visas en URI som anropar API-Internal:

```
https://<domainname>.my.workfront.com/attask/api/api-internal/proj/4c70…
```

I följande exempel visas en URI som anropar API:t stöds inte:

```
https://<domainname>.my.workfront.com/attask/api-unsupported/proj/4c70...
```

>[!NOTE]
>
>API-anrop som inte stöds utelämnar `/api` i URL:en.

I följande exempel visas en URI som anropar version 15.0 av API:t:

```
https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c70…
```

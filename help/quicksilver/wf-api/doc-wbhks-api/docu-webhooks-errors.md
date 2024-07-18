---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Felhantering av webhooks i dokument
description: Felhantering av webhooks i dokument
author: Becky
feature: Workfront API
role: Developer
exl-id: 6e0f3be7-5321-44bd-a404-d5bef1462d82
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---

# Felhantering av webhooks i dokument

Problem kan uppstå vid bearbetning av API-begäranden. Detta bör hanteras på ett konsekvent sätt i alla API-slutpunkter. När ett fel inträffar bör webbkrokprovidern inkludera en felkod i svarshuvudet. Felkoder:

* 403 - Ej tillåtet. Anger att tokens för begäran saknas eller är ogiltiga, eller att autentiseringsuppgifterna som är associerade med tokens inte har åtkomst till den angivna resursen. För OAuth-baserade webbhotell försöker Adobe Workfront hämta nya åtkomsttokens.

* 404 - Hittades inte. Anger att den angivna filen eller mappen inte finns.

* 500 - Internt serverfel. Alla andra typer av fel.

* Beskrivning av felet i svarstexten i följande format:

  ```
  {status: "error"
   error: "Sample error message"}
  ```

---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Felhantering av webhooks i dokument
description: Felhantering av webhooks i dokument
author: Becky
feature: Workfront API
exl-id: 6e0f3be7-5321-44bd-a404-d5bef1462d82
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 0%

---

# Felhantering av webhooks i dokument

Problem kan uppstå vid bearbetning av API-begäranden. Detta bör hanteras på ett konsekvent sätt i alla API-slutpunkter. När ett fel inträffar bör webbkrokprovidern inkludera en felkod i svarshuvudet. Felkoder:

* 403 - Ej tillåtet. Anger att tokens för begäran saknas eller är ogiltiga, eller att autentiseringsuppgifterna som är associerade med tokens inte har åtkomst till den angivna resursen. För OAuth-baserade webbhotell försöker Adobe Workfront hämta nya åtkomsttokens.

* 404 - Hittades inte. Anger att den angivna filen eller mappen inte finns.

* 500 - Internt serverfel. Andra typer av fel.

* Beskrivning av felet i svarstexten i följande format:

   ```
   {status: “error”
    error: “Sample error message”}
   ```

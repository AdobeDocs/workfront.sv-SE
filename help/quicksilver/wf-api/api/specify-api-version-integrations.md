---
content-type: api
navigation-topic: api-navigation-topic
title: Ange en API-version i integreringarna
description: Ange en API-version i integreringarna
author: Becky
feature: Workfront API
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# Ange en API-version i integreringarna

<span class="preview">Den markerade informationen på den här sidan avser funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i förhandsvisningssandlådemiljön.</span>

Alla Adobe Workfront URI:er krävs för att referera till en specifik version av API:t efter delen &quot;attask/api&quot; i URI:n. I följande exempel anropas version 15.0:

`attask/api/v15.0/<objectName>/<objectId>`

Se till att alla integreringar anropar Workfront API:er som stöds för närvarande.

## Schema för lansering och borttagning av Workfront API:er

Nya versioner av API släpps regelbundet, vanligen två gånger per år. Alla versioner stöds i tre år efter releasedatum, med ytterligare ett år i ett föråldrat läge där versionen är tillgänglig men inte stöds.

Mer information om publiceringsgräns och borttagningsschema för Workfront API:er finns i [API-versionshantering och supportschema](../../wf-api/api/api-version-support-schedule.md).

>[!IMPORTANT]
>
>* Efter version 23.2 ställs standardversionen av API in på den senaste versionen. Alla API-anrop utan den angivna versionen använder standardversionen. Varje gång Workfront släpper en ny version av API:t uppdateras standardversionen till den senaste versionen. När en ny version av Workfront API har släppts bör därför alla API-anrop som använder standardversionen kontrolleras för att se till att funktionen fortfarande stöds.
>
>* Om din organisation använder standardgränssnittet har Workfront-administratören fått ett meddelande om att meddelandecentret innehåller ytterligare instruktioner om standardgränssnittet.
>
>* <span class="preview">Standard-API:t i förhandsvisningsmiljön är inställt på den senaste versionen. Standard-API:t i produktionsmiljön anges till den senaste versionen efter version 23.2 (april 2023)</span>.
>
>Information om den senaste versionen av API:t finns i [API-versionshantering och supportschema](../../wf-api/api/api-version-support-schedule.md).


## Bestämma API-versionen som du använder

Du kan avgöra vilken version av API du använder genom att kontrollera URI:n för en HTTP-begäran som skickas till Workfront API. I följande exempel visas en URI för Workfront-begäran som anger version 15 av API:t:

`https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

Om en URI inte anger någon version använder den standardversionen av API:t, vilket visas i följande exempel:

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> Integrationer som inte anger någon version av API:t i URI dirigeras automatiskt till standardversionen av API:t.

## Uppdatera integreringar som ska använda API-versioner som stöds

När du skapar eller underhåller Workfront-integreringar bör du ta med en metod för dynamisk uppdatering av API-versionen och andra egenskaper som kan ändras (till exempel API-nyckeln).

Om du vill göra det enklare att uppdatera integreringar bör du överväga följande förslag för att registrera integreringsvärden:

* Lagra värden som kan komma att ändras i en egenskapsfil som du håller uppdaterad
* Skapa en webbtjänst för att hantera egenskaper i realtid
* Lagra egenskapsvärden i ett datalager som programmet kan läsa

När du utformar dina Workfront-integreringar med detta i åtanke slipper du omfattande utvecklingsarbete när dessa värden oundvikligen ändras.

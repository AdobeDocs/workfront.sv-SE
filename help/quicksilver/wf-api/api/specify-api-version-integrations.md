---
content-type: api
navigation-topic: api-navigation-topic
title: Ange en API-version i integreringarna
description: Ange en API-version i integreringarna
author: John
feature: Workfront API
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: 183f7b766fd6f02b51625778e380cf00c5ecf61f
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Ange en API-version i integreringarna

Alla Adobe Workfront URI:er krävs för att referera till en specifik version av API:t efter delen &quot;attask/api&quot; i URI:n. I följande exempel anropas version 7.0:
`attask/api/v7.0/<objectName>/<objectId>` Se till att alla integreringar anropar Workfront API:er som stöds för närvarande.

## Schema för lansering och borttagning av Workfront API:er

Nya versioner av API:t släpps vartannat år - var sjätte till åttonde månad. Alla versioner stöds i tre år efter releasedatum, med ytterligare ett år i ett föråldrat läge där versionen är tillgänglig men inte stöds.

Mer information om publiceringsgräns och borttagningsschema för Workfront API:er finns i [API-versionshantering och supportschema](../../wf-api/api/api-version-support-schedule.md).

Workfront har ersatt standardversionen av API:t från och med juli 2017. Detta innebär att Workfront inte längre anger att en viss version av API ska vara standardversionen. Alla framtida API-URI:er måste ange en version av API:t för att vara giltiga.

>[!IMPORTANT]
>
> Alla integreringar som använder standardversionen av API måste uppdateras för att anropa en specifik API-version som stöds senast 1 juli 2018.

## Bestämma API-versionen som du använder

Du kan avgöra vilken version av API du använder genom att kontrollera URI:n för en HTTP-begäran som skickas till Workfront API. I följande exempel visas en URI för Workfront-begäran som anger version 7 av API:t:

`https://<domainname>.my.workfront.com/attask/api/v7.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

Om en URI inte anger någon version använder den standardversionen av API:t, vilket visas i följande exempel:

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> Integrationer som inte anger någon version av API:t i URI dirigeras automatiskt till standardversionen av API:t och kommer inte att fungera efter 1 juli 2018.

## Uppdatera integreringar som ska använda API-versioner som stöds

När du skapar eller underhåller Workfront-integreringar bör du ta med en metod för dynamisk uppdatering av API-versionen och andra egenskaper som kan ändras (till exempel API-nyckeln).

Om du vill göra det enklare att uppdatera integreringar bör du överväga följande förslag för att registrera integreringsvärden:

* Lagra värden som kan komma att ändras i en egenskapsfil som du håller uppdaterad
* Skapa en webbtjänst för att hantera egenskaper i realtid
* Lagra egenskapsvärden i ett datalager som programmet kan läsa

När du utformar dina Workfront-integreringar med detta i åtanke slipper du omfattande utvecklingsarbete när dessa värden oundvikligen ändras.

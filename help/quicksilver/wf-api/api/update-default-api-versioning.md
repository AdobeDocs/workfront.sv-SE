---
content-type: api
navigation-topic: api-navigation-topic
title: Uppdatera integreringar som använder API-standardversionshantering
description: Uppdatera integreringar som använder API-standardversionshantering
author: Becky
feature: Workfront API
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 2b9eacc9b2c8f499cdd1794a55879a56224051c8
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---

# Uppdatera integreringar som använder API-standardversionshantering

Vi lanserar nya versioner av Adobe Workfront API vartannat år. Varje version stöds i tre år efter att den släppts, med ytterligare ett år i ett föråldrat läge där versionen är tillgänglig men inte stöds.

Integrationer som inte anger någon version av API:t i URI:n dirigeras automatiskt till Standard. Om du vill att API-anropet ska använda en viss version av API:t måste du ange den versionen i dina Workfront API-begäranden.

>[!NOTE]
>
>Om din organisation använder standardgränssnittet har Workfront-administratören fått ett meddelande om att meddelandecentret innehåller ytterligare instruktioner om standardgränssnittet.

Mer information om hur du anger en version i dina API-begäranden finns i [Ange en API-version i integreringarna](../../wf-api/api/specify-api-version-integrations.md).

## Att tänka på när du använder standard-API

Tänk på följande när du arbetar med Workfront standard-API:

* Standardversionen av API:t är den senaste versionen. Alla API-anrop utan den angivna versionen använder standardversionen. Varje gång Workfront släpper en ny version av API:t uppdateras standardversionen till den senaste versionen. **När en ny version av Workfront API har släppts bör därför alla API-anrop som använder standardversionen kontrolleras för att säkerställa att funktionen fortfarande stöds**.
* Om din organisation använder det tidigare föråldrade standard-API:t har Workfront-administratören fått ett meddelande om att meddelandecentret innehåller ytterligare instruktioner om standard-API:t.

Information om den senaste versionen av API:t finns i [API-versionshantering och supportschema](../../wf-api/api/api-version-support-schedule.md).

## Uppdatera integreringarna till API-versioner som stöds

Om dina Workfront API-begäranden inte anger någon version använder de standardversionen. Vi rekommenderar att du anger en version av API:t som stöds, helst för den senaste API:n som stöds.

Följande Workfront API-begäran anger till exempel ingen API-version:

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

När denna begäran görs får du ett svar med JSON-kodad text som anger data från din Workfront-instans. Eftersom ingen API-version har angetts i denna URI går anropet till Standard.

Om du vill omvandla en standard-API-begäran till en versionshanterad API-begäran anropar du bara en API-version som stöds. Följande URI begär till exempel version 15:

`https://davidwhite.my.workfront.com/attask/api/`**v15.0**`/project/metadata`

När du uppdaterar dina Workfront API-begäranden kan du ange vilken version av vårt API som stöds. Mer information om hur du refererar till ett specifikt API finns i [Ange en API-version i integreringarna](../../wf-api/api/specify-api-version-integrations.md).

För att få maximalt stöd bör du ringa den senaste versionen. Du hittar en lista över API:er som stöds i [API-versionshantering och supportschema](../../wf-api/api/api-version-support-schedule.md).

## Historik för standardversionen av API

Den ursprungliga avsikten med&quot;standard-API&quot;, eller Standard, var att mappa den till den senaste versionen av Workfront API. Detta gör att kunder med grundläggande integreringar som kallas Default aldrig behöver uppdatera sina API-begäranden.

2011 släppte Workfront version 3.0 av API:t. Standard flyttades automatiskt till version 3.0, som gjorde att många kundintegreringar som var för komplexa för att kunna använda version 3.0 utan att uppdateras förstördes. Därför återställde Workfront denna ändring och lämnade standardversionen i version 2.

Sedan 2011 har Workfront ökat API-funktionaliteten avsevärt. Därför har vi ersatt äldre versioner av vårt API. 2017, i stället för att uppdatera Standard, tog vi bort begreppet standardversion helt och hållet. Detta var för att uppmuntra våra kunder att använda stabila versioner av våra API:er och för att upprätthålla integreringen under en cykel på som mest tre år.

Workfront återställer nu standardversionen av API. Standard-API:t är den senaste versionen av Workfront API och uppdateras till den senaste versionen varje gång en ny version släpps.


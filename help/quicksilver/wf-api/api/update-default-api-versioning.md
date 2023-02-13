---
content-type: api
navigation-topic: api-navigation-topic
title: Uppdatera integreringar som använder API-standardversionshantering
description: Uppdatera integreringar som använder API-standardversionshantering
author: John
feature: Workfront API
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 183f7b766fd6f02b51625778e380cf00c5ecf61f
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# Uppdatera integreringar som använder API-standardversionshantering

Vi lanserar nya versioner av Adobe Workfront API vartannat år. Varje version stöds i tre år efter att den släppts, med ytterligare ett år i ett föråldrat läge där versionen är tillgänglig men inte stöds.

Integrationer som inte anger en version av API:t i URI:n dirigeras automatiskt till Standard, som har tagits bort. För att dina Workfront-integreringar ska vara giltiga måste du ange en API-version som stöds i dina Workfront API-begäranden.

Mer information om hur du anger en version i dina API-begäranden finns i [Ange en API-version i integreringarna](../../wf-api/api/specify-api-version-integrations.md).

## Om standardversionen av API:t

Den ursprungliga avsikten med&quot;standard-API&quot;, eller Standard, var att mappa den till den senaste versionen av Workfront API. Detta gör att kunder med grundläggande integreringar som kallas Default aldrig behöver uppdatera sina API-begäranden.

2011 släppte Workfront version 3.0 av API:t. Standard flyttades automatiskt till version 3.0, som gjorde att många kundintegreringar som var för komplexa för att kunna använda version 3.0 utan att uppdateras förstördes. Därför återställde Workfront denna ändring och lämnade standardversionen i version 2.

Tyvärr har det här avsnittet aldrig granskats, och nu när vi planerar att öka API-funktionaliteten avsevärt måste vi överge äldre versioner av vårt API, inklusive Default. I stället för att uppdatera Default, vilket utan tvekan skulle kunna bryta ned fler integreringar, tar vi bort begreppet standardversion helt och hållet. Detta är för att uppmuntra våra kunder att använda stabila versioner av våra API:er och för att upprätthålla integreringen under en cykel på som mest tre år.

## Inaktuellt standard

I ett försök att förbättra Workfront API håller vi på att ta bort äldre API-versioner som har överskridit supportperioden på tre år. En av dessa versioner är version 2, som Standard är mappat till. Den här versionen släpptes 2010 och mycket av logiken som stöds i Attask/Workfront-programmet finns inte längre eller har ändrats avsevärt.

Vi ersatte Default i juli 2017 och vi kommer inte längre att ange att en specifik version av API:t ska vara standardversionen. I stället måste alla Workfront API-begäranden ange en specifik API-version.

>[!IMPORTANT]
>
> Senast den 1 juli 2018 måste alla Workfront-integreringar som använder Default uppdateras för att anropa en specifik API-version som stöds. Efter detta datum kommer alla dina Workfront API-begäranden som används av integreringar som inte anger någon version att misslyckas.

Mer information om Workfront cadence finns i [API-versionshantering och supportschema](../../wf-api/api/api-version-support-schedule.md).

## Uppdatera integreringarna till API-versioner som stöds

Om dina Workfront API-begäranden inte anger någon version använder de standardversionen. Du måste uppdatera dina API-begäranden för att ange en version av API som stöds, helst till den senaste API som stöds.

Följande Workfront API-begäran anger till exempel ingen API-version:

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

När denna begäran görs får du ett svar med JSON-kodad text som anger data från din Workfront-instans. Eftersom ingen API-version har angetts i denna URI går anropet till Standard.

Om du vill omvandla en standard-API-begäran till en versionshanterad API-begäran anropar du bara en API-version som stöds. Följande URI begär till exempel version 9:

`https://davidwhite.my.workfront.com/attask/api/`**v9.0**`/project/metadata`

När du uppdaterar dina Workfront API-begäranden kan du ange vilken version av vårt API som stöds. Mer information om hur du refererar till ett specifikt API finns i [Ange en API-version i integreringarna](../../wf-api/api/specify-api-version-integrations.md).

För att få maximalt stöd bör du ringa den senaste versionen (version 9). Du hittar en lista över API:er som stöds i [API-versionshantering och supportschema](../../wf-api/api/api-version-support-schedule.md).

Det är viktigt att du uppdaterar de integreringar du har som använder Standard. Om du för närvarande har integreringar som inte anger någon version kan du få ett meddelande från din Workfront-säljare, kundframgångsansvarige, supportrepresentant eller ett meddelande från vår kundtjänst.

Se till att integreringarna uppdateras så snart som möjligt för att anropa en version av vårt API som stöds.

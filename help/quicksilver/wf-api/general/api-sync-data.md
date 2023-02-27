---
content-type: api
keywords: API,data,synk,journal,post,objekt
navigation-topic: general-api
title: Synkronisera data för program och tjänster med API:t
description: Synkronisera data för program och tjänster med API:t
author: Becky
feature: Workfront API
exl-id: 1d0583fc-1573-4279-a3fa-a912d9a4213c
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---


# Synkronisera data för program och tjänster med API:t

Detta är några vanliga sätt för dig att använda API:t för att synkronisera data för program och tjänster.

## Nära realtidsuppdateringar

Adobe Workfront använder&quot;Event Subscriptions&quot; (även kallat webhooks) för att skicka nästan realtidsuppdateringar om objekt och åtgärder som stöds via API:n till önskad slutpunkt. Du kan förvänta dig en uppdatering om nya objekt och åtgärder inom 5 sekunder, men i genomsnitt kommer uppdateringar om cirka 1 sekund. Mer information om vilken typ av objekt som stöds finns i vilka typer av åtgärder som stöds, teknisk information och exempel på hur du ställer in händelseprenumerationer. [API för händelseprenumeration](../../wf-api/general/event-subs-api.md) och [Leveranskrav för evenemangsprenumeration](../../wf-api/general/setup-event-sub-endpoint.md).

## Batchuppdateringar

Batchuppdateringar är ett sätt att konfigurera systemet för uppdateringar genom att göra regelbundna förfrågningar till Workfront-servrar. Det finns många sätt att göra detta, men i allmänhet består processen av att låta tjänsten göra en begäran till Workfront API-servrar och söka efter objekt som har skapats eller ändrats sedan den senaste anropet. Information om potentiella förfrågningar och användbara parametrar finns i [GET](../../wf-api/general/api-basics.md#get-behavior) från [Grunderna i API](../../wf-api/general/api-basics.md) artikel.

När du konfigurerar tjänsten för batchuppdateringar här är några viktiga saker att tänka på:

### Anmälningsdatum

Anmälningsdatum lagras med ISO 8601-formatering. Den här standarden innehåller datum-, tids- och tidszonsinformation.

**Exempel:** ISO 8601 datumformat

<!-- [Copy](javascript:void(0);) -->
 
<pre><code>2020-05-18T17:00:00:000-0600</code></pre> 

Både datumet då ett objekt skapas och det senaste datumet som objektet ändrades lagras som &quot;entryDate&quot; respektive &quot;lastUpdateDate&quot;. Mer information om Workfront-objekt, deras associerade fält och fältnamn finns i [API Explorer](../../wf-api/general/api-explorer.md). Observera att entryDate för ett givet Workfront-objekt inte ändras där lastUpdatedDate ändras varje gång objektet ändras.

**Exempel:** GET-begäran för ett problemobjekt, med **lastUpdateDate** fält. Denna begäran returnerar alla utgåvor som har uppdaterats sedan det angivna datumet.

<!-- [Copy](javascript:void(0);) -->
 

```
GET
https://<domain>.my.workfront.com/attask/api/v15.0/OPTASK/search?fields=ID,name,lastUpdateDate&$$LIMIT=200&lastUpdateDate=2020-05-13T18:18:37.255Z&lastUpdateDate_Mod=gte
```

### Journalpostobjekt

Om du är intresserad av att få ändringar som rör ett specifikt fält i ett objekt kan du fråga objektet Journalpost. Objektet Workfront Journal Entry kan ställas in för att logga information om specifika objektfält när dessa fält ändras, se [Konfigurera systemuppdateringar](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md) om du vill ha mer information.

När ett fält har konfigurerats för att loggas som en del av journaltransaktionsobjektet skapas en motsvarande journalpost varje gång fältet ändras. Sedan kan du fråga efter objektet Journal Entry med hjälp av ett API-anrop som ser ut ungefär så här:

<!-- [Copy](javascript:void(0);) -->

<pre><code>GET https://&#123;&#123;domain&#125;&#125;.my.workfront.com/attask/api/v15.0/JRNLE/search?fields=newTextVal,oldTextVal,newDateVal,oldDateVal,newNumberVal,oldNumberVal,entryDate,objObjCode,objID,fieldName&fieldName=name&objObjCode=OPTASK&entryDate=2020-05-13T18:18:37.255Z&entryDate_Mod=gte</code></pre>

>[!NOTE]
>
>&quot;entryDate&quot; används för att titta på en journalpost för en ändring, i motsats till att titta på det ändrade objektet.

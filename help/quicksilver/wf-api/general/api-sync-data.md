---
content-type: api
keywords: API,data,synk,journal,post,objekt
navigation-topic: general-api
title: Synkronisera data för program och tjänster med API:t
description: Synkronisera data för program och tjänster med API:t
author: Becky
feature: Workfront API
role: Developer
exl-id: 1d0583fc-1573-4279-a3fa-a912d9a4213c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---


# Synkronisera data för program och tjänster med API:t

Detta är några vanliga sätt för dig att använda API:t för att synkronisera data för program och tjänster.

## Nära realtidsuppdateringar

Adobe Workfront använder&quot;Event Subscriptions&quot; (även kallat webhooks) för att skicka nästan realtidsuppdateringar om objekt och åtgärder som stöds via API:n till önskad slutpunkt. Du kan förvänta dig en uppdatering om nya objekt och åtgärder inom 5 sekunder, men i genomsnitt kommer uppdateringar om cirka 1 sekund. Mer information om vilka typer av objekt som stöds finns i [Event Subscription API](../../wf-api/general/event-subs-api.md) och [Event Subscription delivery requirements](../../wf-api/general/setup-event-sub-endpoint.md).

## Batchuppdateringar

Batchuppdateringar är ett sätt att konfigurera systemet för uppdateringar genom att göra regelbundna förfrågningar till Workfront-servrar. Det finns många sätt att göra detta, men i allmänhet består processen av att låta tjänsten göra en begäran till Workfront API-servrar och söka efter objekt som har skapats eller ändrats sedan den senaste anropet. Mer information om möjliga anrop och användbara parametrar finns i avsnittet [GET Behavior](../../wf-api/general/api-basics.md#get-behavior) i artikeln [API basics](../../wf-api/general/api-basics.md) .

När du konfigurerar tjänsten för batchuppdateringar här är några viktiga saker att tänka på:

### Anmälningsdatum

Anmälningsdatum lagras med ISO 8601-formatering. Den här standarden innehåller datum-, tids- och tidszonsinformation.

**Exempel:** ISO 8601-datumformat

<!-- [Copy](javascript:void(0);) -->
 
<pre><code>2020-05-18T17:00:00:000-0600</code></pre> 

Både datumet då ett objekt skapas och det senaste datumet som objektet ändrades lagras som &quot;entryDate&quot; respektive &quot;lastUpdateDate&quot;. Mer information om Workfront-objekt, deras associerade fält och fältnamn finns i [API-utforskaren](../../wf-api/general/api-explorer.md). Observera att entryDate för ett givet Workfront-objekt inte ändras där lastUpdatedDate ändras varje gång objektet ändras.

**Exempel:** GET-förfrågan för ett problemobjekt, med hjälp av fältet **lastUpdateDate**. Denna begäran returnerar alla utgåvor som har uppdaterats sedan det angivna datumet.

<!-- [Copy](javascript:void(0);) -->
 

```
GET
https://<domain>.my.workfront.com/attask/api/v15.0/OPTASK/search?fields=ID,name,lastUpdateDate&$$LIMIT=200&lastUpdateDate=2020-05-13T18:18:37.255Z&lastUpdateDate_Mod=gte
```

### Journalpostobjekt

Om du är intresserad av att få ändringar som rör ett specifikt fält i ett objekt kan du skicka en fråga till objektet Journalpost. Workfront Journal Entry-objektet kan konfigureras för att logga information om specifika objektfält när dessa fält ändras. Mer information finns i [Konfigurera systemuppdateringar](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md) .

När ett fält har konfigurerats för att loggas som en del av journaltransaktionsobjektet skapas en motsvarande journalpost varje gång fältet ändras. Sedan kan du fråga efter objektet Journal Entry med hjälp av ett API-anrop som ser ut ungefär så här:

<!-- [Copy](javascript:void(0);) -->

<pre><code>GET https://&#123;&#123;domain&#125;&#125;.my.workfront.com/attask/api/v15.0/JRNLE/search?fields=newTextVal,oldTextVal,newDateVal,oldDateVal,newNumberVal,oldNumberVal,entryDate,objObjCode,objID,fieldName&fieldName=name&objObjCode=OPTASK&entryDate=2020-05-13T18:18:37.255Z&entryDate_Mod=gte</code></pre>

>[!NOTE]
>
>&quot;entryDate&quot; används för att titta på en journalpost för en ändring, i motsats till att titta på det ändrade objektet.

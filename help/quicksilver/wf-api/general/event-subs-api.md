---
content-type: api
navigation-topic: general-api
title: API för händelseprenumeration
description: API för händelseprenumeration
author: Becky
feature: Workfront API
role: Developer
exl-id: c3646a5d-42f4-4af8-9dd0-e84977506b79
source-git-commit: d92dc8581bef1f5fdbef7a853ac27ffc3fa7ddbe
workflow-type: tm+mt
source-wordcount: '2157'
ht-degree: 0%

---


# API för händelseprenumeration

<!--BOB clean this up-->

<!--
{{highlighted-preview}}
-->

När en åtgärd inträffar för ett Adobe Workfront-objekt som stöds av händelseprenumerationer, kan du konfigurera Workfront att skicka ett svar till önskad slutpunkt. Detta innebär att tredjepartsprogram kan ta emot uppdateringar från Workfront-interaktioner via Workfront API så snart de har släppts. Normalt kan du förvänta dig att få webkrokmeddelanden på mindre än 5 sekunder från det att dataändringen loggas. I genomsnitt får kunderna webkrokmeddelanden på mindre än en sekund från den dataändring som loggas.  

För att kunna ta emot händelseprenumerationsnyttolaster via din brandvägg måste du lägga till följande IP-adresser i tillåtelselista:

**För kunder i Europa:**

* 52.30.133.50
* 52.208.159.124
* 54.220.93.204
* 52.17.130.201
* 34.254.76.122
* 34.252.250.191

**För kunder på andra platser än Europa:**

* 54.244.142.219
* 44.241.82.96
* 52.36.154.34
* 34.211.224.9
* 54.218.48.56
* 52.39.217.230

Följande avsnitt har stöd för Event Subscription API:

## Objekt som stöds av händelseprenumerationer

Följande Workfront-objekt stöds av händelseprenumerationer.

* Tilldelning
* Företag
* Kontrollpanel
* Dokument
* Utgift
* Fält
* Timme
* Problem
* Anteckning
* Portfolio
* Program
* Projekt
* Post
* Posttyp
* Rapport
* Uppgift
* Mall
* Tidrapport
* Användare
* Workspace

En lista över fält som stöds av händelseprenumerationsobjekt finns i [Resursfält för händelseprenumerationer](../../wf-api/api/event-sub-resource-fields.md).

## Autentisering av händelseabonnemang

Om du vill skapa, fråga efter eller ta bort en händelseprenumeration behöver din Workfront-användare följande:

* Du måste ha åtkomstnivån &quot;Systemadministratör&quot; för att kunna använda händelseprenumerationer.
* Ett `sessionID`-huvud krävs för att använda API:t för händelseprenumerationer

  Mer information finns i [Autentisering](api-basics.md#authentication) i [API-grunder](api-basics.md).

## Formge prenumerationsresursen

Prenumerationsresursen innehåller följande fält.

* objId (valfritt)

   * **String** - ID:t för objektet för den angivna objCode som händelser utlöses för. Om det här fältet inte anges tar användaren emot händelser för alla objekt av den angivna typen.

* objCode (obligatoriskt)

   * **String** - ObjCode för objektet som prenumererar på ändringar. Möjliga värden för objCode listas i tabellen nedan.

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <thead> 
       <tr> 
        <th><p>Objekt</p></th> 
        <th><p>objCode</p></th> 
       </tr> 
      </thead> 
      <tbody> 
       <tr> 
        <td scope="col">Tilldelning</td> 
        <td scope="col"><p>ASSGN</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Företag </td> 
        <td scope="col"><p>CMPY</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Kontrollpanel</td> 
        <td scope="col">PTLTAB</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Dokument</p></td> 
        <td scope="col">DOCU </td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Utgift</p></td> 
        <td scope="col">EXPNS</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Fält</p></td> 
        <td scope="col"><p>FÄLT</p></td> 
       </tr> 
      <tr> 
        <td scope="col"><p>Timme</p></td> 
        <td scope="col">TIMME</td> 
       </tr> 
       <tr> 
        <td scope="col">Problem</td> 
        <td scope="col"><p>OPTASK</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Anteckning</td> 
        <td scope="col">ANMÄRKNING</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Portfolio</p></td> 
        <td scope="col"><p>PORT</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Program</p></td> 
        <td scope="col"><p>PRGM</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Projekt</p></td> 
        <td scope="col"><p>PROJ</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Post</p></td> 
        <td scope="col"><p>POST</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Posttyp</p></td> 
        <td scope="col"><p>RECORD_TYPE</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Rapport</p></td> 
        <td scope="col"><p>PTLSEC</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Uppgift</p></td> 
        <td scope="col"><p>UPPGIFT</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Mall</p></td> 
        <td scope="col"><p>TMPL</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Tidrapport</td> 
        <td scope="col">TSTIPSE</td> 
       </tr> 
       <tr> 
        <td scope="col">Användare</td> 
        <td scope="col">ANVÄNDARE</td> 
       </tr> 
       <tr> 
        <td scope="col">Workspace</td> 
        <td scope="col">WORKSPACE</td> 
       </tr> 
      </tbody> 
     </table>

* eventType (obligatoriskt)

   * **String** - Ett värde som representerar den typ av händelse som objektet prenumererar på. De tillgängliga händelsetyperna är:

      * SKAPA
      * DELETE 
      * UPPDATERA

* url (obligatoriskt)

   * **String** - URL:en för den slutpunkt till vilken prenumerationshändelsenyttolaster skickas via HTTP.

* authToken (obligatoriskt)

   * **String** - Bearer-token för OAuth2 används för att autentisera med den URL som anges i URL-fältet. 

## Skapa API-begäranden för händelseprenumeration

När du har försäkrat dig om att användaren har administratörsåtkomst och skapar prenumerationsresursen kan du skapa händelseprenumerationer.

Använd följande syntax för att skapa URL:en.

**Begär URL:**


```
POST https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**Begäranrubriker:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Rubriknamn</p> </th> 
   <th> <p>Huvudvärde</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Innehållstyp</p> </td> 
   <td> <p>application/json</p> </td> 
  </tr> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>sessionID-värde</p> </td> 
  </tr> 
 </tbody> 
</table>

**Exempel på begärandebrödtext:**

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua",
                "authToken": "EauthTokenWorkfrontRocks1234_"
            }
```

| Svarskod | Beskrivning |
|---|---|
| 201 (skapad) | Evenemangsprenumerationen har skapats. |
| 400 (felaktig begäran) | URL-fältet för prenumerationsresursen ansågs vara ogiltigt. |
| 401 (obehörig) | Angivet sessions-ID var tomt eller ansågs ogiltigt. |
| 403 (Ej tillåtet) | Användaren som matchar angivet sessions-ID har inte administratörsåtkomst. |

Om du skickar en prenumerationsresurs som innehåll för en begäran (med innehållstypen &quot;application/json&quot;) skapas en händelseprenumeration för det angivna objektet. Svarskoden 201 (Skapad) anger att prenumerationen skapades. En annan svarskod än 201 innebär att prenumerationen **INTE** skapades.

>[!NOTE]
>
> Svarshuvudet &quot;Location&quot; innehåller URI:n för den nyligen skapade händelsprenumerationen.

**Exempel på svarshuvuden:**

| Svarshuvuden | Exempel |
|---|---|
| Content-Length | `→0` |
| Datum | `→Wed, 05 Apr 2017 21:23:33 GMT` |
| Plats | `→https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/750a636c-5628-48f5-ba26-26b7ce537ac2` |
| Server | `→Apache-Coyote/1.1` |

## Fråga om händelseprenumerationer

När du frågar efter Workfront HTTP använder du GET-metoden. Det finns två sätt att fråga efter händelseprenumerationer: Fråga efter prenumerations-ID (se nedan) eller fråga alla händelseprenumerationer.

### Fråga alla händelseprenumerationer

Du kan fråga alla händelseprenumerationer för en kund eller använda följande för att hantera svaret. Du kan också använda följande alternativ för att hantera svaret:

* **sida**: frågeparameteralternativ som anger hur många sidor som ska returneras. Standardvärdet är 1.
* **limit**: frågeparameteralternativ som anger antalet resultat som ska returneras per sida. Standardvärdet är 100 med högst 1 000.

Syntaxen för att ange alla händelseprenumerationer för en viss kund är följande:

**Begär URL:**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**Begäranrubriker:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Rubriknamn</p> </th> 
   <th> <p>Huvudvärde</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>sessionID-värde</p> </td> 
  </tr> 
 </tbody> 
</table>

**Svarskoder:**

| Svarskod | Beskrivning |
|---|---|
| 200 (OK) | Begäran som returnerades med alla händelseprenumerationer som hittades för kunden och som matchar angivet sessions-ID. |
| 401 (obehörig) | Angivet sessions-ID var tomt. |
| 403 (Ej tillåtet) | Användaren, som matchar angivet sessions-ID, har inte administratörsåtkomst. |


**Exempel på svarshuvuden:**

| Svarshuvud | Exempel |
|---|---|
| Content-Type | `→application/json;charset=UTF-8` |
| Datum | `→Wed, 05 Apr 2017 21:29:32 GMT` |
| Server | `→Apache-Coyote/1.1` |
| Överföringskodning | `→chunked` |


**Exempel på svarstext:**

<!-- [Copy](javascript:void(0);) -->

```
                {
                "subscriptions":                
                [
                {
                "id": "37c4bcf5-e0b5-4256-aba3-a51cba7bf997",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": "ObjId1234",
                "objCode": "TASK",
                "url": "http://test.test.net/test/1234",
                "eventType": "UPDATE",
                "authToken": "auth_token"
                },
                {
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": null,
                "objCode": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "eventType": "UPDATE",
                "authToken": "authTokenWorkfrontRocks1234_"
                }
                ],
                "meta":
                {
                "page": 1,
                "page_count": 2,
                "limit": 100,
                "total_count": 150
                }
                }            
```

Plats

* **page** och **limit** är värdena som anges i begäran eller standardvärdet om inga värden anges
* **page_count** är det totala antalet sidor som kan efterfrågas.
* **total_count** är det totala antalet prenumerationer som matchar frågan.

### Fråga efter händelsens prenumerations-ID

Du kan fråga efter händelseprenumerationer med hjälp av händelseprenumerationens ID. Syntaxen för att ange händelseprenumerationer är följande:

**Begär URL:**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**Begäranrubriker:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Rubriknamn</p> </th> 
   <th> <p>Huvudvärde</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>sessionID-värde</p> </td> 
  </tr> 
 </tbody> 
</table>

**Svarskoder:**

| Svarskod | Beskrivning |
|---|---|
| 200 (OK) | Begäran som returnerades med händelseprenumerationen som matchar det angivna prenumerations-ID:t. |
| 401 (obehörig) | Angivet sessions-ID var tomt. |
| 403 (Ej tillåtet) | Användaren, som matchar angivet sessions-ID, har inte administratörsåtkomst. |


**Exempel på svarstext:**

<!-- [Copy](javascript:void(0);) -->

```
{
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": null,
                "objCode": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "eventType": "UPDATE",
                "authToken": "authTokenWorkfrontRocks1234_"
                }
```

## Filtrering av händelseprenumeration

Du kan använda händelseprenumerationsfiltrering för att försäkra dig om att du bara får relevanta meddelanden. Om du skapar filter för dina prenumerationer kan det minska antalet meddelanden som slutpunkten behöver ta emot avsevärt.

En **UPDATE - TASK** -händelseprenumeration kan till exempel bara anges som utlösare när **newState** för en händelsenyttolast definierar **taskStatus** som **current**.

>[!IMPORTANT]
>
>Följande attribut gäller för händelseprenumerationsfiltrering

* När ett filterfält har ett värde som inte är tomt skickas bara meddelanden med en **newState** som innehåller filternycklarna och värdena till den prenumererade URL:en
* Du kan filtrera efter anpassade data som ingår i objektets **newState** AND/OR **oldState**
* Filter utvärderas enbart utifrån om de är lika med ett visst värde eller inte
* Om filtersyntaxen är felaktig eller inte matchar några data som finns i **newState** i nyttolasten, returneras inget valideringsmeddelande som anger att ett fel har inträffat
* Det går inte att uppdatera filter för en prenumeration som redan finns. En ny prenumeration måste skapas med nya filterparametrar.
* Flera filter kan tillämpas på en prenumeration och prenumerationen levereras endast när alla filtervillkor är uppfyllda.
* Att tillämpa flera filter på en prenumeration är en procedur som motsvarar att använda en logisk **AND** -operator.
* Flera händelseprenumerationer kan användas på ett enda objekt så länge som en eller flera parametrar för händelseprenumerationsfält är olika för varje händelseteckning.
* När flera händelseprenumerationer tilldelas till ett enda objekt kan alla händelseprenumerationer som är kopplade till det objektet returneras till en enda slutpunkt. Den här metoden kan användas som en motsvarande ersättning för den logiska operatorn **OR** som inte kan anges med filterparametrar.
* Följande fält kan inte filtreras:

   * DOCU.groups
   * RECORD.data
   * RECORD_TYPE.data
   * RECORD_TYPE.fields

### Använda jämförelseoperatorer

Du kan ange ett jämförelsefält tillsammans med filterfältet. Använd en jämförelseoperator i det här fältet för att filtrera för jämförande resultat. Du kan till exempel skapa en UPDATE - TASK-prenumeration som bara skickar en nyttolast om aktivitetsstatusen INTE är lika med aktuell. Du kan använda följande jämförelseoperatorer:

#### eq: lika

Med det här filtret kan meddelanden visas om ändringen som inträffade matchar `fieldValue` i filtret exakt. Värdet `fieldValue` är skiftlägeskänsligt.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "eq"
        }
    ]
}
```

#### ne: inte lika med

Med det här filtret kan meddelanden visas om ändringen som inträffade inte matchar `fieldValue` i filtret exakt. Värdet `fieldValue` är skiftlägeskänsligt.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "ne"
        }
    ]
}
```

#### gt: större än

Med det här filtret kan meddelanden visas om uppdateringen för den angivna `fieldName` är större än värdet för `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-11T16:00:00.000-0800",
            "comparison": "gt"
        }
    ]
}
```

#### gte: större än eller lika med

Det här filtret tillåter att meddelanden visas om uppdateringen för den angivna `fieldName` är större än eller lika med värdet för `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-11T16:00:00.000-0800",
            "comparison": "gte"
        }
    ]
}
```

#### lt: mindre än

Med det här filtret kan meddelanden visas om uppdateringen för den angivna `fieldName` är mindre än värdet för `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-18T16:00:00.000-0800",
            "comparison": "lt"
        }
    ]
}
```

#### lte: mindre än eller lika med

Det här filtret gör att meddelanden kan visas om uppdateringen för den angivna `fieldName` är mindre än eller lika med värdet för `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-18T16:00:00.000-0800",
            "comparison": "lte"
        }
    ]
}
```

#### innehåller

Med det här filtret kan meddelanden visas om ändringen som inträffade innehåller `fieldValue` i filtret. Värdet `fieldValue` är skiftlägeskänsligt

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains"
        }
    ]
}
```

#### change

Det här filtret tillåter bara att meddelanden visas om det angivna fältet (`fieldName`) har ett annat värde i läget oldstate och newstate. Uppdatering av andra fält förutom det angivna (`fieldName`) returnerar inte den ändringen.

>[!NOTE]
>
>`fieldValue` i filterarrayen nedan har ingen effekt.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "",
            "comparison": "changed"
        }
    ]
}
```

#### läge

Den här kopplingen gör att filtret tillämpas på det nya eller gamla läget för objektet som skapades eller uppdaterades. Detta är praktiskt när du vill veta var en ändring gjordes från något till något annat.
`oldState` är inte möjligt på CREATE `eventTypes`.

>[!NOTE]
>
>Prenumerationen nedan med det angivna filtret returnerar bara meddelanden där aktivitetens namn innehåller `again` på `oldState`, vilket var innan en uppdatering gjordes för aktiviteten.
>Ett användbart exempel för detta skulle vara att hitta objCode-meddelandena som ändrades från en sak till en annan. Om du till exempel vill ta reda på alla uppgifter som har ändrats från &quot;Research Some name&quot; till &quot;Research TeamName Some name&quot;

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains",
            "state": "oldState"
        }
    ]
}
```

### Använda kopplingsfält

I fältet `filterConnector` på prenumerationsnyttolasten kan du välja hur filtren ska tillämpas. Standardvärdet är&quot;AND&quot;, där alla filter måste vara `true` för att prenumerationsmeddelandet ska visas. Om du anger &quot;OR&quot; får bara ett filter matcha för att prenumerationsmeddelandet ska visas.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains"
        },
        {
            "fieldName": "name",
            "fieldValue": "also",
            "comparison": "contains"
        }
    ],
    "filterConnector": "AND"
}
```

## Ta bort händelseprenumerationer

När du tar bort Workfront HTTP använder du metoden DELETE. Syntaxen för begäran om att ta bort en prenumeration för en händelse med prenumerations-ID är följande:

**Begär URL:**

<!-- [Copy](javascript:void(0);) -->

```
DELETE https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**Begäranrubriker:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Rubriknamn</p> </th> 
   <th> <p>Huvudvärde</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p> sessionID-värde </p> </td> 
  </tr> 
 </tbody> 
</table>

**Svarskoder:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Svarskod</p> </th> 
   <th> Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 (inget innehåll)</td> 
   <td>Servern har tagit bort den händelseprenumeration som matchar angivet prenumerations-ID.</td> 
  </tr> 
  <tr> 
   <td>401 (obehörig)</td> 
   <td>Angivet sessions-ID var tomt.</td> 
  </tr> 
  <tr> 
   <td>403 (Ej tillåtet)</td> 
   <td>Användaren som matchar angivet sessions-ID har inte administratörsåtkomst.</td> 
  </tr> 
  <tr> 
   <td>404 (Hittades inte)</td> 
   <td>Servern kunde inte hitta någon händelseteckning som matchar det prenumerations-ID som angavs för borttagning.</td> 
  </tr> 
 </tbody> 
</table>

**Exempel på svarshuvuden:**

| Svarshuvud | Exempel |
|---|---|
| Datum | `→Wed, 05 Apr 2017 21:33:41 GMT` |
| Server | `→Apache-Coyote/1.1` |


**Exempel på svarstext:** Ej tillämpligt

## Exempel på händelsenyttolaster

Nyttolasten som en användare tar emot varierar beroende på objekttypen, men det finns ett konsekvent format som de olika nyttolasterna levereras för.

Följande egenskaper är till exempel konsekventa för alla händelsenyttolaster:

* eventType
* subscriptionId
* oldState
* newState
* eventTime

Även om formatet är konsekvent varierar värdena i egenskaperna mellan olika objekt och objekttyper.

Nedan visas exempel på nyttolaster för en UPDATE-händelse och en CREATE-händelse. Observera i UPDATE-exemplet att objekten oldState och newState är desamma, medan objektet oldState i CREATE-exemplet är tomt (inte NULL).

Nedan följer ett exempel på nyttolast för en UPDATE-händelse:

<!-- [Copy](javascript:void(0);) -->

```
{
                  "eventType": "UPDATE",
                   "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                   "eventTime": {
                       "nano": 998000000,
                       "epochSecond": 1507319336
                   },
                   "newState": {
                "ID": "59d7ddf7000002322d791eb08bafddfb", 
                       "name": "EventSub Test updated",
                       "objCode": "PROJ",
                       "entryDate": "2017-10-06T13:48:07.776-0600",
                       "accessorIDs": [
                           "544820df0000142362741fc0c368de19"
                       ],
                       "lastUpdateDate": "2017-10-06T13:48:56.980-0600",
                       "groupID": "544820df0000140f6a9c1faa7cacadd3",
                       "sponsorID": null,
                       "description": null,
                       "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
                       "enteredByID": "544820df0000142362741fc0c368de19",
                       "ownerID": "544820df0000142362741fc0c368de19",
                       "templateID": null,
                       "priority": 0,
                       "companyID": null,
                       "portfolioID": null,
                       "referenceNumber": 1894,
                       "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                       "customerID": "544820df0000135b7719dcca654391f6",
                       "currency": null,       "categoryID": null,
                      "status": "CUR",
                      "parameterValues": {}
                   },
                   "oldState": {
                       "ID": "59d7ddf7000002322d791eb08bafddfb",
                       "name": "EventSub Test 180fd595-63fb-4fa9-bd47-58bf6e53d964",
                       "objCode": "PROJ",
                       "entryDate": "2017-10-06T13:48:07.776-0600",
                       "accessorIDs": [
                           "544820df0000142362741fc0c368de19"
                       ],
                       "lastUpdateDate": "2017-10-06T13:48:07.792-0600",
                       "groupID": "544820df0000140f6a9c1faa7cacadd3",
                       "sponsorID": null,
                       "description": null,
                       "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
                       "enteredByID": "544820df0000142362741fc0c368de19",
                       "ownerID": "544820df0000142362741fc0c368de19",
                       "templateID": null,
                       "priority": 0,
                       "companyID": null,<
                       "portfolioID": null,
                       "referenceNumber": 1894,
                       "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                       "customerID": "544820df0000135b7719dcca654391f6",
                       "currency": null,
                       "categoryID": null,
                       "status": "CUR",
                       "parameterValues": {}
                   }
                }
```

Nedan följer ett exempel på nyttolast för en CREATE-händelse:

<!-- [Copy](javascript:void(0);) -->

```
{
                "eventType": "CREATE",
                "subscriptionId": "4028e3815ebf03a7015ebfa53b6d0002",
                "eventTime": {
                "nano": 232000000,
                "epochSecond": 1506453831
                },
                "newState": {
                "ID": "59caa946000000e07b0afc3383230c67",
                "name": "EventSub Test fe16d470-0a40-4290-92f4-6a0389fb536c",
                "objCode": "PROJ",
                "entryDate": "2017-09-26T13:23:50.746-0600",
                "accessorIDs": ["544820df0000142362741fc0c368de19"],
                "lastUpdateDate": "2017-09-26T13:23:50.927-0600",
                "groupID": "544820df0000140f6a9c1faa7cacadd3",
                "sponsorID": null,
                "description": null,
                "plannedCompletionDate": "2017-09-26T09:00:00.000-0600",
                "enteredByID": "544820df0000142362741fc0c368de19",
                "ownerID": "544820df0000142362741fc0c368de19",
                "templateID": null,
                "priority": 0,
                "companyID": null,
                "portfolioID": null,
                "referenceNumber": 1750,
                "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                "customerID": "544820df0000135b7719dcca654391f6",
                "currency": null,
                "categoryID": null,
                "status": "CUR",
                "parameterValues": {}
                },
                "oldState": {}
            }
```

## Base 64-kodning

Om en evenemangsprenumeration avvisas på grund av en konflikt mellan specialtecken i dina evenemangsprenumerationer och nätverksinställningarna kan du använda Base64-kodning för att skicka dina evenemangsprenumerationer. Base64 är en uppsättning kodningsscheman som kan översätta alla godtyckliga data till ett ASCII-strängformat. Observera att Base64 inte är en form av säkerhetskryptering.

### Base 64-kodningsfält

base64Encoding-fältet är ett valfritt fält som används för att aktivera Base64-kodning av händelseprenumerationsnyttolaster. Standardvärdet är false och de möjliga värdena är: true, false och &quot; (blank).

### Exempel på en begäran som använder base64Encoding-fältet

Om en begäran görs med base64Encoding-fältet inställt på true, levereras objekten **newState** och **oldState** i nyttolasten som 64-grundkodningssträngar. Om base64Encoding-fältet är inställt på false, lämnas tomt eller inte ingår i begäran, kommer den returnerade nyttolasten inte att kodas i bas 64.

Följande är ett exempel på en begäran som använder base64Encoding-fältet:

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua"",
                "authToken": "EauthTokenWorkfrontRocks1234_",
                "base64Encoding": "true"
            }
```

### Exempel på svarsnyttolaster i bas 64-kodning

<!-- [Copy](javascript:void(0);) -->

```
                {
                "eventType": "UPDATE",
                "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                "eventTime": {
                "nano": 998000000,
                "epochSecond": 1507319336
                },
                "newState": "ewogICAgICAgIklEIjogIjU5ZDdkZGY3MDAwMDAyMzIyZDc5MWViMDhiYWZkZGZiIiwgCiAgICAgICAibmFtZSI6ICJFdmVudFN1YiBUZXN0IHVwZGF0ZWQiLAogICAgICAgIm9iakNvZGUiOiAiUFJPSiIsCiAgICAgICAiZW50cnlEYXRlIjogIjIwMTctMTAtMDZUMTM6NDg6MDcuNzc2LTA2MDAiLAogICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICI1NDQ4MjBkZjAwMDAxNDIzNjI3NDFmYzBjMzY4ZGUxOSIKICAgICAgIF0sCiAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODo1Ni45ODAtMDYwMCIsCiAgICAgICAiZ3JvdXBJRCI6ICI1NDQ4MjBkZjAwMDAxNDBmNmE5YzFmYWE3Y2FjYWRkMyIsCiAgICAgICAic3BvbnNvcklEIjogbnVsbCwKICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAicGxhbm5lZENvbXBsZXRpb25EYXRlIjogIjIwMTctMTAtMDZUMDk6MDA6MDAuMDAwLTA2MDAiLAogICAgICAgImVudGVyZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJ0ZW1wbGF0ZUlEIjogbnVsbCwKICAgICAgICJwcmlvcml0eSI6IDAsCiAgICAgICAiY29tcGFueUlEIjogbnVsbCwKICAgICAgICJwb3J0Zm9saW9JRCI6IG51bGwsCiAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICJsYXN0VXBkYXRlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgImN1c3RvbWVySUQiOiAiNTQ0ODIwZGYwMDAwMTM1Yjc3MTlkY2NhNjU0MzkxZjYiLAogICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICJjYXRlZ29yeUlEIjogbnVsbCwKICAgICAgICJzdGF0dXMiOiAiQ1VSIiwKICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ==",
                "oldState": "ewogICAgICAgICJJRCI6ICI1OWQ3ZGRmNzAwMDAwMjMyMmQ3OTFlYjA4YmFmZGRmYiIsCiAgICAgICAgIm5hbWUiOiAiRXZlbnRTdWIgVGVzdCAxODBmZDU5NS02M2ZiLTRmYTktYmQ0Ny01OGJmNmU1M2Q5NjQiLAogICAgICAgICJvYmpDb2RlIjogIlBST0oiLAogICAgICAgICJlbnRyeURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43NzYtMDYwMCIsCiAgICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiCiAgICAgICAgXSwKICAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43OTItMDYwMCIsCiAgICAgICAgImdyb3VwSUQiOiAiNTQ0ODIwZGYwMDAwMTQwZjZhOWMxZmFhN2NhY2FkZDMiLAogICAgICAgICJzcG9uc29ySUQiOiBudWxsLAogICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAgInBsYW5uZWRDb21wbGV0aW9uRGF0ZSI6ICIyMDE3LTEwLTA2VDA5OjAwOjAwLjAwMC0wNjAwIiwKICAgICAgICAiZW50ZXJlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAidGVtcGxhdGVJRCI6IG51bGwsCiAgICAgICAgInByaW9yaXR5IjogMCwKICAgICAgICAiY29tcGFueUlEIjogbnVsbCw8CiAgICAgICAgInBvcnRmb2xpb0lEIjogbnVsbCwKICAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICAibGFzdFVwZGF0ZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAiY3VzdG9tZXJJRCI6ICI1NDQ4MjBkZjAwMDAxMzViNzcxOWRjY2E2NTQzOTFmNiIsCiAgICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICAiY2F0ZWdvcnlJRCI6IG51bGwsCiAgICAgICAgInN0YXR1cyI6ICJDVVIiLAogICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ=="
                }
 
```

## Föråldrad metod för att fråga alla händelseprenumerationer

Följande API-slutpunkt är föråldrad och bör inte användas för nya implementeringar. Vi rekommenderar också att du övergår från gamla implementeringar till metoden i avsnittet **Fråga efter händelseprenumerationer** som beskrivs ovan.

Du kan fråga alla händelseprenumerationer för en kund enligt värdet för sessionID. Syntaxen för att ange alla händelseprenumerationer för en viss kund är följande URL:

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/list
```

**Begäranrubriker:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Rubriknamn</p> </th> 
   <th> <p>Huvudvärde</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p> sessionID-värde </p> </td> 
  </tr> 
 </tbody> 
</table>

**Svarskoder:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Svarskod</p> </th> 
   <th> Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 (inget innehåll)</td> 
   <td>Begäran returnerade alla händelseprenumerationer som hittades för användaren.</td> 
  </tr> 
  <tr> 
   <td>401 (obehörig)</td> 
   <td>Angivet sessions-ID var tomt.</td> 
  </tr> 
  <tr> 
   <td>403 (Ej tillåtet)</td> 
   <td>Användaren som matchar angivet sessions-ID har inte administratörsåtkomst.</td> 
  </tr> 
 </tbody> 
</table>

 

### Exempel på brödtext i svar

<!-- [Copy](javascript:void(0);) -->

```
                [
                {
                "id": "37c4bcf5-e0b5-4256-aba3-a51cba7bf997",
                "customer_id": "504f9640000013401be513579fbebffa",
                "obj_id": "ObjId1234",
                "obj_code": "TASK",
                "url": "http://test.test.net/test/1234",
                "event_type": "UPDATE",
                "auth_token": "auth_token"
                },
                {
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customer_d": "504f9640000013401be513579fbebffa",
                "obj_id": null,
                "obj_code": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "event_type": "UPDATE",
                "auth_token": "authTokenWorkfrontRocks1234_"
                }                
                ]
```

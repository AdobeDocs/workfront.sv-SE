---
filename: filter-event-sub-messages
content-type: api
navigation-topic: api-navigation-topic
title: Filtrera händelsens prenumerationsmeddelanden
description: Filtrera händelsens prenumerationsmeddelanden
author: John
feature: Workfront API
exl-id: 8364c4b9-5604-47ab-8b4b-db6836dcd8ca
source-git-commit: 606d19b8a83b833aba6d6b15231a8683aa2cee40
workflow-type: tm+mt
source-wordcount: '1800'
ht-degree: 0%

---

# Filtrera händelsens prenumerationsmeddelanden

Du kan skapa mellanliggande bearbetningskomponenter som kan hjälpa dig att endast filtrera och bearbeta de händelseteckningsmeddelanden som ditt företag behöver.

Mer information om händelseprenumerationer finns i [API för händelseprenumeration](../../wf-api/general/event-subs-api.md).

## Filtrera händelsemeddelanden

Det här avsnittet innehåller kodfragment för filtrering som du kan implementera för att minska inläsningen av händelseprenumerationsmeddelanden.  För att du ska kunna se skillnaderna i syntaxen för olika språk visar de här fragmenten samma uppsättning filter skrivna på följande språk:

Du kan se exempel på filtrering på [https://github.com/workfront/workfront-event-subscription-filter-examples](https://github.com/workfront/workfront-event-subscription-filter-examples), där du kan se skillnaderna i syntax för varje språk och hur du interagerar med AWS SDK. De här exemplen skrivs som AWS Lambdas, som är en vanlig metod för att använda mellanliggande filtrerings- och bearbetningskomponenter.

Följande kodfragment är nästan redo för driftsättning och kan användas som en startpunkt för att hjälpa dig att skriva egna, mer komplexa filter och bearbetningskomponenter.

### Java

I följande exempel i Java visas hur du filtrerar projektnyttolaster baserat på projektets grupp-ID, som i [ProjectGroupFiltering.java:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/java/src/main/java/com/workfront/lambda/ProjectGroupFiltering.java)

1. Upprätta det grupp-ID som du letar efter och skapa det som en statisk konstant.

   ```
   private static final String DESIRED_GROUP_ID = "VaqTTVaB0UcbPu4n6824WIYYIV953Mg3";
   ```

   I det här exemplet använder handleRequest-metoden, som är ett standardmetodnamn för AWS Lambda, en Map-typ som sin första parameter, som är händelseprenumerationens meddelandeinnehåll.\
   Den andra parametern som används är sammanhanget för den aktuella Lambda Proxy-begäran.\
   Context-objektet används för att hämta en Lambda-loggare, som används för att skriva ett meddelande till CloudWatchLogs.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
      ...
   }
   ```

2. När handleRequest-metoden anropas hämtar du attributet &quot;newState&quot; i händelseprenumerationsmeddelandet, som representerar resursens uppdaterade tillstånd.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        Map<String, Object> newState = (Map<String, Object>) webHookPayload.get("newState");
        ...
   }
   ```

   Mer information om formatet newState finns i [Utgående meddelandeformat för händelseprenumerationer](../../wf-api/api/message-format-event-subs.md).

3. När du har tolkat kartan &quot;newState&quot; från meddelandet kontrollerar du att objektets grupp-ID matchar det grupp-ID som du identifierade i steg 1.

4. (Villkorligt) Om ID:n **inte** matchar, släpper du meddelandet så att ett tomt svar returneras.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
    String projectGroupId = (String) newState.get("groupID");
    logger.log("String projectGroupID is - " + projectGroupId);    
    if (DESIRED_GROUP_ID.equals(projectGroupId)) {
        //process the message
        ...
      }
    return "";
   }
   ```

   >[!NOTE]
   >
   >Att returnera en tom, framgångsrik respons är avgörande. Allt förutom ett svar på 200 nivåer betraktas som en misslyckad leverans.

5. Bearbeta meddelandet.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        if (DESIRED_GROUP_ID.equals(projectGroupId)) {
        //process the message
        logger.log("Processing Event Subscription message matching groupId " + DESIRED_GROUP_ID + "...");
   
        AWSLambda client = AWSLambdaClientBuilder.standard().build();
        InvokeRequest request = new InvokeRequest()
                .withFunctionName("MyFunction")
                .withInvocationType("Event")
                .withLogType("Tail")
                .withPayload(jsonParser.toJson(webHookPayload))
        InvokeResult response = client.invoke(request);
      }
    ... 
   }
   ```

   AWS SDK används för att anropa en annan Lambda som ansvarar för att leverera det filtrerade meddelandet till önskad slutpunkt.

   Syftet med att överlåta ansvaret för att skicka meddelandet till en annan Lambda är att undvika en timeout i leveransbegäran från tjänsten Event Subscription. Den tillåtna tidsgränsen för leverans är för närvarande fem sekunder. Om filtret tar längre tid än vad inställningen tillåter kan du bearbeta begäran, men tjänsten Event Subscription (Händelseabonnemang) kommer att gå ut och hamna i en repetitionsloop tills den får ett svar på 200 nivåer inom tidsgränsen.

   Mer information om hur du hanterar meddelandeleverans finns i [Förbättra meddelandeleveransen samtidigt som tidsgränser överskrids](#improving-message-delivery-while-accommodating-timeouts).

### Python

Den största skillnaden mellan Java- och Python-exemplen är att i Java-exemplet tas händelsprenumerationsmeddelandet emot som den första parametern, och i Python-exemplet är den första parametern en Lambda-proxyhändelse, som innehåller händelsprenumerationsmeddelandet tillsammans med information om AWS Lambda-proxybegäran.

I följande exempel i Python visas hur du filtrerar projektnyttolaster baserat på projektets grupp-ID, som i  [projectGroupFiltering.py:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/py/projectGroupFiltering.py)

1. Upprätta det grupp-ID som du letar efter och skapa det som en statisk konstant.

   ```
   DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3'
   ```

   Den första parametern är Lambda-proxyhändelsen, som innehåller händelsens prenumerationsmeddelande och viss ytterligare information som behöver tolkas.\
   Den andra parametern är kontexten för den aktuella Lambda-proxybegäran.\
   I det här exemplet används Context-objektet för att hämta en Lambda-loggare, som används för att skriva ett meddelande till CloudWatchLogs.

   ```
   def project_group_filter_handler(event, context):
       ...
   ```

1. Tolka meddelandet från händelsen.

   ```
   event_subscription_message = json.loads(event['body'])
   ```

1. Hämta attributet &quot;newState&quot; för händelsens prenumerationsmeddelande.\
   Attributet newState representerar resursens uppdaterade tillstånd.

   ```
   new_state = json.loads(event_subscription_message['newState'])
   ```

   Mer information om formatet newState finns i [Utgående meddelandeformat för händelseprenumerationer](../../wf-api/api/message-format-event-subs.md).

1. När du har tolkat kartan &quot;newState&quot; från meddelandet kontrollerar du att objektets grupp-ID matchar det grupp-ID som du identifierade i steg 1.

1. (Villkorligt) Om ID:na inte matchar släpper du meddelandet så att ett tomt svar returneras.

   ```
   if new_state['groupID'] == DESIRED_GROUP_ID:
      # Process the message
      print('matched group ID')
      process_message(event_subscription_message)
   
   return {
   'statusCode': 200
   ```

   >[!NOTE]
   >
   >Att returnera en tom, framgångsrik respons är avgörande. Allt förutom ett svar på 200 nivåer betraktas som en misslyckad leverans.

1. Bearbeta meddelandet.

   ```
   def process_message(event_subscription_message):
      aws_lambda.invoke(
         FunctionName='forwardMessageOntoMyEndpoint',
         InvocationType='Event',
         LogType='None',
         Payload=event_subscription_message
      )
   ```

   AWS SDK används för att anropa en annan Lambda som ansvarar för att leverera det filtrerade meddelandet till önskad slutpunkt.

   Syftet med att överlåta ansvaret för att skicka meddelandet till en annan Lambda är att undvika en timeout i leveransbegäran från tjänsten Event Subscription. För närvarande är tidsgränsen för leverans inställd på fem sekunder. Om filtret tar längre tid än vad inställningen tillåter kan du bearbeta begäran, men tjänsten Event Subscription (Händelseabonnemang) kommer att gå ut och hamna i en repetitionsloop tills den får ett svar på 200 nivåer inom tidsgränsen.


### Node.js

Node.js-exemplet med filtrering av projektgrupps-ID kan läsas på liknande sätt som Java- och Python-exemplen. Precis som med Python-exemplet är den första parametern en Lambda-proxyhändelse och den andra parametern är Lambda-kontexten.

I följande exempel i Node.js visas hur du filtrerar projektnyttolaster baserat på projektets grupp-ID, som i  [projectGroupFiltering.js:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/js/projectGroupFiltering.js)

1. Upprätta det grupp-ID som du letar efter och skapa det som en statisk konstant.

   ```
   const DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3';
   ```

   Den första parametern är Lambda-proxyhändelsen, som innehåller händelsens prenumerationsmeddelande och viss ytterligare information som behöver tolkas.\
   Den andra parametern är kontexten för den aktuella Lambda-proxybegäran.\
   I det här exemplet används Context-objektet för att hämta en Lambda-loggare, som används för att skriva ett meddelande till CloudWatchLogs.

   ```
   exports.myProjectGroupFilterHandler = function (event, context) {
      ...
   }
   ```

2. Tolka meddelandet från händelsen.

   ```
   let eventSubscriptionMessage = JSON.parse(event.body);
   ```

3. Hämta projectGroupIDfrom the &quot;newState&quot; attribute of the event subscription message message och matcha den sedan mot grupp-ID:t för gruppen som du identifierade i steg 1.

   ```
   let projectGroupId = eventSubscriptionMessage.newState.groupID; 
   ```

   Mer information om formatet newState finns i [Utgående meddelandeformat för händelseprenumerationer](../../wf-api/api/message-format-event-subs.md).

4. (Villkorligt) Om ID:na inte matchar släpper du meddelandet så att ett tomt svar returneras.\
   I följande exempel visas matchande grupp-ID:

   ```
   if (projectGroupId === DESIRED_GROUP_ID) {
      // Process the message
      console.log('Processing Event Subscription message matching groupId ' + DESIRED_GROUP_ID + '...');
      forwardMessageOntoMyEndpoint(eventSubscriptionMessage, context);
   } else {
      endLambdaRequest(context);
   }
   ```

   >[!NOTE]
   >
   >Att returnera en tom, framgångsrik respons är avgörande. Allt förutom ett svar på 200 nivåer betraktas som en misslyckad leverans.

5. Bearbeta meddelandet.

   ```
   function forwardMessageOntoMyEndpoint(eventSubscriptionMessage, context) {
      let lambdaParams = {
         FunctionName: 'forwardMessageOntoMyEndpoint',
         InvocationType: 'Event',
         LogType: 'None',
         Payload: new Buffer(JSON.stringify(eventSubscriptionMessage))
      };
   
      lambda.invoke(lambdaParams, function (err, data) {
         if (err) {
            console.error(err, err.stack);
         } else {
            console.log('data = ' + data);
         }
         endLambdaRequest(context);
      });
   }
   ```

   AWS SDK används för att anropa en annan Lambda som ansvarar för att leverera det filtrerade meddelandet till önskad slutpunkt.\
   Syftet med att överlåta ansvaret för att skicka meddelandet till en annan Lambda är att undvika en timeout i leveransbegäran från tjänsten Event Subscription. För närvarande är tidsgränsen för leverans inställd på fem sekunder. Om filtret tar längre tid än vad inställningen tillåter kan du bearbeta begäran, men tjänsten Event Subscription (Händelseabonnemang) kommer att gå ut och hamna i en repetitionsloop tills den får ett svar på 200 nivåer inom tidsgränsen.\
   Mer information om hur du hanterar meddelandeleverans finns i [Förbättra meddelandeleveransen samtidigt som tidsgränser överskrids](#improving-message-delivery-while-accommodating-timeouts).

## Förbättra meddelandeleveransen samtidigt som tidsgränser överskrids

Tjänsten Event Subscription har en strikt tidsgräns för **fem sekunder** för alla leveransförfrågningar. Om meddelandets leverans överskrider den tillåtna tiden startar tjänsten Event Subscription en ny testcykel för meddelandet.

Du kan till exempel skapa ett filter för projektgrupp-ID som liknar ett av exemplen i [Filtrera händelsemeddelanden](#filtering-event-messages) och du tar med en databassökning för att avgöra om meddelandet behövs. Det är möjligt att databassökningen tillsammans med den tid som krävs för bearbetning och för att Lambda ska kunna kallstarta kan ta mer än fem sekunder, vilket gör att tjänsten Event Subscription kan försöka leverera meddelandet igen.

Du kan avvärja ett nytt försök genom att separera de tidskrävande delarna av processen från den logik som avgör om meddelandet ska bearbetas och levereras. Genom att göra det kan du acceptera meddelandet och skicka tillbaka ett svar på 200 nivåer till tjänsten Event Subscription, medan du asynkront fortsätter att bearbeta eller filtrera meddelandet i bakgrunden (se steg 5 i [Java](#java) till exempel).


Även om bearbetningen eller filtreringen inte överskrider tidsgränsen på fem sekunder är det ändå bra att separera den första beröringspunkten för meddelandefiltrering eller -bearbetning från andra behandlings- eller leveranssteg på klientsidan. På så sätt har överlämnandet av meddelandet till destinationen från tjänsten Event Subscription minimalt med tid och prestanda för båda parter.

Mer information om återförsöksmekanismen finns i [Återkommande prenumerationer](../../wf-api/api/event-sub-retries.md).

## Implementera värdbaserade filter i den molnlösa arkitekturen

Om du inte kan utnyttja en molnarkitektur för händelseprenumerationsfiltrering kan du ändå använda exemplen i [Filtrera händelsemeddelanden](#filtering-event-messages) som vägkartor över hur du implementerar egna värdbaserade filter eller bearbetningskomponenter.

### Justera filterexempel för fristående tjänster

Innan du använder filterexemplen i en molnfri miljö gör du följande:

* Utelämna de Lambda-specifika delarna i exemplen, till exempel parametern Context.

* Ändra anropen för andra Lambdas i exemplen till att göra ytterligare asynkrona HTTP-begäranden till andra filter eller bearbetningskomponenter som du har som värd.

* Om du refererar till exemplen Python och Node.js ersätter du den första händelseparametern med den första nyttolastparametern som visas i Java-exemplet. Se steg 1 i [Java](#java).

* Distribuera filter och processorer med ett webbaserat API.

### Förhindra missade händelseteckningsmeddelanden

I en molnfri arkitektur kan det ibland vara svårt att nå de tjänster som ansvarar för att ta emot prenumerationsmeddelanden. I sådana fall kan meddelanden överskrida gränsen för antal nya försök och gå förlorade, utan att det går att hämta informationen i meddelandena.

Vi rekommenderar att du, när du startar tjänsten, implementerar en fråga där du tillfrågas om det senaste tillståndet för alla resurser som kan ha inkluderats i de missade meddelandena. Som visas i följande exempel kan du använda filtervillkoren för att fråga efter resurser som matchar villkoret och sedan bearbeta deras aktuella tillstånd.

```
public static List<Map<String, Object>> projectGroupFilteringStartupRecoveryQuery(LambdaLogger logger) {
    HttpClient httpClient = HttpClientBuilder.create().build();

    // Produces a URL of https://<my-domain>.workfront.com/attask/api/v9.0/PROJ/search?groupID=<DESIRED_GROUP_ID>
    replacing <...> with the appropriate values
    URI projectGroupQueryUri = generateProjectRecoveryQueryURI(logger);

    HttpUriRequest projectGroupIdGetRequest = new HttpGet(projectGroupQueryUri);

    // Our preferred method of authentication 
    projectGroupIdGetRequest.addHeader("apiKey", WORKFRONT_API_KEY);
 
    List<Map<String, Object>> projects = null;
    try 
    {
        HttpResponse response = httpClient.execute(projectGroupIdGetRequest);
        InputStream responseBodyStream = response.getEntity().getContent();
        Reader reader = new InputStreamReader(responseBodyStream);
        Type listType = new TypeToken<List<Map<String, Object>>>(){}.getType();
        projects = new GsonBuilder().create().fromJson(reader, listType);
      } catch (IOException e) {
        logger.log("An IOException was thrown while executing a request to Workfront for projects matching the group ID " + DESIRED_GROUP_ID);
    }
    return projects;
}
```

Genom att fråga efter resurser ser du till att dina integrerande system har den senaste versionen av resurser.

### Implementera asynkron bearbetning i Leverera meddelanden

Alla exempel i [Filtrera händelsemeddelanden](#filtering-event-messages) överför ansvaret för att leverera filtrerade meddelanden till en annan AWS Lambda. Detta görs för att undvika att den tidsgräns på fem sekunder som anges i leveransbegäran överskrids, vilket framtvingas av den händelseprenumerationstjänst som utfärdar begäran.

I en molnfri arkitektur kan du behöva implementera en asynkron bearbetningsmekanism som liknar hur AWS SDK tillåter asynkrona anrop till andra AWS Lambdas. De flesta moderna programmeringsspråk har tredjeparts- eller kärnbibliotek som hanterar asynkron bearbetning, vilket gör att du kan utnyttja den asynkrona bearbetning som implementeras i våra exempel.

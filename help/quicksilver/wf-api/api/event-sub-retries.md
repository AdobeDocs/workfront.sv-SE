---
content-type: api
navigation-topic: api-navigation-topic
title: Återkommande prenumerationer på evenemang
description: Återkommande prenumerationer på evenemang
author: Becky
feature: Workfront API
role: Developer
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: 05f8dc8770c185720520fc631e19c75b925a70bf
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Återkommande prenumerationer på evenemang

När du implementerar ett meddelandesystem finns det några kavattningar som måste åtgärdas för att säkerställa stabilitet, konsekvens och en bra användarupplevelse. Ett av bristerna i ett system för meddelandeleverans är att säkerställa att meddelandena når sin destination med framgång och veta vad som ska göras när de inte kommer fram.

Vissa integreringar kan acceptera leveransfel och sedan släppa meddelandet och gå vidare till nästa meddelande.  I andra integreringar kan man inte ignorera om ett meddelande inte levereras. En finansiell integrering kan till exempel försöka leverera ett meddelande, men i stället får en HTTP-statuskod på 404, vilket anger att servern inte kunde hitta slutpunkten som meddelandet skulle levereras till. I sådana fall kan ett saknat meddelande innebära att någon inte får betalt för sin tid eller att en organisation överskridit budgeten för kontraktsanställda resurser.

## Adobe Workfront Strategy for Event Subscription Retries

Eftersom kunderna utnyttjar Workfront-plattformen som en viktig del i sitt dagliga kunskapsarbete, erbjuder Workfront ramverk för händelseteckning en mekanism som säkerställer att alla meddelanden skickas så långt det går.

Händelseutlösta utgående meddelanden som inte kan levereras till kundens slutpunkter skickas igen tills leveransen har slutförts i upp till 48 timmar. Under denna tid sker försök stegvis med ökad frekvens tills leveransen är klar eller tills 11 försök har gjorts.

Formeln för dessa försök är:

`((2^attempt) - 1) * 84800ms`

Det första återförsöket görs efter 1,5 minuter, det andra efter nästan 5 minuter och det elfte efter cirka 48 timmar.

Kunderna måste se till att alla slutpunkter som förbrukar utgående meddelanden från Workfront Event Subscriptions är inställda på att returnera ett 200-nivåsvarsmeddelande till Workfront när leveransen är klar.

## Inaktiverade och frysta prenumerationsregler

* En prenumerations-URL är **inaktiverad** om den har en felfrekvens på över 70 % med över 100 försök ELLER om den har 2 000 efterföljande fel
* En prenumerations-URL är **fryst** om den har fler än 2 000 efterföljande fel och den senaste åtgärden inträffade för över 72 timmar sedan ELLER om den har 50 000 efterföljande fel under någon tidsram.
* En **inaktiverad**-prenumerations-URL fortsätter att försöka leverera var 10:e minut och återaktiveras med en lyckad leverans.
* En **fryst**-prenumerations-URL försöker aldrig levereras om den inte aktiveras manuellt genom att en API-begäran görs.




<!--

## Handling Failed Event-Triggered Outbound Messages

The following flowchart shows the strategy for reattempting message deliveries with Workfront Event Subscriptions:

![](assets/event-subscription-circuit-breaker-retries-350x234.png)

The following explanations correspond with the steps depicted in the flowchart:

1. Message fails to be delivered. 
1. Message delivery failure information is logged.

   All failed attempts to deliver a message are logged so that debugging may be performed to determine the root cause of a given failure or series of failures. 

1. URL failures incremented. 
1. Message attempt count is incremented. 
1. Calculate the delay until this message's delivery will be attempted again. 
1. Message is placed onto the message retry queue.

   As shown in the preceding flowchart, the message queue used for processing message delivery retries is a separate queue from the one that processes the initial delivery attempt for each message. This allows the near real-time flow of messages to continue unimpeded by the failure of any subset of messages. 

1. URL circuit status is evaluated. One of the following occurs:

   * If the circuit is open and not allowing deliveries at this time, restart the process at step 5.
   * If the circuit is half-open, this implies that our circuit is currently open, but enough time has passed to allow testing of the URL to see if the problem with delivering to it has been resolved.
   * If the message delivery attempt limits have been reached (48 hours of retrying) then the message is dropped

1. If the URL circuit is closed and allowing deliveries, attempt to deliver the message. If this delivery fails, the message will restart at step 1 

1. If the URL circuit is closed and allowing deliveries, attempt to deliver the message. If this delivery fails, the message will restart at step 1.
   -->

---
content-type: api;faq
navigation-topic: general-api
title: Frågor och svar - Evenemangsprenumerationer
description: Frågor och svar - Evenemangsprenumerationer
author: Becky
feature: Workfront API
exl-id: a6120939-5d76-4f46-a304-125de6b22502
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '937'
ht-degree: 0%

---

# Frågor och svar - Evenemangsprenumerationer

<!--
{{highlighted-preview}}
-->

Nedan följer vanliga frågor om händelseprenumerationer:

## Vad är en prenumeration?

En prenumeration är en uppsättning data som används för att matcha och leverera Adobe Workfront-händelser till en kunds HTTP-slutpunkt. Den här resursen består av fyra primära attribut:

* customer_id
* obj_code
* obj_id
* url

En prenumeration kan även ha andra attribut, till exempel ett eget unikt ID och det datum då den skapades, men attributen som anges ovan används främst för att matcha händelser och leverera dem till kunder.

## Kan jag välja vilka händelser som ska skickas till en slutpunkt baserat på vissa kriterier i en händelsenyttolast?

Händelseprenumerationsfilter är ett sätt på vilket händelsedelare kan sorteras efter angivna villkor. Vi rekommenderar att du tillämpar filter på händelseprenumerationer eftersom det kan minska antalet meddelanden som en slutpunkt behöver använda avsevärt. Mer information finns i [Filtrering av händelseprenumeration](../../wf-api/general/event-subs-api.md#event).

## Varför returnerar API:t en 409-konfliktsvarskod?

Om du försöker skapa en händelseprenumeration och få en svarskod: 409 är i konflikt. Den prenumeration du försökte skapa är en dubblett. Workfront tillåter inte att duplicerade prenumerationer skapas.

## Vad ska jag göra om mina meddelanden inte levereras till min slutpunkt?

Sök efter följande scenarier och använd den rekommenderade lösningen:

* Se till att prenumerationsslutpunkten som definieras av **url** field - returnerar en 2XX HTTP-svarskod. Om så inte är fallet kontaktar du Workfront Support eller läser [Leveranskrav för evenemangsprenumeration](../../wf-api/general/setup-event-sub-endpoint.md).

* Begäran om händelseleverans kan vara timeout innan den slutförs. Se till att slutpunkten svarar konsekvent inom 5 sekunder. Det här är standardtidsgränsen som anges för HTTP-begäran för att leverera ett händelseprenumerationsmeddelande. Om slutpunkten inte svarar inom 5 sekunder kontaktar du Workfront Support eller läser [Leveranskrav för evenemangsprenumeration](../../wf-api/general/setup-event-sub-endpoint.md).
* Händelserna kanske inte genererar ditt sätt att tänka. Se till att ni inte gör antaganden om hur och när händelser ska och ska utlösas. Du kan till exempel tro att en uppdatering av ett dokument för en uppgift genererar en aktivitetsuppdateringshändelse, men i stället genereras en dokumentskapningshändelse eller en dokumentuppdateringshändelse.
* Din prenumeration kanske inte konfigureras som du förväntar dig. Du kan skapa händelseprenumerationer i olika miljöer och förvänta dig att de överförs på samma sätt som andra Workfront-data gör. Händelseprenumerationsdata är dock inte konfigurerade för kopiering eller befordran till andra miljöer. Kontrollera att du skickar API-begäranden till rätt miljö och att prenumerationerna i den miljön är konfigurerade som förväntat.
* Nyttolasten togs inte emot eftersom den nödvändiga IP-adressen för Workfront inte har lagts till i tillåtelselista på brandväggen. Händelseprenumerationshändelser skickas endast från ett fåtal IP-adresser. Kontrollera att målnätverket har alla IP-undantag som krävs för att ta emot nyttolaster från Workfront Event Subscriptions.

## Varför tar det för lång tid för mina meddelanden att nå min slutpunkt?

Några av följande scenarier kan vara ansvariga:

* En stor åtgärd, till exempel en satsvis uppdatering, i systemet kan leda till att ett stort antal meddelanden köas alla samtidigt, vilket kan ta lite tid att bearbeta.
* Långvariga beräkningar eller tidslinjeberäkningar i stora projekt kan leda till en fördröjning i publiceringen av meddelanden till händelseprenumerationer.
* Prenumerationen kan ha inaktiverats.

   * Efter en respitperiod på 100 meddelanden, om en viss URL - som kan vara kopplad till en eller flera prenumerationer - misslyckas mer än 70 % av tiden eller om URL:en inte kan leverera efter 2000 försök i följd, görs inget försök att leverera meddelanden som matchar prenumerationer med samma URL. I stället står meddelandena omedelbart i kö för ett nytt försök.

      Var 10:e minut efter att en URL har inaktiverats försöker vi leverera nästa meddelande som kommer fram för bearbetning. Om det meddelandet lyckas återaktiverar vi den URL:en och därefter alla matchande prenumerationer. Om det meddelandet inte skickas återställs den 10-minuterstimern och vi försöker igen när det har gått ut.

      Det här beteendet kan uppfattas som inkonsekvent eller fördröjd leverans, men följer bara vår policy för hur händelseprenumerationsmeddelanden hanteras.

   * En URL för en händelseprenumeration är inaktiverad om något av följande villkor uppfylls:

      * Prenumerations-URL:en kunde inte leverera på 7 dagar och har misslyckats med minst 2 000 efterföljande leveransförsök under de senaste 72 timmarna.
      * Prenumerations-URL:en kunde inte leverera 50 000 efterföljande försök.

## Vad ska jag göra om jag får 500-svarsstatus när jag försöker anropa Event Subscription API?

Kontakta Workfront support. Mer information om hur du kontaktar supporten finns i [Kontakta kundsupport](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

## Vilka olika typer av autentisering kan jag använda med Workfront Event Subscriptions?

Du kan använda vilken autentisering som helst som använder en innehavartoken. The **authToken** prenumerationsfältet är en sträng som representerar en OAuth2-bearer-token som används för att autentisera med den URL som anges i **url** fält. Teoretiskt sett kan det här tokenvärdet vara vad som helst så länge målslutpunkten är medveten om hur kodningen ska hanteras, vilket är **utf-8**.

## Hur länge ska det vara innan jag får min händelsenyttolast från Workfront Event Subscriptions?

Vanligtvis kan du förvänta dig att ta emot händelseleveransbegäranden om händelseprenumerationer på händelser på mindre än 5 sekunder från det att dataändringen loggas. I genomsnitt tas webkrockmeddelanden emot inom mindre än en sekund från den tidpunkt då dataändringen görs. Tjänsten kan dock ta emot meddelanden i så stora kvantiteter att den också kan ta längre tid.

## Ytterligare resurser

* **API-dokumentation**: [API för händelseprenumeration](../../wf-api/general/event-subs-api.md)

* **God praxis**: [Bästa praxis för händelseteckning](../../wf-api/general/event-sub-best-practice.md)

* **Fält som utlöser händelseabonnemangsnyttolaster**: [Resursfält för händelseprenumeration](../../wf-api/api/event-sub-resource-fields.md)

* **Förstå återförsök till händelseabonnemang**: [Återkommande prenumerationer](../../wf-api/api/event-sub-retries.md)

* **Konfigurera brandväggen för Workfront**: [Konfigurera brandväggens tillåtelselista](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)

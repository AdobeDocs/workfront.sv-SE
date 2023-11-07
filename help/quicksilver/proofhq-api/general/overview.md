---
title: Ökning
description: Ökning
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: 882b657a-1bde-4efd-93e8-1de80c065b2d
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# Ökning

**Välkommen till Workfront Proof API**

Workfront Proof API är en enkel HTTP-tjänst som skyddas med SSL. API:t ger dig alla funktioner som används i vårt eget program.

## Format som stöds

Det offentliga gränssnittet är SOAP 1.1-kompatibelt med WSDL-stöd. Alla begäranden körs därför med XML via HTTPS.

## API-versionshantering

För att bevara kompatibiliteten med befintliga klientintegrationslösningar har vi infört API-versionshantering från och med version 12.1. Se  [API-uppdateringar](http://api.proofhq.com/new-updates) sida för mer information. Om en metod eller parameter inte har någon versionsinformation betyder det att du kommer att hitta den som en del av vårt standard-API, se&quot;Komma igång med API&quot; nedan.

## Komma igång med API

API-startpunkten:

`https://soap.proofhq.com/soap` (observera användningen av HTTPS)

WSDL finns här:

`https://soap.proofhq.com/soap?wsdl`

>[!NOTE]
>
>**Denna WSDL innehåller alla ändringar fram till version 12.1, därefter introducerades API-versionshantering. På sidan API-uppdateringar finns mer information om olika WSDL-versioner och kommande ändringar**

Varje API-begäran kräver en sessionsnyckel. Denna sessionsnyckel identifierar den Workfront-korrekturanvändare som utför åtgärderna och hämtas genom att anropa metoden doLogin() och ange användarens e-postadress och lösenord. Metoden doLogin() behöver bara anropas en gång före en sekvens med API-begäranden. Sessionsnyckeln är aktiv under en kort period och förnyas för varje metodanrop. *Vi kommer snart att lägga till stöd för tokenbaserad autentisering.*

Alla förfrågningar använder följande kuvert-, huvud- och brödformat:

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:urn="urn:proofhqapi">`
   <soapenv:Header/>
   <soapenv:Body>
       ... API function and data inserted here ...
    </soapenv:Body>
    </soapenv:Envelope>
```

## Frågor och svar

En samling vanliga frågor och svar finns på [this](http://api.proofhq.com/faqs) sida.

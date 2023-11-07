---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Autentisering för dokumentwebbhooks
description: Autentisering för dokumentwebbhooks
author: Becky
feature: Workfront API
role: Developer
exl-id: 2303c202-27c7-4922-a613-e9824910504c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Autentisering för dokumentwebbhooks

## Autentisering

Adobe Workfront dokumentwebhooks stöder två olika typer av autentisering: OAuth2 och ApiKey. I båda fallen skickar Workfront autentiseringstoken i huvudet när ett API-anrop görs.

### OAuth2

Med OAuth2 kan Workfront göra auktoriserade API-anrop till en webkrok-leverantör för en användares räkning. Innan du gör det måste användaren ansluta sitt externa dokumentleverantörskonto till Workfront och bevilja Workfront

behörighet att agera å deras vägnar. Den här handskakningsprocessen utförs bara en gång för varje användare. Så här fungerar det:

1. Användaren börjar ansluta webbkrokintegreringen till sitt konto. För närvarande gör du detta genom att klicka på listrutan Lägg till dokument > Lägg till tjänst > Anpassat integrationsnamn.
1. Workfront navigerar till användaren via autentiserings-URL:en, som kan uppmana användaren att logga in på den externa dokumentleverantören. Den här sidan hanteras av webbkrokprovidern eller det externa dokumenthanteringssystemet. När du gör det lägger Workfront till en state-parameter i autentiserings-URL:en. Detta värde måste skickas tillbaka till Workfront genom att samma värde läggs till i Workfront Retur-URI i steget nedan.
1. När användaren har loggat in på det externa systemet (eller om användaren redan är inloggad) visas sidan Autentisering, som förklarar att Workfront begär åtkomst för att utföra en uppsättning åtgärder för användarens räkning.
1. Om användaren klickar på Tillåt omdirigeras webbläsaren till Workfront omdirigerings-URI och &quot;code=`<code>`&quot; till frågesträngen. Enligt specifikationen OAuth2 är denna token kortlivad. Frågesträngen måste också ha följande, &quot;state=`<sent_by_workfront>`&quot;.
1. Workfront behandlar denna begäran och gör ett API-anrop till Token Endpoint URL med auktoriseringskoden.
1. Token Endpoint URL returnerar en uppdateringstoken och åtkomsttoken.
1. Workfront lagrar en sådan token och tillhandahåller webbkrokintegreringen för den här användaren.
1. Från och med nu kan Workfront göra auktoriserade API-anrop till webkrok-providern. När du ringer dessa samtal skickar Workfront åtkomsttoken i HTTP-begärandehuvudet enligt nedan:

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. Om åtkomsttoken har upphört att gälla, kommer Workfront att anropa tokens slutpunkts-URL för att hämta en ny åtkomsttoken och sedan försöka med det auktoriserade API-anropet igen med den nya åtkomsttoken.

### ApiKey

Det är mycket enklare än OAuth2 att göra auktoriserade API-anrop till en webbkrokleverantör med en ApiKey. När du gör ett API-anrop skickar Workfront bara ApiKey och Workfront-användarnamn i HTTP-begärandehuvudet: 

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

Webkrockprovidern kan använda användarnamnet för att tillämpa användarspecifika behörigheter. Detta fungerar bäst när båda systemen ansluter till LDAP med enkel inloggning (SSO).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Adding Request Headers (optional)</h3>
<p>In addition to using either OAuth2 tokens or an ApiKey for authentication, Workfront can send a predefined set of headers to the webhook provider for every API call. A Workfront admin can setup set this up when&nbsp;registering or editing a Webook Integration, as described in the section above. See Registering a Webhook Integration.</p>
<p>For example, this can be used for Basic Authentication. To do this, the Workfront administrator would add the following Request Header information in the Custom Integration dialog:</p>
<p>&nbsp; &nbsp; &nbsp;Authorization Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==</p>
<p>where QWxhZGRpbjpvcGVuIHNlc2FtZQ== is a base-64 encoded string of "username:password". See Basic Authentication . Provided that this added, Workfront will pass this in the HTTP request header, in addition to other request headers:&nbsp;</p>
<p>-------------------------------</p>
<p>apiKey: 12345</p>
<p>username: johndoe@foo.com</p>
<p>Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­</p>
<p>-------------------------------</p>
</div>
-->

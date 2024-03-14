---
content-type: api
navigation-topic: api-navigation-topic
title: Auktoriseringskodflöde för anpassade OAuth 2-program
description: Auktoriseringskodflöde för anpassade OAuth 2-program
author: Becky
feature: Workfront API
role: Developer
exl-id: a1ab60c4-4255-4d80-87f1-f36d325254c2
source-git-commit: 293b7354e4549e51d78ad1aa75927a21d9044c43
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 0%

---


# Konfigurera och använda organisationens anpassade OAuth 2-program med hjälp av ett auktoriseringskodsflöde

Om du vill integrera med Workfront och tillåta klientappen att kommunicera med Workfront å användarens vägnar måste du:

* Skapa ett OAuth2-program
* Konfigurera tredjepartsprogrammet
* Länk till sidan Autentisera för dina användare
* Konfigurera auktoriseringskodflöde: Användare loggar in på Workfront-instansen och godkänner att klientprogrammet tillåter att de ansluter till Workfront för deras räkning. Därför får du en auktoriseringskod som du byter ut med åtkomst- och uppdateringstokens.
* Konfigurera uppdateringstokenflöde: I det här flödet använder du uppdateringstoken för att hämta en ny åtkomsttoken när den gamla har upphört att gälla.

## Skapa ett OAuth2-program

Instruktioner om hur du skapar OAuth2-programmet finns i [Skapa ett OAuth2-program med användarens inloggningsuppgifter (kodflöde för auktorisering)](../../administration-and-setup/configure-integrations/create-oauth-application.md#create3) in [Skapa OAuth2-program för Workfront-integreringar](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Länk till sidan Autentisera för dina användare

Dina användare måste logga in för att godkänna integreringen på sina egna konton. Sidan som de ska godkänna har ett specifikt format, som beskrivs här. Använd den här informationen för att fastställa adressen till appens auktoriseringssida och förse användarna med den här adressen eller en länk till den.

* Den fullständiga URL:en till din organisations domän. Exempel:

  ```
  https://myorganization.my.workfront.com
  ```


* `client_id`: Detta är det klient-ID som genererades när du skapade OAuth2-appen i Workfront.

* `redirect_uri`: Det här är den omdirigerings-URL som du angav när du skapade programmet. Dina användare dirigeras till den här sidan när de har auktoriserat appen för sitt konto.

* `response_type`: Detta måste ha värdet `code`.

URL:en för auktoriseringssidan är därför:

```
https://<URL of your organization's domain>/integrations/oauth2/authorize?client_id=<Your ClientID>&redirect_uri=<Your redirect URL>&response_type=code
```

>[!NOTE]
>
>Vi rekommenderar att du skapar en knapp eller en annan länk som användarna kan klicka på för att dirigera till den här sidan.

## Konfigurera tredjepartsprogrammet

Tredjepartsprogrammet kan kräva konfiguration. Följande tabell innehåller information om fält som kan behövas när du konfigurerar tredjepartsprogrammet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Auktoriserings-URI</td> 
   <td> <p><code>https://&lt;the full URL of your organization's domain&gt;/integrations/oauth2/authorize</code> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code> https://myorganization.my.workfront.com/integrations/oauth2/authorize</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Token-URL</td> 
   <td> <p><code>https://&lt;the full URL of your organization's domain&gt;/integrations/oauth2/api/v1/token</code> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>https://myorganization.my.workfront.com/integrations/oauth2/api/v1/token</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Omfång</td> 
   <td>Du behöver inte ange omfattningar. </td> 
  </tr> 
 </tbody> 
</table>

## Ställ in auktoriseringskodflöde

![](assets/oauth-2-authorization-code-flow.png)

Så här loggar du in användare med OAuth2:

1. När användaren öppnar auktoriseringssidan dirigeras den om till inloggningssidan för Workfront så att användaren kan logga in på Workfront. Om användaren har en SSO-konfiguration öppnas identitetsleverantörens inloggningssida.

   Om användaren redan är inloggad på Workfront i samma webbläsare, eller loggar in på Workfront utan fel, dirigeras användaren om till godkännandeskärmen:

   ![](assets/consent-screen-350x227.png)

1. Om användaren tillåter åtkomst omdirigeras sidan till `redirect_url`. Omdirigeringen måste innehålla följande frågeparametrar:

* `code`: Auktoriseringskoden som krävs för att hämta åtkomsttoken/uppdateringstoken.
* `domain`: Din organisations domän. Exempel: i `myorganization.my.workfront.com`, domänen är `myorganization`.
* `lane`: begärans körfält. Exempel: i `myorganization.preview.workfront.com`, är `preview`.

  >[!IMPORTANT]
  >
  >The `code` är endast giltigt i 2 minuter. Därför måste du hämta uppdaterings- och åtkomsttoken inom den tiden.

1. När du har en kod kan du begära uppdatering och åtkomst till tokens genom att skicka koden tillsammans med klientprogrammets autentiseringsuppgifter till `/integrations/oauth2/api/v1/token` slutpunkt.

   Den fullständiga URL:en för tokenbegäran är

   ```
   https://<URL of your organization's domain></span>/integrations/oauth2/api/v1/token
   ```

   **Exempel:**  Exempel på CURL-anrop till token-slutpunkt:

   Exempel 1

   ```
      curl --location --request POST '**<workfront host>**/integrations/oauth2/api/v1/token' \
      --header 'Authorization: Basic **<base64(client_id:client_secret)>**' \
      --header 'Content-Type: application/json' \
      --data-raw '{
      "code": "**<code>**",
      "grant_type": "**authorization_code**",
      "redirect_uri": "**<redirect_url>**"
      }'
   ```

   Exempel 2

   ```
      curl --location --request POST '**<workfront host>**/integrations/oauth2/api/v1/token' \
      --header 'Content-Type: application/x-www-form-urlencoded' \
      --data-urlencode 'grant_type=**authorization_code**' \
      --data-urlencode 'redirect_uri=**<redirect_url>**' \
      --data-urlencode 'code=**<code>**' \
      --data-urlencode 'client_id=**<client_id>**' \
      --data-urlencode 'client_secret=**<client_secret>**'  
   ```


   >[!IMPORTANT]
   >
   > Klienthemligheten genererades när appen registrerades i Workfront. Du bör lagra den på en säker plats, eftersom den inte kan återställas om den förloras.

   När alla skickade parametrar är korrekta returnerar tokenslutpunkten följande nyttolast:

   ```
   {
      "token_type": "sessionID",
      "access_token": "string", // the value of sessionID
      "refresh_token": "string",
      "expires_in": 0,
      "wid": "string"
   }
   ```

   Åtkomsttoken är samma som ```sessionID```och upphör på samma sätt som med ```sessionID```

   >[!IMPORTANT]
   >
   > Lagra uppdateringstoken på en säker plats. Du behöver den för att få en ny uppdateringstoken när den gamla har gått ut. Workfront lagrar inte din uppdateringstoken.

1. Nu när du har en åtkomsttoken kan du göra API-anrop till Workfront

   ```
   curl --request GET 'https://<workfront host>/attask/api/v14.0/proj/search \
   --header 'sessionID: <access_token>'
   ```

## Konfigurera åtkomsttoken för uppdatering

![](assets/refresh-access-token-flow-350x142.png)

För att uppdatera access_token måste vi göra ett POST-anrop till tokenslutpunkten igen. Den här gången skickar vi en annan formulärdata enligt följande:

```
curl --location --request POST '<workfront host>/integrations/oauth2/api/v1/token' \
--header 'Authorization: Basic <base64(client_id:client_secret)>' \
--header 'Content-Type: application/json' \
--data-raw '{
   "grant_type": "refresh_token",
   "refresh_token": "<refresh_token>"
}'

###### OR

curl --location --request POST '<workfront host>/integrations/oauth2/api/v1/token' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--data-urlencode 'grant_type=refresh_token' \
--data-urlencode 'redirect_uri=<redirect_url>' \
--data-urlencode 'refresh_token=<refresh_token>' \
--data-urlencode 'client_id=<client_id>' \
--data-urlencode 'client_secret=<client_secret>'
```

Det returnerar följande resultat:

```
{
  "token_type": "sessionID",
  "access_token": "string", // the value of sessionID
  "refresh_token": "string",
  "expires_in": 0,
  "wid": "string"
}
```

Återigen är åtkomsttoken `sessionID` som kan användas för att göra en API-begäran till Workfront.

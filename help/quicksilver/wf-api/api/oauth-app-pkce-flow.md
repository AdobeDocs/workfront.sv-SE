---
content-type: api
navigation-topic: api-navigation-topic
title: Använda PKCE-flöde för OAuth 2-program
description: Använda PKCE-flöde för OAuth 2-program
author: Becky
feature: Workfront API
role: Developer
exl-id: 61fe77b6-c6d7-4f23-bfb6-617bccaa1989
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# Konfigurera och använda organisationens anpassade OAuth 2-program med PKCE-flöde

PKCE är ett säkert auktoriseringsflöde som fungerar bra med dynamiskt uppdaterade program som mobilappar, men som är värdefullt för alla OAuth2-klienter. I stället för en statisk klienthemlighet använder PKCE en dynamiskt genererad sträng, vilket eliminerar risken för en läckt klienthemlighet.

## PKCE - översikt

Ett PKCE-flöde har följande steg. Stegen i det här avsnittet visas endast i informationssyfte. Om du vill utföra dessa procedurer läser du i andra avsnitt i den här artikeln.

1. Klienten skapar `code_challenge` genom att omforma `code_verifier` använda `S256` kryptering.

1. Klienten dirigerar webbläsaren till inloggningssidan för OAuth2, tillsammans med den genererade `code_challenge`. Du måste registrera din app (Client) så att OAuth2 kan godkänna auktoriseringsbegäran. Efter registreringen kan din app dirigera om webbläsaren till OAuth2.

1. Auktoriseringsservern OAuth2 dirigerar om autentiseringsfrågan till användaren.

1. Användaren autentiserar med ett av de konfigurerade inloggningsalternativen och kan se en sida med godkännande där de behörigheter som OAuth2 ger till programmet listas.

1. OAuth2 dirigerar tillbaka till ditt program med en `authorization code`.

1. Programmet skickar den här koden tillsammans med `code_verifier`, till OAuth2.

1. OAuth2 Authorization Server transformerar `code_verifier` med `code_challenge_method` från den ursprungliga auktoriseringsbegäran och kontrollerar resultatet mot `code_challenge`. Om värdet för båda strängarna matchar har servern verifierat att förfrågningarna kommer från samma klient och kommer att skicka ett `access token`.

1. OAuth2 returnerar `access token`och eventuellt en `refresh token`.

1. Programmet kan nu använda dessa token för att anropa resursservern, till exempel ett API för användarens räkning.

1. Resursservern validerar token innan den svarar på begäran.


## Konfigurera programmet

Innan du kan implementera auktorisering måste du registrera din app i OAuth2 genom att skapa en appintegrering från Workfront.

Instruktioner om hur du skapar OAuth2-programmet finns i [Skapa ett ensidigt OAuth2-webbprogram med PKCE](../../administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-single-page-web-application-using-pkce) in [Skapa OAuth2-program för Workfront-integreringar](../../administration-and-setup/configure-integrations/create-oauth-application.md)


## Skapa korrekturnyckeln för kodutbyte

På samma sätt som i det vanliga Authorization Code-flödet börjar din app med att dirigera om användarens webbläsare till din Authorization Server `/authorize` slutpunkt. I det här fallet måste du dock även skicka en kodutmaning.

Det första steget är att generera en kodverifierare och en utmaning.

<table>
  <col/>
  <col/>
    <tbody>
      <tr>
        <td role="rowheader">Kodverifieraren</td>
        <td>
          <p>Slumpmässig URL-säker sträng med minst 43 tecken</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">Kodutmaning</td>
        <td>
          <p>Base64 URL-kodad SHA-256-hash för kodkontrollanten</p>
        </td>
      </tr>
    </tbody>
</table>


Du måste lägga till kod i klientappen för att skapa kodverifieraren och kodutmaningen.

PKCE-generatorkoden skapar utdata som liknar följande:

>[!INFO]
>
>**Exempel:**
>
>```
>{
>  "code\_verifier":"N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat",
>  "code\_challenge":"wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>}
>```

Din app sparar `code_verifier` för senare och skickar `code_challenge` tillsammans med auktoriseringsbegäran till din Authorization Server `/authorize` URL.

## Begär en auktoriseringskod

Om du använder standardservern för anpassad auktorisering ser din begärande-URL ut ungefär så här:

>[!INFO]
>
>**Exempel:**
>
>
>```
>/authorize?client\_id=<clientID>&response\_type=code&redirect\_uri=<redirectURL>
>&code\_challenge\_method=S256&code\_challenge=wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>```

Observera de parametrar som skickas:

* `client_id` matchar klient-ID:t för OAuth2-programmet som du skapade i när du konfigurerade programmet.

  Instruktioner finns i Skapa ett ensidigt OAuth2-webbprogram med PKCE i Skapa OAuth2-program för Workfront-integreringar.

* `response_type` är `code`, eftersom programmet använder behörighetstypen Authorization Code.

* `redirect_uri` är den återanropsplats som användaragenten dirigeras till tillsammans med `code`. Detta måste matcha en av de omdirigerings-URL:er som du angav när du skapade OAuth2-programmet.

* `code_challenge_method` är hash-metoden som används för att generera utmaningen, vilket alltid är `S256` för Workfront Oauth2-program som använder PKCE.

* `code_challenge` är den kodutmaning som används för PKCE.


## Byta ut koden för tokens

Om du vill ändra auktoriseringskoden för en åtkomsttoken skickar du den till din auktoriseringsservers `/token` slutpunkt tillsammans med `code_verifier`.

>[!INFO]
>
>**Exempel:**
>
>```
>/token \\
>  --header 'accept: application/json' \\
>  --header 'cache-control: no-cache' \\
>  --header 'content-type: application/x-www-form-urlencoded' \\
>  --data 'grant\_type=authorization\_code&client\_id=<clientID>&redirect\_uri=<redirectURL>&code=<code>&code\_verifier=N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat
>```

>[!IMPORTANT]
>
> Till skillnad från det reguljära Authorization Code-flödet kräver det här anropet inte auktoriseringshuvudet med klient-ID och hemlighet. Därför är den här versionen av Authorization Code-flödet lämplig för inbyggda appar som mobilappar eller single page-applikationer som saknar serverdel.

Observera de parametrar som skickas:

* `grant_type` är `authorization_code`, eftersom appen använder behörighetstypen Authorization Code.

* `redirect_uri` måste matcha den URI som användes för att hämta auktoriseringskoden.

* `code` är auktoriseringskoden som du fick från slutpunkten /authorized.

* `code_verifier` är PKCE-kodverifieraren som din app genereras i [Skapa korrekturnyckeln för kodutbyte](#Create).

* `client_id` identifierar klienten och måste matcha värdet som är förregistrerat i OAuth2.


Om koden fortfarande är giltig och kodverifieraren matchar, får ditt program en åtkomsttoken.

>[!INFO]
>
>**Exempel:**
>
>```
>{
>    "access\_token": "eyJhd\[...\]Yozv",
>    "expires\_in": 3600,
>    "token\_type": "Bearer"
>}
>```

## Validera åtkomsttoken

När programmet skickar en begäran med en åtkomsttoken måste resursservern validera den.

Du kan validera din åtkomsttoken med ett API-anrop som liknar följande:

>[!INFO]
>
>**Exempel:**
>
>```
>/attask/api/<api version>/proj/search \\
>  --header 'sessionID: <access\_token>' \\
>```

## Begär en uppdateringstoken

Om du vill begära en uppdateringstoken kan du göra ett POST-anrop till API:t på ungefär följande sätt:

>[!INFO]
>
>**Exempel:**
>
>```
>/token \\
>  --header 'accept: application/json' \\
>  --header 'cache-control: no-cache' \\
>  --header 'content-type: application/x-www-form-urlencoded' \\
>  --data 'grant\_type=refresh\_token&client\_id=<clientID>&redirect\_uri=<redirectURL>&refresh\_token=<refresh\_token>
>```

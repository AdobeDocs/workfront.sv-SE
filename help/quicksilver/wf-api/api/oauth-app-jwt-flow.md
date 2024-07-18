---
content-type: api
navigation-topic: api-navigation-topic
title: Använda JWT-flöde för anpassade OAuth 2-program
description: Använda JWT-flöde för anpassade OAuth 2-program
author: Becky
feature: Workfront API
role: Developer
exl-id: 4bd56fe6-1f36-4c36-82cd-96de748ad680
source-git-commit: 6f041459caf040846ffdec5bc75e9d74c99e318b
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Konfigurera och använda organisationens anpassade OAuth 2-program med JWT-flöde

Om du vill integrera med Workfront och tillåta klientappen att kommunicera med Workfront å användarens vägnar måste du:

* Skapa ett OAuth2-program
* Skapa ett certifikat för offentlig nyckel
* Skapa en JSON-webbtoken (JWT)

## Skapa ett OAuth2-program

Instruktioner om hur du skapar OAuth2-programmet finns i [Skapa ett OAuth2-program med serverautentisering (JWT-flöde)](../../administration-and-setup/configure-integrations/create-oauth-application.md#create2) i [Skapa OAuth2-program för Workfront-integreringar](../../administration-and-setup/configure-integrations/create-oauth-application.md) .

>[!NOTE]
>
>Du kan ha upp till totalt tio OAuth2-program samtidigt.

## Skapa ett certifikat för offentlig nyckel

JWT måste signeras och base-64-kodas för att kunna inkluderas i åtkomstbegäran. JWT-biblioteken innehåller funktioner för att utföra dessa åtgärder.

Token måste signeras med den privata nyckeln för ett digitalt signeringscertifikat. Om du gör det kan du använda den privata nyckeln för alla associerade certifikat för att signera din JWT.

Den algoritm som används är RS256 (RSA-signatur med SHA-256). Det här är en asymmetrisk algoritm och använder ett nyckelpar för offentlig/privat nyckel. Identitetsprovidern har en privat (hemlig) nyckel som används för att generera signaturen, och konsumenten av JWT får en offentlig nyckel för att validera signaturen.

Om du vill generera den offentliga nyckeln gör du **något** av följande.

* Öppna din MacOS/Linux-terminal och kör följande kommando. Överför sedan `certificate_pub.crt` med knappen **Lägg till offentlig nyckel** i OAuth2-programkonfigurationen i Workfront.

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>openssl req -x509 -sha256 -nodes -newkey rsa:2048 -keyout private.key -out certificate_pub.crt</code></pre>

* Använd knappen **Skapa ett offentligt/privat nyckelpar** i OAuth2-programkonfigurationen i Workfront för att generera RSA.

## Skapa en JSON-webbtoken

JSON Web Token för autentisering av tjänstkonto kräver en viss uppsättning anspråk och måste signeras med ett giltigt digitalt signeringscertifikat. Vi rekommenderar att du använder ett av de allmänt tillgängliga biblioteken eller verktygen för att skapa en JWT.

Följande tabell innehåller information om fält som kan behövas när du konfigurerar JWT-token.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">exp</td> 
   <td> <p>Obligatoriskt. Parametern expiration är en obligatorisk parameter som mäter den absoluta tiden sedan 1970-01-01. Du måste se till att förfallotiden är senare än tidpunkten för utfärdandet. Efter denna tid är JWT inte längre giltigt. </p> <p>Obs! Vi rekommenderar att du har en mycket kort token (några minuter), så att den upphör att gälla så snart den har bytts ut mot en åtkomsttoken. Varje gång en ny åtkomsttoken krävs signeras en JWT och byts ut. Detta är ett säkrare tillvägagångssätt. Vi rekommenderar inte längre aktiva token som återanvänds för att få åtkomsttoken efter behov.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">is</td> 
   <td>Obligatoriskt. Utfärdaren är ditt kund-ID från OAuth2-appinformationen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">sub</td> 
   <td>Obligatoriskt. Ämnet är ditt användar-ID som skapade den offentliga nyckeln i konfigurationen.</td> 
  </tr> 
 </tbody> 
</table>

## Exchange the JWT to retrieve an access token

1. Skicka en begäran om POST till:

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>https://yourdomain.my.workfront.com/integrations/oauth2/api/v1/jwt/exchange</code></pre>

1. Innehållet i begäran ska innehålla URL-kodade parametrar med ditt klient-ID, klienthemlighet och JWT:

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>client_id={client_id_value}&client_secret={client_secret_value}&jwt_token={base64_encoded_JWT}</code></pre>

 

---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Hämta OAuth2-token
description: Hämta OAuth2-token
author: Becky
feature: Workfront API
role: Developer
exl-id: f3a2630d-d34e-4d36-b2bb-707ba0d3258e
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---


# Hämta OAuth2-token

## Hämtar OAuth2-token

Returnerar OAuth2-uppdateringstoken och åtkomsttoken för en autentiserad användare. Detta anropas en gång när användaren tillhandahåller en dokumentleverantör. Efterföljande anrop görs för att få en uppdaterad åtkomsttoken.

**URL**

POST /any/url

URL:en är konfigurerbar och motsvarar värdet för Token Endpoint URL på sidan Anpassade integrationsinställningar.

### Frågeparametrar

<table style="table-layout:auto">
 <col>
 <col>
 <col>
 <thead>
  <tr>
   <th>Namn</th>
   <th>Obligatoriskt</th>
   <th>Beskrivning</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>grant_type</td>
   <td>ja</td>
   <td><p>Du kan ange värdena "authentication_code" eller "refresh_token". Det angivna värdet anger vilken av de två parametrarna som skickas till det här API-anropet: code eller refresh_token.</p></td>
  </tr>
  <tr>
   <td>kod</td>
   <td>beroende</td>
   <td><p>Auktoriseringskoden som skickas till Adobe Workfront strax efter att användaren har klickat på knappen "Bevilja". Detta är endast obligatoriskt när anslagstypen är "permission_code". Auktoriseringskoden ska vara kortvarig och i allmänhet upphöra om 10 minuter eller mindre.</p></td>
  </tr>
  <tr>
   <td>refresh_token</td>
   <td>beroende</td>
   <td><p>Detta krävs endast vid efterföljande anrop för att hämta en ny access_token, eftersom föregående access_token har upphört att gälla. När du skickar det här värdet anger du parametern grant_type till "refresh_token".</p></td>
  </tr>
  <tr>
   <td>client_id</td>
   <td>ja</td>
   <td>Klient-ID som konfigurerats i Workfront för den här anpassade integreringen.</td>
  </tr>
  <tr>
   <td>client_secrets</td>
   <td>ja</td>
   <td> Klienthemlighet som konfigurerats i Workfront för den här anpassade integreringen.</td>
  </tr>
 </tbody>
</table>

 

## Svar

<table style="table-layout:auto">
 <col>
 <col>
 <col>
 <thead>
  <tr>
   <th>Namn</th>
   <th>Typ </th>
   <th>Beskrivning</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>access_token </td>
   <td>Sträng</td>
   <td><p>En token som används för att göra auktoriserade API-anrop för användarens räkning. Detta bör upphöra att gälla för att förhindra otillåtna API-anrop.</p></td>
  </tr>
  <tr>
   <td>refresh_token </td>
   <td>Sträng</td>
   <td><p>En långvarig token som används för att hämta en ny access_token genom att anropa den här API-metoden.</p></td>
  </tr>
  <tr>
   <td>förfaller_in </td>
   <td>long</td>
   <td><p>(valfritt) Tiden (i sekunder) innan åtkomsttoken upphör att gälla, vanligtvis 3 600.</p></td>
  </tr>
 </tbody>
</table>

**Exempel**

```
POST /oauth2/token
grant_type=authorization_code
code=d9ac7asdf6asdf579d7a8
client_id=123456
client_secret=6asdf7a7a9a4af
```

## Svar

```
{
access_token:"ad8af5ad5ads759",
refresh_token:"9a0h5d87d808ads",
expires_id:3600
}
```

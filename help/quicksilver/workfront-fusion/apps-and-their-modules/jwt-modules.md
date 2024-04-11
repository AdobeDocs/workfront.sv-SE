---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: JWT-moduler
description: The [!DNL Adobe Workfront Fusion] [!UICONTROL JWT] app innehåller en modul som skapar JWT-token baserat på den angivna algoritmen.
author: Becky
feature: Workfront Fusion
source-git-commit: d4f6f5d4919120e37fb94a23ac834a3896019584
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# [!UICONTROL JWT] modul

The [!DNL Adobe Workfront Fusion] [!UICONTROL JWT] app innehåller en modul som skapar JWT-token baserat på den angivna algoritmen.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] eller högre</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licens**</td> 
   <td>
   <p>Aktuellt licenskrav: Nej [!DNL Workfront Fusion] krav på licens.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration],  [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuellt produktbehov: Om du har [!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Adobe Workfront] Planera, din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln. [!DNL Workfront Fusion] ingår i [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>eller</p>
   <p>Krav för äldre produkter: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta din [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## JWT-modulen och dess fält

### Generera JWT

Den här modulen genererar en JWT baserad på den valda algoritmen.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Algorithm]</td> 
   <td> <p>Välj den algoritm med vilken du vill generera JWT.</p> <ul>
   <li><b>HS256</b>: HMAC med SHA-256-hash-algoritm</li>
   <li><b>HS384</b>: HMAC med SHA-384-hash-algoritm</li>
   <li><b>HS512</b>: HMAC med SHA-512-hash-algoritm</li>
   <li><b>RS256</b>: RSASSA-PKCS1-v1_5 med SHA-256-hash-algoritm</li>
   <li><b>RS384</b>: RSASSA-PKCS1-v1_5 med SHA-384-hash-algoritm</li>
   <li><b>RS512</b>: RSASSA-PKCS1-v1_5 med SHA-512-hash-algoritm</li>
   <li><b>PS256</b>: RSASSA-PSS med SHA-256-hash-algoritm (endast nod ^6.12.0 OR &gt;=8.0.0)</li>
   <li><b>PS384</b>: RSASSA-PSS med SHA-384-hash-algoritm (endast nod ^6.12.0 OR &gt;=8.0.0)</li>
   <li><b>PS512</b>: RSASSA-PSS med SHA-512-hash-algoritm (endast nod ^6.12.0 OR &gt;=8.0.0)</li>
   <li><b>ES256</b>: ECDSA med P-256-kurva och SHA-256-hash-algoritm</li>
   <li><b>ES384</b>: ECDSA med P-384-kurva och SHA-384-hash-algoritm</li>
   <li><b>ES512</b>: ECDSA med P-521-kurva och SHA-512-hash-algoritm</li>
   </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Payload] </td> 
   <td> <p>För varje nyttolastobjekt som du vill lägga till klickar du på <b>Lägg till objekt</b> och ange objektets nyckel och värde.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Options] </td> 
   <td> <p>För varje alternativobjekt som du vill lägga till klickar du på <b>Lägg till objekt</b> och ange objektets nyckel och värde.</p> <p>Följande tangenter är tillgängliga:
   <ul>
   <li><b>algoritm</b>: (standard: RS256)</li>
   <li><b>expirresIn</b>: Uttryckt i sekunder eller en sträng som beskriver ett tidsintervall (t.ex. 2 dagar, 10h, 7d). Ett numeriskt värde tolkas som antal sekunder. Om du använder en sträng måste du se till att ange tidsenheter (dagar, timmar osv.), annars används enheten i millisekunder som standard (120 är lika med 120 ms).</li>
   <li><b>notBefore</b>: Uttryckt i sekunder eller en sträng som beskriver ett tidsintervall (t.ex. 2 dagar, 10h, 7d). Ett numeriskt värde tolkas som antal sekunder. Om du använder en sträng måste du se till att ange tidsenheter (dagar, timmar osv.), annars används enheten i millisekunder som standard (120 är lika med 120 ms).
</li>
   <li><b>publik</b></li>
   <li><b>utfärdare</b></li>
   <li><b>jwtid</b></li>
   <li><b>ämne</b></li>
   <li><b>noTimestamp</b></li>
   <li><b>header</b></li>
   <li><b>keyid</b></li>
   <li><b>mutatePayload</b>: If <code>true</code>, ändrar signeringsfunktionen nyttolastobjektet direkt. Detta är användbart om du behöver en oformaterad referens till nyttolasten efter att anspråk har tillämpats på den men innan den har kodats till en token.</li>
   <li><b>allowInsecureKeySizes</b>: If <code>true</code>, tillåter att privata nycklar med en modulus under 2048 används för RSA.</li>
   <li><b>allowInvalidAsymmetricKeyTypes</b>: If <code>true</code>, tillåter asymmetriska nycklar som inte matchar den angivna algoritmen. Detta alternativ är endast avsett för bakåtkompatibilitet och bör undvikas.</li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>


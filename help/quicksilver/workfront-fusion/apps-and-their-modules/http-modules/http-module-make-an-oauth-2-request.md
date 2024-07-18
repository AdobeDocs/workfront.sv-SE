---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: http-modules
title: HTTP-&stämpel;gt; Gör en OAuth 2.0-begärandemodul
description: För att kunna göra en  [!DNL Adobe Workfront Fusion] HTTP(S)-begäran till servrar som kräver en OAuth 2.0-auktorisering måste du först skapa en OAuth-anslutning. [!DNL Adobe Workfront Fusion] ser till att alla anrop som görs med den här anslutningen har rätt auktoriseringshuvuden och att associerade tokens uppdateras automatiskt när det behövs.
author: Becky
feature: Workfront Fusion
exl-id: 6c68c9b9-9f74-44a7-94ed-3785081b8331
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '1937'
ht-degree: 0%

---

# [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request]-modulen

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] kräver en [!DNL Adobe Workfront Fusion]-licens utöver en [!DNL Adobe Workfront]-licens.

För att kunna göra en [!DNL Adobe Workfront Fusion] HTTP(S)-begäran till servrar som kräver en OAuth 2.0-auktorisering måste du först skapa en OAuth-anslutning. [!DNL Adobe Workfront Fusion] ser till att alla anrop som görs med den här anslutningen har lämpliga auktoriseringshuvuden och att associerade tokens uppdateras automatiskt när det behövs.

[!DNL Workfront Fusion] stöder följande OAuth 2.0-autentiseringsflöden:

* Auktoriseringskodflöde
* Implicit flöde

Andra flöden, som t.ex. Resursägarens lösenordsflöde och Klientinloggningsflöde, stöds inte automatiskt i den här modulen.

Mer information om OAuth 2.0-autentisering finns i [OAuth 2.0 Authorization Framework](https://tools.ietf.org/html/rfc6749).

>[!NOTE]
>
>Om du ansluter till en Adobe-produkt som för närvarande inte har någon dedikerad anslutning rekommenderar vi att du använder Adobe Authenticator-modulen.
>
>Mer information finns i [Adobe Authenticator-modulen](/help/quicksilver/workfront-fusion/apps-and-their-modules/adobe-authenticator-modules.md).

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
   <p>Aktuellt licenskrav: Inget [!DNL Workfront Fusion]-licenskrav.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för Automatisering och integrering av arbetet] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuellt produktkrav: Om du har planen [!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Adobe Workfront] måste din organisation köpa både [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln. [!DNL Workfront Fusion] ingår i planen [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>eller</p>
   <p>Äldre produktkrav: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Skapar en anslutning för en [!DNL OAuth]-begäran

* [Allmänna instruktioner för att skapa en anslutning i HTTP > Gör en OAuth 2.0-begärandemodul](#general-instructions-for-creating-a-connection-in-the-http--make-an-oauth-20-request-module)
* [Instruktioner för hur du skapar en anslutning till Google i HTTP >[!UICONTROL Make] och OAuth 2.0-begärandemodulen](#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module)
* [Instruktioner för att ansluta till Microsoft Graph API via HTTP > Gör en OAuth 2.0-begärandemodul](#instructions-for-connecting-to-microsoft-graph-api-via-the-http--make-an-oauth-20-request-module)

### Allmänna instruktioner för att skapa en anslutning i modulen [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request]

1. Skapa en OAuth-klient i tjänsten [!DNL target] som du vill att [!DNL Adobe Workfront Fusion] ska kommunicera med. Det här alternativet finns troligen i avsnittet [!UICONTROL Developer] i den angivna tjänsten.

   1. När du skapar en klient anger du rätt URL i fältet `[!UICONTROL Redirect URL]` eller `[!UICONTROL Callback URL]`:

      | Amerika/APAC | https://app.workfrontfusion.com/oauth/cb/oauth2 |
      |---|---|
      | EMEA | https://app-eu.workfrontfusion.com/oauth/cb/oauth2 |

   1. När du har skapat klienten visar den angivna tjänsten två nycklar: `[!UICONTROL Client ID]` och `[!UICONTROL Client Secret]`. Vissa tjänster anropar dessa `[!UICONTROL App Key]` och `[!UICONTROL App Secret]`. Spara nyckeln och hemligheten på en säker plats så att du kan ange dem när du skapar anslutningen i Workfront Fusion.

1. Sök efter `[!UICONTROL Authorize URI]` och `[!UICONTROL Token URI]` i API-dokumentationen för den angivna tjänsten. Det här är URL-adresser som [!DNL Workfront Fusion] kommunicerar med tjänsten [!DNL target] genom. Adresserna används för OAuth-auktorisering.

   >[!NOTE]
   >
   >Om tjänsten använder implicit flöde behöver du bara `[!UICONTROL Authorize URI]`.

   >[!INFO]
   >
   >**Exempel:** Yahoo-adresser:
   >
   >* Auktorisera URI:
   >
   >`https://api.login.yahoo.com/oauth2/request_auth`
   >
   >* Token-URI:
   >
   >`https://api.login.yahoo.com/oauth2/get_token`

1. (Villkorligt) Om måltjänsten använder omfattningar (åtkomsträttigheter) kontrollerar du hur tjänsten skiljer enskilda omfattningar åt och ser till att du anger avgränsaren i de avancerade inställningarna i enlighet med detta. Om avgränsaren inte är rätt inställd kan [!DNL Workfront Fusion] inte skapa anslutningen och du får ett ogiltigt omfångsfel.
1. När du har slutfört stegen ovan kan du börja skapa OAuth-anslutningen i [!DNL Workfront Fusion]. Lägg till OAuth 2.0 HTTP(S)-begäran och svarsbearbetningsmodulen i ditt scenario.
1. Klicka på **[!UICONTROL Add]** i anslutningsfältet i modulen.

1. Fyll i följande fält för att skapa en anslutning:

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection name] </td> 
      <td> <p>Ange namnet på anslutningen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Flow type]</p> </td> 
      <td> <p>Välj flödet för att hämta tokens.</p> 
       <ul> 
        <li><strong>[!UICONTROL Authorization Code]</strong>: Ange <code>[!UICONTROL Authorize URI]</code> och <code>[!UICONTROL Token URI]</code> från tjänstens API-dokumentation.</li> 
        <li><strong>[!UICONTROL Implicit]</strong>: Ange <code>[!UICONTROL Authorize URI]</code> från tjänstens API-dokumentation.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope] </td> 
      <td> <p>Lägg till enskilda omfattningar. Den här informationen finns i den angivna tjänstens API-dokumentation (developer).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope separator] </td> 
      <td> <p>Välj vilka scope som ska avgränsas av ovan. Den här informationen finns i den angivna tjänstens API-dokumentation (developer).</p> <p>Varning! Om avgränsaren inte är rätt inställd kan [!DNL Workfront Fusion] inte skapa anslutningen och du får ett ogiltigt omfångsfel.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID] </td> 
      <td> <p>Ange klient-ID. Du fick klient-ID när du skapade en OAuth-klient i den tjänst som du vill ansluta.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td> <p> Ange klienthemlighet. Du fick klienthemligheten när du skapade en OAuth-klient i tjänsten som du vill ansluta.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Authorize parameters]</p> </td> 
      <td> <p>Lägg till de parametrar som du vill inkludera i auktoriseringsanropet. Följande standardparametrar inkluderas alltid automatiskt och behöver inte läggas till.</p> <p>Standardparametrar:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL response_type]</strong> </p> <p> <code>code </code>för [!UICONTROL Authorization Code flow] och <code>token </code>för [!UICONTROL Implicit flow]</p> </li> 
        <li> <p><strong>[!UICONTROL redirect_uri]</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">Amerika/APAC</td> 
            <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
           <tr> 
            <td role="rowheader">EMEA </td> 
            <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
          </tbody> 
         </table> </li> 
        <li> <p><strong>[!UICONTROL client_id]</strong> </p> <p> Klient-ID som du fick när du skapade kontot</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Access token parameters]</p> </td> 
      <td> <p>Lägg till de parametrar som du vill ta med i tokenanropet. Följande standardparametrar inkluderas alltid automatiskt och behöver inte läggas till.</p> <p>Standardparametrar:</p> 
       <ul> 
        <li><strong>[!UICONTROL grant_type]</strong>: <code>authorization_code</code></li> 
        <li> <p><strong>[!UICONTROL redirect_uri]:</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">Amerika/APAC</td> 
            <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
           <tr> 
            <td role="rowheader">EMEA </td> 
            <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
          </tbody> 
         </table> </li> 
        <li><strong>[!UICONTROL client_id]</strong>: Det klient-ID som du fick när du skapade kontot inkluderas automatiskt i begärandetexten</li> 
        <li><strong>client_secrets</strong>: Klienthemligheten som du fick när du skapade kontot inkluderas automatiskt i begärandetexten</li> 
        <li><strong>kod</strong>: Koden som returnerades av auktoriseringsbegäran</li> 
       </ul> <p>Obs!  <p>OAuth 2.0-standarden stöder minst två metoder för klientautentisering under det här steget (<code>[!UICONTROL client_secret_basic]</code> och <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] skickar automatiskt angivet klient-ID och hemlighet via metoden <code>[!UICONTROL client_secret_post]</code>. Därför inkluderas dessa parametrar automatiskt som en del av tokenbegärandetexten. </p> <p>Mer information om OAuth 2.0-autentisering finns i <a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0 Authorization Framework</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Refresh token parameters]</p> </td> 
      <td> <p>Lägg till de parametrar som du vill ta med i tokenanropet. Följande standardparametrar inkluderas alltid automatiskt och behöver inte läggas till.</p> <p>Standardparametrar:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL grant_type]</strong>: <code>refresh_token</code></p> </li> 
        <li> <p><strong>[!UICONTROL refresh_token]</strong>: Den senaste uppdateringstoken som erhölls av tjänsten som du ansluter till</p> </li> 
        <li> <p><strong>[!UICONTROL client_id]</strong>: Det klient-ID som du fick när du skapade kontot inkluderas automatiskt i begärandetexten</p> </li> 
        <li> <p><strong>[!UICONTROL client_secret]</strong>: Den klienthemlighet du fick när du skapade kontot inkluderas automatiskt i begärandetexten</p> </li> 
       </ul> <p>Obs!  <p>OAuth 2.0-standarden stöder minst två metoder för klientautentisering under det här steget (<code>[!UICONTROL client_secret_basic]</code> och <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] skickar automatiskt angivet klient-ID och hemlighet via metoden <code>[!UICONTROL client_secret_post]</code>. Därför inkluderas dessa parametrar automatiskt som en del av tokenbegärandetexten. </p> <p>Mer information om OAuth 2.0-autentisering finns i <a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0 Authorization Framework</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Custom Headers]</p> </td> 
      <td> <p>Ange eventuella ytterligare nycklar och värden som ska inkluderas i huvudet i [!UICONTROL Token]- och R[!UICONTROL efresh Token]-stegen.</p> <p>Obs!  <p>OAuth 2.0-standarden stöder minst två metoder för klientautentisering under det här steget (<code>[!UICONTROL client_secret_basic]</code> och <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] stöder inte automatiskt metoden <code>[!UICONTROL client_secret_basic]</code>. Om tjänsten som du ansluter till förväntar sig att klient-ID och klienthemlighet ska kombineras till en enda sträng och sedan base64 kodas i auktoriseringshuvudet, ska du lägga till det huvud- och nyckelvärdet här.</p> <p> Mer information om OAuth 2.0-autentisering finns i <a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0 Authorization Framework</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Token placement]</p> </td> 
      <td> <p>Välj om du vill skicka token i [!UICONTROL header], [!UICONTROL query string] eller i båda vid anslutning till angiven URL.</p> <p>Token skickas oftast i begärandehuvudet.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Header token name] </td> 
      <td> <p>Ange namnet på auktoriseringstoken i huvudet. Standard: <code>[!UICONTROL Bearer]</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Query string parameter name] </td> 
      <td> <p>Ange namnet på auktoriseringstoken i frågesträngen. Standard: <code>[!UICONTROL access_token]</code>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **[!UICONTROL Continue]** om du vill spara anslutningsinställningarna.
1. Fortsätt till [konfigurationen av OAuth 2.0-begärandemodulen](#oauth-20-request-module-setup).

### Instruktioner för att skapa en anslutning till [!DNL Google] i [!UICONTROL HTTP] >[!UICONTROL Make an OAuth 2.0 request module]

I följande exempel visas hur du använder [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0]-begärandemodulen för att ansluta till [!DNL Google].

1. Kontrollera att du har skapat ett projekt, konfigurerat OAuth-inställningar och genererat dina autentiseringsuppgifter enligt beskrivningen i [Anslut [!DNL Adobe Workfront Fusion] till [!DNL Google Services] med en anpassad OAuth-klient](../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).
1. Öppna modulen [!UICONTROL HTTP] >[!UICONTROL Make an OAuth 2.0 request].
1. Klicka på **[!UICONTROL Add]** bredvid anslutningsrutan.
1. Ange följande värden:

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection name] </td> 
      <td> <p>Ange namnet på anslutningen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Flow type]</p> </td> 
      <td> <p>[!UICONTROL Authorization Code]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authorize URI]</td> 
      <td><code>https://accounts.google.com/o/oauth2/v2/auth</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token URI]</td> 
      <td><code>https://www.googleapis.com/oauth2/v4/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope] </td> 
      <td> <p>Lägg till enskilda omfattningar. Mer information om omfång finns i <a href="https://developers.google.com/identity/protocols/oauth2/scopes">OAuth 2.O-omfång för [!DNL Google] API:er </a> i [!DNL Google]-dokumentationen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope separator] </td> 
      <td> <p>[!UICONTROL SPACE]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID] </td> 
      <td> <p>Ange ditt klient-ID för [!DNL Google]. </p> <p>Information om hur du skapar ett klient-ID finns i <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">Skapa OAuth-autentiseringsuppgifter</a> i <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] till [!DNL Google Services] med en anpassad OAuth-klient</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td> <p>Ange din [!DNL Google]-klienthemlighet. </p> <p>Mer information om hur du skapar en klienthemlighet finns i <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">Skapa OAuth-autentiseringsuppgifter</a> i <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] till [!DNL Google] Services med en anpassad OAuth-klient</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Authorize parameters]</p> </td> 
      <td> <p>Lägg till <code>[!UICONTROL access_type]</code> - <code>[!UICONTROL offline] </code> nyckelvärdepar.</p> <p> <img src="assets/google-authentication-http.png"> </p> <p>Obs! Om du får autentiseringsproblem, till exempel när du uppdaterar token, kan du försöka med att lägga till nyckelvärdepar för <code>[!UICONTROL prompt] </code>- <code>[!UICONTROL consent] </code>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **[!UICONTROL Continue]** om du vill spara anslutningsinställningarna.
1. Fortsätt till [konfigurationen av OAuth 2.0-begärandemodulen](#oauth-20-request-module-setup).

### Instruktioner för att ansluta till [!DNL Microsoft Graph API] via modulen [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request]

Anvisningar om [!DNL Microsoft Graph API] finns i [Anropa  [!DNL MS Graph REST API] via  [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request]-modulen](../../../workfront-fusion/connections/call-the-ms-graph-rest-api.md).

## OAuth 2.0-modulkonfiguration för begäran

När du har upprättat en [!DNL Oauth 2].0-anslutning enligt beskrivningen i [Skapa en anslutning för en  [!DNL OAuth] begäran](#creating-a-connection-for-an-oauth-request) fortsätter du att konfigurera modulen efter behov. Alla auktoriseringstoken inkluderas automatiskt i denna begäran och i alla andra begäranden som använder samma anslutning.

När du konfigurerar modulen [!UICONTROL HTTP] >[!UICONTROL Make an OAuth 2.0 request] visar [!DNL Workfront Fusion] fälten som listas nedan. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

<!--
<img src="assets/map-toggle-350x74.png" style="width: 350;height: 74;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Mer information om hur du konfigurerar en anslutning finns i <a href="#creating-a-connection-for-an-oauth-request" class="MCXref xref">Skapa en anslutning för en OAuth-begäran</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Evaluate all states as errors (except for 2xx and 3xx]) </td> 
   <td> <p>Använd det här alternativet om du vill konfigurera felhantering.</p> <p>Mer information finns i <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">Felhantering i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Ange den URL som du vill skicka en begäran till, t.ex. en API-slutpunkt, webbplats osv.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Metoder för HTTP-begäran i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers] </td> 
   <td> <p>Lägg till rubrikerna för begäran i form av ett standard-JSON-objekt. Exempel: <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Ange önskade nyckelvärdepar för frågan.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Body type]</p> </td> 
   <td> <p>HTTP-brödtexten är de databyte som skickas i ett HTTP-transaktionsmeddelande omedelbart efter rubrikerna om något ska användas.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>Raw-brödtexttypen är vanligtvis lämplig för de flesta HTTP-innehållsbegäranden, även i situationer där utvecklardokumentationen inte anger vilka data som ska skickas.</p> <p>Ange en form av tolkning av data i fältet [!UICONTROL Content type].</p> <p>Trots att innehållstypen är vald, anges data i vilket format som helst som anges eller krävs av utvecklardokumentationen.</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>Den här brödtypen är att POST data med <code>[!UICONTROL application/x-www-form-urlencoded]</code>.</p> <p>För <code>[!UICONTROL application/x-www-form-urlencoded]</code> är brödtexten i HTTP-meddelandet som skickas till servern i princip en frågesträng. Nycklarna och värdena kodas i nyckelvärdepar avgränsade med <code>&amp;</code> och med en <code>=</code> mellan nyckeln och värdet. </p> <p>För binära data <code>use [!UICONTROL multipart/form-data]</code> i stället.</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>Exempel: </b></span></span> 
       <p>Exempel på det resulterande formatet för HTTP-begäran:</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL Multipart/form-data]</strong> </p> <p>[!UICONTROL Multipart/form-data] är en HTTP-multipart-begäran som används för att skicka filer och data. Det används ofta för att överföra filer till servern.</p> <p>Lägg till fält som ska skickas i begäran. Varje fält måste innehålla ett nyckelvärdepar.</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Text]</strong> </p> <p>Ange nyckeln och värdet som ska skickas i begärandetexten.</p> </li> 
       <li> <p><strong>[!UICONTROL File]</strong> </p> <p>Ange nyckeln och ange den källfil som du vill skicka i begärandetexten.</p> <p>Mappa filen som du vill överföra från föregående modul (till exempel [!UICONTROL HTTP] &gt;[!UICONTROL Get a File] eller [!UICONTROL Google Drive] &gt;[!UICONTROL Download a File)]) eller ange filnamnet och fildata manuellt.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Parse response]</p> </td> 
   <td> <p>Aktivera det här alternativet om du vill analysera svar automatiskt och konvertera JSON- och XML-svar så att du inte behöver använda [!UICONTROL JSON] &gt; [!UICONTROL Parse JSON] eller [!UICONTROL XML] &gt; [!UICONTROL Parse XML]-moduler.</p> <p>Innan du kan använda tolkat JSON- eller XML-innehåll kör du modulen en gång manuellt, så att modulen kan identifiera svarsinnehållet och mappa det i efterföljande moduler.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timeout] </td> 
   <td> <p>Ange timeout för begäran i sekunder (1-300). Standardvärdet är 40 sekunder.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Share cookies with other HTTP modules]</td> 
   <td> <p> Aktivera det här alternativet om du vill dela cookies från servern med alla HTTP-moduler i ditt scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Self-signed certificate]</td> 
   <td> <p> Överför ditt certifikat om du vill använda TLS med ditt självsignerade certifikat.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reject connections that are using unverified (self-signed) certificates] </td> 
   <td> <p>Aktivera det här alternativet om du vill avvisa anslutningar som använder overifierade TLS-certifikat.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Follow redirect]</td> 
   <td> <p> Aktivera det här alternativet om du vill följa URL-omdirigeringarna med 3xx-svar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Follow all redirects] </td> 
   <td> <p>Aktivera det här alternativet om du vill följa URL-omdirigeringarna med alla svarskoder.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Disable serialization of multiple same query string keys as arrays]</p> </td> 
   <td> <p>Som standard hanterar [!DNL Workfront Fusion] flera värden för samma URL-frågesträngsparameternyckel som matriser. <code>www.test.com?foo=bar&amp;foo=baz</code> konverteras till exempel till <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>. Aktivera det här alternativet om du vill inaktivera funktionen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Request compressed content]</td> 
   <td> <p> Aktivera det här alternativet om du vill begära en komprimerad version av webbplatsen.</p> <p>Detta lägger till en <code>[!UICONTROL Accept-Encoding]</code>-rubrik för att begära komprimerat innehåll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Use Mutual TLS]</td> 
   <td> <p>Aktivera det här alternativet om du vill använda ömsesidig TLS i HTTP-begäran.</p> <p>Mer information om ömsesidigt TLS finns i <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">Använd ömsesidigt TLS i HTTP-moduler i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

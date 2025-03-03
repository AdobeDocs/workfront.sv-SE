---
title: Skapa OAuth2-program för  [!DNL Workfront] integreringar
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Som  [!DNL Adobe Workfront] administratör kan du skapa OAuth2-program för din instans av  [!DNL Workfront], som ger andra program åtkomst till Workfront. Dina användare kan sedan ge dessa andra program behörighet att komma åt sina Workfront-data. På så sätt kan du integrera Workfront med valfria program, inklusive egna, interna program.
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: e13c7dda-8945-47ad-b6d3-4d6a62b368f5
source-git-commit: 09f7e854c2df1291feb150d2169fa6ccd5cdb1d6
workflow-type: tm+mt
source-wordcount: '1831'
ht-degree: 0%

---

# Skapa OAuth2-program för [!DNL Workfront] integreringar

Som [!DNL Adobe Workfront]-administratör kan du skapa OAuth2-program för din instans av [!DNL Workfront], som ger andra program åtkomst till [!DNL Workfront]. Dina användare kan sedan ge dessa andra program behörighet att komma åt sina [!DNL Workfront]-data. På så sätt kan du integrera   med valfria program, inklusive egna, interna tillämpningar.

När du skapar ett [!UICONTROL OAuth2]-program genererar du ett klient-ID och en klienthemlighet. Dina användare kan sedan använda klient-ID i API-anrop för att integrera med det program du har skapat.

>[!NOTE]
>
>I OAuth2-kontexten avser&quot;skapa en app&quot; processen att skapa den här typen av åtkomstlänk mellan en app och en server som [!DNL Workfront].

* Instruktioner om hur du konfigurerar och använder OAuth2-programmet med inloggningsuppgifter (auktoriseringskodflöde) finns i [Konfigurera och använda organisationens anpassade OAuth 2-program med auktoriseringskodflöde](../../wf-api/api/oauth-app-code-token-flow.md).
* Instruktioner om hur du konfigurerar och använder OAuth2-programmet med serverautentisering (JWT-flöde) finns i [Konfigurera och använda organisationens anpassade OAuth 2-program med JWT-flöde](../../wf-api/api/oauth-app-jwt-flow.md).
* Instruktioner om hur du konfigurerar och använder OAuth2-programmet med PKCE finns i [Konfigurera och använda organisationens anpassade OAuth 2-program med PKCE-flöde](../../wf-api/api/oauth-app-pkce-flow.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td><p>Nytt: [!UICONTROL Standard]</p>
   eller
   <p>Aktuell:[!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> Du måste vara en [!DNL Workfront]-administratör. </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## OAuth2 - översikt

Tänk dig att ett program måste hämta viss specifik information från [!DNL Workfront]. Ett program som begär information kallas för en klient. I det här exemplet är klientnamnet ClientApp. ClientApp behöver åtkomst till en viss användares information och måste därför ha åtkomst till [!DNL Workfront] som den användaren. Om användaren ger ClientApp sitt användarnamn och lösenord kan ClientApp komma åt alla data som användaren har åtkomst till. Det här är en säkerhetsrisk eftersom ClientApp bara behöver en liten, specifik uppsättning information.

När du skapar en OAuth2-app för ClientApp talar du i stort sett om för [!DNL Workfront] att ClientApp har åtkomst till [!DNL Workfront], men bara om den användare vars konto ClientApp har åtkomst ger åtkomst till programmet.

## Skapa ett OAuth2-program

När du skapar ett OAuth2-program ska du välja den typ av program som bäst uppfyller integreringens behov.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Programtyp</th> 
   <th>Bäst för</th> 
   <th>Autentiseringsmetod</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Program för dator till dator</p> </td> 
   <td> <p>Passar bäst för CLI, daemon och skript som körs på servern</p> <p>Exempel:</p> 
    <ul> 
     <li> <p>[!DNL Shell] </p> </li> 
     <li> <p>[!DNL Python]</p> </li> 
    </ul> </td> 
   <td> <p>Autentisering via JSON Web Token med offentlig/privat nyckelparskodning.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Webbprogram för en sida</p> </td> 
   <td> <p>Passar bäst för mobil- och enkelsidiga webbapplikationer</p> <p>Exempel:</p> 
    <ul> 
     <li> <p>[!DNL Javascript]</p> </li> 
     <li> <p>[!DNL Angular]</p> </li> 
     <li> <p>[!DNL React]</p> </li> 
     <li> <p>[!DNL Vue]</p> </li> 
    </ul> </td> 
   <td> <p>Autentisering genom OAuth 2.0 Authorization Code med Proof Key for Code Exchange (PKCE).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Webbprogram</p> </td> 
   <td> <p>Passar bäst för program på serversidan som hanterar autentiseringsuppgifter och tokens på servern</p> <p>Exempel:</p> 
    <ul> 
     <li> <p>[!DNL Go]</p> </li> 
     <li> <p>[!DNL Java]</p> </li> 
     <li> <p>[!DNL ASP.Net]</p> </li> 
     <li> <p>[!DNL Node.js]</p> </li> 
     <li> <p>[!DNL PHP]</p> </li> 
    </ul> </td> 
   <td> <p>Autentisering via OAuth 2.0 Authorization Code flow.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Du kan ha upp till totalt tio OAuth2-program samtidigt.

* [Skapa ett OAuth2-program med serverautentisering (JWT-flöde)](#create-an-oauth2-application-using-server-authentication-jwt-flow)
* [Skapa ett OAuth2-program med användarens inloggningsuppgifter (kodflöde för auktorisering)](#create-an-oauth2-application-using-user-credentials-authorization-code-flow)
* [Skapa ett ensidigt OAuth2-webbprogram med PKCE](#create-an-oauth2-single-page-web-application-using-pkce)

### Skapa ett OAuth2-program med serverautentisering (JWT-flöde) {#create-an-oauth2-application-using-server-authentication-jwt-flow}

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL System]** i den vänstra navigeringspanelen och välj sedan **[!UICONTROL OAuth2 Applications]**.
1. Klicka på **[!UICONTROL Create app integration]**.
Rutan **Nytt OAuth2-program** visas.
1. Välj **[!UICONTROL Machine to Machine Application]** i rutan **Nytt OAuth2-program**.
1. Ange ett namn för det nya programmet, till exempel [!DNL Workfront] för ClientApp.
1. Klicka på **[!UICONTROL Create]**.
1. Fyll i fälten för den nya appen.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td> <p>Det här fältet genereras automatiskt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client secret]</td> 
      <td> <p>Det här fältet genereras automatiskt</p> <p><b>VIKTIGT</b>:  <p>Kopiera innehållet i det här fältet till en annan säker fil innan du stänger den här sidan. Du kommer inte att kunna se den här hemliga nyckeln igen.</p> <p>Om du förlorar den här nyckeln tar du bort den och skapar en klienthemlighet.</p> 
        <ol> 
         <li value="1"> <p>Klicka på ikonen <b>[!UICONTROL Delete]</b> <img src="assets/delete.png"> för att ta bort den aktuella klienthemligheten.</p> </li> 
         <li value="2"> <p>Klicka på <b>[!UICONTROL Add client secret]</b> om du vill skapa en ny klienthemlighet.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Public Keys]</td> 
      <td> <p>Server-till-server-appar använder offentliga och privata nycklar för autentisering. Gör något av följande:</p> 
       <ul> 
        <li> <p>Klicka på <b>[!UICONTROL Add a public key]</b> och ange den offentliga nyckeln från det andra programmet.</p> </li> 
        <li> <p>Klicka på <b>[!UICONTROL Generate a public/private keypair]</b> och dela sedan den offentliga nyckeln med det andra programmet.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Det här är samma namn som du gav appen. Det här fältet får inte vara tomt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Ange en beskrivning för integreringen.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **[!UICONTROL Save]**.

Instruktioner om hur du konfigurerar och använder OAuth2-programmet med inloggningsuppgifter (auktoriseringskodflöde) finns i [Konfigurera och använda organisationens anpassade OAuth 2-program med JWT-flöde](../../wf-api/api/oauth-app-jwt-flow.md).

### Skapa ett OAuth2-program med användarens inloggningsuppgifter (kodflöde för auktorisering) {#create-an-oauth2-application-using-user-credentials-authorization-code-flow}

>[!NOTE]
>
>Om du skapar ett program för att ansluta till Workfront Fusion använder du någon av följande omdirigerings-URL:er:
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-workfront`
>* `https://app-eu.workfrontfusion.com/oauth/cb/workfront-workfront` (EU-datacenter)
>* `https://app-az.workfrontfusion.com/oauth/cb/workfront-workfront` (Azure Data Center)

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL System]** i den vänstra navigeringspanelen och välj sedan **[!UICONTROL OAuth2 Applications]**.
1. Klicka på **[!UICONTROL Create app integration]**.

   **Nytt OAuth2-program** visas.
1. Välj **[!UICONTROL Web Application]** i rutan **Nytt OAuth2-program**.
1. Ange ett namn för det nya OAuth2-programmet, till exempel [!DNL Workfront] för ClientApp.
1. Klicka på **[!UICONTROL Create]**.
1. Fyll i fälten för den nya appen.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td> <p>Det här fältet genereras automatiskt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client secret]</td> 
      <td> <p>Det här fältet genereras automatiskt</p> <p><b>VIKTIGT</b>:  <p>Kopiera innehållet i det här fältet till en annan säker fil innan du stänger den här sidan. Du kommer inte att kunna se den här hemliga nyckeln igen.</p> <p>Om du förlorar den här nyckeln tar du bort den och skapar en klienthemlighet.</p> 
        <ol> 
         <li value="1"> <p>Klicka på ikonen <b>[!UICONTROL Delete]</b> <img src="assets/delete.png"> för att ta bort den aktuella klienthemligheten.</p> </li> 
         <li value="2"> <p>Klicka på <b>[!UICONTROL Add client secret]</b> om du vill skapa en ny klienthemlighet.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Redirect URLs]</td> 
      <td>Användare omdirigeras till den här sökvägen efter att de har autentiserats med [!DNL Workfront].</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Refresh token rotation]</td> 
      <td>Aktivera det här alternativet om du vill att en ny uppdateringstoken ska utfärdas när uppdateringstoken används. Programmet måste lagra den nya uppdateringstoken efter varje uppdatering.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Absolute refresh token expiration]</td> 
      <td> <p>Välj hur lång tid du vill att en uppdateringstoken ska finnas innan den upphör att gälla. När den upphör att gälla måste användarna logga in på integreringen igen. Välj [!UICONTROL No expiration] om du inte vill att uppdateringstoken ska förfalla.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Inaktivitetsuppdateringstoken förfaller</td> 
      <td> <p>Välj efter hur lång tid, om användaren inte har varit aktiv i systemet, deras uppdateringstoken förfaller. </p> <p>Om till exempel inaktivitetens utgångsdatum för uppdateringstoken är sex månader och användaren inte loggar in på sex månader, upphör uppdateringstoken att gälla även om den absoluta utgångstiden för uppdateringstoken kan anges längre.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Logo]</td> 
      <td>Du kan lägga till en logotyp för att göra appen mer identifierbar. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Det här är samma namn som du gav appen. Det här fältet får inte vara tomt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Ange en beskrivning för integreringen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL App Description URL]</td> 
      <td>Det kan vara en länk till en"Om oss"-sida eller en sida med mer information om integreringen.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **[!UICONTROL Save]**.

Instruktioner om hur du konfigurerar och använder OAuth2-programmet med inloggningsuppgifter (auktoriseringskodflöde) finns i [Konfigurera och använda organisationens anpassade OAuth 2-program med auktoriseringskodflöde](../../wf-api/api/oauth-app-code-token-flow.md).

### Skapa ett ensidigt OAuth2-webbprogram med PKCE {#create-an-oauth2-single-page-web-application-using-pkce}

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL System]** i den vänstra navigeringspanelen och välj sedan **[!UICONTROL OAuth2 Applications]**.
1. Klicka på **[!UICONTROL Create app integration]**.

   Rutan **Nytt OAuth2-program** visas.
1. Välj **[!UICONTROL Single Page Web Application]** i rutan **Nytt OAuth2-program**.
1. Ange ett namn för det nya [!UICONTROL OAuth2]-programmet, till exempel [!DNL Workfront] för ClientApp.
1. Klicka på **[!UICONTROL Create]**.
1. Fyll i fälten för den nya appen.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td> <p>Det här fältet genereras automatiskt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Redirect URLs]</td> 
      <td>Användare omdirigeras till den här sökvägen när de har autentiserats med Workfront.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Rotate refresh token every time it is used]</td> 
      <td>Aktivera det här alternativet om du vill att en ny uppdateringstoken ska utfärdas när uppdateringstoken används. Programmet måste lagra den nya uppdateringstoken efter varje uppdatering.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Absolute expiration]</td> 
      <td> <p>Välj hur lång tid du vill att en uppdateringstoken ska finnas innan den upphör att gälla. När den upphör att gälla måste användarna logga in på integreringen igen. Välj [!UICONTROL No expiration] om du inte vill att uppdateringstoken ska förfalla.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Inactivity expiration]</td> 
      <td> <p>Välj efter hur lång tid, om användaren inte har varit aktiv i systemet, deras uppdateringstoken förfaller. </p> <p>Om till exempel inaktivitetens utgångsdatum för uppdateringstoken är sex månader och användaren inte loggar in på sex månader, upphör uppdateringstoken att gälla även om den absoluta utgångstiden för uppdateringstoken kan anges längre.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Logo]</td> 
      <td>Du kan lägga till en logotyp för att göra appen mer identifierbar. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Det här är samma namn som du gav appen. Det här fältet får inte vara tomt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Ange en beskrivning för integreringen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Developer name]</td> 
      <td>Detta är namnet på den utvecklare som konfigurerar OAuth2-programmet.</td> 
     </tr> 
   <tr> 
      <td role="rowheader">[!UICONTROL Developer email address]</td> 
      <td>Detta är e-postadressen till den utvecklare som konfigurerar OAuth2-programmet.</td> 
     </tr> 
   <tr> 
      <td role="rowheader">[!UICONTROL Privacy policy URL]</td> 
      <td>Det här är länken till den plats där din organisation lagrar integritetspolicyn.</td> 
     </tr>


   </tbody> 
   </table>

   <!-- removed this from the table, and added "Developer name" and following rows:
   [!UICONTROL App Description URL]</td> 
      <td>This can be a link to an "About us" page or a page with more information about the integration.> -->

1. Klicka på **[!UICONTROL Save]**.

## Konfigurera och använda det skapade OAuth2-programmet

Ytterligare konfiguration och användning av det skapade OAuth2-programmet kräver viss teknisk kunskap, inklusive API-anrop.

* Instruktioner om hur du konfigurerar och använder OAuth2-programmet med inloggningsuppgifter (auktoriseringskodflöde) finns i [Konfigurera och använda organisationens anpassade OAuth 2-program med auktoriseringskodflöde](../../wf-api/api/oauth-app-code-token-flow.md).
* Instruktioner om hur du konfigurerar och använder OAuth2-programmet med serverautentisering (JWT-flöde) finns i [Konfigurera och använda organisationens anpassade OAuth 2-program med JWT-flöde](../../wf-api/api/oauth-app-jwt-flow.md).
* Instruktioner om hur du konfigurerar och använder OAuth2-programmet med PKCE finns i [Konfigurera och använda organisationens anpassade OAuth 2-program med PKCE-flöde](../../wf-api/api/oauth-app-pkce-flow.md).

## OAuth2-processer för auktoriseringskodflöde

>[!NOTE]
>
>Dina användare kommer åt programmet [!UICONTROL OAuth2] via API:t. I det här avsnittet beskrivs funktionaliteten i allmänna termer och finns endast i informationssyfte.
>
>Mer information om hur du använder OAuth2-programmet, inklusive specifika API-anrop, finns i [Konfigurera och använda organisationens anpassade OAuth 2-program med hjälp av auktoriseringskodflöde](../../wf-api/api/oauth-app-code-token-flow.md).

### Auktorisera med en auktoriseringskod och åtkomsttoken {#authorizing-with-an-authorization-code-and-access-token}

1. ClientApp behöver viss information från [!DNL Workfront], så den skickar en begäran till [!DNL Workfront] API `/authorize` -slutpunkten. Begäran innehåller [!UICONTROL response_type] `code` som anger att begäran ska returnera en auktoriseringskod.
1. Detta utlöser [!DNL Workfront] för att skicka en autentiseringsfråga till användaren. Användaren kan ange sina autentiseringsuppgifter i uppmaningen, som ger [!DNL Workfront] behörighet att kommunicera med ClientApp. Om användaren redan är inloggad på [!DNL Workfront] kan det här steget hoppas över.
1. API:t [!DNL Workfront] skickar en auktoriseringskod till ClientApp.
1. ClientApp skickar följande information i en begäran till [!DNL Workfront] API `/token`   slutpunkt:

   * Auktoriseringskoden som skickas till ClientApp i steg 3. Detta identifierar den specifika instansen av användarbehörighet.
   * Klienthemligheten som genererades när du konfigurerade ClientApp OAuth2-appen i [!DNL Workfront]. Detta gör att [!DNL Workfront] kan veta att begäran kommer från ClientApp.

1. Om auktoriseringskoden och klienthemligheten är korrekta skickar [!DNL Workfront] en åtkomsttoken till ClientApp. Denna åtkomsttoken skickas direkt från [!DNL Workfront] till ClientApp och kan inte visas, kopieras eller användas av andra användar- eller klientprogram.
1. ClientApp skickar åtkomsttoken till [!DNL Workfront] tillsammans med den specifika begäran om information.
1. Eftersom åtkomsttoken är korrekt skickar [!DNL Workfront] informationen till ClientApp.

#### Uppdaterar åtkomsttoken

Av säkerhetsskäl upphör åtkomsttoken att gälla efter en kort tid. [!DNL OAuth2] använder uppdateringstoken för att få nya åtkomsttoken utan att behöva ange autentiseringsuppgifter varje gång. Uppdateringstoken lagras av klienten.

Processen för att hämta en uppdateringstoken är densamma som proceduren som beskrivs i avsnittet [Autentisering med en auktoriseringskod och åtkomsttoken](#authorizing-with-an-authorization-code-and-access-token). Begäran för auktoriseringskoden innehåller scopet `offline_access`, som anger att begäran ska returnera en begärandetoken tillsammans med auktoriseringskoden.

---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: connections-annd-webhooks
title: Anslut [!DNL Adobe Workfront Fusion] till [!DNL Google Services] med uppdaterade säkerhetsåtgärder
description: Google har nyligen infört begränsningar för hur användare kan använda sina API:er. I den här artikeln beskrivs hur du ansluter [!DNL Adobe Workfront Fusion]  till Google, vilket anger dessa säkerhetsmätningar för uppdateringar.
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 0%

---

# Anslut [!DNL Adobe Workfront Fusion] till [!DNL Google Services] med uppdaterade säkerhetsåtgärder

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

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Google Services] begränsningar

[!DNL Google] införde begränsningar för hur användare kan använda sina API:er den 1 juni 2020. Dessa säkerhetsåtgärder skyddar [!DNL Google]-användare från att läsa eller missbruka deras personuppgifter på [!DNL Google]. Begränsningarna är relaterade till programmen [!DNL Gmail] och [!DNL Google Drive]. Mer information om dessa begränsningar finns i&quot;Additional Requirements for Specific API Scopes&quot; i [[!DNL Google] API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

Om du vill få åtkomst till begränsade omfattningar måste den anslutna tjänsten ([!DNL Adobe Workfront Fusion] eller någon annan tjänst som vill få åtkomst till användarens data via API:t) verifieras och ha en bedömningsförklaring som visar att tjänsten är säker och transparent med hur informationen används. [!DNL Workfront Fusion] uppfyller alla [!DNL Google]s krav för åtkomst till begränsade omfattningar. De flesta tjänster som är anslutna till tredje part i [!DNL Workfront Fusion] har dock inte utvärderingsbrevet och uppfyller därför inte villkoren för [!DNL Google]. På grund av detta får [!DNL Workfront Fusion] inte skicka data till dessa tjänster.

## Undantag för [!DNL Google Services]-begränsningar

Det finns några undantag som gör det möjligt att skicka data till en ej godkänd tredjepartstjänst som inte har utvärderingsversionsinformationen utan att bryta mot någon av de nya begränsningarna. De skiljer sig åt beroende på [!DNL Google Workspace] med [!DNL Workfront Fusion] OAuth-klienten, [!DNL Google Workspace] med en annan OAuth-klient, eller [!DNL @gmail.com] och [!DNL @google.mail.com].

* [[!DNL Google Workspace] med [!DNL Workfront Fusion] OAuth-klient](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL Google Workspace] med en annan OAuth-klient](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] och [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL Google Workspace] med [!DNL Workfront Fusion] OAuth-klient

[!DNL Workfront Fusion] använder undantaget [!UICONTROL Domain-wide Installation]. Installation i hela domänen passar för [!DNL Google Workspace] användare och tillåter användare att integrera icke godkända tjänster utan några begränsningar. Om du använder Google Workspace behöver du inte utföra några ytterligare steg och kan ansluta direkt till ej godkända tjänster.

### [!DNL Google Workspace] med en annan OAuth-klient

[!DNL Google Workspace] användare som föredrar att använda sin egen OAuth-klient i stället för att använda [!DNL Workfront Fusion] OAuth-klienten kan ansluta till [!DNL Google Services] via [!UICONTROL Internal] Use-metoden. Det här alternativet är avsett för avancerade användare. Instruktioner finns i [Ansluta [!DNL Adobe Workfront Fusion] till [!DNL Google Services] med en anpassad OAuth-klient](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] och [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

Användare som har åtkomst till [!DNL Google Services] via [!DNL @gmail.com] eller [!DNL @googlemail.com] kan ansluta till [!DNL Google Services] via metoden för personlig användning. Det här alternativet är avsett för avancerade användare. Instruktioner finns i [Ansluta [!DNL Adobe Workfront Fusion] till [!DNL Google Services] med en anpassad OAuth-klient](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## Vanliga frågor

* [Vilka appar i [!DNL Adobe Workfront Fusion] påverkas?](#what-apps-in-adobe-workfront-fusion-are-affected)
* [Har jag ett [!DNL Google Workspace] konto?](#do-i-have-a-g-suite-account)
* [Vad ska jag göra om jag är  [!DNL @gmail.com] eller [!DNL @googlemail.com] användare?](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [Vad ska jag göra om jag är en [!DNL Google Workspace] användare?](#what-should-i-do-if-im-a-g-suite-user)

### Vilka appar i [!DNL Adobe Workfront Fusion] påverkas? {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail] och e-post (ansluten till [!DNL Gmail]-kontot).

### Har jag ett [!DNL Google Workspace]-konto? {#do-i-have-a-g-suite-account}

Om din e-postadress slutar med [!DNL @gmail.com] eller [!DNL @googlemail.com] är ditt konto inte ett [!DNL Google Workspace]-konto. Om ditt [!DNL Google]-konto slutar med en anpassad domän som @my-company.com är det ett [!DNL Google Workspace]-konto.

### Vad ska jag göra om jag är [!DNL @gmail.com]- eller [!DNL @googlemail.com]-användare? {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

Dessa nya begränsningar gäller bara om du integrerar [!DNL Google Drive] eller [!DNL Gmail]. Om du vill ansluta till [!DNL Google Drive] eller [!DNL Gmail] kan du

* Växla till [!DNL Google Workspace]

  eller

* Skapa en anpassad OAuth-klient. Det här alternativet är avsett för avancerade användare.

  Instruktioner finns i [Ansluta [!DNL Adobe Workfront Fusion] till [!DNL Google Services] med en anpassad OAuth-klient](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Om du vill integrera någon annan tjänst än [!DNL Google Drive] eller [!DNL Gmail] gäller inte dessa begränsningar.

Instruktioner om hur du ansluter andra [!DNL Google Services] till [!DNL Workfront Fusion] finns i [Ansluta modulens app- eller webbtjänst till  [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) i artikeln [Skapa ett scenario i  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Vad ska jag göra om jag är [!DNL Google Workspace]-användare? {#what-should-i-do-if-im-a-g-suite-user}

Det finns ingen nödvändig åtgärd.

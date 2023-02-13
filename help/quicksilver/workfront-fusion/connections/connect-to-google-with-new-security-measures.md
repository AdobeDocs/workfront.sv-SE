---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: connections-annd-webhooks
title: Anslut [!DNL Adobe Workfront Fusion] till [!DNL Google Services] med uppdaterade säkerhetsåtgärder
description: Google har nyligen infört begränsningar för hur användare kan använda sina API:er. I den här artikeln beskrivs hur du ansluter [!DNL Adobe Workfront Fusion] till Google, som ansvarar för dessa säkerhetsåtgärder.
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '611'
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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Google Services] begränsningar

[!DNL Google] infördes restriktioner för hur användare kan använda sina API:er från och med den 1 juni 2020. Dessa säkerhetsåtgärder skyddar [!DNL Google] användare från att ha läckt eller missbrukat sina personuppgifter på [!DNL Google]. Begränsningarna är relaterade till [!DNL Gmail] och [!DNL Google Drive] appar. Mer information om dessa begränsningar finns i&quot;Ytterligare krav för specifika API-scope&quot; i [[!DNL Google] Användardataprincip för API Services](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

Ansluten tjänst ([!DNL Adobe Workfront Fusion] eller någon annan tjänst som vill få åtkomst till användarens data via API:t) måste verifieras och ha en bedömningsförklaring som visar att tjänsten är säker och öppen om hur informationen används. [!DNL Workfront Fusion] uppfyller alla [!DNL Google]&#39;s requirements for access to restricted scopes. De flesta tjänster från tredje part som är anslutna inom [!DNL Workfront Fusion] inte har bedömningsbrevet och därför inte uppfyller [!DNL Google] villkor. På grund av det, [!DNL Workfront Fusion] får inte skicka data till dessa tjänster.

## Undantag för [!DNL Google Services] begränsningar

Det finns några undantag som gör det möjligt att skicka data till en ej godkänd tredjepartstjänst som inte har utvärderingsversionsinformationen utan att bryta mot någon av de nya begränsningarna. De skiljer sig åt beroende på [!DNL G Suite] med [!DNL Workfront Fusion] OAuth-klient, [!DNL G Suite] med en annan OAuth-klient, eller [!DNL @gmail.com] och [!DNL @google.mail.com].

* [[!DNL G suite] med [!DNL Workfront Fusion] OAuth-klient](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL G suite] med en annan OAuth-klient](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] och [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL G suite] med [!DNL Workfront Fusion] OAuth-klient

[!DNL Workfront Fusion] använder [!UICONTROL Domain-wide Installation] undantag. Installation i hela domänen är lämplig för [!DNL G Suite] -användare och tillåter användare att integrera icke godkända tjänster utan begränsningar. Om du är G Suite-användare behöver du inte utföra några ytterligare steg och kan ansluta direkt till tjänster som inte godkänts.

### [!DNL G suite] med en annan OAuth-klient

[!DNL G Suite] användare som föredrar att använda sin egen OAuth-klient i stället för att använda [!DNL Workfront Fusion] OAuth-klient kan ansluta till [!DNL Google Services] via [!UICONTROL Internal] Använd metod. Det här alternativet är avsett för avancerade användare. Instruktioner finns i [Anslut [!DNL Adobe Workfront Fusion] till [!DNL Google Services] med en anpassad OAuth-klient](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] och [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

Användare som har åtkomst [!DNL Google Services] via [!DNL @gmail.com] eller [!DNL @googlemail.com] kan ansluta till [!DNL Google Services] genom strategin för personlig användning. Det här alternativet är avsett för avancerade användare. Instruktioner finns i [Anslut [!DNL Adobe Workfront Fusion] till [!DNL Google Services] med en anpassad OAuth-klient](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## Vanliga frågor

* [Vilka program i [!DNL Adobe Workfront Fusion] påverkas?](#what-apps-in-adobe-workfront-fusion-are-affected)
* [Har jag ett [!DNL G Suite]-konto?](#do-i-have-a-g-suite-account)
* [Vad ska jag göra om jag är [!DNL @gmail.com] eller [!DNL @googlemail.com] användare?](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [Vad ska jag göra om jag är en [!DNL G Suite]-användare?](#what-should-i-do-if-im-a-g-suite-user)

### Vilka program i [!DNL Adobe Workfront Fusion] påverkas? {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail]och e-post (kopplad till [!DNL Gmail] konto).

### Har jag en [!DNL G Suite] konto? {#do-i-have-a-g-suite-account}

Om din e-postadress slutar med [!DNL @gmail.com] eller [!DNL @googlemail.com] ditt konto är inte en [!DNL G Suite] konto. Om [!DNL Google] kontot avslutas med en anpassad domän som @my-company.com, då är det en [!DNL G Suite] konto.

### Vad ska jag göra om jag är [!DNL @gmail.com] eller [!DNL @googlemail.com] användare? {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

Dessa nya begränsningar gäller endast om du integrerar [!DNL Google Drive] eller [!DNL Gmail]. Om du vill ansluta till [!DNL Google Drive] eller [!DNL Gmail]kan du

* Växla till [!DNL G Suite]

   eller

* Skapa en anpassad OAuth-klient. Det här alternativet är avsett för avancerade användare.

   Instruktioner finns i [Anslut [!DNL Adobe Workfront Fusion] till [!DNL Google Services] med en anpassad OAuth-klient](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Om du vill integrera någon annan tjänst än [!DNL Google Drive] eller [!DNL Gmail], gäller dessa begränsningar inte.

Instruktioner om hur du ansluter andra [!DNL Google Services] till [!DNL Workfront Fusion], se [Anslut modulens app eller webbtjänst till [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) i artikeln [Skapa ett scenario i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Vad ska jag göra om jag är en [!DNL G Suite] användare? {#what-should-i-do-if-im-a-g-suite-user}

Det finns ingen nödvändig åtgärd.

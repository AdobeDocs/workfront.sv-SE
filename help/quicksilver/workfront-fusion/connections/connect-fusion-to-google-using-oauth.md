---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Anslut [!DNL Adobe Workfront Fusion] till [!DNL Google Services] med en anpassad OAuth-klient
description: Du kan använda [!DNL Adobe Workfront Fusion] för att ansluta till [!DNL Google Services] med en anpassad OAuth-klient. Den här proceduren kräver en befintlig [!DNL Google] konto.
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 0%

---

# Anslut [!DNL Adobe Workfront Fusion] till [!DNL Google Services] med en anpassad OAuth-klient

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

## Förutsättningar

Du behöver en befintlig [!DNL Google] för att skapa anslutningen.

## Skapa ett projekt på [!DNL Google Cloud Platform]

Följande förfarande är avsett för:

* Personlig användning ([!DNL @gmail.com] och [!DNL @googlemail.com] användare)
* Intern användning ([!DNL G Suite] användare som föredrar att använda en anpassad OAuth-klient)

Skapa ett projekt på [!DNL Google Cloud] Plattform:

1. Logga in på [[!DNL Google Cloud] Plattform](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) med [!DNL Google] autentiseringsuppgifter.
1. Klicka på i den vänstra panelen **[!UICONTROL Dashboard]**.
1. Klicka **[!UICONTROL Create project]** i skärmens övre högra hörn.
1. Ange **[!UICONTROL Project name]** och sedan klicka **[!UICONTROL Create]**.

1. Klicka på **[!UICONTROL Enable APIs and services]** -fliken i skärmens övre kant.
1. I **[!UICONTROL Search for APIs and Services]** fältet längst upp på skärmen skriver du namnet på den tjänst som du vill använda (till exempel [!DNL Gmail] API eller [!DNL Google Drive] API).
1. När den visas klickar du på den API eller tjänst som du vill ansluta till [!DNL Workfront Fusion].
1. Klicka **[!UICONTROL Enable]** för att aktivera det valda API:t.
1. Upprepa steg 6-8 för varje API som du vill aktivera.

   >[!NOTE]
   >
   >Du måste aktivera [!DNL Google Drive] API och API för alla [!DNL Google] appar som du vill använda (till exempel [!DNL Google Sheets] API).

1. På skärmen som visas klickar du på **[!UICONTROL Create credentials]** i det övre högra hörnet.
1. Fortsätt till avsnittet [Konfigurera inställningar för OAuth-medgivande](#configure-oauth-consent-settings) i den här artikeln.

## Konfigurera [!UICONTROL OAuth consent] inställningar

1. Klicka på i den vänstra panelen **[!UICONTROL OAuth consent screen]**.
1. Välj **[!UICONTROL External]** och sedan klicka **[!UICONTROL Create]**.

   >[!NOTE]
   >
   >Du debiteras inte när du väljer det här alternativet. Mer information finns i [!DNL Google]Information om undantag från verifieringskraven.

1. Fyll i de obligatoriska fälten enligt följande:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App name]</p> </td> 
      <td> <p>Ange namnet på den app som begär samtycke.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span>[!DNL Adobe Workfront Fusion] </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL User support email]</td> 
      <td>Ange en e-postadress dit användare kan kontakta dig med frågor om deras samtycke när de ansluter till den här appen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Email addresses]</td> 
      <td>Ange en eller flera e-postadresser som Google kan använda för att meddela dig om ändringar i projektet.</td> 
     </tr> 
    </tbody> 
   </table>

1. Under [!UICONTROL Authorized domains], klicka **[!UICONTROL Add domain]** och ange `workfrontfusion.com`.

1. Klicka på **[!UICONTROL Save and continue]**.
1. Klicka på **[!UICONTROL Add or remove scopes]**.
1. Aktivera följande scope i den högra panelen:

<table style="table-layout:auto">
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Service/API</th> 
      <th>Obligatoriska omfattningar</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p>[!DNL Gmail]</p> </td> 
      <td> <p>https://mail.google.com/</p> <p>https://www.googleapis.com/auth/gmail.labels</p> <p>https://www.googleapis.com/auth/gmail.send</p> <p>https://www.googleapis.com/auth/gmail.readonly</p> <p>https://www.googleapis.com/auth/gmail.compose</p> <p>https://www.googleapis.com/auth/gmail.insert</p> <p>https://www.googleapis.com/auth/gmail.modify</p> <p>https://www.googleapis.com/auth/gmail.metadata</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!DNL Google Drive]</p> </td> 
      <td> <p>https://www.googleapis.com/auth/drive</p> <p>https://www.googleapis.com/auth/drive.readonly</p> </td> 
     </tr> 
    </tbody> 
   </table>

Du kan behöva utöka listan eller gå till nästa sida i listan för att se alla.

1. Klicka på **[!UICONTROL Update]**.
1. Klicka på **[!UICONTROL Save and continue]**.
1. (Valfritt) Lägg till testanvändare i projektet.
1. Klicka på **[!UICONTROL Save and continue]**.
1. Granska informationen och klicka sedan **[!UICONTROL Back to dashboard]**.

   >[!NOTE]
   >
   >Du behöver inte skicka in ditt samtycke-skärm och din ansökan för verifiering via [!DNL Google].

1. Fortsätt till [Skapa OAuth-autentiseringsuppgifter](#create-oauth-credentials).

## Skapa OAuth-autentiseringsuppgifter

1. Klicka på i den vänstra panelen **[!UICONTROL Credentials]**.

   >[!NOTE]
   >
   >Om detta inte är det första API:t eller tjänsten ([!DNL Gmail] eller [!DNL Google Drive]) som du har aktiverat behöver du inte skapa nya autentiseringsuppgifter.

1. Klicka **[!UICONTROL Create credentials]** nära skärmens övre del och välj **[!UICONTROL OAuth client ID]** i listrutan.

1. Fyll i de obligatoriska fälten enligt följande:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Application type]</td> 
      <td> <p> [!UICONTROL Web application]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>[!DNL Workfront Fusion] </td> 
     </tr> 
    </tbody> 
   </table>

1. Under [!UICONTROL Authorized redirect URIs], klicka **[!UICONTROL Add URI]** och ange **en** av följande:

   * För [!DNL Gmail] eller [!DNL Google Drive]: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * För andra [!DNL Google] appar: `https://app.workfrontfusion.com/oauth/cb/google`

1. Klicka på **[!UICONTROL Create]**.

   The [!UICONTROL Client ID] och [!UICONTROL Client Secret] visning.

1. Kopiera [!UICONTROL Client ID] och [!UICONTROL Client Secret] till en säker plats. Du använder dem för att skapa en anslutning i [!DNL Workfront Fusion].
1. Fortsätt till [Anslut till [!DNL Google] in [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

## Anslut till [!DNL Google] in [!DNL Workfront Fusion]

Processen att skapa en anslutning till [!DNL Google] varierar beroende på om du använder en modul eller en [!DNL Google] tjänst (som [!DNL Google Sheets] eller [!DNL Google Docs]), eller om du ansluter till [!DNL Google] via [!UICONTROL HTTP] >[!UICONTROL Make an OAuth2.0] begärandemodul.

* [Anslut till [!DNL Google] i en [!DNL Google] service](#connect-to-google-in-a-google-service)
* [Anslut till [!DNL Google] i [!UICONTROL HTTP] > [!UICONTROL Make an OAuth2.0 request] modul](#connect-to-google-in-the-http--make-an-oauth20-request-module)

### Anslut till [!DNL Google] i en [!DNL Google] service

1. I [!DNL Workfront Fusion], leta upp [!DNL Google] som du behöver skapa en anslutning för.
1. Klicka **[!UICONTROL Create a connection]** och sedan klicka **[!UICONTROL Show advanced settings]**.

1. Ange [!UICONTROL Client ID] och [!UICONTROL Client Secret] du hämtade i [[!UICONTROL Create OAuth Credentials]](#create-oauth-credentials) i respektive fält och klicka sedan på **[!UICONTROL Continue]**.

1. Logga in med [!DNL Google] konto.

   The **[!UICONTROL This app isn't verified]** visas. Observera att &quot;app&quot; som omnämns i fönstertiteln är OAuth-klienten som du skapade ovan.

1. Klicka **[!UICONTROL Advanced]** och sedan klicka **[!UICONTROL Go to [!DNL Workfront Fusion] (unsafe)]** för att tillåta åtkomst med din anpassade OAuth-klient.

1. Klicka **[!UICONTROL Allow]** att bevilja [!DNL Workfront Fusion] behörighet.
1. Klicka på **[!UICONTROL Allow]** igen för att bekräfta dina val.

   Anslutningen till önskat [!DNL Google] en anpassad OAuth-klient har upprättats.

### Anslut till [!DNL Google] i [!UICONTROL HTTP] > [!UICONTROL Make an OAuth2.0 request] modul {#connect-to-google-in-the-http--make-an-oauth20-request-module}

Anvisningar om hur du ansluter till [!DNL Google] i [!UICONTROL HTTP] > [!UICONTROL Make an OAuth2.0 request] modul, se [Instruktioner för att skapa en anslutning till [!DNL Google] i [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] modul](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instruct) in [[!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] modul](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## Möjligt felmeddelande:[!UICONTROL [403] Access Not Configured]

Om [!UICONTROL [403] Access Not Configured] felmeddelandet visas måste du aktivera motsvarande API i din Google Cloud-plattform. Följ stegen i avsnittet för att aktivera API:t [Skapa ett projekt på [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) i den här artikeln.

---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Anslut [!DNL Adobe Workfront Fusion] till [!DNL Google Services] med en anpassad OAuth-klient
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 0%

---

# Anslut [!DNL Adobe Workfront Fusion] till [!DNL Google Services] med en anpassad OAuth-klient

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [Anslut Adobe Workfront Fusion till Google Services med en anpassad OAuth-klient](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/connect-fusion-to-google-using-oauth.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td> <p>Nytt: [!UICONTROL Standard]</p><p>eller</p><p>Aktuell: [!UICONTROL Work] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licens**</td> 
   <td>
   <p>Aktuell: Inga [!DNL Workfront Fusion]-licenskrav.</p>
   <p>eller</p>
   <p>Äldre: Alla </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Nytt:</p> <ul><li>[!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Workfront] Plan: Din organisation måste köpa [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Planen [!DNL Workfront Fusion] ingår.</li></ul>
   <p>eller</p>
   <p>Aktuell: Din organisation måste köpa [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Förutsättningar

Du behöver ett befintligt [!DNL Google]-konto för att kunna ansluta.

## Anslut Fusion till Google-tjänster med en anpassad OAuth-klient

Om du vill skapa den här anslutningen måste du skapa och konfigurera ett projekt på Google Cloud-plattformen och sedan konfigurera anslutningen i Fusion baserat på det projektet.

* [Skapa ett projekt på  [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform)
* [Konfigurera [!UICONTROL OAuth consent] inställningar](#configure-oauth-consent-settings)
* [Skapa OAuth-autentiseringsuppgifter](#create-oauth-credentials)
* [Anslut till [!DNL Google] i [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion)

>[!NOTE]
>
>Detta förfarande är avsett för
>
>* Personlig användning ([!DNL `@gmail.com`] och [!DNL `@googlemail.com`] användare)
>* Intern användning ([!DNL Google Workspace] användare som föredrar att använda en anpassad OAuth-klient)

### Skapa ett projekt på [!DNL Google Cloud Platform]

Så här skapar du ett projekt på [!DNL Google Cloud]-plattformen:

1. Logga in på [[!DNL Google Cloud] Platform](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) med dina [!DNL Google]-inloggningsuppgifter.
1. Klicka på **[!UICONTROL Dashboard]** i den vänstra panelen.
1. Klicka på **[!UICONTROL Create project]** i skärmens övre högra hörn.
1. Ange **[!UICONTROL Project name]** och klicka sedan på **[!UICONTROL Create]**.

1. Klicka på fliken **[!UICONTROL Enable APIs and services]** i skärmens övre del.
1. I fältet **[!UICONTROL Search for APIs and Services]** högst upp på skärmen skriver du namnet på den tjänst som du vill använda (till exempel [!DNL Gmail] API eller [!DNL Google Drive] API).
1. När den visas klickar du på API:t eller tjänsten som du vill ansluta till [!DNL Workfront Fusion].
1. Klicka på **[!UICONTROL Enable]** om du vill aktivera det valda API:t.
1. Upprepa steg 6-8 för varje API som du vill aktivera.

   >[!NOTE]
   >
   >Du måste aktivera [!DNL Google Drive]-API:t samt API:t för alla [!DNL Google]-program som du vill använda (till exempel [!DNL Google Sheets]-API:t).

1. Klicka på **[!UICONTROL Create credentials]** i det övre högra hörnet på skärmen som visas.
1. Fortsätt till avsnittet [Konfigurera inställningar för OAuth-medgivande](#configure-oauth-consent-settings) i den här artikeln.

### Konfigurera inställningar för [!UICONTROL OAuth consent]

1. Klicka på **[!UICONTROL OAuth consent screen]** i den vänstra panelen.
1. Välj **[!UICONTROL External]** och klicka sedan på **[!UICONTROL Create]**.

   >[!NOTE]
   >
   >Du debiteras inte när du väljer det här alternativet. Mer information finns i informationen om undantag från verifieringskraven för [!DNL Google].

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

1. Klicka **[!UICONTROL Add domain]** under [!UICONTROL Authorized domains] och ange `workfrontfusion.com`.

1. Klicka på **[!UICONTROL Save and continue]**.
1. Klicka på **[!UICONTROL Add or remove scopes]**.
1. Aktivera följande omfång i den högra panelen:

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
1. Granska informationen och klicka sedan på **[!UICONTROL Back to dashboard]**.

   >[!NOTE]
   >
   >Du behöver inte skicka in ditt godkännande-skärmen och din ansökan för verifiering av [!DNL Google].

1. Fortsätt till [Skapa OAuth-autentiseringsuppgifter](#create-oauth-credentials).

### Skapa OAuth-autentiseringsuppgifter

1. Klicka på **[!UICONTROL Credentials]** i den vänstra panelen.

   >[!NOTE]
   >
   >Om detta inte är det första API:t eller tjänsten ([!DNL Gmail] eller [!DNL Google Drive]) som du har aktiverat behöver du inte skapa nya autentiseringsuppgifter.

1. Klicka på **[!UICONTROL Create credentials]** uppe på skärmen och välj sedan **[!UICONTROL OAuth client ID]** i listrutan.

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

1. Klicka på **[!UICONTROL Add URI]** under [!UICONTROL Authorized redirect URIs] och ange **ett** av följande:

   * För [!DNL Gmail] eller [!DNL Google Drive]: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * För andra [!DNL Google]-appar: `https://app.workfrontfusion.com/oauth/cb/google`

1. Klicka på **[!UICONTROL Create]**.

   Visningen [!UICONTROL Client ID] och [!UICONTROL Client Secret].

1. Kopiera [!UICONTROL Client ID] och [!UICONTROL Client Secret] till en säker plats. Du använder dem för att skapa en anslutning i [!DNL Workfront Fusion].
1. Fortsätt till [Anslut till [!DNL Google] in [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

### Anslut till [!DNL Google] i [!DNL Workfront Fusion]

Processen med att skapa en anslutning till [!DNL Google] varierar beroende på om du använder en modul från en [!DNL Google]-tjänst (till exempel [!DNL Google Sheets] eller [!DNL Google Docs]) eller om du ansluter till [!DNL Google] via [!UICONTROL HTTP] >[!UICONTROL Make an OAuth2.0]-begärandemodulen.

* [Anslut till [!DNL Google] i en [!DNL Google] tjänst](#connect-to-google-in-a-google-service)
* [Anslut till  [!DNL Google]  i modulen [!UICONTROL HTTP] > [!UICONTROL Make an OAuth2.0 request]](#connect-to-google-in-the-http--make-an-oauth20-request-module)

#### Anslut till [!DNL Google] i en [!DNL Google]-tjänst

1. I [!DNL Workfront Fusion] letar du reda på modulen [!DNL Google] som du behöver skapa en anslutning för.
1. Klicka på **[!UICONTROL Create a connection]** och sedan på **[!UICONTROL Show advanced settings]**.

1. Ange [!UICONTROL Client ID] och [!UICONTROL Client Secret] du hämtade i [[!UICONTROL Create OAuth Credentials]](#create-oauth-credentials) i respektive fält och klicka sedan på **[!UICONTROL Continue]**.

1. Logga in med ditt [!DNL Google]-konto.

   Fönstret **[!UICONTROL This app isn't verified]** visas. Observera att &quot;app&quot; som omnämns i fönstertiteln är OAuth-klienten som du skapade ovan.

1. Klicka på **[!UICONTROL Advanced]** och sedan på **[!UICONTROL Go to [!DNL Workfront Fusion] (unsafe)]** för att tillåta åtkomst med din anpassade OAuth-klient.

1. Klicka på **[!UICONTROL Allow]** om du vill bevilja [!DNL Workfront Fusion] behörighet.
1. I fönstret som visas klickar du på **[!UICONTROL Allow]** igen för att bekräfta dina val.

   Anslutningen till den önskade [!DNL Google]-tjänsten med en anpassad OAuth-klient har upprättats.

#### Anslut till [!DNL Google] i modulen [!UICONTROL HTTP] > [!UICONTROL Make an OAuth2.0 request] {#connect-to-google-in-the-http--make-an-oauth20-request-module}

Instruktioner om hur du ansluter till [!DNL Google] i modulen [!UICONTROL HTTP] > [!UICONTROL Make an OAuth2.0 request] finns i [Instruktioner för hur du skapar en anslutning till  [!DNL Google]  i modulen [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] ](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module) i [[!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] module](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## Möjligt felmeddelande:[!UICONTROL [403] Access Not Configured]

Om felmeddelandet [!UICONTROL `403 Access Not Configured`] visas måste du aktivera motsvarande API i din Google Cloud-plattform. Om du vill aktivera API:t följer du stegen i avsnittet [Skapa ett projekt på [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) i den här artikeln.

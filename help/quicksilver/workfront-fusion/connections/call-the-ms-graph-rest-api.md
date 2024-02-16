---
title: Anropa MS Graph REST API via [!DNL Adobe Workfront Fusion] HTTP &gt; Gör en OAuth 2.0-begärandemodul
description: Anropa MS Graph REST API via [!DNL Adobe Workfront Fusion] HTTP &gt; Gör en OAuth 2.0-begärandemodul
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 1%

---

# Ring[!UICONTROL  MS Graph REST API] via [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] modul

Många [!DNL Microsoft] webbtjänster nås via [!DNL Microsoft Graph API]. I den här artikeln beskrivs hur du skapar en anslutning till det API:t med hjälp av [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL Make an OAuth 2.0 request] -modul.

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
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p>
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

## Registrera [!DNL Workfront Fusion] i [!DNL Microsoft Application Registration Portal]

Skapa en anslutning till [!DNL Microsoft Graph REST API]måste du först registrera dig [!DNL Adobe Workfront Fusion].

1. Börja registrera ett nytt program enligt beskrivningen i [Registrera din app](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) i [!DNL Microsoft] dokumentation.

   Som en del av registreringen [!DNL Microsoft] kräver följande information:

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Application name]</td>
        <td>Ange ett namn för programmet, till exempel "Min [!DNL Workfront Fusion] program."</td>
      </tr>
      <tr>
        <td>[!UICONTROL Redirect URL]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. När du är klar med registreringen av appen bör du notera [!UICONTROL Application ID].

   >[!IMPORTANT]
   >
   >Du måste ange program-ID:t för att kunna konfigurera anslutningen i [!DNL Workfront Fusion].

1. Generera en [!UICONTROL Application Secret]. Notera denna hemlighet.

   Instruktioner finns i [Registrera din app](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) i [!DNL Microsoft] dokumentation.

   >[!IMPORTANT]
   >
   >Du behöver [!UICONTROL Application Secret] för att konfigurera anslutningen i [!DNL Workfront Fusion].

1. Konfigurera behörigheter för ditt program.

   Mer information om hur du hittar och konfigurerar dessa fält finns i avsnittet&quot;Konfigurera behörigheter för Microsoft Graph&quot; i [Få åtkomst utan användare](https://docs.microsoft.com/en-us/graph/auth-v2-service) i [!UICONTROL Microsoft] dokumentation.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL What type of permissions does your application require?]</td> 
      <td>Välj <code>[!UICONTROL Delegated permissions]</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Select permissions]</td> 
      <td> <p>Välj följande behörigheter:</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>Andra behörigheter som krävs för integreringen (Exempel: <code>User.Read</code>)</p> </li> 
       </ul> <p>Viktigt: Du behöver de valda behörigheterna för att konfigurera anslutningen i [!DNL Workfront Fusion].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fortsätt till [Konfigurera [!DNL MS Graph API] anslutning till [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion).

## Konfigurera [!DNL MS Graph API] anslutning till [!DNL Workfront Fusion]

Efter registreringen [!DNL Workfront Fusion] som beskrivs i [Registrera [!DNL Workfront Fusion] i [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal)kan du konfigurera anslutningen i [!UICONTROL HTTP] >[!UICONTROL Make an Oauth 2.0] begärandemodul.

1. Lägg till en [!UICONTROL HTTP] >[!UICONTROL Make an OAuth 2.0 call] till ditt scenario.
1. Klicka **[!UICONTROL Add]** bredvid [!UICONTROL connection] fält.
1. Konfigurera anslutningsfälten enligt följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection name]</td> 
      <td>Ange ett namn för anslutningen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Flow type]</p> </td> 
      <td><code>[!UICONTROL Authorization Code]</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authorize URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/authorize</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope]</td> 
      <td> <p>Ange de behörigheter som du valde i steg 4 av <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registrera [!DNL Workfront Fusion] i [!DNL Microsoft Application Registration Portal]</a>.</p> <p>För varje omfång klickar du på <b>[!UICONTROL Add]</b> och skriv in behörigheten.</p> <p>Exempel: <code>offline_access</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope separator]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td>Ange [!UICONTROL Application ID] från steg 2 in <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registrera [!DNL Workfront Fusion] i [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td>Ange [!UICONTROL Application Secret] som du skapade i steg 2 i <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registrera [!DNL Workfront Fusion] i [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authorize parameters]</td> 
      <td> <p>Lägg till följande Authorize-parametrar:</p> 
       <ul> 
        <li> <p>[!UICONTROL Key]:<code> response_mode</code> [!UICONTROL Value]: <code>query</code></p> </li> 
        <li> <p>[!UICONTROL Key]: <code>prompt </code>[!UICONTROL Value]: <code>consent</code></p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Access token parameters]</td> 
      <td>Du behöver inte ange något i det här fältet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Refresh token parameters]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Klicka på <b>[!UICONTROL Add]</b>.</p> </li> 
        <li value="2"> <p>I <b>[!UICONTROL Key]</b> fält, ange <code>scope</code>.</p> </li> 
        <li value="3"> <p>I <b>[!UICONTROL Value]</b> fält, ange alla [!UICONTROL scope]som du har angett i omfångsfältet, avgränsade med blanksteg.</p> <p>Exempel: <code>offline_access openid User.Read</code></p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Custom Headers]</td> 
      <td>Du behöver inte ange något i det här fältet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token Placement]</td> 
      <td><code>[!UICONTROL In the header]</code> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **[!UICONTROL Continue]**.
1. Klicka på **[!UICONTROL Accept]** för att slutföra anslutningen och återgå till modulen.

---
title: Anropa MS Graph REST API via  [!DNL Adobe Workfront Fusion] HTTP &gt; Gör en OAuth 2.0-begärandemodul
description: Anropa MS Graph REST API via  [!DNL Adobe Workfront Fusion] HTTP &gt; Gör en OAuth 2.0-begärandemodul
author: Becky
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 1%

---

# Anropa [!UICONTROL  MS Graph REST API] via modulen [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request]

<!-- Audited: 3/2024-->

Många [!DNL Microsoft]-webbtjänster nås via [!DNL Microsoft Graph API]. Du kan skapa en anslutning till [!DNL Microsoft Graph API] genom att använda modulen [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL Make an OAuth 2.0 request].

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

## Registrera [!DNL Workfront Fusion] i [!DNL Microsoft Application Registration Portal]

Om du vill skapa en anslutning till [!DNL Microsoft Graph REST API] måste du först registrera [!DNL Adobe Workfront Fusion].

1. Börja registrera ett nytt program enligt beskrivningen i [Registrera ditt program](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) i [!DNL Microsoft]-dokumentationen.

   Som en del av registreringen kräver [!DNL Microsoft] följande information:

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Application name]</td>
        <td>Ange ett namn för programmet, till exempel "Mitt [!DNL Workfront Fusion]-program".</td>
      </tr>
      <tr>
        <td>[!UICONTROL Redirect URL]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. Observera [!UICONTROL Application ID] när du har slutfört appregistreringen.

   >[!IMPORTANT]
   >
   >Du måste ha ett program-ID för att kunna konfigurera anslutningen i [!DNL Workfront Fusion].

1. Generera en [!UICONTROL Application Secret]. Notera denna hemlighet.

   Instruktioner finns i [Registrera din app](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) i [!DNL Microsoft]-dokumentationen.

   >[!IMPORTANT]
   >
   >Du behöver [!UICONTROL Application Secret] för att konfigurera anslutningen i [!DNL Workfront Fusion].

1. Konfigurera behörigheter för ditt program.

   Mer information om hur du hittar och konfigurerar dessa fält finns i avsnittet Konfigurera behörigheter för Microsoft Graph i [Få åtkomst utan användare](https://docs.microsoft.com/en-us/graph/auth-v2-service) i [!UICONTROL Microsoft]-dokumentationen.

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
        <li> <p>Andra behörigheter som krävs för integreringarna (Exempel: <code>User.Read</code>)</p> </li> 
       </ul> <p><b>Viktigt</b>: Du behöver de valda behörigheterna för att konfigurera anslutningen i [!DNL Workfront Fusion].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fortsätt till [Konfigurera din [!DNL MS Graph API] anslutning i [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion).

## Konfigurera din [!DNL MS Graph API]-anslutning i [!DNL Workfront Fusion]

När du har registrerat [!DNL Workfront Fusion] enligt beskrivningen i [Register [!DNL Workfront Fusion]  i  [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal) kan du konfigurera anslutningen i [!UICONTROL HTTP] > [!UICONTROL Make an Oauth 2.0]-begärandemodulen.

1. Lägg till en [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 call]-modul i ditt scenario.
1. Klicka på **[!UICONTROL Add]** bredvid fältet [!UICONTROL connection].
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
      <td> <p>Ange de behörigheter som du valde i steg 4 av <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registrera [!DNL Workfront Fusion] i [!DNL Microsoft Application Registration Portal]</a>.</p> <p>Klicka på <b>[!UICONTROL Add]</b> för varje scope och ange behörigheten.</p> <p>Exempel: <code>offline_access</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope separator]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td>Ange [!UICONTROL Application ID] från steg 2 i <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registrera [!DNL Workfront Fusion] i [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td>Ange [!UICONTROL Application Secret] som du skapade i steg 3 i <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref"> Registrera [!DNL Workfront Fusion] i [!DNL Microsoft Application Registration Portal]</a>.</td> 
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
        <li value="2"> <p>Ange <code>scope</code> i fältet <b>[!UICONTROL Key]</b>.</p> </li> 
        <li value="3"> <p>I fältet <b>[!UICONTROL Value]</b> anger du alla [!UICONTROL scope] som du har angett i omfångsfältet, avgränsade med blanksteg.</p> <p>Exempel: <code>offline_access openid User.Read</code></p> </li> 
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
1. Klicka på **[!UICONTROL Accept]** i det fönster som visas för att slutföra anslutningen och återgå till modulen.

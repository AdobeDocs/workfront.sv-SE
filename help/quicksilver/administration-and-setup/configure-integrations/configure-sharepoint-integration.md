---
title: Konfigurera [!DNL SharePoint] integration
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Ni kan integrera [!DNL Workfront] med [!DNL SharePoint] online, ger användarna möjlighet att navigera till, länka och lägga till [!DNL SharePoint] dokument i Workfront. Den angivna funktionaliteten liknar den för andra [!DNL Workfront] dokumentintegreringar.
author: Becky
feature: System Setup and Administration, [!DNL Workfront] Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: b090983de417cf6a4dd36c9398da7dcc0296766a
workflow-type: tm+mt
source-wordcount: '1551'
ht-degree: 0%

---

# Konfigurera [!DNL SharePoint] integration

<!--Audited: 12/2023-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>Den nya [!DNL SharePoint] integreringen släpptes till produktion med version 22.3 (juli 2022.) Även om dina användare fortfarande kan komma åt dokument som är länkade via äldre versioner [!DNL SharePoint] måste de använda den nya [!DNL SharePoint] integrering för att länka dokument från SharePoint.
>
>* Den nya SharePoint-integreringen kräver ingen konfiguration av en administratör och kan konfigureras av enskilda användare. För att övergången till den nya SharePoint-integreringen ska bli så smidig som möjligt måste Workfront-administratören göra några smärre ändringar i Workfront Setup-området.
>
>    Mer information och instruktioner finns i [Konfigurera den gamla SharePoint-integreringen för fortsatt åtkomst till dokument](#configure-the-legacy-sharepoint-integration-for-continued-access-to-documents) i den här artikeln.
>    
>* Vi rekommenderar användare att länka dokument som för närvarande är länkade via äldre [!DNL SharePoint] integrering genom den nya integreringen.
>    
>    Instruktioner om hur du länkar dokument finns i [Länka dokument från externa program](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Ni kan integrera [!DNL Workfront] med [!DNL SharePoint Online], ger användarna möjlighet att navigera till, länka och lägga till [!DNL SharePoint] dokument i Workfront. Den angivna funktionaliteten liknar den för andra [!DNL Workfront] integreringar, som [!DNL Google Drive], [!DNL Box]och [!DNL Dropbox].

Den här integreringen är endast kompatibel med [!DNL SharePoint Online]. Lokala instanser av [!DNL SharePoint] stöds inte.

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td>Nytt: Standard <p>eller</p><p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td>Du måste vara en [!DNL Workfront] administratör. För information om [!DNL Workfront] administratörer, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>. </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta din [!DNL Workfront] administratör.

## Förutsättningar

Du måste ha nödvändig åtkomst eller behörighet i [!DNL SharePoint] för att ändra eller konfigurera [!DNL SharePoint] integrering.

## Länka dokument via den nya SharePoint-integreringen

Enskilda användare kan länka dokument via de nya [!DNL SharePoint] integrering. Integreringen kräver ingen administratörskonfiguration. I stället loggar användaren in på sina [!DNL Microsoft] när du länkar ett dokument, vilket gör att integreringen kan komma åt dokument som finns i användarens [!DNL SharePoint].

Första gången en användare ansluter [!DNL Workfront] [!DNL SharePoint] integrering med [!DNL SharePoint] kommer de att se och godkänna alla behörigheter som [!DNL Workfront] använder när de interagerar med [!UICONTROL SharePoint] konto. Läsbehörigheter tillåt [!DNL Workfront] för att se och komma åt filer på [!DNL SharePoint]och skrivbehörigheter tillåter användaren att överföra filer till [!DNL SharePoint].

![SharePoint-behörigheter](assets/sharepoint-permissions.png)

Instruktioner om hur du länkar dokument genom det nya [!DNL SharePoint] integrering, se [Länka ett externt dokument till [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* A [!DNL SharePoint] kan ansluta till en enda [!DNL SharePoint] -instans. Därför kan en användare konfigurera en integrering för en [!DNL SharePoint], men kan inte konfigurera en integrering till en sekund [!DNL SharePoint], även om de har behörighet till och dokument på den andra [!DNL SharePoint].
>
>* En användare har åtkomst till samma platser, samlingar, mappar, undermappar och filer via [!DNL Workfront] [!DNL SharePoint] som de har i sina [!DNL SharePoint] konto.

### Länka dokument från SharePoint

Anvisningar om hur du länkar dokument från SharePoint via nya [!DNL SharePoint] integrering, se [Länka ett externt dokument till [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront).

### Skicka dokument till SharePoint

Skicka ett dokument till SharePoint:

1. Klicka på **Skicka till** icon ![Skicka till](assets/send-to-icon.png) och väljer SharePoint (Graph API).
1. (Valfritt) Sök i sökfältet efter platsen eller mappen dit du vill skicka dokumentet.
1. Markera platsen eller mappen i listan.

   * Platserna är markerade med ![Ikon för webbplats](assets/site-icon.png).

   * Mappar är markerade med ![Mappikon](assets/folder-icon.png).

   * Filerna är inte markerade med en ikon.

1. Klicka **Spara**.


## Säkerhets-, åtkomst- och auktoriseringsinformation för [!DNL SharePoint] integration

### Autentisering och auktorisering

[!DNL Workfront] använder OAuth2 för att hämta en åtkomsttoken och en uppdateringstoken. Denna åtkomsttoken används för auktorisering med alla [!DNL SharePoint] områden.

### Åtkomst och behörigheter

Första gången en användare lägger till ett dokument i [!DNL Workfront] från [!DNL SharePoint]dirigeras de till en skärm som begär följande behörigheter:

| Åtkomst | Orsak |
|---|---|
| Ha fullständig åtkomst till dina filer | Tillåter [!DNL Workfront] för att komma åt en användares filer för att länka resurser. När dokument skickas från [!DNL Workfront] till [!DNL SharePoint], [!DNL Workfront] kräver åtkomst för att skapa resursen. |
| Läs objekt i alla webbplatssamlingar | Tillåter [!DNL Workfront] för att läsa resurser för att aktivera användarnavigering. |
| Redigera eller ta bort objekt i alla webbplatssamlingar | Tillåter [!DNL Workfront] för att skapa resurser på webbplatser och i webbplatssamlingar. Radera används endast när användaren rensar efter misslyckade länkförsök. |
| Bevara åtkomst till data som du har gett åtkomst till | Tillåter [!DNL Workfront] för att generera en uppdateringstoken. |
| Logga in och läs användarprofilen | Tillåter [!DNL Workfront] om du vill använda åtkomsttoken för att agera för användarens räkning via inloggningsflödet OAuth2. |

* Den här åtkomsten beviljas av användaren första gången de använder integreringen och kan återkallas när som helst.
* Behörigheterna som krävs för integreringen är **delegerad** behörigheter.
* [!DNL Workfront] begär den lägsta åtkomstnivå som krävs för att utföra åtgärder i integreringen.
* Åtkomst till att visa, redigera eller ta bort en [!DNL Adobe Workfront] dokument länkat till [!DNL SharePoint] baseras på användarens åtkomst till [!DNL Workfront]. All navigering, hämtning eller redigering av en [!DNL SharePoint] fil eller mapp kräver åtkomst till [!DNL SharePoint]och åtkomsten till dessa åtgärder styrs av [!DNL SharePoint].
* Användare kan visa miniatyrbilder och förhandsgranska bilder som hämtats från [!DNL SharePoint]och kan se fil- och mappnamn i [!DNL SharePoint], utan att logga in [!DNL SharePoint].
* En användares åtkomsttoken används bara när användaren är offline och en annan användare visar innehållet i en mapp som är länkad till [!DNL Workfront]. Åtkomsttoken används för att identifiera om några dokument i mappen har lagts till, tagits bort eller redigerats.

### Säkerhet

All kommunikation mellan [!DNL Workfront] och [!DNL SharePoint] utförs via HTTPS, som krypterar informationen.

[!DNL Workfront] lagrar, kopierar eller duplicerar inte data från [!DNL SharePoint]. Det enda undantaget är att [!DNL Workfront] lagrar miniatyrbilder från [!DNL SharePoint] som ska visas i listvyn och i förhandsvisningen.

Om en resurs först överfördes till [!DNL Workfront]och sedan skicka till [!DNL SharePoint], [!DNL Workfront] sparar data för den första filen eftersom användare kan hämta en tidigare version av en [!DNL Workfront] -dokument. Om ett dokument har skapats i [!DNL SharePoint], [!DNL Workfront] lagrar inte dessa fildata.

## Konfigurera äldre [!DNL SharePoint] integration för fortsatt åtkomst till dokument

För att säkerställa att dina användare har fortsatt åtkomst till dokument som är länkade till Workfront via äldre [!DNL SharePoint] integreringen måste du konfigurera om åtkomsten till det gamla [!DNL SharePoint] integrering och håller SharePoint Client Secret uppdaterat.

* [Konfigurera om åtkomst till äldre [!DNL SharePoint] integration](#reconfigure-access-to-the-legacy-sharepoint-integration)
* [Konfigurera klienthemligheten för fortsatt åtkomst till äldre [!DNL SharePoint] integration](#configure-the-client-secret-for-continued-access-to-the-legacy-sharepoint-integration)

### Konfigurera om åtkomst till äldre [!DNL SharePoint] integration

Omkonfigurera äldre [!DNL SharePoint] integreringen ger användarna tillgång till dokument som länkats via äldre [!DNL SharePoint] integreringen, samtidigt som man ser till att användarna inte kan länka nya dokument genom integreringen.

>[!NOTE]
>
> * Det gamla [!DNL SharePoint] integreringen är märkt &quot;[!DNL SharePoint].&quot;
> * Den nya [!DNL SharePoint] integreringen är märkt &quot;[!UICONTROL [!DNL SharePoint] (Graph API)].&quot;

1. Klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om tillgängligt), klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Setup]** ![Ikonen Inställningar](/help/_includes/assets/gear-icon-setup.png).
1. Välj **[!UICONTROL Documents]** i den vänstra navigeringen väljer du **[!UICONTROL Cloud Providers]**.
1. Se till att **[!DNL SharePoint]** och **[!UICONTROL [!DNL SharePoint] (Graph API)]** båda är aktiverade.
1. Klicka på **[!UICONTROL Save]**.
1. Välj **[!UICONTROL Documents]** i den vänstra navigeringen väljer du **[!UICONTROL [!DNL SharePoint] Integration]**.
1. Markera bockmarkeringen till vänster i listan för alla befintliga integreringar och välj sedan **[!UICONTROL Disable]**.
   ![](assets/disable-old-sharepoint.png)


### Konfigurera klienthemligheten för fortsatt åtkomst till äldre [!DNL SharePoint] integration

Dina [!DNL SharePoint] Klienthemlighet upphör en gång om året. För att säkerställa fortsatt åtkomst till dokumenten i ditt äldre system [!DNL SharePoint] integreringen måste du behålla [!DNL SharePoint] Klienthemligheten är uppdaterad.

>[!IMPORTANT]
>
> För [!DNL SharePoint] Klienthemligheter hanteras av [!DNL Microsoft], funktioner och procedurer för klienthemlighet kan ändras baserat på uppdateringar av [!DNL SharePoint] gjord av [!DNL Microsoft]. Kontrollera alltid [!DNL Microsoft] dokumentation för den senaste informationen om procedurer och funktioner i [!DNL SharePoint].

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. Generera en ny klienthemlighet enligt beskrivningen i [Ersätta en utgående klienthemlighet i en [!DNL SharePoint] Tillägg](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret).
1. Kopiera den här klienthemligheten till en säker plats.
1. Logga in [!DNL Workfront] som administratör.
1. Klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om tillgängligt), klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Setup]** ![Ikonen Inställningar](/help/_includes/assets/gear-icon-setup.png).
1. Klicka på i den vänstra panelen **[!UICONTROL Documents]** > **[!UICONTROL [!DNL SharePoint] Integration]**.
1. Klicka på [!DNL SharePoint] integrering som du vill uppdatera och klicka sedan på **[!UICONTROL Edit]**.
1. Leta reda på **Anslutningsinformation** i redigeringsfönstret anger du den nya klienthemligheten i **[!UICONTROL SharePoint Client Secret]** fält.
1. Klicka på **[!UICONTROL Save]**.

<!--

## Instructions for setting up the legacy SharePoint integration

>[!IMPORTANT]
>
>This integration has been deprecated. The instructions here are for information only and will be removed in the near future.


Workfront connects to [!DNL SharePoint] Online using OAuth 2.0, a standard used by most web-based integrations for the authentication and authorization of users.

To configure OAuth, you need to create a [!DNL SharePoint] site and a Site App within [!DNL SharePoint]. This process is described in the following sections.

For more information about OAuth, see [http://oauth.net](http://oauth.net/).

>[!TIP]
>
>To make it easy to copy and paste information between [!DNL Workfront] and [!DNL SharePoint] in these steps, we recommend keeping both applications open in separate tabs.

* [Create and configure a [!DNL SharePoint] site](#create-and-configure-a-sharepoint-site) 
* [Grant write permissions to the site app](#grant-write-permissions-to-the-site-app) 
* [Create a [!DNL Workfront] [!DNL SharePoint] integration instance](#create-a-workfront-sharepoint-integration-instance) 
* [Complete your integration](#complete-your-integration) 
* [Add documents](#add-documents)

### Create and configure a [!DNL SharePoint] site  {#create-and-configure-a-sharepoint-site}

In order for [!DNL Workfront] to authenticate with [!DNL SharePoint], [!DNL Workfront] ca use a master site where users have the [!UICONTROL Full Control] permission level or specific Manage permissions. This master site acts as an Authentication Entry Point for [!DNL Workfront].

To create and configure a [!DNL SharePoint] Site:

1. (Optional) If you do not want to use your organization's root site, you can create a master site in [!DNL SharePoint].

   For instructions, visit [Create a site](https://docs.microsoft.com/en-us/sharepoint/create-site-collection) in the [!DNL Microsoft] Documentation.

   * Select the **[!UICONTROL Team Site]** option when creating the site.

1. (Conditional) If you created a site in step 1, go to the site you just created.

   Or

   If you did not create a site in step 1, go to your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.
1. Configure the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client ID]</p> </td> 
      <td> <p>Click <strong>[!UICONTROL Generate]</strong> to generate a Client ID. Copy this ID to a secure location. You will use it later when you set up the [!DNL SharePoint] integration in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client Secret]</p> </td> 
      <td> <p>Click <strong>[!UICONTROL Generate]</strong> to generate a Client Secret. Copy this Secret to a secure location. You will use it later when you set up the [!DNL SharePoint] integration in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Title</p> </td> 
      <td> <p>Enter a title, such as [!DNL Workfront] Site App. Users see this title when adding documents..</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App Domain]</p> </td> 
      <td> <p><code>my.workfront.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Redirect URI]</p> </td> 
      <td> <p><code>https://oauth.my.workfront.com/oauth2/redirect</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Create]**
1. Continue to [Grant write permissions to the site app](#grant-write-permissions-to-the-site-app).

### Grant write permissions to the site app  {#grant-write-permissions-to-the-site-app}

At this point, you have successfully created a Site App and registered it within [!DNL Workfront]. This site app is also known as an app principal in [!DNL SharePoint]. It resides within your tenant. New site apps do not automatically have access to site collections within the tenant. Permissions must be granted explicitly, for each site collection. The steps below will show you how to grant Write permission to the new Site App a site collection. Repeat these steps for each of the site collections you added under [!UICONTROL Visible Site Collections] in the steps above.

This site app must have [!UICONTROL Write] permission to any site collections that users need to access through [!DNL Workfront].

1. Add '/_layouts/15/appinv.aspx' to the URL in [!DNL Sharepoint].

   **Example:**

   ```
   https://mycompany.sharepoint.com/sites/mysite/_layouts/15/appinv.aspx
   ```

1. Configure the following fields

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL App ID]</td> 
      <td> <p>Add the Client ID that you created in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>and click <strong>[!UICONTROL Lookup]</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client] / [!UICONTROL App Domain] / [!UICONTROL Redirect URL]</p> </td> 
      <td> <p>These automatically fill when you click [!UICONTROL Lookup].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Permission Request XML]</td> 
      <td> <p>Copy the following XML to the [!UICONTROL Permission Request XML] field. Make sure that it is added exactly as shown without additional spaces etc. in order to avoid errors.</p> 
      <div></a> 
      <div style="mc-code-lang: XML;" class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False"> 
       <pre><code><span style="color: #63a35c; ">&lt;AppPermissionRequests&gt;</span><br><span style="color: #63a35c; ">&lt;AppPermissionRequest <span style="color: #795da3; ">Scope</span><span style="color: #df5000; ">="http://sharepoint/content/sitecollection/web"</span> <span style="color: #795da3; ">Right</span><span style="color: #df5000; ">="Write"</span>/&gt;</span><br><span style="color: #63a35c; ">&lt;/AppPermissionRequests&gt;</span></code></pre> 
      </div> 
      </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Create]**. 
1. In the dialog that appears, click **[!UICONTROL Trust it]**.
1. Verify that the site app has access to the site collection by clicking the **[!UICONTROL Site collection app permissions]** link in [!UICONTROL Site Settings].
1. Repeat the steps above for the remaining site collections, then continue with [Create a [!DNL Workfront] [!DNL SharePoint] integration instance](#create-a-workfront-sharepoint-integration-instance).

### Create a [!DNL Workfront] [!DNL SharePoint] integration instance {#create-a-workfront-sharepoint-integration-instance}

When you have created a site app in [!DNL SharePoint], you can now copy information from the site app into [!DNL Workfront]. The site app is an app principal and acts as the conduit through which OAuth requests are made to access documents within site collections.

1. Log into [!DNL Workfront] as an administrator.
1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. In the left panel, click **[!UICONTROL Documents]** > **[!UICONTROL [!DNL SharePoint] Integration]**.
1. Click **[!UICONTROL Add [!DNL SharePoint]]**.
1. Configure the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Name]</p> </td> 
      <td> <p>Enter a name for the [!DNL SharePoint] integration. Users see this name when they click [!UICONTROL Add] &gt; [!UICONTROL From] 'name of integration'. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL SharePoint] Host Instance]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.sharepoint.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL Azure] Access Domain]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.onmicrosoft.com</code> </p> <p>This refers to the Master Site that users will use to authenticate through. It is likely the same domain as the [!UICONTROL [!DNL SharePoint] Host Instance].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>
      </p> </td> 
      <td> <b>Important</b> Site collections are used only in the Legacy [!DNL SharePoint] Integration.
       <ul> 
        <li> <p><b>If you are using your organization's root site</b><b>:</b> </p> <p>Enter <code>/</code></p> </li> 
        <li> <p><b>If you are using a master site and subsites:</b> </p> <p><b>IMPORTANT</b>: [!DNL Microsoft SharePoint] no longer recommends the use of subsites.</p> <p>Enter the URL stem for the site collection that you created in the section above.</p> <p>This is the section of the URL after .com.</p> <p>Example: for the URL <code>https://mycompany.sharepoint.com/sites/mysite</code>, the stem would be <code>/sites/mysite</code>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Client ID]</td> 
      <td>Enter the Client ID that you generated in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Client Secret]</td> 
      <td>Enter the Client Secret that you generated in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Visible Site Collections]</td> 
      <td> <b>Important</b> Site collections are used only in the Legacy [!DNL SharePoint] integration.
       <ul> 
        <li> <p><b> If you are using your organization's root site</b><b>:</b> </p> <p>Enter <code>/</code></p> </li> 
        <li> <p><b>If you are using a master site and subsites:</b> </p> <p><b>IMPORTANT</b>: [!DNL Microsoft SharePoint] no longer recommends the use of subsites.</p> <p>For each subsite you want to add to your [!DNL SharePoint] integration, enter the stem of the subsite.</p> <p>Example: for the URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, the stem would be <code>/sites/mysite/mysubsite</code>.</p> <p><b>NOTE</b>:   <p>If you want to test your configuration only (no subsites), enter the stem of the master site. </p> <p>Example: for the URL <code> https://mycompany.sharepoint.com/sites/mysite</code>, the stem would be <code>/sites/mysite</code>.</p> <p>When you have tested your configuration as described in <a href="#complete-your-integration" class="MCXref xref">Complete your integration</a>, you must remove the master site and enter the subsites.</p> 
          <ol> 
           <li value="1">Click the <strong>[!UICONTROL Main Menu]</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of [!DNL Adobe Workfront], then click <strong>[!UICONTROL Setup]</strong> <img src="assets/gear-icon-settings.png">.<li><p>In the left panel, click <strong>[!UICONTROL Documents]</strong> &gt; <strong>[!UICONTROL [!DNL SharePoint] Integration]</strong>.</p></li><li><p>Click the [!DNL SharePoint] integration you are setting up, then click Edit.</p></li><li><p>Delete the stem for the master site from the [!UICONTROL Visible Site Collections] field.</p></li><li><p>For each subsite you want to add to your [!DNL SharePoint] integration, enter the stem of the subsite.</p></li><p>Example: for the URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, the stem would be <code>/sites/mysite/mysubsite</code>.</p></li> 
          </ol> </p> </li> 
       </ul> <p> </p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Save]**
1. Continue to [Complete your integration](#complete-your-integration).

### Complete your integration {#complete-your-integration}

The basic configuration is almost complete.

1. In Workfront, Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Documents]** ![](assets/document-icon.png).
1. Click **[!UICONTROL Add new]**.
1. Click **[!UICONTROL From] `<title of your [!DNL SharePoint] site>`** in the dropdown.

   A dialog that invites you to Trust this site appears.

   >[!NOTE]
   >
   >If this dialog does not appear, your [!DNL SharePoint] integration is not configured correctly.

1. Click **[!UICONTROL Trust it]**.

### Add documents {#add-documents}

You can now add documents from your [!DNL SharePoint] site.

For instructions, see [Link an external document to [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) in [Link documents from external applications](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!IMPORTANT]
>
>If the user who linked a folder no longer has access to the external application, [!DNL Workfront] can no longer access the contents of the folder. This may happen, for example, if the user who originally linked the folder leaves the company. To ensure continued access, a user with access to the folder must re-link the folder.
> 

-->

## Felsökning

* [Problem: Användarna får autentiseringsbaserade fel när de använder [!DNL SharePoint] integrering.](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [Problem: När du försöker bläddra [!DNL SharePoint] filer i [!DNL Workfront], jag ser inte någon eller alla webbplatssamlingar.](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [Problem: Jag har inte åtkomst till tidigare länkade mappar och dokument i [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### Problem: Användarna får autentiseringsbaserade fel när de använder [!DNL SharePoint] integrering. {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

Lösningar:

Användarna måste ha rätt behörigheter för [!DNL SharePoint] webbplats.

Användare med [!UICONTROL Full Control] har alla behörigheter som krävs för din [!DNL SharePoint] integrering. Om du inte vill ge användarna fullständig behörighet måste du ge följande behörigheter:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Design]</p> </td> 
   <td> <p>Kan visa, lägga till, uppdatera, ta bort, godkänna och anpassa</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Edit]</p> </td> 
   <td> <p>Kan lägga till, redigera och ta bort listor; kan visa, lägga till, uppdatera och ta bort listobjekt och dokument</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contribute]</p> </td> 
   <td> <p>Kan visa, lägga till, uppdatera och ta bort listobjekt och dokument</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL View only]</p> </td> 
   <td> <p>Kan visa sidor, listobjekt och dokument (dokumenttyper med filhanterare på serversidan kan visas i webbläsaren men inte hämtas)</p> </td> 
  </tr> 
 </tbody> 
</table>

Instruktioner om hur du skapar och redigerar behörighetsnivåer finns i [Så här skapar och redigerar du behörighetsnivåer](https://docs.microsoft.com/en-us/sharepoint/how-to-create-and-edit-permission-levels) i Microsoft-dokumentationen.

<!--

### Problem: As a [!DNL Workfront] user, I am unable to provision a new [!DNL SharePoint] instance. When I attempt to do I see an error. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

Solutions:

This can be caused by a number of things, originating in either [!DNL Workfront] or [!DNL SharePoint]'s configuration. Verify that:

* The Client ID, Client Secret, return URL and other configuration fields are correctly mapped between the [!DNL Workfront] [!DNL SharePoint] Integration instance and the [!DNL SharePoint] Site App.
* The user has [!UICONTROL Full Control] permission to the Site Collection used for authentication.
* The Site App is listed under [!UICONTROL Site App Permissions] for the [!UICONTROL Site Collection] used for authentication.

-->

### Problem: När du försöker bläddra [!DNL SharePoint] filer i [!DNL Workfront], jag ser inte någon eller alla webbplatssamlingar. {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

Lösningar:

Så här visar du en webbplatssamling i [!DNL Workfront]måste följande villkor vara uppfyllda:

<!--

* The site collection must be registered in the [!DNL Workfront] [!DNL SharePoint] Integration instance.

  To verify this in [!DNL Workfront]:

   1. Go to [!UICONTROL Setup] > [!UICONTROL Documents] > [!UICONTROL [!DNL SharePoint] Integration].
   1. Edit the [!DNL SharePoint] Integration instance information.
   1. Verify that the site collection is listed under [!UICONTROL Visible Site Collections].
   -->

* Användaren måste ha vyåtkomst till webbplatssamlingen i [!DNL SharePoint].

  Så här verifierar du [!DNL SharePoint]kontrollerar du webbplatssamlingens behörigheter i SharePoint.

<!--* The [!DNL SharePoint] Site App must have access to the site collection.

  To verify this in [!DNL SharePoint]:

   1. Go to the site collection > [!UICONTROL Settings] > [!UICONTROL Site app permissions].
   1. Ensure that the [!UICONTROL Site App] used by [!DNL Workfront] is listed here.
   1. (Conditional) If the Site App is not listed, add to the site collection using _layouts/15/appinv.aspx.

      For information about adding the site collection, see Granting Write Permissions To The Site App.
      
-->

### Problem: Jag har inte åtkomst till tidigare länkade mappar och dokument i [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

Lösning:

Om användaren som länkade en [!DNL SharePoint] mappen inte längre kan autentiseras, [!DNL Workfront] kan inte längre komma åt innehållet i mappen. Detta kan till exempel inträffa om användaren som ursprungligen länkade mappen lämnar företaget.

För att säkerställa fortsatt åtkomst måste en användare med åtkomst till mappen länka om mappen.

Mer information om hur du länkar mappar från externa leverantörer finns i [Länka dokument från externa program](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<!--

### Problem: I see a "404 not found" error when attempting to add a document from [!DNL Sharepoint]

#### Solution:

This error might occur if one of the sites configured in the [!UICONTROL Visible Site Collections] list has been deleted in Sharepoint. Check the [!UICONTROL Visible Site Collections] list, and remove any sites that have been deleted in Sharepoint.-->
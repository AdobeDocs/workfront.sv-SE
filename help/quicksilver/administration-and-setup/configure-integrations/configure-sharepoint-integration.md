---
title: Konfigurera [!DNL SharePoint] integration
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Ni kan integrera [!DNL Workfront] med [!DNL SharePoint] online, ger användarna möjlighet att navigera till, länka och lägga till [!DNL SharePoint] dokument i Workfront. Den angivna funktionaliteten liknar den för andra [!DNL Workfront] integreringar som Google Drive, Box och Dropbox.
author: Becky, Caroline
feature: System Setup and Administration, [!DNL Workfront] Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: 5292069412a73f824dbcd967d47737cff5ef58fa
workflow-type: tm+mt
source-wordcount: '2351'
ht-degree: 0%

---

# Konfigurera äldre [!DNL SharePoint] integration

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Du måste vara en [!DNL Workfront] administratör. För information om [!DNL Workfront] administratörer, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Förutsättningar

Du måste ha nödvändig åtkomst eller behörighet i [!DNL SharePoint] för att ändra eller konfigurera organisationens [!DNL SharePoint].

## Länka dokument via den nya SharePoint-integreringen

Enskilda användare kan länka dokument via de nya [!DNL SharePoint] integrering. Integreringen kräver ingen administratörskonfiguration. I stället loggar användaren in på sina [!DNL Microsoft] när du länkar ett dokument, vilket gör att integreringen kan komma åt dokument som finns i användarens [!DNL SharePoint].

Första gången en användare ansluter [!DNL Workfront] [!DNL SharePoint] integrering med [!DNL SharePoint] kommer de att se och godkänna alla behörigheter som [!DNL Workfront] använder när de interagerar med [!UICONTROL SharePoint] konto. Läsbehörigheter tillåt [!DNL Workfront] för att se och komma åt filer på [!DNL SharePoint]och skrivbehörigheter tillåter användaren att överföra filer till [!DNL SharePoint].

Instruktioner om hur du länkar dokument genom det nya [!DNL SharePoint] integrering, se [Länka ett externt dokument till [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* A [!DNL SharePoint] kan ansluta till en enda [!DNL SharePoint] -instans. Därför kan en användare konfigurera en integrering för en [!DNL SharePoint], men kan inte konfigurera en integrering till en sekund [!DNL SharePoint], även om de har behörighet till och dokument på den andra [!DNL SharePoint].
>
>* En användare har åtkomst till samma platser, samlingar, mappar, undermappar och filer via [!DNL Workfront] [!DNL SharePoint] som de har i sina [!DNL SharePoint] konto.


## Konfigurera den gamla SharePoint-integreringen för fortsatt åtkomst till dokument

För att säkerställa att dina användare har fortsatt åtkomst till dokument som är länkade till Workfront via den tidigare SharePoint-integreringen måste du konfigurera om åtkomsten till den gamla SharePoint-integreringen och hålla SharePoint Client Secret uppdaterat.

* [Konfigurera om åtkomst till äldre [!DNL SharePoint] integration](#reconfigure-access-to-the-legacy-dnl-sharepoint-integration)
* [Konfigurera klienthemligheten för fortsatt åtkomst till äldre [!DNL SharePoint] integration](#configure-the-client-secret-for-continued-access-to-the-legacy-dnl-sharepoint-integration)

### Konfigurera om åtkomst till äldre [!DNL SharePoint] integration

För att säkerställa att du kan komma åt dokument som är länkade via äldre [!DNL SharePoint] integreringen, och samtidigt vara säker på att användarna inte kan länka nya dokument genom integreringen, ska du slutföra följande procedur.

>[!NOTE]
>
> * Det gamla [!DNL SharePoint] integreringen heter &quot;[!DNL SharePoint].&quot;
> * Den nya [!DNL SharePoint] integreringen heter &quot;[!UICONTROL [!DNL SharePoint] (Graph API)].&quot;


1. Klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **[!UICONTROL Setup]** ![Inställningar](../get-started-wf-administration/assets/gear-icon-settings.png).
1. Välj **[!UICONTROL Documents]** i den vänstra navigeringen väljer du **[!UICONTROL Cloud Providers]**.
1. Se till att **[!DNL SharePoint]** och **[!UICONTROL [!DNL SharePoint] (Graph API)]** båda är aktiverade.
1. Klicka på **[!UICONTROL Save]**.
1. Välj **[!UICONTROL Documents]** i den vänstra navigeringen väljer du **[!UICONTROL [!DNL SharePoint] Integration]**.
1. Markera bockmarkeringen till vänster i listan för alla befintliga integreringar och välj sedan **[!UICONTROL Disable]**.


### Konfigurera klienthemligheten för fortsatt åtkomst till äldre [!DNL SharePoint] integration

Dina [!DNL SharePoint] Klienthemlighet upphör en gång om året. För att säkerställa fortsatt åtkomst till dokumenten i ditt äldre system [!DNL SharePoint] integreringen måste du behålla [!DNL SharePoint] Klienthemligheten är uppdaterad.

>[!IMPORTANT]
>
> För [!DNL SharePoint] Client Secrets hanteras av [!DNL Microsoft], funktioner och procedurer för klienthemlighet kan ändras baserat på uppdateringar av [!DNL SharePoint] gjord av [!DNL Microsoft]. Kontrollera alltid [!DNL Microsoft] dokumentation för den senaste informationen om procedurer och funktioner i [!DNL SharePoint].

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. Generera en ny klienthemlighet enligt beskrivningen i [Ersätta en utgående klienthemlighet i en [!DNL SharePoint] Tillägg](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret)
1. Kopiera den här klienthemligheten till en säker plats.
1. Logga in [!DNL Workfront] som administratör.
1. I Workfront klickar du på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).
1. Klicka på i den vänstra panelen **[!UICONTROL Documents]** > **[!UICONTROL [!DNL SharePoint] Integration]**.
1. Klicka på [!DNL SharePoint] integrering som du vill uppdatera och klicka sedan på **[!UICONTROL Edit]**.
1. Ange den nya klienthemligheten i **[!UICONTROL Client Secret]** fält.
1. Klicka på **[!UICONTROL Save]**.



## Instruktioner för hur du konfigurerar SharePoint-integreringen

>[!IMPORTANT]
>
>Den här integreringen har tagits bort. Instruktionerna här gäller endast information och kommer att tas bort inom den närmaste framtiden.


Workfront ansluter till [!DNL SharePoint] Online med OAuth 2.0, en standard som används av de flesta webbaserade integreringar för autentisering och auktorisering av användare.

Om du vill konfigurera OAuth måste du skapa en [!DNL SharePoint] webbplats och en webbplatsapp inom [!DNL SharePoint]. Den här processen beskrivs i följande avsnitt.

Mer information om OAuth finns i [http://oauth.net](http://oauth.net/).

>[!TIP]
>
>Så här gör du det enkelt att kopiera och klistra in information mellan [!DNL Workfront] och [!DNL SharePoint] I de här stegen rekommenderar vi att du håller båda programmen öppna på separata flikar.

* [Skapa och konfigurera en [!DNL SharePoint] webbplats](#create-and-configure-a-sharepoint-site)
* [Bevilja skrivbehörighet till webbplatsappen](#grant-write-permissions-to-the-site-app)
* [Skapa en [!DNL Workfront] [!DNL SharePoint] integrationsinstans](#create-a-workfront-sharepoint-integration-instance)
* [Slutför integreringen](#complete-your-integration)
* [Lägga till dokument](#add-documents)

### Skapa och konfigurera en [!DNL SharePoint] webbplats  {#create-and-configure-a-sharepoint-site}

För att [!DNL Workfront] att autentisera med [!DNL SharePoint], [!DNL Workfront] kan använda en överordnad webbplats där användarna har [!UICONTROL Full Control] behörighetsnivå eller specifika hanteringsbehörigheter. Den här överordnad webbplatsen fungerar som en autentiseringspoäng för [!DNL Workfront].

Skapa och konfigurera en [!DNL SharePoint] Plats:

1. (Valfritt) Om du inte vill använda organisationens rotplats kan du skapa en överordnad webbplats i [!DNL SharePoint].

   Instruktioner finns på [Skapa en plats](https://docs.microsoft.com/en-us/sharepoint/create-site-collection) i [!DNL Microsoft] Dokumentation.

   * Välj **[!UICONTROL Team Site]** när du skapar platsen.

1. (Villkorligt) Om du skapade en plats i steg 1 går du till den plats du just skapade.

   eller

   Om du inte skapade en plats i steg 1 går du till organisationens rotwebbplats.

1. Lägg till `/_layouts/15/appregnew.aspx` till slutet av URL:en i sökfältet högst upp i webbläsarfönstret.
1. Konfigurera följande fält:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client ID]</p> </td> 
      <td> <p>Klicka <strong>[!UICONTROL Generate]</strong> för att generera ett klient-ID. Kopiera detta ID till en säker plats. Du kommer att använda den senare när du konfigurerar [!DNL SharePoint] integration i [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client Secret]</p> </td> 
      <td> <p>Klicka <strong>[!UICONTROL Generate]</strong> för att skapa en klienthemlighet. Kopiera hemligheten till en säker plats. Du kommer att använda den senare när du konfigurerar [!DNL SharePoint] integration i [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Titel</p> </td> 
      <td> <p>Ange en titel, till exempel [!DNL Workfront] Webbplatsapp. Användarna ser den här titeln när de lägger till dokument.</p> </td> 
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

1. Klicka på **[!UICONTROL Create]**
1. Fortsätt till [Bevilja skrivbehörighet till webbplatsappen](#grant-write-permissions-to-the-site-app).

### Bevilja skrivbehörighet till webbplatsappen  {#grant-write-permissions-to-the-site-app}

Nu har du skapat en webbplatsapp och registrerat den i [!DNL Workfront]. Den här webbplatsappen kallas även för ett programhuvud i [!DNL SharePoint]. Den finns hos er hyresgäst. Nya webbplatsappar har inte automatiskt åtkomst till webbplatssamlingar i klientorganisationen. Behörigheter måste beviljas explicit för varje webbplatssamling. Stegen nedan visar hur du tilldelar skrivbehörighet till det nya webbplatsprogrammet till en webbplatssamling. Upprepa dessa steg för var och en av webbplatssamlingarna som du lade till under [!UICONTROL Visible Site Collections] i stegen ovan.

Den här webbplatsappen måste ha [!UICONTROL Write] behörighet till alla webbplatssamlingar som användare behöver åtkomst till via [!DNL Workfront].

1. Lägg till /_layouts/15/appinv.aspx i URL:en i [!DNL Sharepoint].

   **Exempel:**

   ```
   https://mycompany.sharepoint.com/sites/mysite/_layouts/15/appinv.aspx
   ```

1. Konfigurera följande fält

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL App ID]</td> 
      <td> <p>Lägg till klient-ID som du skapade i <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Skapa och konfigurera en [!DNL SharePoint] webbplats </a>och klicka <strong>[!UICONTROL Lookup]</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client] / [!UICONTROL App Domain] / [!UICONTROL Redirect URL]</p> </td> 
      <td> <p>Dessa fylls automatiskt när du klickar [!UICONTROL Lookup].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Permission Request XML]</td> 
      <td> <p>Kopiera följande XML-kod till [!UICONTROL Permission Request XML] fält. Se till att den läggs till exakt så som visas utan ytterligare blanksteg osv. för att undvika fel.</p> 
      <div></a> 
      <div style="mc-code-lang: XML;" class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False"> 
       <pre></pre></div></div></td></tr></tbody></table>

1. Klicka på **[!UICONTROL Create]**.
1. Klicka på **[!UICONTROL Trust it]**.
1. Kontrollera att webbplatsappen har åtkomst till webbplatssamlingen genom att klicka på **[!UICONTROL Site collection app permissions]** länk in [!UICONTROL Site Settings].
1. Upprepa stegen ovan för de återstående webbplatssamlingarna och fortsätt sedan med [Skapa en [!DNL Workfront] [!DNL SharePoint] integrationsinstans](#create-a-workfront-sharepoint-integration-instance).

### Skapa en [!DNL Workfront] [!DNL SharePoint] integrationsinstans {#create-a-workfront-sharepoint-integration-instance}

När du har skapat en webbplatsapp i [!DNL SharePoint]kan du nu kopiera information från webbplatsappen till [!DNL Workfront]. Webbplatsappen är ett programhuvudprogram och fungerar som den kanal genom vilken OAuth-begäranden görs för att komma åt dokument inom webbplatssamlingar.

1. Logga in [!DNL Workfront] som administratör.
1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **[!UICONTROL Documents]** > **[!UICONTROL [!DNL SharePoint] Integration]**.
1. Klicka på **[!UICONTROL Add [!DNL SharePoint]]**.
1. Konfigurera följande fält:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Name]</p> </td> 
      <td> <p>Ange ett namn för [!DNL SharePoint] integrering. Användarna ser det här namnet när de klickar [!UICONTROL Add] &gt; [!UICONTROL From] 'integreringens namn'. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL SharePoint] Värdinstans]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.sharepoint.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL Azure] Åtkomstdomän]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.onmicrosoft.com</code> </p> <p>Detta avser den Överordnad webbplats som användare kommer att använda för att autentisera via. Det är troligtvis samma domän som [!UICONTROL [!DNL SharePoint] Värdinstans].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>
      </p> </td> 
      <td> <b>Viktigt</b> Webbplatssamlingar används endast i äldre [!DNL SharePoint] Integrering.
       <ul> 
        <li> <p><b>Om du använder organisationens rotplats</b><b>:</b> </p> <p>Retur <code>/</code></p> </li> 
        <li> <p><b>Om du använder en överordnad webbplats och underwebbplatser:</b> </p> <p><b>VIKTIGT</b>: [!DNL Microsoft SharePoint] rekommenderar inte längre att underwebbplatser används.</p> <p>Ange URL-adressen för webbplatssamlingen som du skapade i avsnittet ovan.</p> <p>Det här är avsnittet i URL:en efter .com.</p> <p>Exempel: för URL <code>https://mycompany.sharepoint.com/sites/mysite</code>skulle stammen vara <code>/sites/mysite</code>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Klient-ID]</td> 
      <td>Ange det klient-ID som du skapade i <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Skapa och konfigurera en [!DNL SharePoint] webbplats </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Klienthemlighet]</td> 
      <td>Ange den klienthemlighet som du skapade i <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Skapa och konfigurera en [!DNL SharePoint] webbplats </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Visible Site Collections]</td> 
      <td> <b>Viktigt</b> Webbplatssamlingar används endast i äldre [!DNL SharePoint] integrering.
       <ul> 
        <li> <p><b> Om du använder organisationens rotplats</b><b>:</b> </p> <p>Retur <code>/</code></p> </li> 
        <li> <p><b>Om du använder en överordnad webbplats och underwebbplatser:</b> </p> <p><b>VIKTIGT</b>: [!DNL Microsoft SharePoint] rekommenderar inte längre att underwebbplatser används.</p> <p>För varje underwebbplats som du vill lägga till [!DNL SharePoint] integration, ange underplatsens stamm.</p> <p>Exempel: för URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>skulle stammen vara <code>/sites/mysite/mysubsite</code>.</p> <p><b>ANMÄRKNING</b>:   <p>Om du bara vill testa konfigurationen (inga underwebbplatser) anger du stammen för den överordnad platsen. </p> <p>Exempel: för URL <code> https://mycompany.sharepoint.com/sites/mysite</code>skulle stammen vara <code>/sites/mysite</code>.</p> <p>När du har testat konfigurationen enligt beskrivningen i <a href="#complete-your-integration" class="MCXref xref">Slutför integreringen</a>måste du ta bort den överordnad webbplatsen och ange underwebbplatser.</p> 
          <ol> 
           <li value="1">Klicka på <strong>[!UICONTROL Main Menu]</strong> icon <img src="assets/main-menu-icon.png"> i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka <strong>[!UICONTROL Setup]</strong> <img src="assets/gear-icon-settings.png">.<li><p>Klicka på i den vänstra panelen <strong>[!UICONTROL Documents]</strong> &gt; <strong>[!UICONTROL [!DNL SharePoint] Integration]</strong>.</p></li><li><p>Klicka på [!DNL SharePoint] integreringen som du konfigurerar och klickar sedan på Redigera.</p></li><li><p>Ta bort stammen för den överordnad platsen från [!UICONTROL Visible Site Collections] fält.</p></li><li><p>För varje underwebbplats som du vill lägga till [!DNL SharePoint] integration, ange underplatsens stamm.</p></li><p>Exempel: för URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>skulle stammen vara <code>/sites/mysite/mysubsite</code>.</p></li> 
          </ol> </p> </li> 
       </ul> <p> </p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **[!UICONTROL Save]**
1. Fortsätt till [Slutför integreringen](#complete-your-integration).

### Slutför integreringen {#complete-your-integration}

Den grundläggande konfigurationen är nästan slutförd.

1. I Workfront klickar du på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **[!UICONTROL Documents]** ![](assets/document-icon.png).
1. Klicka på **[!UICONTROL Add new]**.
1. Klicka **[!UICONTROL From]`<title of your [!DNL SharePoint] site>`** i listrutan.

   En dialogruta öppnas där du kan ange att du litar på den här webbplatsen.

   >[!NOTE]
   >
   >Om den här dialogrutan inte visas kan du [!DNL SharePoint] integreringen är inte korrekt konfigurerad.

1. Klicka på **[!UICONTROL Trust it]**.

### Lägga till dokument {#add-documents}

Nu kan du lägga till dokument från [!DNL SharePoint] webbplats.

Instruktioner finns i [Länka ett externt dokument till [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) in [Länka dokument från externa program](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!IMPORTANT]
>
>Om användaren som länkade en mapp inte längre har åtkomst till det externa programmet, [!DNL Workfront] kan inte längre komma åt innehållet i mappen. Detta kan till exempel inträffa om användaren som ursprungligen länkade mappen lämnar företaget. För att säkerställa fortsatt åtkomst måste en användare med åtkomst till mappen länka om mappen.

## Felsökning

* [Problem: Användarna får autentiseringsbaserade fel när de använder [!DNL SharePoint] integrering.](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [Problem: Som [!DNL Workfront] användare, jag kan inte etablera en ny [!DNL SharePoint] -instans. När jag försöker göra det ser jag ett fel.](#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error)
* [Problem: När du försöker bläddra [!DNL SharePoint] filer i [!DNL Workfront], jag ser inte någon eller alla webbplatssamlingar.](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [Problem: Jag har inte åtkomst till tidigare länkade mappar och dokument i [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### Problem: Användarna får autentiseringsbaserade fel när de använder [!DNL SharePoint] integrering. {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

Lösningar:

Användarna måste vara medlem i en grupp som har lämplig behörighet för [!DNL SharePoint] webbplats.

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

Instruktioner om hur du skapar och redigerar behörighetsnivåer finns i [Skapa och redigera behörighetsnivåer](https://docs.microsoft.com/en-us/sharepoint/how-to-create-and-edit-permission-levels) i Microsoft-dokumentationen.

### Problem: Som [!DNL Workfront] användare, jag kan inte etablera en ny [!DNL SharePoint] -instans. När jag försöker göra det ser jag ett fel. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

Lösningar:

Detta kan orsakas av ett antal saker, som har sitt ursprung i antingen [!DNL Workfront] eller [!DNL SharePoint]&#39;s configuration. Verifiera att:

* Klient-ID, Klienthemlighet, retur-URL och andra konfigurationsfält mappas korrekt mellan [!DNL Workfront] [!DNL SharePoint] Integrationsinstans och [!DNL SharePoint] Webbplatsapp.
* Användaren har [!UICONTROL Full Control] behörighet till webbplatssamlingen som används för autentisering.
* Webbplatsappen listas under [!UICONTROL Site App Permissions] för [!UICONTROL Site Collection] används för autentisering.

### Problem: När du försöker bläddra [!DNL SharePoint] filer i [!DNL Workfront], jag ser inte någon eller alla webbplatssamlingar. {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

Lösningar:

Så här visar du en webbplatssamling i [!DNL Workfront]måste följande villkor vara uppfyllda:

* Webbplatssamlingen måste vara registrerad i [!DNL Workfront] [!DNL SharePoint] Integrationsinstans.

   Så här verifierar du [!DNL Workfront]:

   1. Gå till [!UICONTROL Setup] > [!UICONTROL Documents] > [!UICONTROL [!DNL SharePoint] Integration].
   1. Redigera [!DNL SharePoint] Instansinformation om integrering.
   1. Verifiera att webbplatssamlingen listas under [!UICONTROL Visible Site Collections].

* Användaren måste ha vyåtkomst till webbplatssamlingen i [!DNL SharePoint].
* Så här verifierar du [!DNL SharePoint], gå till [!DNL SharePoint]och öppna webbplatssamlingen > [!UICONTROL Settings] > [!UICONTROL Site permissions].
* The [!DNL SharePoint] Webbplatsappen måste ha åtkomst till webbplatssamlingen.

   Så här verifierar du [!DNL SharePoint]:

   1. Gå till webbplatssamlingen > [!UICONTROL Settings] > [!UICONTROL Site app permissions].
   1. Se till att [!UICONTROL Site App] används av [!DNL Workfront] anges här.
   1. (Villkorligt) Om webbplatsappen inte finns med i listan lägger du till i webbplatssamlingen med _layouts/15/appinv.aspx.

      Mer information om hur du lägger till webbplatssamlingen finns i Bevilja skrivbehörigheter i webbplatsappen.

### Problem: Jag har inte åtkomst till tidigare länkade mappar och dokument i [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

Lösning:

Om användaren som länkade en [!DNL SharePoint] mappen inte längre kan autentiseras, [!DNL Workfront] kan inte längre komma åt innehållet i mappen. Detta kan till exempel inträffa om användaren som ursprungligen länkade mappen lämnar företaget.

För att säkerställa fortsatt åtkomst måste en användare med åtkomst till mappen länka om mappen.

Mer information om hur du länkar mappar från externa leverantörer finns i [Länka dokument från externa program](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Problem: Jag ser ett felmeddelande &quot;404 hittades inte&quot; när jag försöker lägga till ett dokument från [!DNL Sharepoint]

#### Lösning:

Det här felet kan inträffa om någon av platserna som konfigurerats i [!UICONTROL Visible Site Collections] listan har tagits bort i Sharepoint. Kontrollera [!UICONTROL Visible Site Collections] och ta bort alla webbplatser som har tagits bort i Sharepoint.

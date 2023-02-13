---
title: Konfigurera [!DNL Workfront] med [!DNL Adobe Experience Manager] äldre koppling
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Som en [!DNL Adobe Workfront] administratör kan du integrera [!DNL Workfront] med Adobe Experience Manager (AEM) Assets och förse organisationen med en omfattande innehållshanteringslösning för att skapa, dela och underhålla resurser i arbetsflödet.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 024b8606-a9b7-413a-b393-8e5cdff37dd4
source-git-commit: 2f840ea68c9efb78acb4c24346c6775671ed0334
workflow-type: tm+mt
source-wordcount: '1663'
ht-degree: 0%

---

# Konfigurera [!DNL Workfront] med [!DNL Adobe Experience Manager] äldre koppling

Som en [!DNL Adobe Workfront] administratör kan du integrera [!DNL Workfront] med [!UICONTROL Adobe Experience Manager (AEM) Assets] och ge er organisation en omfattande innehållshanteringslösning för att skapa, dela och underhålla resurser i ert arbetsflöde.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Du måste vara en [!DNL Workfront] administratör. För information om [!DNL Workfront] administratörer, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## [!DNL Workfront for AEM Assets]

The [!DNL Workfront for AEM Assets connector] kan din organisation göra följande:

* Samarbeta och hantera kreativt innehåll genom att länka AEM resurser och mappar till projekt, uppgifter, ärenden och förfrågningar i [!DNL Workfront].

   Mer information om hur du konfigurerar dokumentationsintegreringar med tredjepartsprogram finns i  [Konfigurera dokumentintegreringar](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

* Integrera med [!DNL AEM Digital Asset Managemen]t (DAM)-databas, så att du kan använda [!DNL Workfront] för att hantera och dela digitala resurser som lagras i DAM.

   Mer information om hur du länkar dokument och resursmappar finns i   [Länka dokument från externa program](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

* Kombinera och använd metadata från båda programmen på en resurs.
* Visa en heltäckande kommunikationsström för en tillgång. Uppdateringar och kommentarer som gjorts för en resurs antingen i [!DNL Workfront] eller [!UICONTROL AEM Assets] synkroniseras med det andra programmet, vilket ger en omfattande historik över kommunikationen som gjorts med tillgången.

   Mer information om hur du gör kommentarer i [!DNL Workfront], se [Lägga till en uppdatering i ett dokument](../../documents/managing-documents/add-update-documents.md).

## Krav för installation av [!DNL AEM Assets] koppling

Innan du kan installera [!DNL Workfront] anslutning för [!UICONTROL AEM Assets]kontrollerar du att följande krav är uppfyllda:

* [!UICONTROL AEM Assets] installerat och konfigurerat, version 6.5 eller senare. Mer information om installation [!UICONTROL AEM Assets], se [[!DNL Adobe Experience Manager] dokumentation](https://experienceleague.adobe.com/docs/experience-manager.html).
* (Villkorligt) Om brandväggsreglerna inte tillåter trafik som förväntat lägger du till klustrets IP-adress och/eller domän i tillåtelselista. Mer information finns i [Konfigurera brandväggens tillåtelselista](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Installera [!DNL Workfront for AEM Assets] kopplingspaket {#install-the-workfront-for-aem-assets-connector-package}

>[!IMPORTANT]
>
>Följande instruktioner gäller för [!DNL Workfront with AEM Assets] äldre koppling som har ersatts av [[!DNL Workfront for Experience Manager] förbättrad koppling](../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-for-aem-enhanced-connector.md). Kontakta din kontorepresentant om du vill ha mer information.

Så här installerar du [!DNL Workfront for AEM Assets] måste du importera kopplingen till AEM som ett paket med [!UICONTROL CRX Package Manager].

1. På en arbetsstation där du redan har installerat AEM hämtar du [!DNL Workfront for AEM Assets] Installationsfil för anslutning.

   Du kan få [!DNL Workfront for AEM Assets] från din [!DNL Workfront] -representant.

1. Logga in på AEM med ett administratörskonto.
1. Klicka på **[!UICONTROL Tools]** > **[!UICONTROL Deployment]** > **[!UICONTROL Packages]**.

   The [!UICONTROL CRX Package Manager] öppnas.

1. Klicka på **[!UICONTROL Upload Package].**

1. I [!UICONTROL Upload Package] , bläddra efter och markera [!UICONTROL Workfront Connector] paketet och klicka sedan på **[!UICONTROL OK]**.\
   Paketet visas i [!UICONTROL CRX Package Manager].

1. Klicka på **[!UICONTROL Install].**

1. På [!UICONTROL Package] ignorera de avancerade inställningarna och klicka på **[!UICONTROL Install]**.
1. (Valfritt) Kontrollera att följande programsats visas i dialogrutan [!UICONTROL Activity Log]:

   ```
   Package installed in <time>
   ```

1. Stäng [!UICONTROL CRX Package Manager].

   Kopplingen är installerad och du kan nu konfigurera [!DNL AEM Assets] integrera med [!DNL Workfront].

1. Fortsätt med [Konfigurera [!DNL AEM Assets] integrera med [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront).

## Konfigurera [!DNL AEM Assets] integrera med [!DNL Workfront] {#configure-aem-assets-to-integrate-with-workfront}

När du har installerat anslutningsprogrammet importerar du anslutningsprogrammet till AEM och konfigurerar AEM att länka till dokument i [!DNL Workfront].

Information om hur du installerar anslutningsprogrammet finns i  [Installera [!DNL Workfront for AEM Assets] kopplingspaket](#install-the-workfront-for-aem-assets-connector-package).

* [Förutsättningar](#prerequisites)
* [Integrera AEM med [!DNL Workfront]](#integrate-aem-with-workfront)
* [Konfigurera [!UICONTROL AEM Externalizer]](#configure-the-aem-externalizer)

### Förutsättningar {#prerequisites}

Innan du börjar måste du aktivera behörigheter för Workfront Service:

1. I AEM, gå till **[!UICONTROL Tools]**> **[!UICONTROL Security]**> **[!UICONTROL Permissions]**.
1. I det övre vänstra hörnet väljer du **[!UICONTROL Users]**&#x200B; i listrutan och ange *[!UICONTROL workfront-service]* i **[!UICONTROL Search]**&#x200B;. Välj [!UICONTROL workfront-service] användare.
1. På skärmens högra sida väljer du **[!UICONTROL Add ACE]** för att skapa nya poster.
1. I &#x200B;**[!UICONTROL Add New Entry]**&#x200B; väljer du kryssruteikonen i **[!UICONTROL Path]**&#x200B; och välj mapp: */conf*
1. I fältet Behörigheter anger du: *jcr:read*
1. Välj **[!UICONTROL Add]**&#x200B; i det övre högra hörnet
1. (Valfritt) Upprepa stegen för att skapa fler poster.

### Integrera AEM med [!DNL Workfront] {#integrate-aem-with-workfront}

1. Logga in på AEM Assets som administratör.
1. Klicka **[!UICONTROL Tools]** >**[!UICONTROL Cloud Services]**>**[!UICONTROL Workfront Integration Configuration]** >**[!UICONTROL Global-Workfront].**&#x200B;**&#x200B;**

1. (Villkorligt) Om du inte har gjort det än skapar du en [!DNL Workfront] molnkonfigurationsfil.

   1. Klicka  **[!UICONTROL Create]** i det övre högra hörnet av [!DNL Global-Workfront] sida.
   1. I **[!UICONTROL Workfront URL]** anger du webbadressen till [!DNL Workfront] -instans.

      Till exempel: [!DNL https]:/`<account>`.my.workfront.com, där `<account>` är det konto du använder för integrering med AEM.

   1. I &#x200B;**[!UICONTROL Base Folder]** markerar du kryssruteikonen och väljer sedan sökvägen till de dokument som är länkade till i listrutan [!DNL Workfront] -objekt lagras.
   1. I AEM som visas följer du sökvägen till mappen med de dokument som är anslutna till [!DNL Workfront] objekt. Välj mapp och tryck på **[!UICONTROL Select]**&#x200B; i det övre högra hörnet.

      Du kan länka till valfri mapp under roten /content/dam/.

   1. I **[!UICONTROL Workfront API Key]** ruta, ange [!UICONTROL Workfront] API-nyckel.

      Så här hämtar du [!DNL Workfront] API-nyckel:

      1. Öppna en webbläsarflik och logga in på [!DNL Workfront] konto som [!DNL Workfront] administratör.
      1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

      1. Klicka på **[!UICONTROL System]** >**[!UICONTROL Customer Info]**.

         Om du redan har genererat en API-nyckel kan du [!DNL Workfront] API-nyckeln visas under användarens API-nyckeletikett.

      1. (Villkorligt) Om du ännu inte har genererat någon API-nyckel måste du generera en:

         1. I **[!UICONTROL API Key Settings]** ska du se till att **[!UICONTROL After Creation, API keys expire in]** är inställt på Ingen.

            Om du väljer en förfalloperiod slutar kopplingen att fungera när API-nyckeln har upphört att gälla. Du måste sedan generera om en API-nyckel och uppdatera din [!DNL Workfront] konfiguration.

         1. Under **[!UICONTROL Your User's API Key]** etikett, klicka **[!UICONTROL Generate API Key]**.

            En API-nyckel för [!DNL Workfront] genererar och visar.
      1. Kopiera API-nyckeln till Urklipp.
      1. Öppna webbläsarfliken för AEM Connector och i **[!DNL Workfront API Key]** klistra in API-nyckeln som du kopierade.
   1. (Villkorligt) Klicka på **[!UICONTROL Advanced]** i det övre vänstra hörnet av [!UICONTROL [!DNL Workfront] Integration Configuration] och välj följande alternativ om tillämpligt:

      **[!UICONTROL Allow Collection Browsing]:**&#x200B; Välj det här alternativet om din organisation tillåter det [!DNL Workfront] användare länka AEM Assets-samlingar till [!DNL Workfront] objekt.

      **[!UICONTROL User Federated ID]:** Välj det här alternativet om din organisation använder Federated ID:n eller enkel inloggning (SSO) vid inloggning på Workfront.

      **[!UICONTROL Ignore Email Domain]:** Välj det här alternativet om dina AEM inte använder domännamnet i sitt användar-ID.

      **[!UICONTROL Restrict Access]:** Välj det här alternativet för att ange lämplig [!DNL Workfront] IP-adresser som måste läggas till i tillåtelselista. Mer information om tillåtelselista finns i [Konfigurera brandväggens tillåtelselista](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   1. Klicka på **[!UICONTROL Basic]** i det övre vänstra hörnet på sidan Konfiguration av Workfront-integrering och klicka sedan på **[!UICONTROL Connect]**.

      >[!NOTE]
      >
      >Det kan ta en stund innan ändringarna tillämpas. Det kan gå snabbare att starta om paketet.



1. (Villkorligt) Om du redan har skapat en [!DNL Workfront] molnkonfigurationsfil, välj **[!UICONTROL Global-[!DNL Workfront]]** och sedan i det övre vänstra hörnet klickar du på **[!UICONTROL Properties]**.

1. Generera AEM API-nyckel genom att klicka på **[!UICONTROL Generate Key],** kopiera sedan AEM API-nyckeln till Urklipp.

   Du behöver AEM API-nyckeln senare när du konfigurerar [!UICONTROL Workfront] integrera med [!UICONTROL AEM Assets]. Mer information finns i [Konfigurera Workfront för integrering med AEM](#configure-workfront-to-integrate-with-aem-assets).

1. Klicka på i det övre högra hörnet **[!UICONTROL Save]**.

   The [!UICONTROL Global-[!DNL Workfront]] visas.

   ![Properties.png](assets/properties-350x117.png)

1. (Valfritt) Synkronisera dubbelriktad kommunikation mellan AEM och [!DNL Workfront].

   1. Klicka på **[!UICONTROL Global-[!DNL Workfront]].**
   1. Klicka i fönstrets övre vänstra hörn på **[!UICONTROL Properties]**.

      The [!UICONTROL [!DNL Workfront] Integration Configuration] visas.

      ![Egenskaper2.png](assets/properties2-350x444.png)

   1. (Valfritt) Aktivera synkronisering av kommentarer mellan [!UICONTROL AEM Assets] och [!DNL Workfront], klicka **[!UICONTROL Enable Comment Sync]**.

      >[!IMPORTANT]
      >
      >Du måste aktivera [!UICONTROL Document Sync] för att synkronisera resurserna.

   1. (Valfritt) Om du vill inaktivera kommentarsynkronisering klickar du på **[!UICONTROL Disable Comment Sync].**

      eller

      Ta bort [!UICONTROL NOTE CREATE] en prenumeration registrerad på din AEM.

      Mer information om händelseprenumerationer finns i [API för händelseprenumeration](../../wf-api/general/event-subs-api.md).

1. Fortsätt med [Konfigurera [!UICONTROL AEM Externalizer]](#configure-the-aem-externalizer).

### Konfigurera [!UICONTROL AEM Externalizer] {#configure-the-aem-externalizer}

The [!UICONTROL AEM Externalizer] tillåter AEM att skicka URL:er i ett format som kan användas i [!DNL Workfront]. Om den inte är korrekt konfigurerad [!DNL Workfront] kan inte anropa AEM-API:t, och URL:er som länkar AEM dokument i Workfront fungerar inte.

1. I AEM klickar du på **[!UICONTROL Tools]** > **[!UICONTROL Operations]** >**[!UICONTROL Web Console]**.

1. Klicka **[!UICONTROL OSGI]** och sedan klicka **[!UICONTROL Configuration]** i listrutan.

1. Välj &#x200B; i konfigurationslistan **[!UICONTROL Day CQ Link Externalizer].**

   The [!UICONTROL Externalizer] visas.

1. I **[!UICONTROL Domains]** kontrollerar du att domänen som anges i [!UICONTROL Author] -fältet är det domännamn som är externt tillgängligt för AEM användare.

   Domännamnet i [!UICONTROL author] ska matcha domänen som anges på URL-raden för din AEM.

   ![[!DNL Extenalizer].png](assets/extenalizer-350x128.png)

1. (Villkorligt) Uppdatera domänen i [!UICONTROL Author] fält.
1. Klicka på **[!UICONTROL Save]**.

   [!UICONTROL AEM Assets] är nu konfigurerat att länka dokument med [!DNL Workfront]

1. Fortsätt med [Konfigurera [!DNL Workfront] integrera med [!DNL AEM assets]](#configure-workfront-to-integrate-with-aem-assets).

## Konfigurera [!DNL Workfront] integrera med [!DNL AEM assets] {#configure-workfront-to-integrate-with-aem-assets}

När du har installerat [!UICONTROL Workfront for AEM Assets] Koppling (enligt beskrivning i [Installera [!UICONTROL Workfront for AEM Assets] kopplingspaket](#install-the-workfront-for-aem-assets-connector-package)) och konfigurera [!UICONTROL AEM Assets] (enligt beskrivning i [Konfigurera[!UICONTROL  AEM Assets] integrera med [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront)) måste du konfigurera [!DNL Workfront] för att länka dokument mellan [!DNL Workfront] och [!DNL AEM Assets].

1. Logga in på [!DNL Workfront] som [!UICONTROL Workfront] administratör.

   >[!TIP]
   >
   >[!UICONTROL Workfront] rekommenderar att du skapar [!UICONTROL Workfront] administratör som enbart är dedikerad för din AEM. Mer information om hur du tilldelar [!UICONTROL Workfront] administratörsåtkomstnivå för en användare, se [Ge användarna administrativ åtkomst till vissa områden](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på **[!UICONTROL Documents]**> **[!UICONTROL Custom Integration].**

1. Klicka på **[!UICONTROL Add Custom Integration]**.
1. I **[!UICONTROL Name]** anger du namnet på den anpassade integrationen.

   Det här är namnet som användarna ser när de använder integreringen i [!UICONTROL Workfront]; Du kan till exempel skriva *&quot;[!DNL AEM Assets]&quot;* för namnet.

1. I **[!UICONTROL Base API URL]** anger du URL:en för AEM.

   Bas-API-URL:en består av URL:en för din AEM-instans följt av sökvägen: /bin/webhooks/api/

   ![mceclip3.png](assets/mceclip3-350x130.png)

1. I **[!UICONTROL Authentication Type]** nedrullningsbar meny, välja **[!UICONTROL ApiKey].**

1. I &#x200B;**[!UICONTROL API Key]** , klistra in AEM API-nyckel som du kopierade när du konfigurerade [!UICONTROL AEM Assets].
1. Klicka på **[!UICONTROL Save]**.
1. (Valfritt) Se till att integreringen är markerad [!UICONTROL Active].\
   ![aem_custom_integration_active.png](assets/aem-custom-integration-active-350x81.png)

   [!DNL Workfront] är nu konfigurerat att fungera med [!DNL AEM Assets].

   För att få åtkomst till resurser i AEM [!DNL Workfront] användare som behöver använda anslutningen måste ställas in som användare i AEM. Mer information om hur du skapar användare finns i  [Konfigurera användare att använda kopplingen](#set-up-users-to-use-the-connector).

## Konfigurera användare att använda kopplingen {#set-up-users-to-use-the-connector}

Användarna måste ha en användarprofil i AEM och tillhöra en [!DNL Workfront] grupp som har åtkomstnivåer som innehåller [!UICONTROL Create] och [!UICONTROL Delete] behörigheter.

Mer information om [!DNL Workfront] behörigheter, se [Skapa eller ändra anpassade åtkomstnivåer](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* [Konfigurera användare i [!DNL AEM assets]](#set-up-users-in-aem-assets)

### Konfigurera användare i [!DNL AEM assets] {#set-up-users-in-aem-assets}

1. Logga in på [!DNL AEM Assets] som [!DNL Workfront] administratör.
1. Klicka på **[!UICONTROL Tools]** >**&#x200B;**&#x200B;**[!UICONTROL Security]** >**[!UICONTROL Users]**.

1. (Villkorligt) Om användaren inte har någon användarprofil i AEM skapar du en AEM användarprofil.

   1. Klicka på **[!UICONTROL Create User].**
   1. Ange användarens personliga information.

      ![64NewUser.png](assets/64newuser-350x524.png)

      Det enda obligatoriska fältet är ID-fältet. Användarens AEM-ID måste matcha deras [!DNL Workfront] ID, som är användarens [!DNL Workfront] e-postadress.

      Om du valde [!UICONTROL Ignore Email Domain] när du har konfigurerat AEM att integrera med [!DNL Workfront], kommer AEM-ID inte att matcha [!DNL Workfront] e-postadress.

1. (Villkorligt) Om användaren har en AEM profil öppnar du användarens AEM.

   1. Klicka på&#x200B;**[!UICONTROL User].**

      The [!UICONTROL User Management] visas.

   1. Klicka på den användare som du vill lägga till och klicka sedan på **[!UICONTROL Properties]**.

      Användarens inställningssida visas.

1. Klicka på **[!UICONTROL Groups]** -fliken.

   ![](assets/groupstab.png)

1. Se till att användaren tillhör minst en [!DNL Workfront] grupp som har åtkomstnivåer som innehåller [!UICONTROL Create] och [!UICONTROL Delete] behörigheter.

   1. Om du vill lägga till användaren i en befintlig grupp börjar du med att skriva gruppnamnet i **[!UICONTROL Type Group Name]** markerar du gruppen när den visas i listrutan.

      eller

      Om du vill välja en grupp som användaren är medlem i väljer du en grupp i **[!UICONTROL Groups that this user is a member of]** -avsnitt.

1. Klicka på **[!UICONTROL Save].**

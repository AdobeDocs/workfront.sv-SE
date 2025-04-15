---
title: Konfigurera [!DNL Workfront] med [!DNL Adobe Experience Manager] Äldre anslutning
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Som  [!DNL Adobe Workfront] administratör kan du integrera [!DNL Workfront] med Adobe Experience Manager (AEM) Assets och ge din organisation en omfattande innehållshanteringslösning för att skapa, dela och underhålla resurser i ditt arbetsflöde.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 024b8606-a9b7-413a-b393-8e5cdff37dd4
source-git-commit: 5d818b2e3c3314c6af076df46f7f806214f97bab
workflow-type: tm+mt
source-wordcount: '1648'
ht-degree: 0%

---

# Konfigurera [!DNL Workfront] med [!DNL Adobe Experience Manager] äldre anslutning

Som [!DNL Adobe Workfront]-administratör kan du integrera [!DNL Workfront] med [!UICONTROL Adobe Experience Manager (AEM) Assets] och ge din organisation en omfattande innehållshanteringslösning för att skapa, dela och underhålla resurser i ditt arbetsflöde.

## Åtkomstkrav

<!-- Audited: 4/2025 -->

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

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
   <td><p>Nytt: Standard</p>
   <p>eller</p>
   <p>Aktuell: Planera</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>Systemadministratör </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## [!DNL Workfront for AEM Assets]

Med [!DNL Workfront for AEM Assets connector] kan din organisation göra följande:

* Samarbeta och hantera kreativt innehåll genom att länka AEM resurser och mappar till projekt, uppgifter, problem och förfrågningar i [!DNL Workfront].

  Mer information om hur du konfigurerar dokumentintegreringar med tredjepartsprogram finns i [Konfigurera dokumentintegreringar](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

* Integrera med DAM-databasen ([!DNL AEM Digital Asset Managemen]t) så att du kan använda [!DNL Workfront] för att hantera och dela digitala resurser som lagras i DAM.

  Mer information om hur du länkar dokument och resursmappar finns i   [Länka dokument från externa program](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

* Kombinera och använd metadata från båda programmen på en resurs.
* Visa en heltäckande kommunikationsström för en tillgång. Uppdateringar och kommentarer som görs för en resurs i [!DNL Workfront] eller [!UICONTROL AEM Assets] synkroniseras med det andra programmet, vilket skapar en omfattande historik över kommunikation som gjorts för resursen.

  Mer information om att göra kommentarer i [!DNL Workfront] finns i [Lägga till en uppdatering i ett dokument](../../documents/managing-documents/add-update-documents.md).

## Krav för installation av [!DNL AEM Assets]-anslutningen

Innan du kan installera [!DNL Workfront]-anslutningen för [!UICONTROL AEM Assets] måste du kontrollera att följande krav uppfylls:

* [!UICONTROL AEM Assets] är installerat och konfigurerat, version 6.5 eller senare. Mer information om hur du installerar [!UICONTROL AEM Assets] finns i [[!DNL Adobe Experience Manager] dokumentationen](https://experienceleague.adobe.com/docs/experience-manager.html).
* (Villkorligt) Om brandväggsreglerna inte tillåter trafik som förväntat lägger du till klustrets IP-adress och/eller domän i tillåtelselista. Mer information finns i [Konfigurera brandväggens tillåtelselista](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Installera [!DNL Workfront for AEM Assets]-anslutningspaketet {#install-the-workfront-for-aem-assets-connector-package}

>[!IMPORTANT]
>
>Följande instruktioner gäller för en [!DNL Workfront with AEM Assets]-äldre koppling, som har ersatts av den [[!DNL Workfront for Experience Manager] förbättrade kopplingen](../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-for-aem-enhanced-connector.md). Kontakta din kontorepresentant om du vill ha mer information.

Om du vill installera [!DNL Workfront for AEM Assets]-anslutningen måste du importera kopplingen till AEM som ett paket med hjälp av [!UICONTROL CRX Package Manager].

1. Hämta installationsfilen för [!DNL Workfront for AEM Assets] Connector på en arbetsstation där du redan har installerat AEM.

   Du kan hämta [!DNL Workfront for AEM Assets]-anslutningen från din [!DNL Workfront]-representant.

1. Logga in på AEM med ett administratörskonto.
1. Klicka på **[!UICONTROL Tools]** > **[!UICONTROL Deployment]** > **[!UICONTROL Packages]**. [!UICONTROL CRX Package Manager] öppnas.

1. Klicka på **[!UICONTROL Upload Package].**

1. Bläddra efter och markera paketet **[!UICONTROL Workfront Connector]** i dialogrutan **[!UICONTROL Upload Package]** och klicka sedan på **[!UICONTROL OK]**. Paketet visas i [!UICONTROL CRX Package Manager].

1. Klicka på **[!UICONTROL Install].**

1. Ignorera de avancerade inställningarna i dialogrutan **[!UICONTROL Package]** och klicka på **[!UICONTROL Install]**.
1. (Valfritt) Kontrollera att följande programsats visas i [!UICONTROL Activity Log] för att bekräfta att anslutningen har installerats:

   ```
   Package installed in <time>
   ```

1. Stäng [!UICONTROL CRX Package Manager]. Kopplingen är installerad och du kan nu konfigurera [!DNL AEM Assets] för integrering med [!DNL Workfront].

1. Fortsätt med [Konfigurera [!DNL AEM Assets] för integrering med [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront).

## Konfigurera [!DNL AEM Assets] för integrering med [!DNL Workfront] {#configure-aem-assets-to-integrate-with-workfront}

När du har installerat anslutningsprogrammet importerar du anslutningsprogrammet till AEM och konfigurerar AEM att länka med dokument i [!DNL Workfront].

Information om hur du installerar anslutningsprogrammet finns i [Installera  [!DNL Workfront for AEM Assets] anslutningsprogrammet](#install-the-workfront-for-aem-assets-connector-package).

* [Förutsättningar](#prerequisites)
* [Integrera AEM med  [!DNL Workfront]](#integrate-aem-with-workfront)
* [Konfigurera [!UICONTROL AEM Externalizer]](#configure-the-aem-externalizer)

### Förutsättningar {#prerequisites}

Innan du börjar måste du aktivera behörigheter för Workfront Service:

1. Gå till **[!UICONTROL Tools]** > **[!UICONTROL Security]** > **[!UICONTROL Permissions]** i AEM.
1. I det övre vänstra hörnet väljer du **[!UICONTROL Users]** &#x200B; i listrutan och anger *[!UICONTROL workfront-service]* i &#x200B; **[!UICONTROL Search]** . Välj användaren [!UICONTROL workfront-service].
1. Välj **[!UICONTROL Add ACE]** till höger på skärmen för att skapa nya poster.
1. I fönstret &#x200B;**[!UICONTROL Add New Entry]** &#x200B; markerar du kryssruteikonen i &#x200B; **[!UICONTROL Path]** och väljer mappen: */conf*
1. I fältet **Behörigheter** anger du: *jcr:read*
1. Välj **[!UICONTROL Add]** &#x200B; i det övre högra hörnet.
1. (Valfritt) Upprepa stegen ovan om du vill skapa fler poster.

### Integrera AEM med [!DNL Workfront] {#integrate-aem-with-workfront}

1. Logga in på AEM Assets som administratör.
1. Klicka på **[!UICONTROL Tools]** > **[!UICONTROL Cloud Services]** > **[!UICONTROL Workfront Integration Configuration]** > **[!UICONTROL Global-Workfront].** &#x200B;**&#x200B;**

1. (Villkorligt) Om du inte har gjort det än skapar du en [!DNL Workfront]-molnkonfigurationsfil:

   1. Klicka på **[!UICONTROL Create]** i det övre högra hörnet på sidan [!DNL Global-Workfront].
   1. I rutan **[!UICONTROL Workfront URL]** anger du URL:en för [!DNL Workfront]-instansen.

      Exempel: [!DNL https]://`<account>`.my.workfront.com, där `<account>` är det konto du använder för integreringar med AEM.

   1. Markera kryssruteikonen i fältet &#x200B;**[!UICONTROL Base Folder]**.
   1. I listrutan väljer du den sökväg där dokument som är länkade till [!DNL Workfront]-objekt lagras.
   1. I AEM modal som visas följer du sökvägen till mappen med dokumenten som är anslutna till [!DNL Workfront]-objekt. Välj mappen och tryck sedan på **[!UICONTROL Select]** &#x200B; i det övre högra hörnet.

      Du kan länka till valfri mapp under roten /content/dam/.

   1. Ange [!UICONTROL Workfront] API-nyckeln i rutan **[!UICONTROL Workfront API Key]**.

      Så här hämtar du [!DNL Workfront] API-nyckeln:

      1. Öppna en webbläsarflik och logga in på ditt [!DNL Workfront]-konto som [!DNL Workfront]-administratör.

      {{step-1-to-setup}}

      1. Klicka på **[!UICONTROL System]** > **[!UICONTROL Customer Info]**.

         Om du redan har genererat en API-nyckel visas [!DNL Workfront] API-nyckeln under **användarens API-nyckel**-etikett.

      1. (Villkorligt) Om du ännu inte har genererat någon API-nyckel måste du generera en:

         1. Kontrollera att alternativet **[!UICONTROL After Creation, API keys expire in]** är **Inget** i avsnittet **[!UICONTROL API Key Settings]**.

            Om du väljer en förfalloperiod slutar kopplingen att fungera när API-nyckeln har upphört att gälla. Du måste sedan återskapa en API-nyckel och uppdatera din [!DNL Workfront]-konfiguration.

         1. Klicka på **[!UICONTROL Generate API Key]** under etiketten **[!UICONTROL Your User's API Key]**. En API-nyckel för [!DNL Workfront] genererar och visar.
      1. Kopiera API-nyckeln till Urklipp.
      1. Öppna webbläsarfliken för AEM Connector och klistra sedan in API-nyckeln som du kopierade i rutan **[!DNL Workfront API Key]**.
   1. (Villkorligt) Klicka på fliken **[!UICONTROL Advanced]** i det övre vänstra hörnet på sidan [!UICONTROL [!DNL Workfront] Integration Configuration] och välj följande alternativ om tillämpligt:

      **[!UICONTROL Allow Collection Browsing]:** &#x200B; Välj det här alternativet om din organisation tillåter [!DNL Workfront]-användare att länka AEM Assets-samlingar till [!DNL Workfront] objekt.

      **[!UICONTROL User Federated ID]:** Välj det här alternativet om din organisation använder Federated ID eller enkel inloggning (SSO) vid inloggning på Workfront.

      **[!UICONTROL Ignore Email Domain]:** Välj det här alternativet om dina AEM-användare inte använder domännamnet i sitt användar-ID.

      **[!UICONTROL Restrict Access]:** Välj det här alternativet om du vill ange lämpliga [!DNL Workfront] IP-adresser som ska läggas till i tillåtelselista. Mer information om tillåtelselista finns i [Konfigurera tillåtelselista för brandväggen](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   1. Klicka på fliken **[!UICONTROL Basic]** i det övre vänstra hörnet på konfigurationssidan för Workfront-integrering och klicka sedan på **[!UICONTROL Connect]**.

      >[!NOTE]
      >
      >Det kan ta en stund innan ändringarna tillämpas. Det kan gå snabbare att starta om paketet.



1. (Villkorligt) Om du redan har skapat en [!DNL Workfront] molnkonfigurationsfil väljer du **[!UICONTROL Global-[!DNL Workfront]]** och klickar sedan på **[!UICONTROL Properties]** i det övre vänstra hörnet.

1. Generera AEM API-nyckeln genom att klicka på **[!UICONTROL Generate Key],** och sedan kopiera AEM API-nyckeln till Urklipp.

   Du behöver AEM API-nyckeln senare när du konfigurerar [!UICONTROL Workfront] för integrering med [!UICONTROL AEM Assets]. Mer information finns i [Konfigurera Workfront för integrering med AEM-resurser](#configure-workfront-to-integrate-with-aem-assets).

1. Klicka på **[!UICONTROL Save]** i det övre högra hörnet. Fönstret [!UICONTROL Global-[!DNL Workfront]] visas.

   ![Properties.png](assets/properties-350x117.png)

1. (Valfritt) Synkronisera dubbelriktad kommunikation mellan AEM och [!DNL Workfront]:

   1. Klicka på **[!UICONTROL Global-[!DNL Workfront]].**
   1. Klicka på **[!UICONTROL Properties]** i fönstrets övre vänstra hörn. Sidan **[!UICONTROL [!DNL Workfront] Integration Configuration]** visas.

      ![Properties2.png](assets/properties2-350x444.png)

   1. (Valfritt) Om du vill aktivera synkronisering av kommentarer mellan [!UICONTROL AEM Assets] och [!DNL Workfront] klickar du på **[!UICONTROL Enable Comment Sync]**.

      >[!IMPORTANT]
      >
      >Du måste aktivera [!UICONTROL Document Sync] för att synkronisera resurserna.

   1. (Valfritt) Om du vill inaktivera kommentarsynkronisering klickar du på **[!UICONTROL Disable Comment Sync].**

      eller

      Ta bort den [!UICONTROL NOTE CREATE]-händelseprenumeration som är registrerad på din AEM-instans.

      Mer information om händelseprenumerationer finns i [API för händelseprenumeration](../../wf-api/general/event-subs-api.md).

1. Fortsätt med [Konfigurera [!UICONTROL AEM Externalizer]](#configure-the-aem-externalizer).

### Konfigurera [!UICONTROL AEM Externalizer] {#configure-the-aem-externalizer}

[!UICONTROL AEM Externalizer] tillåter att AEM skickar URL:er i ett format som kan användas i [!DNL Workfront]. Om den inte är korrekt konfigurerad kan [!DNL Workfront] inte ringa anrop till AEM API, och URL:erna som länkar AEM-dokument i Workfront fungerar inte.

1. I AEM klickar du på **[!UICONTROL Tools]** > **[!UICONTROL Operations]** > **[!UICONTROL Web Console]**.

1. Klicka på **[!UICONTROL OSGI]** och sedan på **[!UICONTROL Configuration]** i listrutan.

1. Välj &#x200B;**[!UICONTROL Day CQ Link Externalizer]i konfigurationslistan.** Sidan **[!UICONTROL Externalizer]** visas.

1. I avsnittet **[!UICONTROL Domains]** ser du till att domänen som visas i fältet **[!UICONTROL Author]** är det domännamn som är externt tillgängligt för AEM-användare.

   Domännamnet i fältet [!UICONTROL author] ska matcha domänen som anges på URL-raden för din AEM-instans.

   ![[!DNL Extenalizer].png](assets/extenalizer-350x128.png)

1. (Villkorligt) Uppdatera domänen i fältet **[!UICONTROL Author]** om det behövs.
1. Klicka på **[!UICONTROL Save]**. [!UICONTROL AEM Assets] har nu konfigurerats för att länka dokument med [!DNL Workfront].

1. Fortsätt med [Konfigurera [!DNL Workfront] för integrering med [!DNL AEM assets]](#configure-workfront-to-integrate-with-aem-assets).

## Konfigurera [!DNL Workfront] för integrering med [!DNL AEM assets] {#configure-workfront-to-integrate-with-aem-assets}

När du har installerat [!UICONTROL Workfront for AEM Assets] Connector (enligt beskrivningen i [ Installera [!UICONTROL Workfront for AEM Assets]-anslutningspaketet](#install-the-workfront-for-aem-assets-connector-package)) och konfigurerat [!UICONTROL AEM Assets] (enligt beskrivningen i [Konfigurera[!UICONTROL  AEM Assets] för integrering med  [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront)) måste du konfigurera [!DNL Workfront] för att länka dokument mellan [!DNL Workfront] och [!DNL AEM Assets].

1. Logga in på Workfront som administratör.

   >[!TIP]
   >
   >[!UICONTROL Workfront] rekommenderar att du skapar en [!UICONTROL Workfront]-administratör som är dedikerad enbart till din AEM-integrering. Mer information om hur du tilldelar [!UICONTROL Workfront]-administratörsåtkomstnivån till en användare finns i [Bevilja användare administrativ åtkomst till vissa områden](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Documents]** > **[!UICONTROL Custom Integration].**

1. Klicka på **[!UICONTROL Add Custom Integration]**.
1. Ange namnet på den anpassade integrationen i rutan **[!UICONTROL Name]**.

   Det här namnet visas för användarna när integreringen används i [!UICONTROL Workfront].

1. Ange URL-adressen för din AEM-instans i rutan **[!UICONTROL Base API URL]**.

   Bas-API-URL:en består av URL:en för din AEM-instans följt av sökvägen: /bin/webhooks/api/

   ![mceclip3.png](assets/mceclip3-350x130.png)

1. I listrutan **[!UICONTROL Authentication Type]** väljer du **[!UICONTROL ApiKey].**

1. Klistra in AEM API-nyckeln som du kopierade när du konfigurerade [!UICONTROL AEM Assets] i rutan &#x200B;**[!UICONTROL API Key]**.
1. Klicka på **[!UICONTROL Save]**.
1. (Valfritt) Kontrollera att integreringen är markerad som [!UICONTROL Active].\
   ![aem_custom_integration_active.png](assets/aem-custom-integration-active-350x81.png)

   [!DNL Workfront] har nu konfigurerats för att fungera med [!DNL AEM Assets].

   För att kunna komma åt resurser i AEM måste varje [!DNL Workfront]-användare som behöver använda anslutningen konfigureras som en användare i AEM. Mer information om hur du skapar användare finns i [Konfigurera användare att använda anslutningen](#set-up-users-to-use-the-connector).

## Konfigurera användare att använda kopplingen {#set-up-users-to-use-the-connector}

För att användare ska kunna komma åt anslutningen måste de ha en användarprofil i AEM och tillhöra en [!DNL Workfront]-grupp som har åtkomstnivåer som inkluderar behörigheterna [!UICONTROL Create] och [!UICONTROL Delete].

Mer information om [!DNL Workfront] behörigheter finns i [Skapa eller ändra anpassade åtkomstnivåer](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* [Konfigurera användare i  [!DNL AEM assets]](#set-up-users-in-aem-assets)

### Konfigurera användare i [!DNL AEM assets] {#set-up-users-in-aem-assets}

1. Logga in på [!DNL AEM Assets] som Workfront-administratör.
1. Klicka på **[!UICONTROL Tools]** > **&#x200B;** &#x200B;**[!UICONTROL Security]** > **[!UICONTROL Users]**.

1. (Villkorligt) Om användaren inte har någon användarprofil i AEM skapar du en AEM-användarprofil.

   1. Klicka på **[!UICONTROL Create User].**
   1. Ange användarens personliga information.

      ![64NewUser.png](assets/64newuser-350x524.png)

      Det enda obligatoriska fältet är fältet **ID**. Användarens AEM-ID måste matcha användarens [!DNL Workfront]-ID, som är användarens [!DNL Workfront]-e-postadress.

      Om du valde alternativet **[!UICONTROL Ignore Email Domain]** när du konfigurerade AEM att integrera med [!DNL Workfront], kommer AEM-ID:t inte att matcha e-postadressen [!DNL Workfront].

1. (Villkorligt) Om användaren har en AEM-profil öppnar du användarens AEM-profil:

   1. Klicka på &#x200B;**[!UICONTROL User]**. Sidan **[!UICONTROL User Management]** visas.

   1. Klicka på den användare som du vill lägga till och klicka sedan på **[!UICONTROL Properties]**. Användarens inställningssida visas.

1. Klicka på fliken **[!UICONTROL Groups]**.

   ![Fliken Grupper](assets/groupstab.png)

1. Se till att användaren tillhör minst en [!DNL Workfront]-grupp som har åtkomstnivåer som innehåller behörigheterna **[!UICONTROL Create]** och **[!UICONTROL Delete]**.

   1. Om du vill lägga till användaren i en befintlig grupp börjar du skriva gruppnamnet i rutan **[!UICONTROL Type Group Name]** och markerar sedan gruppen när den visas i listrutan.

      eller

      Om du vill välja en grupp som användaren är medlem i, markerar du en grupp i avsnittet **[!UICONTROL Groups that this user is a member of]**.

1. Klicka på **[!UICONTROL Save].**

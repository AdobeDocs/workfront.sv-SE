---
title: Uppdatera SAML 2.0-metadata i din IDP med förbättrad autentisering
description: Som Adobe Workfront-administratör kan du integrera Workfront single sign-on (SSO) med alla identitetsleverantörer som stöder SAML 2.0-protokollet (Security Assertion Markup Language).
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 55d7d8a8-0dfe-45bc-a23a-47111347e9ca
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 0%

---

# Uppdatera SAML 2.0-metadata i din IDP med förbättrad autentisering

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Som Adobe Workfront-administratör kan du integrera Workfront single sign-on (SSO) med alla identitetsleverantörer som stöder SAML 2.0-protokollet (Security Assertion Markup Language).

I följande avsnitt beskrivs integrationsprocessen när ditt Workfront-konto har uppgraderats till den förbättrade autentiseringsupplevelsen (som ännu inte är tillgänglig för alla organisationer). Mer information om den förbättrade autentiseringen finns i [Översikt över utökad autentisering](../../../administration-and-setup/manage-workfront/security/get-started-enhanced-authentication.md).

Mer information om hur du konfigurerar SAML innan du migrerar till det förbättrade autentiseringsgränssnittet finns i [Uppdatera SAML 2.0-metadata hos identitetsleverantören](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).


## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Använd Okta som identitetsleverantör

Okta är ett exempel på en identitetsleverantör som stöder SAML 2.0. I det här avsnittet beskrivs hur du använder Okta som identitetsleverantör. Liknande steg krävs när en annan identitetsleverantör som stöder SAML 2.0 konfigureras.

>[!NOTE]
>
>Användare mappas baserat på deras e-postadress. För att kunna logga in på Workfront med Okta måste du ha en användare med samma (skiftlägesokänslig) e-postadress som skapats hos din Workfront-kund.

Slutför följande avsnitt för att konfigurera Okta som din identitetsleverantör i Workfront.

* [Skapa en Workfront-app i Okta](#create-a-workfront-app-in-okta)
* [Lägg till din Okta-instans som en identitetsleverantör i Workfront](#add-your-okta-instance-as-an-identity-provider-in-workfront)

### Skapa en Workfront-app i Okta {#create-a-workfront-app-in-okta}

1. Logga in i din Okta-miljö.
1. Se till att **Klassiskt användargränssnitt** markeras i det övre vänstra hörnet av Okta-gränssnittet.
1. Klicka på **Program** > **Program**.

1. Klicka **Lägg till program** och sedan klicka **Skapa ny app**.

1. I **Skapa en ny dialogruta för programintegrering** ruta, markera **SAML 2.0** och sedan klicka **Skapa**.

1. Ange ett namn för din Workfront-app och klicka sedan på **Nästa**.
1. På sidan SAML-inställningar som visas letar du reda på den information som krävs för sidan SAML-inställningar:

   1. Öppna en separat webbläsarflik eller ett separat fönster utan att stänga webbläsarfliken där Okta-gränssnittet visas.
   1. Ange följande URL i webbläsaren:

      `https://[your_customer_subdomain].my.workfront.com/auth/saml2/metadata`

   1. Identifiera värdena för **entityID** och **Plats**.

      ![sso-okta.png](assets/sso-okta.png)

   1. Kopiera värdet från **entityID** till systemets Urklipp. Stäng inte den här webbläsarfliken.

1. Gå tillbaka till sidan SAML-inställningar som du öppnade i steg 6.
1. Klistra in värdet från **entityID** till **Målgrupps-URI (SP-enhets-ID)** fält.

1. Kopiera värdet från XML-filen på den andra webbläsarfliken **Plats** fält.
1. Klistra in värdet från **Plats** till **Enkel inloggning** **URL** fält.

1. Bläddra till **Attributsatser (valfritt)** -avsnitt.
1. I **Namn** fält, ange **e-post**.

1. I **Värde** fält, ange **user.email**.

1. (Valfritt) Lägg till eventuella avancerade värden.
1. Klicka **Nästa**.
1. Välj, **Jag är en Okta-kund som lägger till en intern app** och sedan klicka **Slutför**.

### Lägg till din Okta-instans som en identitetsleverantör i Workfront {#add-your-okta-instance-as-an-identity-provider-in-workfront}

Den här proceduren ger viktig information för att konfigurera Okta som identitetsleverantör i Workfront. Mer information om andra mappningar eller konfigurationsalternativ finns i [Konfigurera Adobe Workfront med SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

1. Hämta identitetsleverantörens metadata för din Okta-instans:

   1. Logga in i din Okta-miljö.
   1. Se till att **Klassiskt användargränssnitt** markeras i det övre vänstra hörnet av Okta-gränssnittet.
   1. Klicka på **Program** > **Program**.

   1. Klicka på den Workfront-app du skapade, enligt beskrivningen i avsnittet, [Skapa en Workfront-app i Okta](#create-a-workfront-app-in-okta)
   1. På **Logga in** flik, klicka **Metadata för identitetsleverantör**.

      ![idp_okta_metadata.png](assets/idp-okta-metadata.png)

      Metadata öppnas som XML på en ny flik i webbläsaren.

   1. Kopiera URL-adressen som visas i webbläsarens URL-fält.

1. Logga in på Workfront som Workfront-administratör.
1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **System** > **enkel inloggning (SSO)**.

1. (Villkorligt) Om två flikar visas klickar du på **Nya SSO-providers** -fliken.

   ![sso_idp_halflife.png](assets/sso-idp-halflife-350x234.png)

   >[!IMPORTANT]
   >
   >Ta inte bort dina befintliga inställningar för enkel inloggning i dialogrutan **Aktuell SSO-provider** tills ditt konto har uppdaterats till det förbättrade autentiseringsupplevelsen och den nya SSO-konfigurationen fungerar helt.

1. Klicka **Ny SSO-provider**.
1. Ange ett namn, till exempel Okta IDP, och ange sedan en beskrivning.
1. I **Fyll i fält från identitetsleverantörens metadata** klistrar du in den URL som du kopierade i steg 1 i **Metadata URL** fält.\
   Du kan också klicka **Välj fil** om du vill överföra en XML-fil, men vi rekommenderar att du klistrar in URL-adressen.

1. I **Mappa användarattribut** i **Katalogattribut** fält, typ **e-post**. (**E-postadress** redan har fyllts i i **Workfront-användarattribut** fält.)

1. (Valfritt) Aktivera **Använd SSO-standardprovider** för att skicka oautentiserade användare till identitetsleverantörens inloggningsskärm i stället för till inloggningsskärmen för Workfront för autentisering. Vi rekommenderar att du bara aktiverar det här alternativet om alla användare i ditt system får tillgång till Workfront via identitetsleverantören.
1. Välj **Aktivera** kryssrutan. Innan du gör detta bör du se till att användarna i ditt system är medvetna om den nya inloggningsupplevelsen så att de inte förlorar åtkomsten till Workfront-systemet.
1. Klicka **Testanslutning**.\
   Du bör få ett meddelande om att anslutningen lyckades.

1. Klicka **Spara**.

## Använda andra identitetsleverantörer

När du använder andra identitetsleverantörer än Okta (till exempel Ping eller Centrify) måste du överföra Workfront-metadata på nytt till din identitetsleverantör.

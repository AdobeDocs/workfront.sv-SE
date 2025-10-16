---
title: Uppdatera SAML 2.0-metadata i din IDP med förbättrad autentisering
description: Som Adobe Workfront-administratör kan du integrera Workfront single sign-on (SSO) med alla identitetsleverantörer som stöder SAML 2.0-protokollet (Security Assertion Markup Language).
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 55d7d8a8-0dfe-45bc-a23a-47111347e9ca
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 75fea812b4574191522af4721a013b57aa5d609f
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 0%

---

# Uppdatera SAML 2.0-metadata i din IDP med förbättrad autentisering

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Som Adobe Workfront-administratör kan du integrera Workfront single sign-on (SSO) med alla identitetsleverantörer som stöder SAML 2.0-protokollet (Security Assertion Markup Language).

I följande avsnitt beskrivs integrationsprocessen när ditt Workfront-konto har uppgraderats till den förbättrade autentiseringsupplevelsen (som ännu inte är tillgänglig för alla organisationer). Mer information om den förbättrade autentiseringen finns i [Översikt över den förbättrade autentiseringen](../../../administration-and-setup/manage-workfront/security/get-started-enhanced-authentication.md).

Mer information om hur du konfigurerar SAML innan du migrerar till det förbättrade autentiseringsgränssnittet finns i [Uppdatera SAML 2.0-metadata i identitetsleverantören](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).


## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
1. Kontrollera att **Klassiskt användargränssnitt** har valts i det övre vänstra hörnet av Okta-gränssnittet.
1. Klicka på **Program** > **Program** på menyn.

1. Klicka på **Lägg till program** och sedan på **Skapa ny app**.

1. I dialogrutan **Skapa en ny programintegrering** väljer du **SAML 2.0** och klickar sedan på **Skapa**.

1. Ange ett namn för din Workfront-app och klicka sedan på **Nästa**.
1. På sidan SAML-inställningar som visas letar du reda på den information som krävs för sidan SAML-inställningar:

   1. Öppna en separat webbläsarflik eller ett separat fönster utan att stänga webbläsarfliken där Okta-gränssnittet visas.
   1. Ange följande URL i webbläsaren:

      `https://[your_customer_subdomain].my.workfront.com/auth/saml2/metadata`

   1. Identifiera värdena för **entityID** och **Location** i den resulterande XML-filen.

      ![sso-okta.png](assets/sso-okta.png)

   1. Kopiera värdet från fältet **entityID** till systemets Urklipp. Stäng inte den här webbläsarfliken.

1. Gå tillbaka till sidan SAML-inställningar som du öppnade i steg 6.
1. Klistra in värdet från fältet **entityID** i fältet **Audience URI (SP Entity ID)**.

1. Kopiera värdet från fältet **Plats** i XML-filen på den andra webbläsarfliken.
1. Klistra in värdet från fältet **Plats** i fältet **Enkel inloggning** **URL**.

1. Bläddra till avsnittet **Attributsatser (valfritt)**.
1. Ange **email** i fältet **Name**.

1. Ange **user.email** i fältet **Value**.

1. (Valfritt) Lägg till eventuella avancerade värden.
1. Klicka på **Nästa**.
1. Välj **Jag är en Okta-kund som lägger till en intern app** och klicka sedan på **Slutför**.

### Lägg till din Okta-instans som en identitetsleverantör i Workfront {#add-your-okta-instance-as-an-identity-provider-in-workfront}

Den här proceduren ger viktig information för att konfigurera Okta som identitetsleverantör i Workfront. Mer information om andra mappningar eller konfigurationsalternativ finns i [Konfigurera Adobe Workfront med SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

1. Hämta identitetsleverantörens metadata för din Okta-instans:

   1. Logga in i din Okta-miljö.
   1. Kontrollera att **Klassiskt användargränssnitt** har valts i det övre vänstra hörnet av Okta-gränssnittet.
   1. Klicka på **Program** > **Program** på menyn.

   1. Klicka på den Workfront-app som du skapade, enligt beskrivningen i avsnittet [Skapa en Workfront-app i Okta](#create-a-workfront-app-in-okta)
   1. Klicka på **Metadata för identitetsleverantör** på fliken **Logga in**.

      ![idp_okta_metadata.png](assets/idp-okta-metadata.png)

      Metadata öppnas som XML på en ny flik i webbläsaren.

   1. Kopiera URL-adressen som visas i webbläsarens URL-fält.

1. Logga in på Workfront som Workfront-administratör.

{{step-1-to-setup}}

1. Klicka på **System** > **enkel inloggning (SSO)** i den vänstra panelen.

1. (Villkorligt) Om två flikar visas klickar du på fliken **Nya SSO-providers** .

   ![sso_idp_halflife.png](assets/sso-idp-halflife-350x234.png)

   >[!IMPORTANT]
   >
   >Ta inte bort dina befintliga inställningar för enkel inloggning på fliken **Aktuell SSO-provider** förrän ditt konto har uppdaterats till den förbättrade autentiseringsupplevelsen och den nya SSO-konfigurationen fungerar helt.

1. Klicka på **Ny SSO-provider**.
1. Ange ett namn, till exempel Okta IDP, och ange sedan en beskrivning.
1. I avsnittet **Fyll i fält från Identity Provider Metadata** klistrar du in den URL som du kopierade i steg 1 i fältet **Metadata URL**.\
   Du kan också klicka på **Välj fil** om du vill överföra en XML-fil, men vi rekommenderar att du klistrar in URL:en.

1. I avsnittet **Mappa användarattribut** skriver du **email** i fältet **Katalogattribut**. (**E-postadress** har redan fyllts i i fältet **Workfront-användarattribut**.)

1. (Valfritt) Aktivera **Gör SSO-standardprovidern** för att skicka oautentiserade användare till identitetsleverantörens inloggningsskärm i stället för till inloggningsskärmen för Workfront för autentisering. Vi rekommenderar att du bara aktiverar det här alternativet om alla användare i ditt system får tillgång till Workfront via identitetsleverantören.
1. Markera kryssrutan **Aktivera**. Innan du gör detta bör du se till att användarna i ditt system är medvetna om den nya inloggningsupplevelsen så att de inte förlorar åtkomsten till Workfront-systemet.
1. Klicka på **Testa anslutning**.\
   Du bör få ett meddelande om att anslutningen lyckades.

1. Klicka på **Spara**.

## Använda andra identitetsleverantörer

När du använder andra identitetsleverantörer än Okta (till exempel Ping eller Centrify) måste du överföra Workfront-metadata på nytt till din identitetsleverantör.

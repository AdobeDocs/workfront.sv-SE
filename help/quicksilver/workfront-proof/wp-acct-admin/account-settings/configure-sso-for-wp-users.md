---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Konfigurera enkel inloggning för [!DNL Workfront Proof] användare
description: Om du har Select- eller Premium-planen kan du tillhandahålla enkel inloggning (SSO) som gör att du kan använda den befintliga organisationens användarnamn och lösenord för att få tillgång till din [!DNL Workfront Proof] konto.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 52ac1919-1821-424f-89f8-72865b236e4e
source-git-commit: 007a603ef1df2a02959d7fb623ac784bf5b9cb80
workflow-type: tm+mt
source-wordcount: '1234'
ht-degree: 0%

---

# Konfigurera enkel inloggning för [!DNL Workfront Proof] användare

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Om du har Select- eller Premium-planen kan du tillhandahålla enkel inloggning (SSO) som gör att du kan använda den befintliga organisationens användarnamn och lösenord för att få tillgång till din [!DNL Workfront Proof] konto.

Det innebär att du autentiserar mot ditt eget inloggningssystem, inte mot [!DNL Workfront Proof] inloggningssida.

>[!NOTE]
>
>Du måste ha konfigurerat en anpassad underdomän eller domän på din [!DNL Workfront Proof] konto för att aktivera SAML. Anpassade underdomäner kan konfigureras. Se [Varumärke](https://support.workfront.com/hc/en-us/sections/115000921208-Branding) för mer information.Du kan läsa mer om fullt anpassade domäner i våra [Varumärken [!DNL Workfront Proof] webbplats - avancerad](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

## Aktivera enkel inloggning inom [!DNL Workfront Proof]

Funktionen för enkel inloggning kan aktiveras på [!UICONTROL Single sign-on] -fliken i [!UICONTROL Account settings]och det gäller alla användare på [!DNL Workfront Proof] konto. Se [Kontoinställningar](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) för mer information.

## Enhets-ID

Som tjänsteleverantör har vi publicerat vårt enhets-ID här:

[https://yoursubdomain.proofhq.com/saml/module.php/saml/sp/metadata.php/phq](https://yoursubdomain.proofhq.com/saml/module.php/saml/sp/metadata.php/phq) (där &quot;din underdomän&quot; är ditt kontos underdomän)

[!DNL Workfront Proof] kräver användarens e-postadress som sin unika identifierare, som kan skickas som ett av följande attribut:

* urn:mace:dir:attribute-def:emailAddress
* http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress
* http://schemas.xmlsoap.org/claims/EmailAddress
* urn:oid:0.9.2342.19200300.100.1.3
* http://axschema.org/contact/email
* openid.sreg.email
* mail
* e-post
* emailAddress

Så här konfigurerar du enkel inloggning:

1. Öppna **[!UICONTROL Single Sign-On]** tab (1).
1. Ange **URL för enkel inloggning** (2).
Det här är länken till SSO-servern (till exempel **https://sso.mycompany.com/opensso**).

1. Ange **Inloggnings-URL** (3).
Det här är den URL som kommer att anropas för att dirigera om användarna till din identitetsleverantör.

1. Det här är inte en faktisk URL som du anger i webbläsaren, utan en slutpunkt som bearbetar den information som vi skickar för att visa inloggningsskärmen.

Ange **Utloggnings-URL** (4).
Detta är den URL som du kommer att returnera till efter att du loggat ut, till exempel

**https://www.yourcompany.com/services/logout.asp**

1. Ange **Intygets fingeravtryck** (5).
1. SHA1-fingeravtryck för SAML-certifikatet som tillhandahålls av din SAML-identitetsleverantör.
1. Se till att du inkluderar nyckelinformationen genom att ange detta för din identitetsleverantör.
1. Byt **SSO** till **[!UICONTROL Enabled]** (6).
När enkel inloggning är aktiverad loggar du in och andra användare på ditt konto med din egen autentiseringsmekanism. Det innebär att när användarna öppnar [!DNL Workfront Proof] inloggningsskärm för konto (till exempel **yourcompany.proofhq.com/login**) får de en uppmaning om att överföra till din inloggningssida för autentisering.

1. (Valfritt) Aktivera **Tillhandahåll användare automatiskt** (7).
När det här alternativet är aktiverat skapas användarkonton automatiskt för personer som inte har egna konton [!DNL Workfront Proof] -profiler, men kommer att ha tillgång till [!DNL Workfront Proof] med sina inloggningsuppgifter. Detta fungerar bara när användargränsen ännu inte har nåtts för ditt konto.

1. Nya användare som har etablerats får som standard hanterarprofilbehörigheterna tilldelade. Om du behöver mer information kan du läsa [Korrektur för behörighetsprofiler i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

![Enable_SSO_SAML_2.0.png](assets/enable-sso-saml-2.0-350x236.png)

## Aktivera enkel inloggning för satellitkonton

När du har satellitkonton anslutna till ditt navkonto kan du administrera dem från navkontonivån.

Single Sign-On är en Select- och Premium-funktion så enkel inloggning kan bara aktiveras på satelliter som finns i Select- och Premium-planer.

1. Klicka **[!UICONTROL Settings]** > **[!UICONTROL Account settings]** (1).

1. Klicka på satellitkontot i listrutan (2).
1. Öppna **[!UICONTROL Single Sign-On]** tabben (3).
1. Börja redigera SSO-konfigurationen (4).
1. ![Aktivera_SSO_-_Satellite_Account.png](assets/enabling-sso---satellite-account-350x266.png)
Här finns två konfigurationsmetoder (5):

1. **Ärvd:** enkel inloggning med konfigurationen som hämtats från ditt navkonto.
Om en användare har åtkomst [!DNL Workfront Proof] via **standardinloggningssida** ([https://www.proofhq.com/login](https://www.proofhq.com/login)) finns det **två behörighetsnivåer**: Först uppmanas användaren att logga in med [!DNL Workfront Proof] få tillgång till data (e-post och lösenord), sedan överförs användaren via ett SSO-fönster till inloggningssidan för enkel inloggning.
Om SSO-tjänsten är aktiverad rekommenderar vi att du loggar in via din egen [!DNL Workfront Proof] subdomän/domän.

   >[!NOTE]
   >
   >När enkel inloggning är aktiverad på din [!DNL Workfront Proof] kommer du inte att kunna logga in på iPhone-appen med dessa autentiseringsuppgifter.

   1. **Manuell** (standard): enkel inloggning med en annan konfiguration (t.ex. som pekar på en annan identitetsleverantör).

      >[!NOTE]
      >
      >Om satellitkontot ärver SSO-konfigurationen från navkontot blir inloggningsskärmen den för navkontot. När satellitkontoanvändaren anger sin inloggningsinformation för enkel inloggning på den här sidan dirigeras de tillbaka till satellitkontot.

      ![Aktivera_SSO_-_satellitkonto_2.png](assets/enabling-sso---satellite-account-2-350x224.png)

   1. Klicka **[!UICONTROL Save]** (6).

## SSO-inställningar ärvda från ett hubbkonto

När du väljer att ärva inställningarna från ditt hubbkonto kommer du att märka att alla fält nu fylls i med data från ditt hubbkonto (7) och att enkel inloggning automatiskt aktiveras/inaktiveras(8) som på ditt huvudkonto. Det finns inte längre några redigeringslänkar i fälten eftersom hela SSO-konfigurationen för satellitkontot nu har angetts och hanterats från ditt hubbkonto.

![Satellite_Account_-_Inherited_SSO.png](assets/satellite-account---inherited-sso-350x99.png)

På ditt hubbkonto (9) visas [!UICONTROL SSO Usage] visas att den här konfigurationen används av satellitkonton (10).\
![Hub_Account_-_Inherited_SSO.png](assets/hub-account---inherited-sso-350x275.png)

## SSO har konfigurerats manuellt

Om manuell konfiguration för enkel inloggning har valts för ett satellitkonto (1) måste du manuellt ange data för enkel inloggning.

1. Klicka **[!UICONTROL Settings]** > **[!UICONTROL Account settings]** (1).

1. Öppna **[!UICONTROL Single sign-on]** -fliken.
1. Klicka **[!UICONTROL Edit],** fylla i fältet och sedan klicka **[!UICONTROL Save]** (2).

1. På **[!UICONTROL SSO]** rad, klicka **[!UICONTROL Enabled]** (3).

![Satellite_Account_-_Manual_SSO.png](assets/satellite-account---manual-sso-350x280.png)

## SSO-inloggning

1. Klicka **[!UICONTROL Settings]** > **[!UICONTROL Account settings]** (1).

1. Öppna **[!UICONTROL Single sign-on]** -fliken.
1. Se till att [!DNL Workfront Proof] domän/underdomän (1) är konfigurerad och att dina användare har åtkomst till dina [!DNL Workfront Proof] via denna anpassade domän/underdomän.
   ![SAML_Subdomain.png](assets/saml-subdomain-350x150.png)
När enkel inloggning är aktiverad visar din subdomän-inloggnings-URL (t.ex. yourcompany.proofhq.com/login) en överföringsskärm (2) som tar dig direkt till inloggningssidan för enkel inloggning.
   ![SSO_login_page.png](assets/sso-login-page-350x164.png)

1. Om en användare har åtkomst [!DNL Workfront Proof] via **standardinloggningssida** ([https://www.proofhq.com/login](https://www.proofhq.com/login)) finns det **två behörighetsnivåer**. Först uppmanas användaren att logga in med [!DNL Workfront Proof] få åtkomst till data (e-post och lösenord). Användaren överförs sedan via ett SSO-fönster (2) till inloggningssidan för enkel inloggning.\
   Om SSO-tjänsten är aktiverad rekommenderar vi att du loggar in via din egen [!DNL Workfront Proof] subdomän/domän.

1. När enkel inloggning är aktiverad på ditt Workfront-korrekturkonto kan du för närvarande inte logga in på iPhone-appen med dessa autentiseringsuppgifter.

## Lägga till en ny användare

När funktionen för enkel inloggning är aktiverad på din [!DNL Workfront Proof] nya användare får inga bekräftelsemeddelanden eftersom deras konton aktiveras automatiskt och kan användas.

Från [!DNL Workfront Proof] inloggningssida, efter att du klickat på [!UICONTROL Login] kommer användarna till inloggningssidan för enkel inloggning och uppmanas att ange inloggningsuppgifterna för enkel inloggning.

>[!IMPORTANT]
>
>Användare identifieras via en e-postadress under autentiseringsprocessen, vilket innebär att e-postkontot som används för din SSO-inloggning måste vara e-postadressen till den användare som är registrerad i ditt konto.

## AD FS (Active Directory Federation Services)

AD FS (Active Directory Federation Services) är en [!DNL Microsoft] programvarukomponent som kan installeras på Windows Server-operativsystem för att ge användare enkel inloggning åtkomst till system och program som finns över organisatoriska gränser. Mer information finns i&quot;Active Directory Federation Services&quot; på webbplatsen Microsoft Developer Network.

The [!DNL Workfront Proof] systemet stöder SAML 2.0 och är endast kompatibelt med AD FS version 2.0 eller senare.

Se [Enkel inloggning [!DNL Workfront Proof]: AD FS-konfiguration](../../../workfront-proof/wp-acct-admin/account-settings/sso-in-wp-adfs-configuration.md) för detaljerade anvisningar.

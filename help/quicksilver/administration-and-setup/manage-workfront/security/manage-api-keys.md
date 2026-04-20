---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Hantera API-nycklar
description: För att minimera säkerhetsluckor i API:t kan Adobe Workfront-administratörer hantera de API-nycklar som används för att ge program åtkomst till Workfront för en användares räkning.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: aeb471fd63269d30a675e44fe1a47db6141eb9ed
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 0%

---

# Hantera API-nycklar

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->



>[!IMPORTANT]
>
>Workfront rekommenderar inte längre att du använder `/login`-slutpunkten eller API-nycklarna. Använd i stället någon av följande autentiseringsmetoder:
>
>* Serverautentisering med JWT
>* Användarautentisering med OAuth2
>
>Instruktioner om hur du konfigurerar dessa autentiseringsmetoder finns i [Skapa OAuth2-program för Workfront-integreringar](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)
>
>Instruktioner om hur du använder serverautentisering i Workfront finns i [Konfigurera och använda organisationens anpassade OAuth 2-program med JWT-flöde](/help/quicksilver/wf-api/api/oauth-app-jwt-flow.md)
>
>Instruktioner om hur du använder användarautentisering i Workfront finns i [Konfigurera och använda organisationens anpassade OAuth 2-program med hjälp av auktoriseringskodflöde](/help/quicksilver/wf-api/api/oauth-app-code-token-flow.md)

För att minimera säkerhetsluckor i API:t kan Adobe Workfront-administratörer hantera de API-nycklar som används för att ge program åtkomst till Workfront för en användares räkning.

Du kan återställa eller ta bort den aktuella API-administratörens nyckel, konfigurera API-nycklar så att de upphör att gälla och ta bort API-nycklarna för alla användare.

Exempel på program som utnyttjar Workfront API är:

* Dokumentintegrationer som Dropbox, Google Drive och Workfront DAM
* Workfront mobilappar

>[!IMPORTANT]
>
>När du återställer eller tar bort en API-nyckel måste alla program som använder Workfront API och autentiserar till Workfront via denna API-nyckel konfigureras om för att få tillgång till Workfront igen.

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

## Workfront API-nycklar

Varje användare i Workfront har en unik API-nyckel. Nyckeln genereras per användare när användaren öppnar en integrering som utnyttjar Workfront API (t.ex. Workfront mobilapp eller dokumentintegrering).

>[!NOTE]
>
> API-nycklar som du genererar i produktionsmiljön kopieras till förhandsvisningsmiljön under veckouppdateringen. Alla API-nycklar som du genererar i förhandsvisningsmiljön skrivs över med dina produktions-API-nycklar under veckouppdateringen.

Workfront-administratörer har också en unik API-nyckel. När ett program använder en API-administratörsnyckel för att komma åt Workfront har programmet administratörsåtkomst till Workfront.

## Hantera en administratör-API-nyckel

Du kan generera, återställa eller ta bort API-nyckeln för ditt administratörsanvändarkonto.

{{step-1-to-setup}}

1. Klicka på **System >** **Kundinformation.**
1. (Villkorligt) Utför någon av följande åtgärder:

   Så här genererar du en API-nyckel: Klicka på **Generera API-nyckel** i avsnittet **API-nyckelinställningar**.

   eller\
   Så här återställer du en API-nyckel: I avsnittet **API-nyckelinställningar** klickar du på **Återställ** och sedan på **Återställ.**

   eller

   Så här tar du bort API-nyckeln: Klicka på **Ta bort** i avsnittet **API-nyckelinställningar** och sedan på **Ta bort**.

<!--

   Remove me October 2026

## Generate an API Key for Non-Admin Users

You can generate and manage API Keys for users in roles other than Workfront administrator.

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

1. (Conditional) If your organization uses Single Sign-On (SSO) access management, temporarily disable the option requiring SSO authentication.

   {{step-1-to-setup}} 
   
   1. Expand **System**, then click **Single Sign-on (SSO)**. 
   1. In the **Type** field, select the type of SSO your organization uses.
   1. With the type selected, scroll down and clear the **Enable** checkbox. 
      ![Enable SSO](assets/sysadmin-security-sso-disable-31620-350x320.png)  
   1. Click **Save**.


1. In the address bar of a browser, enter the following API call:

   `<domain>`.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&username=**username**&password=**password**&method=PUT

   Replace `<domain>` with your Workfront domain name, and username and password with the user's Workfront credentials.

1. (Conditional) Enable the option requiring SSO authentication if you disabled it in Step 1.

   {{step-1-to-setup}}
   
   1. Expand **System**, then click **Single Sign-on (SSO)**.
   
   1. Select your SSO method in the **Type** drop down menu.
   1. Check the checkbox requiring SSO authentication.

   -->

## Konfigurera när API-nycklar upphör att gälla

Du kan konfigurera API-nycklar så att de upphör att gälla för alla användare i systemet. När API-nyckeln för en användare upphör att gälla måste användaren autentisera på nytt för alla program som använder Workfront API för att få åtkomst till Workfront. Du kan ändra hur ofta API-nycklarna förfaller. Du kan också konfigurera om API-nycklar ska förfalla när lösenordet för en användare förfaller.

{{step-1-to-setup}}

1. Klicka på **System** > **Kundinformation**.
1. I området **API-nyckelinställningar**, i listrutan **Efter skapande**, förfaller **API-nycklar i**, väljer du den tidsram som du vill att API-nycklarna ska förfalla.

   När du ändrar det här alternativet börjar den nya tidsramen från den tidpunkt du gjorde ändringen. Om du till exempel ändrar det här alternativet från *1 månad* till *6 månader* förfaller API-nycklarna sex månader från den tidpunkt du gör ändringen.

   API-nycklar förfaller som standard varje månad.

1. Aktivera **Ta bort API-nyckel när en användares lösenord upphör att gälla** om du vill konfigurera API-nycklar så att de förfaller när användarens lösenord förfaller.

   Som standard är det här alternativet inte aktiverat.

   Mer information om hur du konfigurerar användarlösenord så att de upphör att gälla finns i [Konfigurera systemsäkerhetsinställningar](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

1. Klicka på **Spara**.

## Ta bort API-nycklarna för alla användare

Om du är orolig för en viss säkerhetsöverträdelse i ditt Workfront-system kan du ta bort API-nycklar samtidigt för alla användare.

>[!IMPORTANT]
>
>Om du tar bort API-nycklar för alla användare blir ALLA API-nycklar ogiltiga för alla användare i systemet. Den här åtgärden gör att alla integreringar i Workfront misslyckas tills du genererar en ny API-nyckel i Workfront och uppdaterar alla integreringar.

{{step-1-to-setup}}

1. Expandera **System** och klicka sedan på **Kundinformation**.

1. I området **API-nyckelinställningar** klickar du på **Ta bort alla API-nycklar** och sedan på **Ta bort** **alla**.

<!--

Remove me October 2026

## Restricting API logins with an X.509 certificate

>[!IMPORTANT]
>
>The procedure described in this section applies only to organizations that have not yet been onboarded to the Adobe Business Platform. Logging in to Workfront through the Workfront API is not available if your organization has been onboarded to the Adobe Business Platform.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

Third-party applications can communicate with Workfront through the API. To increase the security of your Workfront site, you can configure Workfront to restrict API login requests by uploading an X.509 certificate to Workfront. Once enabled, all login requests through the API must include a client certificate in addition to username and password.

* [Obtain the X.509 certificate](#obtain-the-x-509-certificate) 
* [Upload the certificate to Workfront](#upload-the-certificate-to-workfront) 
* [Verify API login calls are restricted](#verify-api-login-calls-are-restricted)

### Obtain the X.509 certificate {#obtain-the-x-509-certificate}

Obtain a valid X.509 certificate from a trusted Certificate Authority (such as Verisign), and save it to a temporary location on your workstation. 

### Upload the certificate to Workfront {#upload-the-certificate-to-workfront}

After you have obtained the X.509 certificate from your Certificate Authority, you need to upload it to Workfront.

1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).  

1. Expand **System**, then click **Customer Info**.

1. In the **API Key Settings** area, select **Require X.509 Certificate for API logins**.
1. Click **Change Certificate**.
1. On your workstation, browse to and select the X.509 certificate that you previously downloaded.
1. (Optional) Click **View Details** next to the certificate name to view the following details about the certificate:

   * Subject Common Name
   * Subject Organization
   * Subject Organization Unit
   * Issuer Common Name
   * Issuer Organization
   * Issuer Organization Unit
   * Serial Number
   * Issue Date
   * Expiration Date

1. Click **Save**. 

### Verify API login calls are restricted {#verify-api-login-calls-are-restricted}

Prior to configuring your instance of Workfront to require an X.509 certificate, perform an API request to the `/login` endpoint using valid username and password parameters. You will receive a 200 response that contains a sessionID.

After making the X.509 certificate a requirement via the customer info page in your instance of Workfront, make another login attempt. This time you will receive a 500 error response with the following message: "Untrusted request. Please contact your system administrator and attach certificate."

After confirming that the X.509 certificate is required, perform the same login request with an additional parameter for apiCertificate set to the value of your certificate. If this operation was performed correctly you will receive a 200 response that contains a valid sessionID.

-->

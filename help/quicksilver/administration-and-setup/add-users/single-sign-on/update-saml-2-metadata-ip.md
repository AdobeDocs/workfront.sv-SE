---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Uppdatera SAML 2.0-metadata hos identitetsleverantören
description: Du kan uppdatera SAML 2.0-metadata i din identitetsleverantör.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 75cd0ab5-8d76-40a4-96a8-00e9f0f4fec6
source-git-commit: 96f1d50024605328713ca2019f3b726e27dc569c
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 0%

---

# Uppdatera SAML 2.0-metadata hos identitetsleverantören

{{important-admin-console-onboard}}

I följande avsnitt beskrivs hur du uppdaterar SAML 2.0-metadata (Security Assertion Markup Language) när du använder Active Directory Federation Services (ADFS) som identitetsleverantör.

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

## Använd ADFS som identitetsleverantör

Du kan uppdatera dina ADFS-metadata innan Adobe Workfront uppdaterar SAML 2.0-certifikatet eller senare. Om du väljer att uppdatera ADFS-metadata innan Workfront uppdaterar SAML 2.0-certifikatet krävs ytterligare steg.

* [Uppdatera dina ADFS-metadata](#update-your-adfs-metadata)
* [Tvinga ADFS-metadata att uppdatera](#force-your-adfs-metadata-to-update)

### Uppdatera dina ADFS-metadata {#update-your-adfs-metadata}

Slutför stegen i det här avsnittet om du vill att ADFS-metadata ska uppdateras automatiskt.

Som standard är ADFS konfigurerat att automatiskt söka efter uppdateringar av alla sina förlitande partsförtroendemata. Standardinställningen är dock att avsökning sker endast var 24:e timme. Du kan ändra det här värdet med PowerShell-kommandon.

1. Logga in på ADFS-servern och öppna ADFS-hanteringskonsolen.
1. Expandera på den vänstra panelen **ADFS 2.0,** expandera **Förtroenderelationer.**

1. Klicka på **Förlitande part-förtroenden** mapp.
1. Markera förlitande part-förtroendet som du tidigare konfigurerat för användning med Workfront och klicka sedan på&#x200B;**Uppdatera från federationsmetadata**.
1. (Villkorligt) Om det här alternativet är nedtonat (vilket innebär att förlitande part-förtroendet tidigare har konfigurerats med en metadatafil) fyller du i följande.

   1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

   1. Klicka **System** > **enkel inloggning (SSO)**.

   1. Klicka **Redigera inställningar.**
   1. Klicka **Redigera konfiguration** väljer **SAML 2.0** i **Typ** nedrullningsbar lista.

   1. Kopiera **Metadata URL**, som bör likna följande:

      `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. Högerklicka på förlitande part-förtroendet som du tidigare konfigurerat på ADFS-servern och klicka sedan på **Egenskaper.**
   1. Klicka på **Övervakning** klistra sedan in den URL som du kopierade från Workfront i **URL för förlitande parts federationsmetadata** fält.

   1. Markera alternativen för att **Övervaka förlitande part** och **Uppdatera förlitande part automatiskt**.

   1. Klicka **OK.**
   1. Välj förlitande part-förtroendet som du tidigare konfigurerat för användning med Workfront. klicka sedan på **Uppdatera från federationsmetadata.**

1. Klicka **OK** om du vill ignorera meddelandet om en del av innehållet i federationsmetadata som inte stöds av ADFS 2.0.
1. Öppna **Windows PowerShell-moduler.**
1. När alla moduler har lästs in kör du följande kommando i powershell:

   `Get-ADFSProperties`

1. Leta efter värdet bredvid **Övervakningsintervall.**

   Det blir ett tal som representerar antalet minuter mellan omröstningar. Standardvärdet ska vara 1 440 (1 440 minuter = 24 timmar).

1. Ange ett nytt värde genom att köra följande kommando i powershell:

   `Set-ADFSProperties -MonitoringInterval 1`

   Detta ändrar övervakningsintervallet från 24 timmars till varje minut. Du kan ändra värdet 1 till ett annat större värde om du vill att det ska avfrågas mindre ofta.

1. Använd **Event Viewer** om du vill söka efter följande information i ADFS2.0-loggarna:

   **Händelse-ID 156 och 157**

### Tvinga ADFS-metadata att uppdatera {#force-your-adfs-metadata-to-update}

Uppdatera dina ADFS-metadata genom att utföra stegen i följande avsnitt.

Så här tvingar du fram utbyte av metadata mellan Workfront och SAML 2.0-providern när du använder ADFS (Active Directory Federation Services):

>[!NOTE]
>
>Vissa av dessa ändringar kan behöva göras av IT-avdelningen.

1. Logga in på ADFS-servern och öppna **ADFS-hanteringskonsol**.
1. Expandera på den vänstra panelen **ADFS 2.0** och sedan expandera **Förtroenderelationer**.

1. Klicka på **Förlitande part-förtroenden** mapp.
1. Markera förlitande part-förtroendet som du tidigare konfigurerat för användning med Workfront och klicka sedan på **Uppdatera från federationsmetadata**.

   Om det här alternativet är nedtonat och inte kan markeras fyller du i följande:

   (Alternativet är bara nedtonat när förlitande part-förtroendet tidigare konfigurerats med hjälp av en metadatafil.)

   1. I Workfront kopierar du **Metadata URL** från installationsskärmen för Workfront Single Sign-On.

      Så här får du åtkomst till informationen för **Metadata URL**:

      1. Klicka **Inställningar** nära Adobe Workfront övre högra hörn på Global Navigation Bar.
      1. Klicka > **System** > **enkel inloggning (SSO)**.
      1. Klicka **Redigera inställningar.**
      1. Klicka **Redigera konfiguration** väljer **SAML 2.0** i **Typ** nedrullningsbar lista.
      1. Kopiera **Metadata URL**, som bör likna följande:

         `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`
   1. Högerklicka på förlitande part-förtroendet som du tidigare konfigurerat på ADFS-servern och klicka sedan på **Egenskaper.**
   1. Klicka på **Övervakning** klistra sedan in den URL som du kopierade från Workfront i **URL för förlitande parts federationsmetadata** fält.
   1. Markera alternativen för att **Övervaka förlitande part** och **Uppdatera förlitande part automatiskt**.
   1. Klicka **OK**.
   1. Markera förlitande part-förtroendet som du tidigare konfigurerat för användning med Workfront och klicka sedan på **Uppdatera från federationsmetadata.**


1. Klicka **OK** om du vill ignorera meddelandet om en del av innehållet i federationsmetadata som inte stöds av ADFS 2.0.
1. Klicka **Uppdatera** för att slutföra uppdateringen av federationsmetadata.

Användare som har åtkomst till Workfront via den inbyggda inloggningsskärmen med inloggningsuppgifter för Workfront (detta kan konfigureras från varje användares profilsida på **Åtkomst** -avsnittet) kan logga in med sitt användarnamn och lösenord för Workfront genom att gå till följande URL: `https://<yourdomain>.my.workfront.com/Workfront/login.cmd`.

## Använda andra identitetsleverantörer

När du använder andra identitetsleverantörer än ADFS (till exempel Ping, Okta eller Centrify) måste du överföra Workfront-metadata på nytt till din identitetsleverantör.

Mer information om hur du får en ny Workfront-metadata-URL finns i [Uppdatera dina ADFS-metadata](#update-your-adfs-metadata).

Mer information om hur du använder Active Directory Federation Services (ADFS) med SAML 2.0 i Workfront finns i [Konfigurera Adobe Workfront med SAML 2.0 med ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).

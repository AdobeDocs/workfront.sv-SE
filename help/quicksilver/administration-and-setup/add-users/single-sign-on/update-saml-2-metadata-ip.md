---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Uppdatera SAML 2.0-metadata i din identitetsleverantör
description: Du kan uppdatera SAML 2.0-metadata i din identitetsleverantör.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 75cd0ab5-8d76-40a4-96a8-00e9f0f4fec6
source-git-commit: 93f4c1691210d88531fcc269bd40ee7ed8633309
workflow-type: tm+mt
source-wordcount: '1050'
ht-degree: 0%

---

# Uppdatera SAML 2.0-metadata hos identitetsleverantören

>[!IMPORTANT]
>
>Den procedur som beskrivs på denna sida gäller endast organisationer som ännu inte har anslutit sig till Adobe Admin Console.
>
>Mer information om hur du mappar användarattribut i organisationer som har anslutit till Adobe Admin Console finns i [Mappa användarattribut i den enhetliga Adobe-upplevelsen](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md#map-user-attributes-in-the-adobe-unified-experience) i artikeln Mappa användarattribut.

I följande avsnitt beskrivs hur du uppdaterar SAML 2.0-metadata (Security Assertion Markup Language) när du använder Active Directory Federation Services (ADFS) som identitetsleverantör.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Använd ADFS som identitetsleverantör

Du kan uppdatera dina ADFS-metadata innan Adobe Workfront uppdaterar SAML 2.0-certifikatet eller senare. Om du väljer att uppdatera ADFS-metadata innan Workfront uppdaterar SAML 2.0-certifikatet krävs ytterligare steg.

* [Uppdatera dina ADFS-metadata](#update-your-adfs-metadata)
* [Tvinga ADFS-metadata att uppdatera](#force-your-adfs-metadata-to-update)

### Uppdatera dina ADFS-metadata {#update-your-adfs-metadata}

Slutför stegen i det här avsnittet om du vill att ADFS-metadata ska uppdateras automatiskt.

Som standard är ADFS konfigurerat att automatiskt söka efter uppdateringar av alla sina förlitande part-förtroendemetadata, men standardinställningen är att avsöka endast var 24:e timme. Du kan ändra det här värdet med PowerShell-kommandon.

1. Logga in på ADFS-servern och öppna ADFS-hanteringskonsolen.
1. Expandera **ADFS 2.0,** och expandera sedan **Lita på relationer i den vänstra panelen.**

1. Klicka på mappen **Förlitande partsförtroenden**.
1. Markera förlitande part-förtroendet som du tidigare konfigurerat för användning med Workfront och klicka sedan på **Uppdatera från federationsmetadata** på den högra panelen.
1. (Villkorligt) Om det här alternativet är nedtonat (vilket innebär att förlitande part-förtroendet tidigare har konfigurerats med en metadatafil) fyller du i följande.

   1. Klicka på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på ikonen **Konfigurera** ![Nätövertoningsinställningar](assets/gear-icon-settings.png) .

   1. Klicka på **System** > **enkel inloggning (SSO)**.

   1. Klicka på **Redigera inställningar.**
   1. Klicka på **Redigera konfiguration** och välj sedan **SAML 2.0** i listrutan **Typ**.

   1. Kopiera **Metadata-URL:en**, som ska likna följande:

      `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. Högerklicka på förlitande part-förtroendet som du tidigare konfigurerat på ADFS-servern och klicka sedan på **Egenskaper.**
   1. Klicka på fliken **Övervakning** och klistra sedan in den URL som du kopierade från Workfront i fältet **URL för förlitande parts federationsmetadata**.

   1. Kontrollera alternativen för **Övervaka förlitande part** och **Uppdatera förlitande part automatiskt**.

   1. Klicka på **OK.**
   1. Markera förlitande part-förtroendet som du tidigare konfigurerat för användning med Workfront. Klicka sedan på **Uppdatera från federationsmetadata på den högra panelen.**

1. Klicka på **OK** om du vill ignorera meddelandet om en del av innehållet i federationsmetadata som inte stöds av ADFS 2.0.
1. Öppna **Windows PowerShell-moduler.**
1. När alla moduler har lästs in kör du följande kommando i powershell:

   `Get-ADFSProperties`

1. Leta efter värdet intill **övervakningsintervallet.**

   Det blir ett tal som representerar antalet minuter mellan omröstningar. Standardvärdet ska vara 1 440 (1 440 minuter = 24 timmar).

1. Ange ett nytt värde genom att köra följande kommando i powershell:

   `Set-ADFSProperties -MonitoringInterval 1`

   Detta ändrar övervakningsintervallet från 24 timmars till varje minut. Du kan ändra värdet 1 till ett annat större värde om du vill att det ska avfrågas mindre ofta.

1. Använd **Loggboken** för att kontrollera att detta fungerar korrekt och leta efter följande information i ADFS2.0-loggarna:

   **Händelse-ID 156 och 157**

### Tvinga ADFS-metadata att uppdatera {#force-your-adfs-metadata-to-update}

Uppdatera dina ADFS-metadata genom att utföra stegen i följande avsnitt.

Så här tvingar du fram utbyte av metadata mellan Workfront och SAML 2.0-providern när du använder ADFS (Active Directory Federation Services):

>[!NOTE]
>
>Vissa av dessa ändringar kan behöva göras av IT-avdelningen.

1. Logga in på ADFS-servern och öppna **ADFS-hanteringskonsolen**.
1. Expandera **ADFS 2.0** i den vänstra panelen och expandera sedan **Lita på relationer**.

1. Klicka på mappen **Förlitande partsförtroenden**.
1. Markera förlitande part-förtroendet som du tidigare konfigurerat för användning med Workfront och klicka sedan på **Uppdatera från federationsmetadata** på den högra panelen.

   Om det här alternativet är nedtonat och inte kan markeras fyller du i följande:

   (Alternativet är bara nedtonat när förlitande part-förtroendet tidigare konfigurerats med hjälp av en metadatafil.)

   1. I Workfront kopierar du **Metadata URL** från installationsskärmen för Workfront Single Sign-On i inställningsområdet.

      Så här kommer du åt informationen för **Metadata-URL:en**:

      1. Klicka på **Konfigurera** i det övre högra hörnet av Adobe Workfront i det globala navigeringsfältet.
      1. Klicka på > **System** > **Enkel inloggning (SSO)**.
      1. Klicka på **Redigera inställningar.**
      1. Klicka på **Redigera konfiguration** och välj sedan **SAML 2.0** i listrutan **Typ**.
      1. Kopiera **Metadata-URL:en**, som ska likna följande:

         `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. Högerklicka på förlitande part-förtroendet som du tidigare konfigurerat på ADFS-servern och klicka sedan på **Egenskaper.**
   1. Klicka på fliken **Övervakning** och klistra sedan in den URL som du kopierade från Workfront i fältet **URL för förlitande parts federationsmetadata**.
   1. Kontrollera alternativen för **Övervaka förlitande part** och **Uppdatera förlitande part automatiskt**.
   1. Klicka på **OK**.
   1. Markera förlitande part-förtroendet som du tidigare konfigurerat för användning med Workfront och klicka sedan på **Uppdatera från federationsmetadata på den högra panelen.**

1. Klicka på **OK** om du vill ignorera meddelandet om en del av innehållet i federationsmetadata som inte stöds av ADFS 2.0.
1. Klicka på **Uppdatera** för att slutföra uppdateringen av federationsmetadata.

Användare som har åtkomst till Workfront via den inbyggda inloggningsskärmen med Workfront inloggningsuppgifter (detta kan konfigureras från varje användares profilsida i **Access** -avsnittet) kan logga in med sitt Workfront-användarnamn och lösenord genom att gå till följande URL: `https://<yourdomain>.my.workfront.com/Workfront/login.cmd`.

## Använda andra identitetsleverantörer

När du använder andra identitetsleverantörer än ADFS (till exempel Ping, Okta eller Centrify) måste du överföra Workfront-metadata på nytt till din identitetsleverantör.

Mer information om hur du hämtar en ny Workfront-metadata-URL finns i [Uppdatera ADFS-metadata](#update-your-adfs-metadata).

Mer information om hur du använder Active Directory Federation Services (ADFS) med SAML 2.0 i Workfront finns i [Konfigurera Adobe Workfront med SAML 2.0 med hjälp av ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).

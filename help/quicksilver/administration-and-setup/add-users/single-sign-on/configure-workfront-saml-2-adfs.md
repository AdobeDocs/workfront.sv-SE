---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Konfigurera Adobe Workfront med SAML 2.0 med ADFS
description: Du kan aktivera autentisering till Workfront med SAML 2.0.
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9bc5987b-6e32-47df-90c8-08ea4b1b7451
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '870'
ht-degree: 0%

---

# Konfigurera Adobe Workfront med SAML 2.0 med ADFS

{{important-admin-console-onboard}}

Som Adobe Workfront-administratör kan du integrera Workfront med en SAML 2.0-lösning (Security Assertion Markup Language) för enkel inloggning när du använder Active Directory Federation Services (ADFS).

Den här guiden fokuserar på att konfigurera ADFS utan automatisk etablering eller attributmappningar. Vi rekommenderar att du slutför konfigurationen och testar den innan du konfigurerar någon automatisk etablering.

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

## Aktivera autentisering till Workfront med SAML 2.0

Fyll i följande avsnitt för att aktivera autentisering till Workfront webbprogram och Workfront mobilprogram med SAML 2.0:

* [Hämta Workfront SSO-metadatafilen](#retrieve-the-workfront-sso-metadata-file)
* [Konfigurera förlitande part-förtroenden](#configure-relying-party-trusts)
* [Konfigurera anspråksregler](#configure-claim-rules)
* [Överför metadatafilen och testa anslutningen](#upload-the-metadata-file-and-test-the-connection)

### Hämta Workfront SSO-metadatafilen {#retrieve-the-workfront-sso-metadata-file}

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).
1. Klicka på i den vänstra panelen **System** > **enkel inloggning (SSO)**.
1. I **Typ** nedrullningsbar meny, klicka **SAML 2.0** om du vill visa ytterligare information och alternativ.
1. Kopiera den URL som visas efter **Metadata URL**.
1. Fortsätt till följande avsnitt, [Konfigurera förlitande part-förtroenden](#configure-relying-party-trusts).

### Konfigurera förlitande part-förtroenden {#configure-relying-party-trusts}

1. Öppna **ADFS Manager** med Windows Server 2008 R2 (versionen kan variera).
1. Gå till **Börja.**
1. Klicka **Administrationsverktyg.**
1. Klicka **ADFS 2.0-hantering.**
1. Välj **ADFS** och expandera **Förtroenderelationer**.
1. Högerklicka **Förlitande part-förtroenden** väljer **Lägg till förlitande part-förtroende** för att starta guiden Lägg till förlitande part-förtroende.
1. Från **Välkomstsida**, markera **Starta**.
1. I **Välj datakälla** , klistra in metadata-URL:en från Workfront.
1. Klicka **Nästa**.
1. Klicka **OK** för att bekräfta varningsmeddelandet.
1. I **Ange visningsnamn** avsnitt, lägga till **Visningsnamn** och **Anteckningar** för att skilja på pålitliga klickar du **Nästa**.
1. Välj **Tillåt alla användare att komma åt den förlitande parten** (Eller **Ingen** om du vill konfigurera detta senare).
1. Klicka **Nästa**.

   Det här tar dig till **Klar att lägga till förtroende** -avsnitt.

1. Fortsätt till följande avsnitt [Konfigurera anspråksregler](#configure-claim-rules).

### Konfigurera anspråksregler {#configure-claim-rules}

1. Klicka **Nästa** i **Klar att lägga till förtroende** -avsnittet, kontrollera sedan att **Öppna dialogrutan Redigera anspråksregler** är markerat.

   Detta gör att du kan redigera anspråksregler i ett framtida steg.

1. Klicka **Stäng**.
1. Klicka **Lägg till regel.**
1. Välj **Skicka LDAP-attribut som anspråk**.
1. Klicka **Nästa** för att visa **Konfigurera anspråksregel** steg.
1. Ange följande minimikrav för att konfigurera anspråksregeln: (Detta kommer att finnas i **Federations-ID** på användarinställningarna och används för att avgöra vem som loggar in.)


   <table >                
      <tbody>
            <tr>
               <td>Namn på anspråksregel
               </td>
               <td>Ange ett namn för anspråksregeln. Exempel:"Workfront."</td>
            </tr>
            <tr>
               <td>Attributarkiv</td>
               <td >Välj <b>Active Directory</b> i listrutan.</td>
            </tr>
            <tr>
               <td>LDAP-attribut</td>
               <td>Detta kan vara vilken typ av attribut som helst. Vi rekommenderar att du använder <b>SAM-Kontonamn</b> för det här attributet.</td>
            </tr>
            <tr>
               <td>Typ av utgående anspråk</td>
               <td>Du måste välja <b>Namn-ID</b> som typ av utgående anspråk</td>
            </tr>
      </tbody>
   </table>

1. (Valfritt) Om du vill upprätta automatisk etablering lägger du till följande ytterligare anspråk i både LDAP-attributet och typen av utgående anspråk:

   * Förnamn
   * Efternamn
   * E-postadress

1. Klicka **Slutför** och sedan klicka **OK** på nästa skärm.
1. Högerklicka på den nya **Förlitande part-förtroende** väljer **Egenskaper**.
1. Välj **Avancerad flik**. Och under **Säker hash-algoritm** välj SHA-1 eller SHA-256.

   >[!NOTE]
   >
   >Det alternativ du väljer under Säker hash-algoritm måste matcha fältet Säker hash-algoritm i Workfront under Inställningar > System > Enkel inloggning (SSO).

1. Fortsätt till följande avsnitt [Överför metadatafilen och testa anslutningen](#upload-the-metadata-file-and-test-the-connection).

### Överför metadatafilen och testa anslutningen {#upload-the-metadata-file-and-test-the-connection}

1. Öppna en webbläsare och navigera till `https://<yourserver>/FederationMetadata/2007-06/FederationMetadata.xml` .

   Detta bör hämta en fil från FederationMetadata.xml.

1. Klicka **Välj fil** under **Fyll i fält från identitetsleverantörens metadata** och väljer **FederationMetadata.xml** -fil.

1. (Valfritt) Om certifikatinformationen inte innehöll metadatafilen kan du överföra en fil separat. Välj **Välj fil** i **Certifikat** -avsnitt.

1. Klicka **Testanslutning**. Om du har ställt in rätt bör du se en sida som liknar den som visas nedan:

   ![](assets/success-saml-2.png)

   >[!NOTE]
   >
   >Om du vill konfigurera attributmappning kopierar du attributen från Test Connection till katalogattributet. Mer information finns i Mappa användarattribut.

1. Välj **Administratörsundantag** så att Workfront-administratörer kan logga in med Workfront-inloggningsuppgifter med bypass-URL:en.

   Bokmärken som pekar på `<yourdomain>`.my.workfront.com/login kringgår omdirigeringen.

1. Välj **Aktivera** för att aktivera konfigurationen.
1. Klicka **Spara**.

## Uppdatera användare för enkel inloggning

Följ den här guiden och **SSO-användarnamn** kommer **Active Directory-användarnamn**.

Som Workfront-administratör kan du uppdatera användare för enkel inloggning satsvis. Mer information om hur du uppdaterar användare för enkel inloggning finns i [Uppdatera användare för enkel inloggning](../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md).

Som Workfront-administratör kan du även manuellt tilldela ett Federations-ID som redigerar användarens profil och fyller i fältet Federations-ID. Mer information om hur du redigerar en användare finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

>[!NOTE]
>
>När du redigerar användarprofiler för att inkludera ett Federations-ID, välja **Tillåt endast SAML 2.0-autentisering** tar bort möjligheten att logga in på Workfront med bypass-URL:en (`<yourdomain>`.my.workfront.com/login).

---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Hantera API-nycklar
description: För att minimera säkerhetsluckor i API:t kan Adobe Workfront-administratörer hantera de API-nycklar som används för att ge program åtkomst till Workfront för en användares räkning.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
source-git-commit: cbbc743cfd69aaf0e5e7468980bef730a1c8fbf5
workflow-type: tm+mt
source-wordcount: '1386'
ht-degree: 0%

---

# Hantera API-nycklar

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

För att minimera säkerhetsluckor i API:t kan Adobe Workfront-administratörer hantera de API-nycklar som används för att ge program åtkomst till Workfront för en användares räkning.

Du kan återställa eller ta bort den aktuella API-administratörens nyckel, konfigurera API-nycklar så att de upphör att gälla och ta bort API-nycklarna för alla användare.

Exempel på program som utnyttjar Workfront API är:

* Dokumentintegrationer som Dropbox, Google Drive och Workfront DAM
* Workfront mobilappar

>[!IMPORTANT]
>
>När du återställer eller tar bort en API-nyckel måste alla program som använder Workfront API och autentiserar till Workfront via denna API-nyckel konfigureras om för att få tillgång till Workfront igen.

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

## Workfront API-nycklar

Varje användare i Workfront har en unik API-nyckel. Nyckeln genereras per användare när användaren öppnar en integrering som utnyttjar Workfront API (t.ex. Workfront mobilapp eller dokumentintegrering).

>[!NOTE]
>
> API-nycklar som du genererar i produktionsmiljön kopieras till förhandsvisningsmiljön under veckouppdateringen. Alla API-nycklar som du genererar i förhandsvisningsmiljön skrivs över med dina produktions-API-nycklar under veckouppdateringen.

Workfront-administratörer har också en unik API-nyckel. När ett program använder en API-administratörsnyckel för att komma åt Workfront har programmet administratörsåtkomst till Workfront.

## Hantera en administratör-API-nyckel

Du kan generera, återställa eller ta bort API-nyckeln för ditt administratörsanvändarkonto.

>[!NOTE]
>
>Du kan också generera en API-nyckel via API:t. Mer information finns i [API för händelseprenumeration](../../../wf-api/general/event-subs-api.md) avsnitt i [API för händelseprenumeration](../../../wf-api/general/event-subs-api.md).

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **System >** **Kundinformation.**
1. (Villkorligt) Utför någon av följande åtgärder:

   Så här genererar du en API-nyckel: i **API-nyckelinställningar** avsnitt, klicka **Generera API-nyckel**.

   eller\
   Så här återställer du en API-nyckel: **API-nyckelinställningar** avsnitt, klicka **Återställ** sedan **Återställ.**

   eller

   Så här tar du bort API-nyckeln: i **API-nyckelinställningar** avsnitt, klicka **Ta bort** sedan **Ta bort**.

## Generera en API-nyckel för icke-admin-användare

Du kan generera och hantera API-nycklar för användare i andra roller än Workfront-administratören.

>[!NOTE]
>
>Detta är inte tillgängligt om din organisations Workfront-instans har aktiverats med Adobe IMS. Kontakta nätverks- eller IT-administratören om du behöver mer information.

1. (Villkorligt) Om din organisation använder enkel inloggning (SSO), kan du tillfälligt inaktivera alternativet som kräver SSO-autentisering.

   1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

   1. Expandera **System** och sedan klicka **Enkel inloggning (SSO)**.
   1. I **Typ** väljer du den typ av enkel inloggning som används i organisationen.
   1. När texten är markerad rullar du nedåt och tar bort **Aktivera** kryssrutan.
      ![](assets/sysadmin-security-sso-disable-31620-350x320.png)
   1. Klicka **Spara**.


1. Ange följande API-anrop i adressfältet i en webbläsare:

   `<domain>`**.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&amp;username=**användarnamn**&amp;password=**lösenord**&amp;method=PUT

   Ersätt `<domain>` med ditt Workfront domännamn och användarnamn och lösenord med användarens Workfront-uppgifter.

1. (Villkorligt) Aktivera alternativet som kräver SSO-autentisering om du inaktiverade det i steg 1.

   1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

   1. Expandera **System** och sedan klicka **Enkel inloggning (SSO)**.

   1. Välj din SSO-metod i **Typ** listrutemeny.
   1. Markera kryssrutan som kräver SSO-autentisering.

## Konfigurera när API-nycklar upphör att gälla

Du kan konfigurera API-nycklar så att de upphör att gälla för alla användare i systemet. När API-nyckeln för en användare upphör att gälla måste användaren autentisera på nytt för alla program som använder Workfront API för att få åtkomst till Workfront. Du kan ändra hur ofta API-nycklarna förfaller. Du kan också konfigurera om API-nycklar ska förfalla när lösenordet för en användare förfaller.

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **System** > **Kundinformation**.
1. I **API-nyckelinställningar** området, i **Efter skapande**, **API-nycklar förfaller om** väljer du en tidsram när du vill att API-nycklarna ska förfalla.

   När du ändrar det här alternativet börjar den nya tidsramen från den tidpunkt du gjorde ändringen. Om du till exempel ändrar det här alternativet från *1 månad* till *6 månader*, upphör API-nycklarna att gälla 6 månader efter den tidpunkt du gör ändringen.

   API-nycklar förfaller som standard varje månad.

1. Om du vill konfigurera API-nycklar så att de förfaller när användarens lösenord förfaller väljer du **Ta bort API-nyckeln när en användares lösenord upphör att gälla**.

   Som standard är det här alternativet inte markerat.

   Mer information om hur du konfigurerar användarlösenord att upphöra finns i [Konfigurera säkerhetsinställningar för system](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

1. Klicka **Spara**.

## Ta bort API-nycklarna för alla användare

Om du är orolig för en viss säkerhetsöverträdelse i ditt Workfront-system kan du ta bort API-nycklar samtidigt för alla användare.

>[!IMPORTANT]
>
>Om du tar bort API-nycklar för alla användare blir ALLA API-nycklar ogiltiga för alla användare i systemet. Den här åtgärden gör att alla integreringar i Workfront misslyckas tills du genererar en ny API-nyckel i Workfront och uppdaterar alla integreringar.

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Expandera **System** och sedan klicka **Kundinformation.**

1. I **API-nyckelinställningar** område, klicka **Ta bort alla API-nycklar** och sedan klicka **Ta bort** **Alla**.

## Begränsa API-inloggningar med ett X.509-certifikat

>[!IMPORTANT]
>
>Det förfarande som beskrivs i detta avsnitt gäller endast organisationer som ännu inte har anslutit sig till Adobe Business Platform. Det går inte att logga in på Workfront via Workfront API om din organisation har anslutit sig till Adobe Business Platform.
>
>En lista över procedurer som skiljer sig åt beroende på om din organisation har anslutit sig till Adobe Business Platform finns på [Plattformsbaserade administrationsskillnader (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Tredjepartsprogram kan kommunicera med Workfront via API:t. Om du vill öka säkerheten på din Workfront-webbplats kan du konfigurera Workfront att begränsa API-inloggningsbegäranden genom att överföra ett X.509-certifikat till Workfront. När den är aktiverad måste alla inloggningsbegäranden via API:t innehålla ett klientcertifikat förutom användarnamn och lösenord.

>[!NOTE]
>
>Detta är inte tillgängligt om din organisations Workfront-instans har aktiverats med Adobe IMS. Kontakta nätverks- eller IT-administratören om du behöver mer information.

* [Hämta X.509-certifikatet](#obtain-the-x-509-certificate)
* [Överför certifikatet till Workfront](#upload-the-certificate-to-workfront)
* [Verifiera att API-inloggningsanrop är begränsade](#verify-api-login-calls-are-restricted)

### Hämta X.509-certifikatet {#obtain-the-x-509-certificate}

Hämta ett giltigt X.509-certifikat från en betrodd certifikatutfärdare (till exempel Verisign) och placera det på en tillfällig plats på din arbetsstation.

### Överför certifikatet till Workfront {#upload-the-certificate-to-workfront}

När du har fått X.509-certifikatet från din certifikatutfärdare måste du överföra det till Workfront.

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Expandera **System** och sedan klicka **Kundinformation**.

1. I **API-nyckelinställningar** område, markera **Aktivera X.509-certifikat**.
1. På din arbetsstation bläddrar du till och väljer det X.509-certifikat som du har hämtat tidigare.
1. (Valfritt) Klicka på **Visa detaljer** bredvid certifikatnamnet för att visa följande information om certifikatet:

   * Ämnesnamn
   * Ämnesorganisation
   * Enhet för ämnesorganisation
   * Namn på utfärdare
   * Utfärdarorganisation
   * Utfärdarorganisationsenhet
   * Serienummer
   * Utgivningsdatum
   * Förfallodatum

1. Klicka **Spara**.

### Verifiera att API-inloggningsanrop är begränsade {#verify-api-login-calls-are-restricted}

Innan du konfigurerar din instans av Workfront så att den kräver ett X.509-certifikat utför du en API-begäran till `/login` slutpunkt med giltiga parametrar för användarnamn och lösenord. Du får ett 200-svar som innehåller ett sessions-ID.

När du har gjort X.509-certifikatet till ett krav via kundinformationssidan i din instans av Workfront, gör du ett nytt inloggningsförsök. Den här gången får du ett 500-felsvar med följande meddelande:&quot;Untrusted request request. Kontakta systemadministratören och bifoga certifikatet.&quot;

När du har bekräftat att X.509-certifikatet krävs utför du samma inloggningsbegäran med en extra parameter för apiCertificate som är inställd på värdet för ditt certifikat. Om den här åtgärden utfördes korrekt får du ett 200-svar som innehåller ett giltigt sessions-ID.

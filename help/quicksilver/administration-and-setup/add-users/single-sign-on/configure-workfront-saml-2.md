---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Konfigurera Adobe Workfront med SAML 2.0
description: Som Adobe Workfront-administratör kan du konfigurera Workfront webb- och mobilprogram så att de integreras med en SAML 2.0-lösning för enkel inloggning (SSO).
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: cf09859c-7d6f-4bf0-9b7f-c57096233c94
source-git-commit: 16a34e4315d508e31859e962edd01026d01ee193
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 0%

---

# Konfigurera Adobe Workfront med SAML 2.0

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.** </p>
-->

<!-- Audited: 12/2023 -->

{{important-admin-console-onboard}}

Som Adobe Workfront-administratör kan du konfigurera Workfront webb- och mobilprogram så att de integreras med en SAML 2.0-lösning för enkel inloggning (SSO).

När du har konfigurerat SAML 2.0 i Workfront, enligt beskrivningen i följande avsnitt, kan du upprätthålla konfigurationen enligt beskrivningen i [Uppdatera SAML 2.0-metadata hos identitetsleverantören](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).

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
   <td><p>Nytt: Standard </p>
       <p>eller</p> 
       <p>Aktuell: Planera </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Aktivera autentisering till Workfront med SAML 2.0

{{step-1-to-setup}}

1. Klicka **System** > **enkel inloggning (SSO).**

1. I **Typ** nedrullningsbar lista, välja **SAML 2.0.**

1. Långt upp i alternativen som visas klickar du på **Ladda ned SAML 2.0-metadata** om du vill hämta filen på datorn.

   Din SAML 2.0-identitetsleverantör kräver en XML-fil med information som genereras i din Workfront-instans. När du har laddat ned filen måste du komma åt din SAML 2.0 Identity Provider-server och ladda upp XML-filen för Workfront SAML 2.0.

1. Ange följande information i Workfront:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">Tjänsteleverantörens ID </td>
      <td> Denna URL, som redan är ifylld för dig, identifierar Workfront för identitetsleverantören. Till exempel: <code>&lt;yourcompany&gt;.com/SAML2</code>.</td>
     </tr>
     <tr>
      <td role="rowheader">Bindningstyp</span> </td>
      <td> <p>Välj den metod som stöds av IDP-servern för att skicka autentiseringsinformation:</p>
       <ul>
       <li>POST</li>
       <li>OMDIRIGERA</li>
       </ul> </td>
     </tr>
     <tr>
      <td role="rowheader">Fyll i fält från identitetsleverantörens metadata </td> 
      <td>I SAML 2.0 Identity Provider-lösningen exporterar du en XML-fil för tjänstleverantörens metadata och sparar den på en tillfällig plats på datorn. Välj <strong>Välj fil</strong>söker du efter och markerar filen som du har sparat och lägger till den i din Workfront-konfiguration.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL för inloggningsportal</span> </td> 
      <td>Ange din organisations gemensamma inloggningsportal. Det här är den URL där användare loggar in för att få tillgång till Workfront och alla andra program som är integrerade med SAML 2.0.</td> 
     </tr>
     <tr>
      <td role="rowheader">Utloggnings-URL</span> </td> 
      <td> <p>Ange URL:en för utloggning för IDP-servern. Workfront skickar en HTTP-begäran till den här URL:en innan Workfront loggas ut. Detta stänger användarens session på fjärrservern när Workfront-sessionen stängs.</p> <p><b>ANMÄRKNING</b>: Du omdirigeras bara till utloggnings-URL om du har möjlighet <strong>Tillåt endast SAML 2.0-autentisering</strong> aktiverat i din användarprofil.</p> </td>
     </tr>
     <tr>
      <td role="rowheader">Ändra lösenord-URL </td> 
      <td> <p> Ange den URL som användarna ska omdirigeras till för att ändra sina lösenord. </p> <p>Eftersom inloggningsuppgifterna för SAML 2.0 används för att få åtkomst till Workfront måste man omdirigera användare till en sida där de kan ändra sitt SAML 2.0-lösenord i stället för att slutföra den här aktiviteten via Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Säker hash-algoritm </td> 
      <td> <p>Välj den SHA (Secure Hash Algorithm) som din IDP stöder:</p> 
       <ul> 
       <li>SHA-1</li> 
       <li>SHA-256</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Etablera användare automatiskt</span> </td> 
      <td> <p>Det här alternativet skapar automatiskt en användare i systemet när en ny användare med ett kataloganvändarnamn och lösenord försöker logga in på Workfront för första gången.</p> <p>Om du vill skapa användare i Workfront måste du mappa Workfront-dataattribut till följande användardataattribut i din katalogleverantör:</p> 
       <ul> 
       <li>Förnamn</li> 
       <li>Efternamn</li> 
       <li>E-postadress</li> 
       </ul> 
       <p>När du markerar kryssrutan visas följande alternativ:</p> 
       <p> <img src="assets/saml-2.0-auto-provision-users-ui.png"> </p> 
       <p>Markera det Workfront-användarattribut som du vill mappa i listrutan och ange sedan motsvarande katalogattribut i användarkatalogen.</p> 
       <p>The <strong>Katalogattribut</strong> fältet ska innehålla katalogattributnamnet från tabellen för användarattribut som du sparade när din SAML 2.0-konfiguration testades.</p> 
       <p>Du kan ange ett standardvärde för Workfront i dialogrutan <strong>Standardvärde</strong> fält. Du kan också ange regler baserat på värdena från din SAML 2.0-identitetsleverantör.</p> 
       <p><b>VARNING</b>: Workfront försöker mappa de attribut som anges nedan varje gång en användare loggar in i systemet. Därför rekommenderar vi inte att åtkomstnivåer mappas. Du kan enkelt ta bort administrativ åtkomst om ett attribut är felaktigt mappat. Klicka <strong>Lägg till mappning</strong> om du vill lägga till ytterligare regler.
       </p> 
       <p>Du kan mappa följande Workfront-attribut:</p> 
      <ul> 
      <li> <p>Åtkomstnivå</p> </li> 
      <li> <p>Adress</p> </li> 
      <li> <p>Adress 2</p> </li> 
      <li> <p>Fakturering per timme</p> </li> 
      <li> <p>Ort</p> </li> 
      <li> <p>Företag</p> </li> 
      <li> <p>Kostnad per timme</p> </li> 
      <li> <p>E-postadress</p> </li> 
      <li> <p>Tillägg</p> </li> 
      <li> <p>Förnamn</p> </li> 
      <li> <p>Hemgrupp</p> </li> 
      <li> <p>Hemteam</p> </li> 
      <li> <p>Jobbroll</p> </li> 
      <li> <p>Efternamn</p> </li> 
      <li> <p>Layoutmall</p> </li> 
      <li> <p>Manager</p> </li> 
      <li> <p>Mobiltelefon</p> </li> 
      <li> <p>Telefonnummer</p> </li> 
      <li> <p>Postnummer</p> </li> 
      <li> <p>Schema</p> </li> 
      <li> <p>Läge</p> </li> 
      <li> <p>Tidrapportprofil</p> </li> 
      <li> <p>Titel</p> </li> 
      </ul>
      <p>Klicka <strong>Spara</strong> när du är klar med mappningen av användarattribut.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Certifikat </td> 
      <td> <p>Överför ett giltigt SSL-certifikat för att säkerställa en säker anslutning mellan autentiseringstjänsten och Workfront. För OnDemand-konton krävs alltid ett certifikat. Du kan hämta det här certifikatet från din SAML 2.0-systemadministratör.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Administratörsundantag </td> 
      <td> <p>Gör att Workfront-administratörer kan komma åt Workfront via sin Workfront-inloggning. Om det här alternativet inte är markerat måste Workfront-administratörer använda sitt SAML 2.0-användarnamn och -lösenord.</p> 
      <p>Workfront försöker först logga in på Workfront via SAML 2.0 för användare med åtkomstnivån Workfront System Administrator. Om SAML 2.0-autentiseringen misslyckas använder Workfront lokal autentisering för Workfront-administratörer.</p> 
      <p>Vi rekommenderar att du alltid har valt det här alternativet så att Workfront-administratören kan logga in på Workfront om din SAML 2.0-leverantör inte är tillgänglig för tillfället.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aktivera </td> 
      <td> <p>Aktiverar enkel inloggning på Workfront-systemet. Kontrollera att du har skickat inloggningsinstruktioner till användarna.</p> <p>När du har aktiverat SSO-konfigurationen i Workfront måste du aktivera <strong>Tillåt endast SAML 2.0-autentisering</strong> inställning för alla användare så att de kan använda enkel inloggning.</p> <p>Mer information om hur du uppdaterar användare för enkel inloggning finns i <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Uppdatera användare för enkel inloggning</a>.</p> <p>Mer information om användarinställningar finns i <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Redigera en användares profil</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bekräfta konfiguration </td> 
      <td> 
      <p>Klicka <strong>Testanslutning</strong> verifiera att Workfront och SAML 2.0-identitetsleverantören kan kommunicera med varandra. Anslutningen fungerar bara om du har bytt ut XML-filerna.
      </p> 
      <p>När du har testat länken mellan din SAML 2.0-identitetsleverantör och Workfront visas en skärm som liknar bilden nedan.</p>
      <p><b>ANMÄRKNING</b>: Den här skärmen visas i ett webbläsarpopup-fönster så att du kan inaktivera popup-blockerare i webbläsaren.</p>
      <p>Spara informationen som visas i tabellen för senare bruk.</p>
      <p><img src="assets/success-table-saml-2.png"></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **Spara** för att spara SAML 2.0-konfigurationen.

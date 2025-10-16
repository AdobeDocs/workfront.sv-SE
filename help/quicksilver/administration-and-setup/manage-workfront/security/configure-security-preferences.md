---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Konfigurera systeminställningar
description: Som Adobe Workfront-administratör kan du konfigurera inställningar för ditt Workfront-system, inklusive säkerhetsinställningar.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: 1a56846647e443cf3f5f09eed8c3084434de5ddb
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# Konfigurera systeminställningar

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

<!--Audited: 05/2024-->

{{important-admin-console-onboard}}

Som Adobe Workfront-administratör kan du konfigurera inställningar för ditt Workfront-system, bland annat:

* Tillgång till Workfront från mobilappar och andra integrerade program
* Regler för inbäddning av Workfront i en iframe

De ändringar du gör i systeminställningarna påverkar alla användare i systemet och deras upplevelse i Workfront.

Vi rekommenderar att du konfigurerar dina systeminställningar under Workfront-implementeringen och endast tillfälligt kan gå igenom dem efter det.

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

## Konfigurera systeminställningarna

{{step-1-to-setup}}

1. Klicka på **System** > **Inställningar** i den vänstra panelen.

1. Välj något av följande fält för att ange inställningar för din organisation:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Aktivera processen för snabb release</p> </td> 
      <td>Gör att du kan aktivera månadsvisa Workfront-utgåvor för din organisation istället för kvartalsvisa utgåvor.</p><p>Mer information om processen för snabb släppning finns i <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md" class="MCXref xref">Aktivera eller inaktivera snabba releaser för din organisation</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Tillåt inbäddning av Workfront i en iframe</p> </td> 
      <td>Gör att du kan bädda in Workfront i en iframe.<p>Det här alternativet är inaktiverat som standard.</p><p><b>VIKTIGT</b>: Om du visar ett webbaserat program i en iframe kan programmet bli känsligt för en klickjacking-säkerhetslucka.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tillåt SAML 2.0-autentisering i Office 365-tillägg</td> 
      <td> <p>Gör att du kan bädda in Workfront i en iframe endast för Office 365-tillägg när Workfront är integrerat med en SAML 2.0-lösning för enkel inloggning. </p> <p>Det här alternativet är aktiverat som standard.</p> <p><b>Obs!</b> Om du aktiverar alternativet ovan <strong>Tillåt inbäddning av Workfront i en iframe</strong> aktiveras och nedtonas alternativet <strong>Tillåt SAML 2.0-autentisering i Office 365-tillägg</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aktivera användning av sessionsinformation när du skapar URL-adresser för externa sidor</td> 
      <td> <p>Tillåter användare att använda information om sessions-ID för en webbplats när en extern sida läggs till på en instrumentpanel.</p> <p>Det här alternativet är osäkert och inaktiverat som standard. Vi rekommenderar att du använder OAuth för integreringar i stället.</p> <p>Mer information om hur du lägger till externa sidor på en kontrollpanel finns i <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">Bädda in en extern webbsida på en kontrollpanel</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Låt andra använda Workfront mobilprogram och Workfront Outlook-tillägget</td> 
      <td> <p>Tillåter användare åtkomst till mobilapparna (Workfront View för iPad och mobilappar) och Workfront Outlook-appen.</p> <p>Det här alternativet är aktiverat som standard. </p> <p>Mer information om Workfront View finns i <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Use Adobe Workfront View</a>. Mer information om mobilapparna finns i <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Använda Adobe Workfront-mobilappen: artikelindex</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Samarbeta med personer utan Workfront-konton via e-postadresser</p> </td> 
      <td>Workfront-användare kan dela vissa objekt med personer utan ett Workfront-konto genom att ta med sin e-postadress i stället för sitt namn. Användare kan dela följande objekt med externa användare via sin e-postadress:
       <ul>
        <li>Dokument<br></li>
        <li>Dokumentförfrågan<br></li>
        <li>Godkännande av dokument</li>
        <li>Kalender</li>
       </ul><p>Det här alternativet är aktiverat som standard.</p> <p><b>Viktigt</b>: Åtkomstnivån Extern användare är inte tillgänglig i din Workfront-instans om det här alternativet är inaktiverat. Mer information finns i <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Inbyggda åtkomstnivåer</a>.</p> </td> 
     </tr> 
     <!--<tr> 
      <td role="rowheader">Require external users to register with a password</td> 
      <td> <p>Requires external users to register before they are able to view items in Workfront. By default, this option is disabled. When you enable this option, people without a Workfront account who are included in certain updates by their email address, will be prompted to create an account before they can view the item they are included on. This creates an External User account for them.</p> <p>This option is disabled by default.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log users out after</td> 
      <td> Lets you specify when a user is logged out of Workfront, after a period of inactivity. By default, users are logged out after 8 hours of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log mobile users out after </td> 
      <td>Lets you specify when a user is logged out of the Workfront application, after a period of inactivity. By default, users are logged out after 7 days of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr> -->
     <tr> 
      <td role="rowheader">Anpassad hjälp-URL</td> 
      <td>Här kan du definiera en intern anpassad hjälpwebbplats där hjälpikonen för huvudmeny kan visas. Mer information finns i <a href="/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md">Konfigurera en anpassad hjälp-URL</a>.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Aktivera arbetslistan Prioriteter </td> 
      <td>Gör att du kan välja att aktivera eller inaktivera arbetslistan Prioriteter för dina användare. Användarna kommer fortfarande att se Prioritetsikonerna i Workfront, men de kommer inte att ha tillgång till funktionerna. Mer information om prioriteringar finns i <a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">Kom igång med prioriteringar</a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Aktivera AI </td> 
      <td>Gör att du kan välja att aktivera AI, inklusive AI-assistenten. <p><b>Obs!</b> Din organisation måste uppfylla specifika krav för att kunna aktivera AI. Mer information om AI, inklusive kraven, finns i <a href="/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md">Översikt över AI Assistant</a>.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Fyll i formulär automatiskt </td> 
      <td>Gör att du kan välja att aktivera möjligheten att fylla i begärandeformulär automatiskt baserat på tidigare begärandedata. Mer information om Komplettera automatiskt i formulär finns i <a href="/help/quicksilver/manage-work/requests/create-requests/autofill-suggestions-from-previous.md">Fyll i en begäran automatiskt från tidigare data</a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Anmäl dig till AI Betas </td> 
      <td>&gt;Här kan du välja att aktivera AI-funktioner som finns i Beta. Om du aktiverar det här alternativet kan du välja vilka AI Beta-funktioner som ska aktiveras. Mer information om alla AI Beta-funktioner får du om du klickar på informationsikonen bredvid den funktionen.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Testmiljöer</td> 
      <td>Här kan du komma åt Workfront testmiljöer. Mer information finns i <a href="/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md">Sandlådemiljön för Adobe Workfront Preview</a>.</p></td> 
    </tbody> 
   </table>

1. Klicka på **Spara**.

   De ändringar du har sparat här påverkar upplevelsen för alla användare i Workfront och alla som interagerar med systemet som externa användare.

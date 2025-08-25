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
source-git-commit: 99113ac4f2ceca6bd50f078916e33cec7f577362
workflow-type: tm+mt
source-wordcount: '894'
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
   <td><p>Nytt: Standard</p>
   <p>eller</p>
   <p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
      <td> <p>Tillåter användare åtkomst till mobilapparna (Workfront View för iPad och mobilappar) och Workfront Outlook-appen.</p> <p>Det här alternativet är aktiverat som standard. </p> <p>Mer information om Workfront View finns i <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Use Adobe Workfront View</a>. Mer information om mobilapparna finns i <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Använda Adobe Workfront-mobilappen: artikelindex</a>.</p> <p>Mer information om Outlook-plugin-programmet finns i <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">Konfigurera Adobe Workfront för Outlook</a>.</p> </td> 
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
     <tr> 
      <td role="rowheader">Kräv att externa användare registrerar sig med ett lösenord</td> 
      <td> <p>Kräver att externa användare registrerar sig innan de kan visa objekt i Workfront. Som standard är det här alternativet inaktiverat. När du aktiverar det här alternativet ombeds personer som saknar ett Workfront-konto och som är inkluderade i vissa uppdateringar via sin e-postadress att skapa ett konto innan de kan visa det objekt de är inkluderade i. Detta skapar ett externt användarkonto åt dem.</p> <p>Det här alternativet är inaktiverat som standard.</p> </td> 
     </tr>
<!-- DELETE THIS SECTION MARCH 2026   <tr> 
      <td role="rowheader">Automatically log users out after</td> 
      <td> Lets you specify when a user is logged out of Workfront, after a period of inactivity. By default, users are logged out after 8 hours of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Automatically log mobile users out after </td> 
      <td>Lets you specify when a user is logged out of the Workfront application, after a period of inactivity. By default, users are logged out after 7 days of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr>  -->
    &lt;tr>
    &lt;td role=&quot;rowheader&quot;>Anpassad hjälp-URL&lt;/td>
    &lt;td>Gör att du kan definiera en intern anpassad hjälpwebbplats som hjälpikonen för huvudmenyn ska gå till. Mer information finns i &lt;a href=&quot;/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md&quot;>Konfigurera en anpassad hjälp-URL&lt;/a>.&lt;/p>&lt;/td>
    &lt;/tr>
    &lt;tr>
    &lt;td role=&quot;rowheader&quot;>Användare i systemet ser som standard den nya hemupplevelsen &lt;/td>
    &lt;td>Ange om användarna ska se den nya hemupplevelsen som standard. När det här alternativet är aktiverat visas den nya hemupplevelsen som standard, men du kan fortfarande välja att aktivera eller inaktivera Nytt hem på individnivå. När alternativet är inaktiverat visas inte den banderoll som gör att användaren kan växla till Nytt hem, men användaren kan fortfarande navigera till sin nya hemsida genom att ange &lt;code>/home/workspaces&lt;/code> manuellt i slutet av sin instans-URL. Den här inställningen är aktiverad som standard.&lt;/td>
    &lt;/tr>
    &lt;tr>
    &lt;td role=&quot;rowheader&quot;>Aktivera prioritetsarbetslistan &lt;/td>
    &lt;td>Gör att du kan välja att aktivera eller inaktivera prioritetsarbetslistan för dina användare. Användarna kommer fortfarande att se Prioritetsikonerna i Workfront, men de kommer inte att ha tillgång till funktionerna. Mer information om prioriteringar finns i &lt;a href=&quot;/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md&quot;>Komma igång med prioriteringar&lt;/a>.&lt;/td>
    &lt;/tr>
    &lt;tr>
    &lt;td role=&quot;rowheader&quot;>Testmiljöer&lt;/td>
    &lt;td>Gör att du kan komma åt dina testmiljöer i Workfront. Mer information finns i &lt;a href=&quot;/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md&quot;>Adobe Workfront Preview Sandbox Environment&lt;/a>.&lt;/p>&lt;/td>
    &lt;/tbody>
</table>

1. Klicka på **Spara**.

   De ändringar du har sparat här påverkar upplevelsen för alla användare i Workfront och alla som interagerar med systemet som externa användare.

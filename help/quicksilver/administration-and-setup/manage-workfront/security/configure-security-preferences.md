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
source-git-commit: 5cc1acffff12d78e48228f3ae223514c0ff379ef
workflow-type: tm+mt
source-wordcount: '866'
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

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Konfigurera systeminställningarna

{{step-1-to-setup}}

1. Klicka på i den vänstra panelen **System** > **Inställningar**.

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
      <td>Gör att du kan bädda in Workfront i en iframe.<p>Det här alternativet är inaktiverat som standard.</p><p><b>VIKTIGT</b>: Om du visar ett webbaserat program i en iframe kan programmet drabbas av en klickjacking-säkerhetslucka.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tillåt SAML 2.0-autentisering i Office 365-tillägg</td> 
      <td> <p>Gör att du kan bädda in Workfront i en iframe endast för Office 365-tillägg när Workfront är integrerat med en SAML 2.0-lösning för enkel inloggning. </p> <p>Det här alternativet är aktiverat som standard.</p> <p><b>ANMÄRKNING</b>: Om du aktiverar alternativet ovan <strong>Tillåt inbäddning av Workfront i en iframe</strong>, alternativet <strong>Tillåt SAML 2.0-autentisering i Office 365-tillägg</strong> är aktiverat och nedtonat.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aktivera användning av sessionsinformation när du skapar URL-adresser för externa sidor</td> 
      <td> <p>Tillåter användare att använda information om sessions-ID för en webbplats när en extern sida läggs till på en instrumentpanel.</p> <p>Det här alternativet är osäkert och inaktiverat som standard. Vi rekommenderar att du använder OAuth för integreringar i stället.</p> <p>Mer information om hur du lägger till externa sidor på en kontrollpanel finns i <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">Bädda in en extern webbsida i en instrumentpanel</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Låt andra använda Workfront mobilprogram och Workfront Outlook-tillägget</td> 
      <td> <p>Tillåter användare åtkomst till mobilapparna (Workfront View för iPad och mobilappar) och Workfront Outlook-appen.</p> <p>Det här alternativet är aktiverat som standard. </p> <p>Mer information om Workfront View finns i <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Använd Adobe Workfront View</a>. Mer information om mobilapparna finns i <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Använda Adobe Workfront mobilapp: artikelindex</a>.</p> <p>Mer information om Outlook-plugin-programmet finns i <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">Konfigurera Adobe Workfront för Outlook</a>.</p> </td> 
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
     <tr> 
      <td role="rowheader">Logga ut användare automatiskt efter</td> 
      <td> Här kan du ange när en användare loggas ut från Workfront efter en viss inaktivitetsperiod. Som standard loggas användare ut efter 8 timmars inaktivitet. <p>Det här alternativet påverkar även Workfront-kunder som använder en enda inloggningslösning.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Logga ut användare automatiskt efter </td> 
      <td>Här kan du ange när en användare är utloggad från Workfront-programmet, efter en tids inaktivitet. Som standard loggas användare ut efter 7 dagars inaktivitet. <p>Det här alternativet påverkar även Workfront-kunder som använder en enda inloggningslösning.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anpassad hjälp-URL</td> 
      <td>Här kan du definiera en intern anpassad hjälpwebbplats där hjälpikonen för huvudmeny kan visas. Mer information finns i <a href="/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md">Konfigurera en anpassad hjälp-URL</a>.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Användare i systemet ser som standard den nya hemupplevelsen </td> 
      <td>Här kan du ange om användare ska se den nya hemupplevelsen som standard. När det här alternativet är aktiverat visas den nya hemupplevelsen som standard, men du kan fortfarande välja att aktivera eller inaktivera Nytt hem på individnivå. När alternativet är inaktiverat visas inte den banderoll som gör att användaren kan växla till Nytt hem, men användaren kan fortfarande navigera till sin nya hemsida genom att ange <code>/home/workspaces</code> i slutet av instansens URL. Den här inställningen är aktiverad som standard.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Testmiljöer</td> 
      <td>Här kan du komma åt Workfront testmiljöer. Mer information finns i <a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">Sandlådemiljön Adobe Workfront Preview</a>.</p></td> 
    </tbody> 
   </table>

1. Klicka **Spara**.

   De ändringar du har sparat här påverkar upplevelsen för alla användare i Workfront och alla som interagerar med systemet som externa användare.

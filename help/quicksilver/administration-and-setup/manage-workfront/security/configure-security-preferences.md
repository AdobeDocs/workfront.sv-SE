---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Konfigurera säkerhetsinställningar för system
description: Som Adobe Workfront-administratör kan du konfigurera säkerhetsinställningar för ditt Workfront-system.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: 281712542566aec87c51a2eccb301dd3a83a94b3
workflow-type: tm+mt
source-wordcount: '747'
ht-degree: 0%

---

# Konfigurera systeminställningar

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

{{important-admin-console-onboard}}

Som Adobe Workfront-administratör kan du konfigurera inställningar för ditt Workfront-system:

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Konfigurera systeminställningarna

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **System** > **Inställningar**.

1. Välj något av följande fält för att ange inställningar för din organisation:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Tillåt inbäddning av <strong>Workfront</strong> i en iframe</p> </td> 
      <td>Gör att du kan bädda in Workfront i en iframe.<p>Det här alternativet är inaktiverat som standard.</p><p><b>VIKTIGT</b>: Om du visar ett webbaserat program i en iframe kan programmet drabbas av en klickjacking-säkerhetslucka.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tillåt SAML 2.0-autentisering i Office 365-tillägg</td> 
      <td> <p>Gör att du kan bädda in Workfront i en iframe endast för Office 365-tillägg när Workfront är integrerat med en SAML 2.0-lösning för enkel inloggning. </p> <p>Det här alternativet är aktiverat som standard.</p> <p><b>ANMÄRKNING</b>: Om du aktiverar alternativet ovan <strong>Tillåt inbäddning av Workfront i en iframe</strong>, alternativet <strong>Tillåt SAML 2.0-autentisering i Office 365-tillägg</strong> är aktiverat och nedtonat.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aktivera användning av sessionsinformation när du skapar URL-adresser för externa sidor</td> 
      <td> <p>Tillåter användare att använda information om sessions-ID för en webbplats när en extern sida läggs till på en instrumentpanel.</p> <p>Mer information om hur du lägger till externa sidor på en kontrollpanel finns i <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">Bädda in en extern webbsida i en instrumentpanel</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Låt användare använda Workfront mobilapplikationer och <strong>Workfront</strong> Outlook-tillägg</td> 
      <td> <p>Tillåter användare åtkomst till mobilapparna (Workfront View för iPad och mobilappar) och Workfront Outlook-appen.</p> <p>Det här alternativet är aktiverat som standard. </p> <p>Mer information om Workfront View finns i <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Använd Adobe Workfront View</a>. Mer information om mobilapparna finns i <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Använda Adobe Workfront mobilapp</a>.</p> <p>Mer information om Outlook-plugin-programmet finns i <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">Konfigurera Adobe Workfront för Outlook</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Samarbeta med personer utan Workfront-konton via e-postadresser</p> </td> 
      <td>Workfront-användare kan dela vissa objekt med personer utan ett Workfront-konto genom att ta med sin e-postadress i stället för sitt namn. Användare kan dela följande objekt med externa användare via sin e-postadress:
       <ul>
        <li>Dokument<br></li>
        <li>Dokumentförfrågan<br></li>
        <li>Godkännande av dokument</li>
        <li>Kalender</li>
       </ul><p>Det här alternativet är aktiverat som standard.</p> <p><b>Viktigt</b>: Åtkomstnivån Extern användare är inte tillgänglig i din Workfront-instans om det här alternativet är inaktiverat. Mer information finns i <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Inbyggda åtkomstnivåer i Workfront</a>.</p> </td> 
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
      <td role="rowheader">Användare i systemet ser som standard den nya hemupplevelsen </td> 
      <td>Här kan du ange om användare ska se den nya hemupplevelsen som standard. I båda fallen kan användarna välja att aktivera eller inaktivera Nytt hem på individnivå. Det här alternativet är aktiverat som standard.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **Spara**.

   De ändringar du har sparat här påverkar upplevelsen för alla användare i Workfront och alla som interagerar med dem som externa användare.

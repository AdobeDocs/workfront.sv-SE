---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Konfigurera grundläggande information för ditt system
description: Som en del av konfigureringen av ditt Adobe Workfront-system kan du hantera information om din organisation under Grundläggande information på kundinformationssidan.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bad5e700-79a6-49ed-bcf9-f0b5b3eaa909
source-git-commit: 83d236a4d50c0eef7062f161757d2f9fe6bc4e06
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 0%

---

# Konfigurera grundläggande information för ditt system

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>-->

Som en del av konfigureringen av ditt Adobe Workfront-system kan du hantera information om din organisation under Grundläggande information på kundinformationssidan.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p>Nytt: Standard</p>
   eller
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

## Visa kundinformation

Kunden representerar Workfront-instansen för er organisation. Alternativen här är unika för dig som kund till Workfront.

Så här öppnar du sidan Kundinformation:

{{step-1-to-setup}}

1. Klicka på **System** > **Kundinformation** i den vänstra panelen.

   Beroende på vilken Workfront-plan du har köpt kan vissa avsnitt saknas på sidan Kundinformation. Kontakta din kontorepresentant om du behöver ta reda på vilken Workfront-plan din organisation använder.

   De avsnitt som är tillgängliga i området Kundinformation är:

   * **Grundläggande information**

     Information om hur du konfigurerar grundläggande information i Workfront finns i [Konfigurera grundläggande information](#configure-basic-info).

   * **API-nyckelinställningar**

     Mer information om API-nyckelinställningar finns i [Hantera API-nycklar](../../administration-and-setup/manage-workfront/security/manage-api-keys.md).

   * **IP-Tillåtelselista**

     Mer information om hur du lägger till IP-adresserna till tillåtelselista för var dina användare kan få åtkomst till Workfront finns i [Konfigurera din brandväggs tillåtelselista](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   * **E-post Tillåtelselista**

     Mer information om hur du lägger till e-postmeddelanden till tillåtelselista finns i [Konfigurera din e-post med tillåtelselista](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).

   <!--
   * **License**

     For information about licenses, see [Manage available licenses in your system](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).-->

## Konfigurera grundläggande information {#configure-basic-info}

I området Grundläggande information på kundinformationssidan konfigureras viss kundinformation av Workfront och visas i skrivskyddat läge. Du kan konfigurera annan information. Alla alternativ som du kan redigera i det här området påverkar alla användare i Workfront globalt.

Så här konfigurerar du avsnittet Grundläggande information i området Kundinformation:

{{step-1-to-setup}}

1. Klicka på **System** > **Kundinformation** i den vänstra panelen.

1. I avsnittet **Grundläggande information** högst upp på sidan **Kundinformation** hittar du följande information om din instans med Workfront:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Namn</td> 
      <td>Namnet på din organisation, som också matchar namnet på ditt företag. Detta har lagts till av Workfront och kan inte redigeras.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Klusterinställning </td> 
      <td>Klusternumret för din instans.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Admin-e-postadress</td> 
      <td> <p>E-postadressen till din Workfront-administratör. Du kan redigera det här fältet så att det matchar e-postadressen för en av dina Workfront-administratörer. Den användare som är kopplad till den här e-postadressen betraktas som Workfront-huvudadministratör för ditt Workfront-system. All kommunikation från Workfront på hela webbplatsen dirigeras till den här e-postadressen, så det är viktigt att du håller den uppdaterad.</p> <p><b>Obs!</b> Du kan inte inaktivera, ta bort eller ändra åtkomstnivån för användaren som är kopplad till Admin-e-postadressen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Domän</td> 
      <td> <p>Domänen anges av Workfront när ditt konto skapas.</p> <p>Domänen identifierar din unika underdomän till den URL som du använder för att komma åt Workfront.<p>Om din organisation till exempel har tilldelats domänen "mincompany" är den URL som du använder för att komma åt Workfront <i>https://mycompany.my.workfront.com.</i></p><p>Du kan inte redigera domänen själv. Om du vill byta domän kan du kontakta Workfront kundsupport. Mer information om hur du kontaktar Workfront kundsupport finns i <a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Kontakta kundsupport</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tidszon</td> 
      <td> <p>Detta är standardtidszonen för din Workfront-instans. Du kan redigera det här fältet så att det matchar tidszonen för din primära Workfront-plats. Den tidszon du väljer avgör följande: </p> 
       <ul> 
        <li>Datum och tid som visas i utgående e-postmeddelanden</li> 
        <li>Standardtidszonen för nya användare när de skapas</li> 
       </ul> <p>Användare kan ändra tidszonen för sin Workfront-instans under sin profil. När användare ändrar sin tidszon matchar datumet och tiden i sina e-postmeddelanden från Workfront deras profilinställningar. Mer information om hur du ändrar inställningar för användarprofiler finns i <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Konfigurera mina inställningar</a>. Den väljs som standardtidszon när du skapar ett nytt schema. Mer information om hur du skapar scheman finns i <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Skapa ett schema</a>.</p> <p>Mer information om hur du använder scheman för att hjälpa användare att samarbeta i Workfront över tidszoner finns i <a href="../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Arbeta över tidszoner</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Standardspråk för e-post</td> 
      <td>Styr vilket språk, datum och nummerformat som används i utgående e-postmeddelanden. Det språkområde som väljs här är standard när nya användare skapas. Användare kan ändra sina nationella inställningar i sin användarprofil. När användare ändrar sitt språkområde matchar formatet för språk, datum och nummer i sina e-postmeddelanden från Workfront deras profilinställningar. Mer information om hur du ändrar profilinställningarna finns i <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Konfigurera mina inställningar</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lagringskvot</td> 
      <td> <p>Detta är mängden tillgängligt dokumentlagringsutrymme i din Workfront-instans.<br>Kvoten innehåller dokument som du överför direkt till Workfront.<br>Den innehåller inte:</p> 
       <ul> 
        <li>Dokument som du länkar till Workfront från någon annan tredjepartstjänsteleverantör (SharePoint, Google Drive, Webdam, Box, Dropbox eller någon annan leverantör av Document Asset Management).</li> 
        <li>Dina Workfront-data (projekt, uppgifter, problem, användare och så vidare).</li> 
       </ul> </td> 
     </tr>
    </tbody> 
   </table>

1. Klicka på **Spara**.

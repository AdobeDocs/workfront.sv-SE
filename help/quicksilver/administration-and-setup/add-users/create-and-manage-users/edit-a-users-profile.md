---
title: Redigera en användares profil
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Som Adobe Workfront-administratör kan du skapa nya användare och hantera befintliga profiler.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: 20cb940de1d42057ed11e4e7d59f1875cdba38bb
workflow-type: tm+mt
source-wordcount: '3297'
ht-degree: 0%

---

# Redigera en användares profil

{{highlighted-preview}}

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

Som Adobe Workfront-administratör kan du skapa användare och hantera befintliga profiler. Mer information om hur du skapar användare finns i [Lägg till användare](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande för att kunna utföra stegen i den här artikeln:

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
   <td> <p>Nytt: Standard</p>
   eller
   <p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste ha något av följande:</p> 
    <ul> 
     <li> <p>Åtkomstnivån Systemadministratör. Mer information finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>. </p> </li> 
     <li> <p>Objektet <b>Användare</b> på din åtkomstnivå har konfigurerats till <b>Redigera</b> åtkomst, med <b>Skapa</b> och minst ett av följande två <b>användaradmin</b>-alternativ som har aktiverats under <b>Finjustera inställningarna</b> <img src="assets/gear-icon-in-access-levels.png">. </p> 
     <ul><li> Användaradministratör (alla användare)</li>
     <li>Användaradministratör (gruppanvändare)</li></ul>
     <p>Om <b>Användaradministratör (gruppanvändare)</b> är aktiverat måste du vara gruppadministratör för en grupp där användaren är medlem för att kunna redigera användaren.</p> 
     <p>Mer information om inställningen <b>Användare</b> på en åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst till användare</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

+++

## Redigera en användarprofil

{{step-1-to-users}}

1. Markera användaren och klicka sedan på ikonen **Redigera** ![](assets/edit-icon.png) .

   Rutan Redigera användare visas.

1. I rutan **Redigera användare** ändrar du någon av följande information och klickar sedan på **Spara ändringar** när som helst:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Personlig information </td> 
      <td> 
       <ul> 
        <li><p><b>Förnamn</b></p></li>
        <li><p><b>Efternamn</b></p></li> 
        <li> <p><b>E-postadress:</b> E-postadressen för en användare är även användarens användarnamn i Workfront. Fältet är skiftlägeskänsligt och måste vara unikt. Om någon användare försöker lägga till en icke-unik e-postadress tre gånger i ett 10-minutersfönster visas ett reCAPTCHA-svar.</p> <p> Välj inställningen <b>Jag är inte en robot</b> innan du kan fortsätta.</p><p>Om du använder e-postadressen tillåtelselista och anger en e-postdomän som inte finns med i listan får användaren inga e-postmeddelanden. Mer information om tillåtelselista finns i <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">Konfigurera din e-postadress med tillåtelselista</a>.</p> </li> 
        <li> <p><b>Återställ lösenord</b>: Klicka på den här länken om du vill återställa användarens lösenord. Du måste ange ditt eget lösenord innan du kan återställa en annan användares lösenord.</p> <p>Om du vill återställa en annan användares lösenord måste du vara Workfront-administratör eller gruppadministratör.</p> <p><b>OBS</b>:  
          <ul> 
           <li> <p>Om du är gruppadministratör kan du bara återställa lösenord för användare i de grupper där du är utsedd till administratör. Behörigheten Användaradministratör (gruppanvändare) måste även aktiveras på din åtkomstnivå:</p> <p> <img src="assets/group-admin-user.png" > </p> <p>Den här inställningen är inaktiverad som standard. Mer information finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </li> 
           <li> <p>Du kan inte återställa lösenordet för en Workfront-administratör.</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;SSO-konfiguration&gt; Användarnamn</b>: Om Workfront-administratören har aktiverat en SSO-integrering med Workfront visas SSO-användarnamnet i det här fältet. Den typ av SSO-konfiguration som är aktiverad för din Workfront-instans visas i det här fältet. </li> 
        <li> <p><b>Tillåt endast &lt;SSO-konfiguration&gt;-autentisering</b>: Om din Workfront-administratör har aktiverat en SSO-integrering med Workfront och har uppdaterat alla användare för enkel inloggning, är det här fältet markerat som standard. Den typ av SSO-konfiguration som är aktiverad för din Workfront-instans visas i det här fältet.</p> <p>När det här fältet är markerat måste användaren logga in på Workfront med sina SSO-inloggningsuppgifter. Om du avmarkerar den kan de logga in på Workfront med sina Workfront-inloggningsuppgifter.</p> <p>Mer information om hur du konfigurerar Workfront med en SSO-lösning finns i <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Översikt över enkel inloggning i Adobe Workfront</a></p> <p>Mer information om hur du uppdaterar användare för enkel inloggning finns i <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Uppdatera användare för enkel inloggning</a>.</p> 
        <p><b>OBS</b>:</p> 
        <p> Om du är gruppadministratör kan du bara redigera fälten för &lt;SSO-konfiguration&gt; för användare i de grupper där du är utsedd som sådan. Behörigheten Användaradministratör (gruppanvändare) måste även aktiveras på din åtkomstnivå.
        <p>Om du är gruppadministratör och har behörigheten Användaradministratör (alla användare) aktiverad på din åtkomstnivå kan du redigera &lt;SSO-konfiguration&gt;-fälten för alla användare.</p> </li> 
        <li><b>Jobbinformation:</b> Information om jobbet, t.ex. jobbtiteln (i fältet <b>Titel</b>) och vilket expertområde användaren ansvarar för (i fältet <b>Tala med mig om</b>).</li> 
        <li><p><b>Kontaktinformation</b>: Användarens telefonnummer (i telefonnumret <b>Ext).</b> och <b>Mobile number</b> (fält) och adress (i fälten <b>Address, City, State, Postal Code, Country</b> ).</p>
        <p>Om användaren har aktiverats för Unified User Management (UUM) eller Adobe Identity Management System (IMS), godtar fältet <b>Country</b> i avsnittet Kontaktinformation bara landskodsvärden (till exempel US, GB, IN).</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inställningar </td> 
      <td> 
       <ul> 
      <li> <p><b>Tidszon:</b> Användarens tidszon.</p> <p>Mer information om hur du kan hjälpa användare att samarbeta i Workfront över tidszoner finns i <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Arbeta över tidszoner</a>.</p> </li> 
       <li><b>Språk för e-post</b>: Användarens rekommenderade e-postspråk. Detta påverkar formatet för siffror och datum i e-postmeddelanden som kommer från Workfront till den här användaren.</li>

   <li><b>Ta emot e-postmeddelanden från den här testmiljön</b>: Markera det här alternativet om du vill ta emot e-postmeddelanden från miljön som du är inloggad i.
      <p><b>ANMÄRKNING</b></p>
      <p>Det här alternativet är bara tillgängligt i förhandsgransknings- och sandlådemiljöer. E-postmeddelanden är som standard aktiverade i produktionsmiljön. </p>
      </li>

   </li> 
       <li><b>Skicka jobb som jag själv har tilldelat mig själv till fliken Arbeta med</b>: Markera det här alternativet om du vill att allt som användaren tilldelar sig ska visas direkt i listan Arbeta på hemsidan. Som standard visas allt som tilldelats en användare i listorna Ready to Start eller Not Ready (Klart att starta) i området Home (Hem).</li> 
       <li><b>Generera automatiskt korrektur när dokument överförs</b>: Markera det här alternativet om du vill att de dokument som användaren överför ska generera ett korrektur omedelbart. </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Meddelanden</td> 
      <td> <p>Välj de e-postmeddelanden som ska aktiveras för den nya användaren.</p> <p>Du kan välja både snabbmeddelanden och dagliga sammanfattningsmeddelanden.</p> <p>Mer information finns i <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Konfigurera händelsemeddelanden för alla i systemet</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Åtkomst</td> 
      <td> 
       <ul> 
      <li><b>Är aktiv:</b> Markera den här rutan för att ange att användaren är aktiv. Aktiva användare använder en Workfront-licens. Om du avmarkerar rutan inaktiveras användaren och användaren hindras från att logga in på Workfront.</li> 
       <li> <p><b>Åtkomstnivå:</b> Välj den åtkomstnivå som ska tilldelas den här användaren.</p> 
       <p>När du tilldelar en åtkomstnivå till en användare kan du tilldela en nivå som är lika med eller lägre än din egen åtkomstnivå.</p>
       <p>Om åtkomstnivån till exempel är Plan kan du inte tilldela åtkomstnivån Administratör. Du kan dock inte tilldela en åtkomstnivå som är lägre än din egen åtkomstnivå om Workfront-administratören har aktiverat icke-standardbehörigheter på åtkomstnivån som inte är aktiverade på din egen åtkomstnivå. </p>
       <p>Om du t.ex. har en planlicens utan tillgång till borttagningsuppgifter, kan du inte tilldela någon en arbetslicens med åtkomst till borttagningsuppgifter även om arbetslicensen är lägre än planlicensen. Mer information finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>. </p> 
       <p>Mer information om åtkomstnivåer finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Konfigurera åtkomst till Adobe Workfront</a>.</p>
       <p> <b>OBS!</b></p> 
       <p> Om din organisation använder den nya åtkomstmodellen (Standard/Light/Contributor) kan du inte tilldela om en Standard- eller Light-användare till en Contributor-åtkomstnivå om användaren redan har nått sin beslutsgräns för månaden. </p><p>Mer information om den nya åtkomstmodellen finns i <a href="../how-access-levels-work/access-level-overview.md" class="MCXref xref">Översikt över nya åtkomstnivåer</a>. </p><p>Mer information om beslutsbegränsningar finns i <a href="/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md" class="MCXref xref">Begränsat dokument och en översikt över korrektur för obetalda användare</a>.</p></li> 
       <li> <p><b>Layoutmall</b>: Välj en layoutmall för användaren. Den här layoutmallen har företräde framför alla layoutmallar som har tilldelats användarens hemgrupp, hemteam eller primära roll. Mer information om tilldelningsprioriteten för layoutmallar finns i <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Skapa och hantera layoutmallar</a>.</p> <p><b>OBS</b>:  <p>Följande lista beskriver hur listan med mallar som du har tillgängliga i det här fältet beror på din åtkomst:</p> 
       <ul> 
       <li>Som Workfront-administratör kan du se alla layoutmallar på system- och gruppnivå.</li> 
       <li>Som gruppadministratör kan du se layoutmallar på systemnivå samt de som är kopplade till de grupper som du hanterar.</li> 
       <li>Som användare med en planlicens och möjlighet att redigera användare, kan du bara se layoutmallar på systemnivå.</li> 
       </ul> <p>Mer information om layoutmallar på gruppnivå finns i <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Skapa och hantera layoutmallar</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organisation </td> 
      <td> 
       <ul> 
      <li><b>Företag</b>: Användarens företag. Användare kan bara associeras med ett företag. Du måste skapa ett företag innan du kan associera det med en användare. Endast aktiva företag visas i listan. Mer information om hur du skapar företag finns i <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Skapa och redigera företag</a>.</li> 
      <li><b>Rapporterar till:</b> Om du har angett ett företag för användaren kan du även ange användarens direkta hanterare i det här fältet. En användare kan bara ha en hanterare. Det här fältet visas inte om användaren inte är associerad med ett företag först. </li> 
      <li><b>Direktrapporter:</b> Om du har angett ett företag för användaren kan du även ange användares direktrapporter. En användare kan ha flera direktrapporter. Det här fältet visas inte om användaren inte är associerad med ett företag först.</li> 
      <li><b>Hemteam</b>: Ange hemteamet för användaren. Användare kan bara ha ett hemteam. Hemteamet är viktigt när du tilldelar en layoutmall eller när du definierar knappen Arbeta med det för uppgifter och ärenden som tilldelats användaren. </li> 
      <li><b>Andra team</b>: Användare kan tillhöra flera team. En användare kan visa arbetsobjekt som är tilldelade något av deras team i hemområdet. </li> 
      <li> <p><b>Hemgrupp:</b> Välj en lämplig grupp att tilldela användaren till. Detta ger användaren möjlighet att komma åt objekt som delas med gruppen. Du kan också dela layoutmallar med användarens hemgrupp.</p> <p>Detta är ett obligatoriskt fält. Alla användare måste vara kopplade till en hemgrupp. Om du inte väljer någon grupp tilldelas gruppen som den nya användarens hemgrupp.</p> <p><b>OBS</b>:</p> 
      <p> Du kan bara tilldela en grupp till en användare om något av följande är sant:</p>
      <ul><li>du är Workfront-administratör</li>
      <li>du är administratör för gruppen</li>
      <li>Gruppen är offentlig.</li></ul> 
      <li> <p><b>Andra grupper</b>: Användare kan tillhöra flera grupper. Du kan bara tilldela en grupp till en användare om du är Workfront-administratör, är administratör för gruppen eller om gruppen är offentlig.</p> <p><b>VIKTIGT</b>:</p> 
      <p>Om du lägger till en användare i fler än 100 grupper kan prestandaproblem uppstå i alla områden i Workfront som läser in listan med grupper.</p> <p>Mer information om publika grupper finns i <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Skapa en grupp</a>.</p> <p>Mer information om grupper finns i <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Översikt över grupper</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resursplanering </td> 
      <td> 
       <ul>
       <li>
       <b>Arbetstid</b>: Representerar den procentandel av heltidsekvivalenttiden (FTE) som användaren är tillgänglig för det faktiska arbetet, exklusive extrakostnader. Arbetstiden måste vara ett decimaltal upp till 1 och får inte vara 0. Exempel: 20 % tillgänglighet för faktiskt arbete är 0,2.

   Fältets standardvärde är 1, vilket anger att en användare tillbringar hela sitt heltidsanställda på faktiskt, projektrelaterat arbete.

   Systemet använder det här talet för att beräkna användarens tillgänglighet för faktiskt, projektrelaterat arbete.

   Mer information om hur du skapar scheman i Workfront finns i <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Skapa ett schema</a>.

   Schemalagda undantag och ledig tid kan också påverka användarens kapacitet.

   Workfront beräknar en användares tillgänglighet beroende på inställningarna för resurshantering i inställningsområdet. Mer information finns i <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Konfigurera inställningar för resurshantering</a>.

   <b>TIPS</b>

   Ange värdet 1 för Arbetstid för att ange att användaren är tillgänglig för projektrelaterat arbete och hela heltidsekvivalenten.
   </li> 
      <li> <b>Schemalägg inaktivering</b>: Markera den här kryssrutan om du vill schemalägga att den här användaren ska inaktiveras ett visst datum och vid en viss tidpunkt. </li> 
       <li><b>Schemalagt inaktiveringsdatum</b>: Det datum och den tidpunkt då användaren inaktiverades. Information om schemaläggning av användare för inaktivering finns i <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Schemalägg användare för inaktivering</a> i <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Inaktivera eller återaktivera en användare</a>.</li> 
       <li> <p><b>Primär roll</b>: Det här är den primära jobbrollen som användaren kan utföra i Workfront. Alla uppgifter och utgåvor som användaren är tilldelad till tilldelas även den här jobbrollen. Jobbroller är viktiga i resurshanteringen. Du kan bara uppdatera det här fältet om du har en planlicens med administratörsåtkomst eller om du är Workfront-administratör. Mer information om hur du konfigurerar användare med administrativ användaråtkomst finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst till användare</a>.</p> <p>Endast aktiva jobbroller visas i listan. </p> </li> 
       <li>Om du valde en <b>primär roll</b> visas fältet <b>Procent av FTE-tillgänglighet</b> . Ange hur många procent av tiden i användarens schema som ska tilldelas den här jobbrollen. Standardvärdet för procentandelen FTE-tillgänglighet för den primära rollen är 100 %. </li> 
       <li> <p><b>Andra roller</b>: En användare kan ha flera jobbroller i Workfront. Jobbroller är viktiga i resurshanteringen. Det finns ingen gräns för hur många jobbroller en användare kan utföra. Vi rekommenderar dock att du inte tilldelar en användare till ett för stort antal jobbroller eftersom resurshanteringen kan bli alltför komplex för dessa användare.<p>Endast aktiva jobbroller visas i listan. Mer information om jobbroller finns i <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Skapa och hantera jobbroller</a>.</p> <p>Du kan bara uppdatera det här fältet om du har en planlicens med administratörsåtkomst eller om du är Workfront-administratör. <br>Mer information om hur du konfigurerar användare med administrativ användaråtkomst finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst till användare</a>.</p> </li> 
       <li> <p>(Villkorligt) Om du markerade en eller flera <b>andra roller</b> visas fältet <b>Procent av FTE-tillgänglighet</b> för varje roll. Ange hur stor procentandel av tiden i användarens schema som ska tilldelas varje jobbroll. Standardvärdet för procentandelen FTE-tillgänglighet för andra roller är 0 %.</p> <p><b>Obs!</b> Om andra roller har FTE-tillgänglighet på 0 % visas de inte i resursplaneraren, såvida inte användarna har tilldelats till aktiviteter i de här rollerna.</p> <p> <img alt="user_settings_roles_and_date_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>OBS</b>: <p>Summan av alla <b>procent FTE-tillgänglighet</b> för alla roller måste vara lika med 100 %. Varje procentandel av FTE-tillgänglighet beräknar tillgängliga timmar för varje roll per användare i resursplaneraren. Tillgängliga timmar för varje roll per användare beror på användarens tillgängliga tid.</p> <p>Den tillgängliga tiden för användaren beräknas av Workfront utifrån den metod som Workfront-administratören har valt för att beräkna FTE i Inställningar för resurshantering.</p> <p>Mer information om hur du beräknar tillgänglighet för användaren finns i <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Översikt över beräkning av timmar och FTE för användare och roller i resursplaneraren</a>.</p> <p>Mer information om hur du konfigurerar inställningar för resurshantering finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Konfigurera inställningar för resurshantering</a>.</p> </p>
       <span class="preview"><p>(Valfritt) Rolltilldelningar för giltighetsdatum används i ekonomiska beräkningar om användarens jobbroll ändras under ett projekt.</p><p>Klicka på <b>Definiera roller efter datum</b>, välj <b>Primär roll</b> och <b>Andra roller</b> och ange allokeringsprocenten för varje roll. Rollerna kan vara desamma som de befintliga rollerna (med olika procentandelar) eller nya roller. Välj <b>Startdatum</b> när de här rollerna blir aktiva. Detta kan vara ett framtida datum. När de senaste rollerna blir aktiva kan du klicka på <b>Visa tidigare roller</b> för att visa föregående, inaktiva roller.</p> </li></span>
       <li> <p><b>Schema</b>: Associera ett schema med användaren. Schemat för användaren beräknar tidslinjen för de uppgifter som användaren är tilldelad till.</p> <p>Du måste skapa ett schema innan du kan associera det med en användare. Mer information om hur du skapar scheman finns i <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Skapa ett schema</a>.</p> <p><b>Obs!</b> Vi rekommenderar att schemat som du associerar med användaren matchar användarens tidszon.</p> </li> 
       <li> <p><b>Tidrapportprofil</b>: Associera en tidrapportprofil med användaren för att säkerställa att tidrapporter genereras automatiskt för användaren.</p> <p><b>OBS</b>: Listan med profiler som du har tillgängliga i det här fältet beror på din åtkomst:
       <ul>
       <li>Som Workfront-administratör kan du se alla tidrapportprofiler på systemnivå och på gruppnivå.</li>
       <li>Som gruppadministratör kan du visa tidrapportprofiler på systemnivå, samt de som är kopplade till de grupper som du hanterar.</li>
       <li>Som användare med en planlicens och tillgång till att redigera användare kan du bara se tidrapportprofiler på systemnivå. Mer information om tidrapportprofiler på gruppnivå finns i <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">Skapa, redigera och tilldela tidrapportprofiler</a>.</li>
      </ul></p> </li> 
       <li><b>Standardtimtyp</b>: Välj standardtimtyp för användaren. Det här är timtypen som används som standard när användaren loggar tid.</li> 
       <li><b>Tillgängliga timtyper</b>: Välj de timtyper som ska vara tillgängliga för användaren. Dessa timtyper visas överallt i Workfront där användaren kan logga tid. En användare kan bara se timtyperna som är aktiverade på projektnivå och på användarnivå. Mer information om vilka timtyper som är tillgängliga för användare finns i <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Definiera timtyper och tillgänglighet</a>.</li> 
       <li><b>Logga in:</b> Välj om användaren ska logga in på arbetsposter i timmar eller dagar. Mer information finns i <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">Konfigurera om tiden är inloggad i timmar eller dagar</a>.</li>

   <li> <b>FTE</b>: Detta är heltidsmotsvarigheten för användaren. Workfront använder det här numret för att beräkna användarens tillgänglighet baserat på standardschemat endast när inställningarna för resurshantering på systemnivå är inställda på standardschemat.

   <p>FTE anger hur lång tid användaren kan tillbringa på jobbet. Detta inkluderar overheadkostnader och tid för projektarbete. Till exempel ingår även tid som används i möten eller utbildning i heltidsanställda.</p>

   FTE måste vara ett decimaltal upp till 1 och det får inte vara 0. Om till exempel FTE-värdet är 0,5 och standardschemat i Workfront är 40 timmar är användaren tillgänglig för 20 timmar i veckan.

   Fältets standardvärde är 1.

   Schemalägg undantag, eventuell ledig tid och värdet på Arbetstid kan påverka användarens tillgänglighet.

   Workfront beräknar en användares tillgänglighet beroende på inställningarna för resurshantering i inställningsområdet.

   Om inställningarna för resurshantering på systemnivå är inställda på Användarens schema, ignoreras det värde du anger här och användaren anses vara tillgänglig enligt det som anges i deras schema.

   Mer information finns i <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Konfigurera inställningar för resurshantering</a>.

   Mer information om hur du skapar scheman i Workfront finns i <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Skapa ett schema</a>.
   </li>

   <li><b>Resurspooler</b>: Associera användaren med resurspooler. Mer information finns i <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Associera resurspooler med användare </a>.</li>

   <li><b>Kostnadsnivå</b>: Kostnadsbeloppet per timme för användaren.
      <p>Klicka på <strong>Lägg till kurs</strong> om du vill se datumfaktiska kostnadstariffer. Ange värdet för kostnadstariffen för tidsperioden och tilldela startdatum och slutdatum efter behov. Kostnadsnivå 1 har inget startdatum och den sista kostnadstariffen har inget slutdatum.</p><p>Vissa datum läggs till automatiskt. Om t.ex. Kostnadsgrad 1 inte har ett slutdatum och du lägger till Kostnadsnivå 2 med startdatumet 1 maj 2023, läggs ett slutdatum som är 30 april 2023 till Kostnadsnivå 1 så att inga luckor uppstår.</p></li>

   <li><b>Faktureringshastighet</b>: Användarens faktureringsbelopp per timme.
      <p>Klicka på <strong>Lägg till ränta</strong> om du vill se gällande faktureringspriser för datum. Ange faktureringsvärdet för tidsperioden och tilldela startdatum och slutdatum efter behov. Faktureringsränta 1 har inget startdatum och den senaste faktureringstakten har inget slutdatum.</p> <p>Vissa datum läggs till automatiskt. Om till exempel Faktureringstariff 1 inte har något slutdatum och du lägger till en andra med startdatumet 1 maj 2023, läggs ett slutdatum som är 30 april 2023 till Faktureringstariff 1 så att inga luckor uppstår.</p><p> <img alt="Användarkostnader och faktureringstariffer" src="assets/edit-user-cost-billing-rate-2.png"> </p></li>

   </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anpassad Forms</td> 
      <td><p>Koppla ett befintligt anpassat formulär till den här användaren. Du måste skapa ett anpassat formulär innan du kan koppla det till en användare. Endast aktiva anpassade formulär visas i listan. Fält som du inte har behörighet att redigera visas inte i ett anpassat formulär.</p> <p><strong>Obs!</strong> Avancerade anpassade formulärfunktioner som externa sökningsfält och inbyggda Workfront-fält är bara tillgängliga när du öppnar användarposten på informationssidan, inte i dialogrutan Redigera användare. (I listan över användare klickar du på användarnamnet för att öppna informationen.)</p> <p>Mer information om hur du skapar anpassade formulär finns i <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md" class="MCXref xref">Designa ett formulär med formulärdesignern</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kommentar</td> 
      <td>Skriv den kommentar du vill skicka till användarna och till uppdateringsområdet för deras användarprofiler.</td> 
     </tr> 
    </tbody> 
   </table>

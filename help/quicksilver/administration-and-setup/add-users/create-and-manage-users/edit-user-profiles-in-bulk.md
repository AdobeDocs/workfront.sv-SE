---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Redigera användarprofiler gruppvis
description: Som Adobe Workfront-administratör kan du redigera flera användarkonton samtidigt.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: cb709b2f-659e-4110-81ac-a1ef967d534c
source-git-commit: c7b91828e5a4f961fc48e857eb63756b9b38f664
workflow-type: tm+mt
source-wordcount: '2625'
ht-degree: 0%

---

# Redigera användarprofiler gruppvis

{{highlighted-preview}}

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Bulk Upload Users](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

Du kan redigera flera användarkonton samtidigt. När användare gruppredigeras uppdateras endast de fält som du specifikt markerar med samma information för alla markerade användare. Alla andra fält som du lämnar omarkerade förblir desamma för varje enskild användare, även om de är olika för varje användare.

>[!NOTE]
>
>* Du kan inte redigera personlig information i användarprofilerna gruppvis eftersom informationen måste vara unik för varje användare.
>* För att säkerställa att data är korrekta och att prestanda är optimala rekommenderar vi att du inte väljer fler än 2 000 användare åt gången för en massredigering.
>

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
   <td><p>Nytt: Standard</p><p>eller</p><p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste ha något av följande:</p> 
    <ul> 
     <li> <p>Åtkomstnivån Systemadministratör. </li> 
     <li> <p><b>Användare</b> i din åtkomstnivå har konfigurerats till <b>Redigera</b> åtkomst, med <b>Skapa</b> och minst ett av de två <b>användaradministratörsalternativen</b> som har aktiverats under <b>Finjustera inställningarna</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Om <b>Användaradministratör (gruppanvändare)</b> är aktiverat måste du vara gruppadministratör för en grupp där användaren är medlem.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Redigera flera användarkonton samtidigt

{{step-1-to-users}}

1. Markera flera användare och klicka sedan på ikonen **Redigera** ![Redigera](assets/edit-icon.png) .

1. I rutan **Redigera användare** ändrar du informationen i något av avsnitten och klickar sedan på **Spara ändringar** <span class="preview"> eller **Spara**</span> när som helst.

### Inställningar

* **Tidszon**: Användarens tidszon.

  Mer information om hur du kan hjälpa användare att samarbeta i Workfront över tidszoner finns i [Arbeta över tidszoner](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

* **Språk för e-post**: Användarens rekommenderade e-postspråk. Detta påverkar formatet för siffror och datum i e-postmeddelanden som kommer från Workfront till den här användaren.

  >[!NOTE]
  >
  >När din organisation använder Adobe Unified Experience lagras användarens språkinställningar i sin Adobe-profil och e-postspråkinställningen används inte. Mer information om hur du använder de här inställningarna finns i [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

### Meddelanden

Välj de e-postmeddelanden som ska aktiveras för användarna.

Du kan välja både snabbmeddelanden och dagliga sammanfattningsmeddelanden. Alla dagliga meddelanden om sammandrag levereras någon gång efter samma tid för alla användare som du har valt.

Mer information finns i [Konfigurera händelsemeddelanden för alla i systemet](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

### Åtkomst

* **Är aktiv** / <span class="preview">**Användaren är aktiv**</span>: Aktivera det här alternativet om du vill ange att användarna är aktiva. Aktiva användare använder en Workfront-licens. Om du inaktiverar fältet inaktiveras användarna och de hindras från att logga in på Workfront.

* **Åtkomstnivå**: Välj den åtkomstnivå som ska tilldelas dessa användare. Alla användare som du har valt får samma åtkomstnivå.

  När du tilldelar en åtkomstnivå till användare kan du tilldela en nivå som är lika med eller lägre än din egen åtkomstnivå. (Om åtkomstnivån till exempel är Standard kan du inte tilldela åtkomstnivån Administratör.)

  Du kan dock inte tilldela en åtkomstnivå som är lägre än din egen åtkomstnivå om Workfront-administratören har aktiverat icke-standardbehörigheter på åtkomstnivån som inte är aktiverade på din egen åtkomstnivå.

  Om du till exempel har en Standard-licens utan åtkomst till borttagningsåtgärder, kan du inte tilldela någon en Light-licens med åtkomst till borttagningsåtgärder även om Light-licensen är lägre än Standard-licensen. Mer information finns i [Skapa eller ändra anpassade åtkomstnivåer](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

  Mer information om åtkomstnivåer finns i [Konfigurera åtkomst till Adobe Workfront](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md).

  >[!NOTE]
  >
  >Om din organisation använder den nya åtkomstmodellen (Standard/Light/Contributor) kan du inte tilldela om en Standard- eller Light-användare till en Contributor-åtkomstnivå om användaren redan har nått sin beslutsgräns för månaden.
  >
  >Mer information om den nya åtkomstmodellen finns i [Översikt över nya åtkomstnivåer](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).
  >
  >Mer information om beslutsbegränsningar finns i [Begränsat dokument och en översikt över korrektur för obetalda användare](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

* **Layoutmall**: Välj en layoutmall för användarna. den här layoutmallen har företräde framför layoutmallar som tilldelats till deras hemgrupp, hemteam eller primära roll. Mer information om tilldelningsprioriteten för layoutmallar finns i [Skapa och hantera layoutmallar](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

  Följande lista beskriver hur listan med mallar som du har tillgängliga i det här fältet beror på din åtkomst:

   * Som Workfront-administratör kan du se alla layoutmallar på system- och gruppnivå.
   * Som gruppadministratör kan du se layoutmallar på systemnivå samt de som är kopplade till de grupper som du hanterar.
   * Som användare med en Standard- eller Plan-licens och tillgång till redigeringsanvändare kan du bara se layoutmallar på systemnivå.

     Mer information om layoutmallar på gruppnivå finns i [Skapa och ändra en grupps layoutmallar](/help/quicksilver/administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

### Organisation

* **Företag**: Användarnas företag. Användare kan bara associeras med ett företag. Du måste skapa ett företag innan du kan associera det med en användare. Endast aktiva företag visas i listan. Mer information om hur du skapar företag finns i [Skapa och redigera företag](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* **Hemteam**: Ange hemteamet för användarna. Användare kan bara ha ett hemteam.
* **Andra team**: Användare kan tillhöra flera team.
* **Hemgrupp** / <span class="preview">**Aktuell hemgrupp**</span>: Välj en lämplig grupp att tilldela användarna. Detta ger användarna möjlighet att komma åt objekt som delas med gruppen. Du kan också dela layoutmallar med en hemgrupp.

  Detta är ett obligatoriskt fält. Alla användare måste vara kopplade till en hemgrupp. Om du inte väljer någon får din hemgrupp behörigheten Hemgrupp.

  Du kan bara tilldela en grupp till en användare om något av följande är sant:

   * du är Workfront-administratör
   * du är administratör för gruppen
   * gruppen är offentlig

* **Andra grupper**: Användare kan tillhöra flera grupper. Du kan bara tilldela en grupp till en användare om du är Workfront-administratör, är administratör för gruppen eller om gruppen är offentlig.

  >[!IMPORTANT]
  >
  >Om du lägger till en användare i fler än 100 grupper kan prestandaproblem uppstå i alla områden i Workfront som läser in listan med grupper.

  Mer information om publika grupper finns i [Skapa en grupp](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

  Mer information om grupper finns i [Översikt över grupper](/help/quicksilver/administration-and-setup/manage-groups/groups-overview/groups.md).

### Resursplanering

* **Arbetstid**: Representerar den procentandel av heltidsekvivalenttiden (FTE) som användarna är tillgängliga för det faktiska arbetet, exklusive extrakostnader. Arbetstiden måste vara ett decimaltal upp till 1 och får inte vara 0. Exempel: 20 % tillgänglighet för faktiskt arbete är 0,2.

  Fältets standardvärde är 1, vilket anger att en användare tillbringar hela sitt heltidsanställda på faktiskt, projektrelaterat arbete.

  Systemet använder det här talet för att beräkna användarens tillgänglighet för faktiskt, projektrelaterat arbete.

  Mer information om hur du skapar scheman i Workfront finns i [Skapa ett schema](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

  Schemalagda undantag och ledig tid kan också påverka användarens kapacitet.

  Workfront beräknar en användares tillgänglighet beroende på inställningarna för resurshantering i inställningsområdet. Mer information finns i [Konfigurera inställningar för resurshantering](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

  >[!TIP]
  >
  >Ange värdet 1 för Arbetstid för att ange att användaren är tillgänglig för projektrelaterat arbete och hela heltidsekvivalenten.

* **Schemalägg inaktivering** / <span class="preview">**Ange inaktiveringsdatum**</span>: Markera den här kryssrutan / <span class="preview">klicka på den här knappen</span> om du vill att de här användarna ska inaktiveras ett visst datum och vid en viss tidpunkt.
* **Schemalagt inaktiveringsdatum** / <span class="preview">**Inaktiveringsdatum**</span>: Det datum och den tidpunkt då användarna inaktiverades. Mer information om schemaläggning av användare för inaktivering finns i [Schemalägg användare för inaktivering](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#schedule-users-for-deactivation) i [Inaktivera eller återaktivera en användare](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
* **Primär roll**: Detta är den primära jobbrollen som användare kan utföra i Workfront. Alla uppgifter och utgåvor som användarna har tilldelats tilldelas också den här jobbrollen. Jobbroller är viktiga i resurshanteringen. Du kan bara uppdatera det här fältet om du har en Standard- eller Plan-licens med administratörsbehörighet eller om du är Workfront-administratör. Mer information om hur du konfigurerar användare med administrativ användaråtkomst finns i [Bevilja åtkomst till användare](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

  Endast aktiva jobbroller visas i listan.

* (Villkorligt) Om du valde en **primär roll** visas fältet **Procent av FTE-tillgänglighet** . Ange hur många procent av tiden för användarens scheman som ska tilldelas den här jobbrollen. Standardvärdet för procentandelen FTE-tillgänglighet för den primära rollen är 100 %.
* **Andra roller**: Användare kan ha flera jobbroller i Workfront. Jobbroller är viktiga i resurshanteringen. Det finns ingen gräns för hur många jobbroller en användare kan utföra. Vi rekommenderar dock att du inte tilldelar en användare till ett för stort antal jobbroller eftersom resurshanteringen kan bli alltför komplex för dessa användare.

  Endast aktiva jobbroller visas i listan. Mer information om jobbroller finns i [Skapa och hantera jobbroller](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

  Du kan bara uppdatera det här fältet om du har en Standard- eller Plan-licens med administratörsbehörighet eller om du är Workfront-administratör.

  Mer information om hur du konfigurerar användare med administrativ användaråtkomst finns i [Bevilja åtkomst till användare](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

* (Villkorligt) Om du markerade en eller flera **andra roller** visas fältet **Procent av FTE-tillgänglighet** för varje roll. Ange hur stor procentandel av tiden för användarens scheman som ska tilldelas varje jobbroll. Standardvärdet för procentandelen FTE-tillgänglighet för andra roller är 0 %.

  Om andra roller har 0 % FTE-tillgänglighet visas de inte i resursplaneraren, såvida inte användarna har tilldelats till uppgifter i de här rollerna.

  Summan av alla **procent FTE-tillgänglighet** för alla roller måste vara lika med 100 %. Varje procentandel av FTE-tillgänglighet beräknar tillgängliga timmar för varje roll per användare i resursplaneraren. Tillgängliga timmar för varje roll per användare beror på användarens tillgängliga tid.

  Den tillgängliga tiden för användaren beräknas av Workfront utifrån den metod som Workfront-administratören har valt för att beräkna FTE i Inställningar för resurshantering.

  Mer information om hur du beräknar tillgänglighet för användaren finns i [Översikt över beräkning av timmar och FTE för användare och roller i resursplaneraren](/help/quicksilver/resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

  Mer information om hur du konfigurerar inställningar för resurshantering finns i [Konfigurera inställningar för resurshantering](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **Schema**: Associera ett schema med användarna. Schemat för användarna beräknar tidslinjen för de uppgifter som användarna är tilldelade till.

  Du måste skapa ett schema innan du kan associera det med användare. Mer information om hur du skapar scheman finns i [Skapa ett schema](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

  >[!IMPORTANT]
  >
  >Workfront använder schemat för en användare endast när inställningen **Beräkna resurstillgänglighet med** är inställd på **Användarens schema**. Information om hur den här inställningen påverkar vilket schema som används för resurshantering finns i [Konfigurera inställningar för resurshantering](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **Tidrapportprofil**: Associera en tidrapportprofil med användarna för att säkerställa att tidrapporterna genereras automatiskt.

  Listan med profiler som är tillgängliga i det här fältet beror på din åtkomst:

   * Som Workfront-administratör kan du se alla tidrapportprofiler på systemnivå och på gruppnivå.
   * Som gruppadministratör kan du visa tidrapportprofiler på systemnivå, samt de som är kopplade till de grupper som du hanterar.
   * Som användare med en Standard- eller Plan-licens och tillgång till redigeringsanvändare kan du bara se tidrapportprofiler på systemnivå. Mer information om tidrapportprofiler på gruppnivå finns i [Skapa, redigera och tilldela tidrapportprofiler](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **Standardtimtyp**: Välj standardtimtyp för användarna. Det här är timtypen som används som standard när användaren loggar tid.
* **Tillgängliga timtyper**: Välj de timtyper som ska vara tillgängliga för användarna. De här timtyperna visas överallt i Workfront där användarna kan logga tid. Användarna kan bara se timtyperna som är aktiverade på projektnivå och på användarnivå. Mer information om vilka timtyper som är tillgängliga för användare finns i [Definiera timtyper och tillgänglighet](/help/quicksilver/timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
* **FTE**: Detta är heltidsmotsvarigheten för användarna. Workfront använder det här numret för att beräkna tillgängligheten för användare baserat på standardschemat endast när inställningarna för resurshantering på systemnivå är inställda på standardschemat.

  FTE anger hur lång tid användarna kan tillbringa på jobbet. Detta inkluderar overheadkostnader och tid för projektarbete. Till exempel ingår även tid som används i möten eller utbildning i heltidsanställda.

  FTE måste vara ett decimaltal upp till 1 och det får inte vara 0. Om till exempel FTE-värdet är 0,5 och standardschemat i Workfront är 40 timmar är användarna tillgängliga i 20 timmar i veckan.

  Fältets standardvärde är 1.

  Schemalägg undantag, ledig tid och värdet för Arbetstid kan påverka användarnas tillgänglighet.

  Workfront beräknar en användares tillgänglighet beroende på inställningarna för resurshantering i inställningsområdet.

  Om inställningarna för resurshantering på systemnivå är inställda på Användarens schema, ignoreras det värde du anger här och användaren anses vara tillgänglig enligt det som anges i deras schema.

  Mer information finns i [Konfigurera inställningar för resurshantering](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

  Mer information om hur du skapar scheman i Workfront finns i [Skapa ett schema](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* **Resurspooler**: Associera användarna med resurspooler.

  >[!NOTE]
  >
  >Endast de resurspooler som är gemensamma för alla markerade användare visas i det här fältet. Om de användare du har valt inte har några delade resurspooler är det här fältet tomt. Om det här fältet är tomt skrivs de resurspooler som du anger här över sina enskilda resurspooler.

  Mer information om resurspooler finns i [Associera resurspooler med användare](/help/quicksilver/resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md).

* **Kostnadsnivå**: Kostnadsbeloppet per timme för användaren.

  Klicka på **Lägg till kurs** om du vill se datumfaktiska kostnadstariffer. Ange värdet för kostnadstariffen för tidsperioden och tilldela startdatum och slutdatum efter behov. Kostnadsnivå 1 har inget startdatum och den sista kostnadstariffen har inget slutdatum.

  Vissa datum läggs till automatiskt. Om t.ex. Kostnadsgrad 1 inte har ett slutdatum och du lägger till Kostnadsnivå 2 med startdatumet 1 maj 2023, läggs ett slutdatum som är 30 april 2023 till Kostnadsnivå 1 så att inga luckor uppstår.

* **Faktureringshastighet**: Användarens faktureringsbelopp per timme.

  Klicka på **Lägg till ränta** om du vill se gällande faktureringspriser för datum. Ange faktureringsvärdet för tidsperioden och tilldela startdatum och slutdatum efter behov. Faktureringsränta 1 har inget startdatum och den senaste faktureringstakten har inget slutdatum.

  Vissa datum läggs till automatiskt. Om till exempel Faktureringstariff 1 inte har något slutdatum och du lägger till en andra med startdatumet 1 maj 2023, läggs ett slutdatum som är 30 april 2023 till Faktureringstariff 1 så att inga luckor uppstår.

### Anpassad Forms

Koppla ett befintligt anpassat formulär till användarna. Du måste skapa ett anpassat formulär innan du kan koppla det till en användare. Endast aktiva anpassade formulär visas i listan. Fält som du inte har behörighet att redigera visas inte i ett anpassat formulär.

>[!NOTE]
>
>Avancerade anpassade formulärfunktioner som externa sökningsfält och inbyggda Workfront-fält är bara tillgängliga när du öppnar användarposten på informationssidan, inte i dialogrutan Redigera användare. (I listan över användare klickar du på användarnamnet för att öppna informationen.)

Du kan också välja alternativet **Beräkna om anpassade uttryck** för att se till att alla beräknade anpassade fält i anpassade formulär som är kopplade till de valda användarna är uppdaterade.

Mer information om hur du skapar anpassade formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Kommentar

Skriv den kommentar du vill skicka till användarna och till uppdateringsområdet för deras användarprofiler.

<!--
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Preferences</td> 
      <td> 
       <ul> 
        <li><b>Time Zone:</b> The users' time zone.</li> 
        <li><b>Locale</b>: The users' preferred locale. This affects the format of numbers and dates in the emails that come from Workfront.</li> 
        <li><b>Send work I assign to myself to my Working On tab</b>: This setting refers to a deprecated feature that has been removed from Workfront.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications</td> 
      <td>Select the email notifications which should be enabled for the new user.<p>You can select instant as well as daily digest notifications. All the daily digest notifications are delivered sometime after the same time for all the users selected. For more information, see <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configure event notifications for everyone in the system</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Access</td> 
      <td> 
       <ul> 
        <li><b>Is Active:</b> Select this field to indicate whether the users are active. Active users use a Workfront license. Deselecting the field deactivates the users.</li> 
        <li> 
        <p><b>Access Level:</b> Select the access level to assign to these users. All users selected will have the same access level.
        </p> 
        <p>When you assign an access level to users, you can assign a level equal to or less than your own access level. (For example, if your access level is Planner, you cannot assign the Administrator access level.) </p>
        <p>However, you cannot assign an access level that is lower than your own if the Workfront administrator has enabled permissions on the access level that are not also enabled in your own (via the Fine-Tune settings, as described in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>).</p> 
        <p>For more information about access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configure access to Adobe Workfront</a>.</p> 
         </li> 
        <li> 
        <p><b>Layout Template</b>: Choose a layout template for the users. The layout template assigned to the users will take precedence over any layout template assigned to their Home Group, Home Team or primary job role. For more information about the assignment priority of layout template, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p> 
        <p><b>NOTE</b>:  The list of layout templates you have available in this field depends on your access:
          <ul>
           <li>As a Workfront administrator, you can see all system-level and group-level layout templates.</li>
           <li>As a group administrator, you can see system-level layout templates, as well as those associated with the groups that you manage.</li>
           <li><p>As a user with a Planner license and access to edit users, you can see only system-level layout templates. </p>
           <p>For information about group-level layout templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organization</td> 
      <td> 
       <ul> 
        <li><b>Company</b>: The company of the users. Users can be associated only with one company. You must create a company before you can associate it with a user. Only active companies display in the list. For information about creating companies, see Understanding and Managing Companies.</li> 
        <li><b>Home Team</b>: Specify the home team for the users. Users can only have one home team. </li> 
        <li><b>Other Teams</b>: Users can belong to multiple teams. </li> 
        <li> <p><b>Home Group:</b> Select an appropriate group to assign the users as their Home Group. This gives the user the ability to access objects that are shared with the group.</p> <p><b>NOTE</b>:  This is a required field. You cannot have users not associated with a Home Group.</p> <p>You can assign a group to users only in the following situations:</p> 
         <ul> 
          <li>You are a Workfront administrator.</li> 
          <li>You are the administrator of that group.</li> 
          <li>The group is public.</li> 
         </ul> </li> 
        <li> <p><b>Other Groups</b>: Users can belong to multiple groups. You can assign a group to a user only  in the following situations:</p> 
         <ul> 
          <li>You are a Workfront administrator.</li> 
          <li>You are the administrator of that group.</li> 
          <li> <p>The group is public. </p> 
          <p>For more information about public groups, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Create a group</a>.</p> 
          <p>For more information about groups, see <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Groups overview</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resource Planning</td> 
      <td> 
       <ul> 
      
      <li>
       <b>Work Time</b>: Represents the percentage of the Full Time Equivalent (FTE) time that the user is available for actual work, not including overhead. Work Time must be a decimal number up to 1, and it cannot be 0. For example, a 20% availability for actual work would be 0.2.

      The field's default is 1, indicating that a user spends their entire FTE on actual, project-related work. 

      The system uses this number to calculate the availability of the user for actual, project-related work. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.

      Schedule exceptions and time off might also affect the user capacity. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      <b>TIP</b>

      Set the Work Time value to  1 to indicate that the user is available for project-related work their entire full-time equivalent.
      </li> 

      <li><b>Schedule Deactivation</b>: Check this box if you want to schedule users to be deactivated after a period of time.</li> 
       <li><b>Scheduled Deactivation Date</b>: The date after which the users become deactivated. For more information about scheduling users for deactivation, see the section <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Schedule users for deactivation</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</li> 
       <li> <p><b>Primary Role</b>: This is the primary job role that a user has in Workfront. Every task and issue that the users are assigned to is also assigned to this job role, by default. Job roles are essential in resource management. For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a></p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li>(Conditional) If you selected a <b>Primary Role</b>, the <b>Percentage of FTE Availability</b> field displays. Specify what percentage of time of the users' schedules is allocated to this job role. The default value for the Percentage of FTE Availability for the Primary Role is 100%.</li> 
       <li> <p><b>Other Roles</b>: Users can have multiple job roles in Workfront. Job roles are essential in resource management. There is no limit for how many job roles a user can fulfill. However, we recommend to not assign one user to an excessively large number of job roles, because resource management might become too complex for these users.</p> <p>For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li> <p>(Conditional) If you selected one or multiple <b>Other Roles</b>, the <b>Percentage of FTE Availability</b> field displays for each role. Specify what percentage of time of the users' schedules is allocated to each job role. The default value for the Percentage of FTE Availability for the Other Roles is 0%.</p> <p><b>NOTE</b>:  
       <ul> 
       <li>If Other Roles have a 0% FTE Availability, they do not display in the Resource Planner, unless the users are assigned to tasks in these roles.</li> 
       <li> <p>The sum of all Percentages of FTE Availability for all roles must equal 100%. Each Percentage of FTE Availability calculates the Available Hours for each role per user in the Resource Planner. The Available Hours for each role per user depends on the available time for the user.</p> <p>The available time for the user is calculated by Workfront depending on the method that has been selected by the Workfront administrator to calculate the FTE in the Resource Management Preferences.</p> <p>For more information about calculating availability for the user, see <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> <p>For more information about configuring Resource Management preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>Schedule</b>: Associate a schedule with the users. The schedule of the users calculates the timeline of the tasks the users are assigned to.</p> <p>A Workfront administrator or a group administrator must create a schedule before it can be associated with users.</p> <p>Select a system-level or a group schedule to assign it to the selected users.</p> <p>For more information about system-level and group schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</p> <p><b>IMPORTANT</b>: Workfront uses the schedule of a user only when the Calculate Resource Availability Using setting is set to The User's Schedule. For information about how the Calculate Resource Availability Using setting affects which schedule is used for Resource Management, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </li> 
       <li> <p><b>Timesheet Profile</b>: Associate a Timesheet Profile with the users. This ensures that timesheets generate automatically for the users.</p> 
       <p><b>NOTE</b>:  
       <ul> 
       <li>The list of timesheet profiles you have available in this field depends on your access:
       <ul>
       <li>As a Workfront administrator, you can see all system-level and group-level timesheet profiles.</li>
       <li><p>As a group administrator, you can see system-level timesheet profiles, as well as those associated with the groups that you manage.</p></li>
       <li><p>As a user with a Planner license and access to edit users, you can see only system-level timesheet profiles.</p></li>
       </ul></li> 
       <li>If you are a group administrator, all of the users you are editing must be members of a group that you administer.</li> 
       </ul> </p> </li> 
       <li><b>Default Hour Type</b>: Select the default hour type for the users. This is the hour type that is used by default when the users log time.</li> 
       <li> <p><b>Available Hour Types</b>: Select the hour types that should be available to the user. These hour types are visible everywhere in Workfront where the users can log time. A user can only see the hour types that are enabled at the project level as well as the user level.</p> 
       <p>For more information about what hour types are available to users, see <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Define hour types and availability</a>.</p> 
       </li> 
       <li> <b>FTE</b>: This is the Full Time Equivalent of the user. Workfront uses this number to calculate the availability of the user based on the Default Schedule only when the Resource Management Preferences at the system level are set to The Default Schedule. 

      <p>The FTE indicates the amount of time that the user can spend at work. This includes overhead, as well as time spent on project work. For example, time that is spent in meetings, or training is also included in the FTE.</p> 

      The FTE must be a decimal number up to 1, and it cannot be 0. For example, if the FTE value is 0.5 and the Default Schedule in Workfront is 40 hours, the user is available for 20 hours a week. 

      The field's default is 1.

      Schedule exceptions, time off might, and the value of Work Time may affect the availability of the user. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area.

      If the Resource Management Preferences at the system level are set to The User's Schedule, the value you specify here is ignored and the user is considered to be available according to what is specified in their schedule. 

      For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.
      </li> 
       <li> <p><b>Resource Pools</b>: Associate the users with resource pools.</p> <p><b>NOTE</b>:  Only the resource pools that are common to all the users selected appear in this field. If the users selected have no shared resource pools, this field is empty. If this field is empty, the resource pools you specify here will overwrite their individual resource pools.</p> 
       <p>For more information about resource pools, see <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resource pools overview </a>.</p> </li> 
       <li><b>Cost Per Hour</b>: The amount of cost per hour for the user. </li> 
       <li><b>Billing Per Hour</b>: The amount of billing per hour for the user.</li> 
       <li><b>Custom Forms</b>: Associate an existing user custom form with the users. You must create a custom form before you can associate it with a user. Only active custom forms display in the list. For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a>.</li> 
       <li><b>Comment</b>: Enter a comment in the field provided. All users selected will receive an in-app notification as well as an email notification with your comment. The comment shows in the Updates tab of the users' profile.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
-->


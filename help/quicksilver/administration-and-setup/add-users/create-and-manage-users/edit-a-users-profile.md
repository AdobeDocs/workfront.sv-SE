---
title: Redigera en användares profil
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Som Adobe Workfront-administratör kan du skapa nya användare och hantera profiler för befintliga användare.
author: Courtney, Alina
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: 95c999a72020ce825f3a8377662c71e35a194d80
workflow-type: tm+mt
source-wordcount: '2760'
ht-degree: 0%

---

# Redigera en användares profil


<span class="preview">Den markerade informationen på den här sidan avser funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i förhandsvisningsmiljön.</span>

>[!IMPORTANT]
>
>Det förfarande som beskrivs på denna sida gäller endast organisationer som ännu inte har anslutit sig till Admin Console. Om du har anslutit dig till Adobe Admin Console måste du utföra den här åtgärden via Adobe Admin Console.
>
>Instruktioner om hur du redigerar en användarprofil i Adobe Admin Console finns i avsnittet Redigera användarinformation i artikeln [Hantera användare individuellt](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) eller kontakta din Adobe Admin Console-administratör.
>
>En lista över procedurer som skiljer sig åt beroende på om din organisation har anslutit sig till Adobe Admin Console finns på [Plattformsbaserade administrationsskillnader (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Som Adobe Workfront-administratör kan du skapa nya användare och hantera profiler för befintliga användare. Mer information om hur du skapar användare finns i [Lägg till användare](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Användare med en planlicens kan också skapa och hantera användare. Mer information om vilken åtkomst som krävs för att redigera användare finns i [Bevilja åtkomst för användare](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## Åtkomstkrav

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste ha något av följande:</p> 
    <ul> 
     <li> <p>Åtkomstnivån Systemadministratör. Mer information finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>. </p> </li> 
     <li> <p><b>Användare</b> ange din åtkomstnivå som <b>Redigera</b> åtkomst, med <b>Skapa</b> och minst en av de två <b>Användaradministratör</b> alternativ aktiverade under <b>Finjustera inställningarna</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Om användaren <b>Administratör (gruppanvändare)</b> är aktiverat måste du vara gruppadministratör för en grupp där användaren är medlem.</p> <p>Mer information om <b>Användare</b> ange en åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst för användare</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Redigera en användarprofil

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Användare** ![](assets/users-icon-in-main-menu.png).
1. Markera användaren och klicka sedan på ikonen Redigera ![](assets/edit-icon.png).

1. I **Redigera användare** som visas ändrar du följande information och klickar sedan på **Spara ändringar**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Personlig information </td> 
      <td> 
       <ul> 
        <li><b>Förnamn</b>, <b>Efternamn</b></li> 
        <li> <p><b>E-postadress:</b> E-postadressen till en användare är även användarens användarnamn i Workfront. Fältet är skiftlägeskänsligt och måste vara unikt. Om någon användare försöker lägga till en icke-unik e-postadress tre gånger i ett 10-minutersfönster visas ett reCAPTCHA-svar.</p> <p>Om du använder e-postadressen tillåtelselista och anger en e-postdomän som inte finns med i listan får användaren inga e-postmeddelanden. Mer information om tillåtelselista finns i <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">Konfigurera din e-postadress tillåtelselista</a>.</p> </li> 
        <li> <p><b>Återställ lösenord</b>: Klicka på den här länken om du vill återställa användarens lösenord. Du ombeds ange ditt eget lösenord innan du kan återställa användarens lösenord.</p> <p>Om du vill återställa en annan användares lösenord måste du vara Workfront-administratör eller gruppadministratör.</p> <p><b>ANMÄRKNING</b>:  
          <ul> 
           <li> <p>Om du är gruppadministratör kan du bara återställa lösenord för användare i de grupper där du är utsedd som sådana. Behörigheten Användaradministratör (gruppanvändare) måste även aktiveras på din åtkomstnivå:</p> <p> <img src="assets/group-admin-user.png" > </p> <p>Den här inställningen är inaktiverad som standard. Mer information finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </li> 
           <li> <p>Du kan inte återställa lösenordet för en Workfront-administratör.</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;sso configuration=""&gt; Användarnamn</b>: Om Workfront-administratören har aktiverat SSO-integrering med Workfront, visas SSO-användarnamnet i det här fältet. Den typ av SSO-konfiguration som är aktiverad för din Workfront-instans visas i det här fältet. </li> 
        <li> <p><b>OnlyAllow &lt;sso configuration=""&gt; Autentisering</b>: Om Workfront-administratören har aktiverat en SSO-integrering med Workfront och har uppdaterat alla användare för enkel inloggning (SSO), är det här fältet markerat som standard. Den typ av SSO-konfiguration som är aktiverad för din Workfront-instans visas i det här fältet.</p> <p>När det här fältet är markerat måste användaren logga in på Workfront med sina SSO-inloggningsuppgifter. Om du avmarkerar den kan de logga in på Workfront med sina Workfront-inloggningsuppgifter.</p> <p>Mer information om hur du konfigurerar Workfront med en SSO-lösning finns i <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Översikt över enkel inloggning i Adobe Workfront</a></p> <p>Mer information om hur du uppdaterar användare för enkel inloggning finns i <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Uppdatera användare för enkel inloggning</a>.</p> <p><b>ANMÄRKNING</b>: Om du är gruppadministratör kan du redigera &lt;sso configuration=""&gt; endast för användare i de grupper där du är utsedd som sådana. Behörigheten Användaradministratör (gruppanvändare) måste även aktiveras på din åtkomstnivå.
        <p>Om du är gruppadministratör och har behörigheten Användaradministratör (alla användare) aktiverad på din åtkomstnivå kan du redigera &lt;sso configuration=""&gt; fält för alla användare.</p> </li> 
        <li><b>Jobbinformation:</b> Information om jobbet, t.ex. befattning, och vilket expertområde användaren ansvarar för.</li> 
        <li><p><b>Kontaktinformation</b>: Användarens telefonnummer och adress.</p>
        <p>Om användaren är aktiverad för UUM (Unified User Management) eller Adobe Identity Management System (IMS) är <b>Land</b> i avsnittet Kontaktinformation accepterar bara landskodsvärden (till exempel USA, GB, IN).</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inställningar </td> 
      <td> 
       <ul> 
        <li> <p><b>Tidszon:</b> Användarens tidszon.</p> <p>Mer information om hur du kan hjälpa användare att samarbeta i Workfront över olika tidszoner finns i <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Arbeta över tidszoner</a>.</p> </li> 
        <li><b>Språk för e-post</b>: Användarens förvalda e-postspråk. Detta påverkar formatet för siffror och datum i e-postmeddelanden som kommer från Workfront.</li> 
        <li><b>Visa procent färdigt vid uppdateringsstatus</b>: Markera det här alternativet om du vill att ett procenttal ska vara klart i området Uppdatera för den här användarens uppgifter.</li> 
        <li><b>Skicka jobb som jag har tilldelat mig själv till fliken Arbeta med</b>: Markera det här alternativet om du vill att allt som användaren tilldelar sig ska visas direkt på fliken Arbeta med. Som standard visas allt som tilldelats en användare på fliken Arbetsbegäran.</li> 
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
      <li><b>Är aktiv:</b> Markera den här rutan om du vill ange att användaren är aktiv. Aktiva användare använder en Workfront-licens. Om du rensar rutan inaktiveras användaren.</li> 
       <li> <p><b>Åtkomstnivå:</b> Välj den åtkomstnivå som ska tilldelas den här användaren.</p> 
       <p>När du tilldelar en åtkomstnivå till en användare kan du tilldela en nivå som är lika med eller mindre än din egen åtkomstnivå. (Om din åtkomstnivå till exempel är Planering kan du inte tilldela administratörsåtkomstnivån.) Du kan dock inte tilldela en åtkomstnivå som är lägre än din egen åtkomstnivå om Workfront-administratören har aktiverat icke-standardbehörigheter på åtkomstnivån som inte är aktiverade på din egen åtkomstnivå (via finjusteringsinställningarna som beskrivs i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>). </p> 
       <p>Mer information om åtkomstnivåer finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Konfigurera åtkomst till Adobe Workfront</a>.</p> </li> 
       <li> <p><b>Layoutmall</b>: Välj en layoutmall för användaren. Den här layoutmallen har företräde framför alla layoutmallar som har tilldelats användarens hemgrupp, hemteam eller primära jobbroll. Mer information om tilldelningsprioriteten för layoutmallar finns i <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Skapa och hantera layoutmallar</a>.</p> <p><b>ANMÄRKNING</b>:  <p>Listan med mallar som är tillgängliga i det här fältet beror på din åtkomst:</p> 
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
      <li><b>Rapporter till:</b> Om du har angett ett företag för användaren kan du även ange användarens direkta hanterare i det här fältet. En användare kan bara ha en hanterare.</li> 
      <li><b>Direktrapporter:</b> Om du har angett ett företag för användaren kan du även ange användares direkta rapporter. En användare kan ha flera direktrapporter.</li> 
      <li><b>Hemteam</b>: Ange hemteamet för användaren. Användare kan bara ha ett hemteam.</li> 
      <li><b>Andra team</b>: Användare kan tillhöra flera team.</li> 
      <li> <p><b>Hemgrupp:</b> Välj en lämplig grupp att tilldela användaren till. Detta ger användaren möjlighet att komma åt objekt som delas med gruppen.</p> <p>Detta är ett obligatoriskt fält. Alla användare måste vara kopplade till en hemgrupp. Om du inte väljer någon grupp tilldelas gruppen som den nya användarens hemgrupp.</p> <p><b>ANMÄRKNING</b>: Du kan bara tilldela en grupp till en användare om du är Workfront-administratör, är administratör för gruppen eller om gruppen är offentlig.</p> </li> 
      <li> <p><b>Andra grupper</b>: Användare kan tillhöra flera grupper. Du kan bara tilldela en grupp till en användare om du är Workfront-administratör, är administratör för gruppen eller om gruppen är offentlig.</p> <p><b>VIKTIGT</b>: Om du lägger till en användare i fler än 100 grupper kan prestandaproblem uppstå i alla områden i Workfront som läser in listan med grupper.</p> <p>Mer information om publika grupper finns i <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Skapa en grupp</a>.</p> <p>Mer information om grupper finns i <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Översikt över grupper</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resursplanering </td> 
      <td> 
       <ul>
       <li>
       <b><span class="preview">Arbetstid</span></b>: <span class="preview">Representerar den procentandel av heltidsekvivalenttiden (FTE) som användaren är tillgänglig för faktiskt arbete, exklusive overhead. Arbetstiden måste vara ett decimaltal upp till 1 och får inte vara 0. Exempel: 20 % tillgänglighet för faktiskt arbete är 0,2.</span>

   <span class="preview">Fältets standardvärde är 1, vilket anger att en användare tillbringar hela sitt heltidsanställda på faktiskt, projektrelaterat arbete.</span>

   <span class="preview">Systemet använder det här talet för att beräkna användarens tillgänglighet för faktiskt, projektrelaterat arbete. </span>

   <span class="preview">Mer information om hur du skapar scheman i Workfront finns i <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Skapa ett schema</a>.</span>

   <span class="preview">Schemalagda undantag och ledig tid kan också påverka användarkapaciteten.

   Workfront beräknar en användares tillgänglighet beroende på inställningarna för resurshantering i inställningsområdet. Mer information finns i <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Konfigurera inställningar för resurshantering</a>.

   <b>TIPS</b>

   <span class="preview">Ange värdet 1 för Arbetstid för att ange att användaren är tillgänglig för projektrelaterat arbete och hela heltidsekvivalenten.</span>
   </li> 
      <li> <b>Schemalägg inaktivering</b>: Markera den här rutan om du vill att den här användaren ska inaktiveras efter en viss tid. </li> 
       <li><b>Schemalagt inaktiveringsdatum</b>: Datumet efter vilket användaren inaktiveras. Information om hur du schemalägger användare för inaktivering finns i <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Schemalägg användare för inaktivering</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Inaktivera eller återaktivera en användare</a>.</li> 
       <li> <p><b>Primär roll</b>: Det här är den primära rollen som användaren kan utföra i Workfront. Alla uppgifter och utgåvor som användaren är tilldelad till tilldelas även den här jobbrollen. Jobbroller är viktiga i resurshanteringen. Du kan bara uppdatera det här fältet om du har en planlicens med administratörsåtkomst eller om du är Workfront-administratör. Mer information om hur du konfigurerar användare med administrativ användaråtkomst finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst för användare</a>.</p> <p>Endast aktiva jobbroller visas i listan. </p> </li> 
       <li>Om du valde en <b>Primär roll</b>, <b>Procent tillgängliga heltidsanställda</b> visas. Ange hur många procent av tiden i användarens schema som ska tilldelas den här jobbrollen. Standardvärdet för procentandelen FTE-tillgänglighet för den primära rollen är 100 %. </li> 
       <li> <p><b>Andra roller</b>: En användare kan ha flera jobbroller i Workfront. Jobbroller är viktiga i resurshanteringen. Det finns ingen gräns för hur många jobbroller en användare kan utföra. Vi rekommenderar dock att du inte tilldelar en användare till ett för stort antal jobbroller eftersom resurshanteringen kan bli alltför komplex för dessa användare.<p>Endast aktiva jobbroller visas i listan. Mer information om jobbroller finns i <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Skapa och hantera jobbroller</a>.</p> <p>Du kan bara uppdatera det här fältet om du har en planlicens med administratörsåtkomst eller om du är Workfront-administratör. <br>Mer information om hur du konfigurerar användare med administrativ användaråtkomst finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst för användare</a>.</p> </li> 
       <li> <p>(Villkorligt) Om du markerade en eller flera <b>Andra roller</b>, <b>Procent tillgängliga heltidsanställda</b> visas för varje roll. Ange hur stor procentandel av tiden i användarens schema som ska tilldelas varje jobbroll. Standardvärdet för procentandelen FTE-tillgänglighet för andra roller är 0 %.</p> <p><b>ANMÄRKNING</b>: Om andra roller har 0 % FTE-tillgänglighet visas de inte i resursplaneraren, såvida inte användarna har tilldelats till uppgifter i de här rollerna.</p> <p> <img alt="user_settings_roles_and_date_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>ANMÄRKNING</b>: <p>Summan av alla <b>Procentsatser för FTE-tillgänglighet</b> för alla roller måste vara 100 %. Varje procentandel av FTE-tillgänglighet beräknar tillgängliga timmar för varje roll per användare i resursplaneraren. Tillgängliga timmar för varje roll per användare beror på användarens tillgängliga tid.</p> <p>Den tillgängliga tiden för användaren beräknas av Workfront utifrån den metod som Workfront-administratören har valt för att beräkna FTE i Inställningar för resurshantering.</p> <p>Information om hur du beräknar tillgänglighet för användaren finns i <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Översikt över beräkning av timmar och heltidsekvivalent för användare och roller i resursplaneraren</a>.</p> <p>Mer information om hur du konfigurerar inställningar för resurshantering finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Konfigurera inställningar för resurshantering</a>.</p> </p> </li> 
       <li> <p><b>Schema</b>: Koppla ett schema till användaren. Schemat för användaren beräknar tidslinjen för de uppgifter som användaren är tilldelad till.</p> <p>Du måste skapa ett schema innan du kan associera det med en användare. Mer information om hur du skapar scheman finns i <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Skapa ett schema</a>.</p> <p><b>ANMÄRKNING</b>: Vi rekommenderar att schemat som du associerar med användaren matchar användarens tidszon.</p> </li> 
       <li> <p><b>Tidrapportprofil</b>: Koppla en tidrapportprofil till användaren för att säkerställa att tidrapporterna genereras automatiskt för användaren.</p> <p><b>ANMÄRKNING</b>: Listan med profiler som är tillgängliga i det här fältet beror på din åtkomst:
       <ul>
       <li>Som Workfront-administratör kan du se alla tidrapportprofiler på systemnivå och på gruppnivå.</li>
       <li>Som gruppadministratör kan du visa tidrapportprofiler på systemnivå, samt de som är kopplade till de grupper som du hanterar.</li>
       <li>Som användare med en planlicens och tillgång till att redigera användare kan du bara se tidrapportprofiler på systemnivå. Mer information om tidrapportprofiler på gruppnivå finns i <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">Skapa, redigera och tilldela tidrapportprofiler</a>.</li>
      </ul></p> </li> 
       <li><b>Standardtimtyp</b>: Välj standardtimtyp för användaren. Det här är timtypen som används som standard när användaren loggar tid.</li> 
       <li><b>Tillgängliga timtyper</b>: Välj de timtyper som ska vara tillgängliga för användaren. Dessa timtyper visas överallt i Workfront där användaren kan logga tid. En användare kan bara se timtyperna som är aktiverade på projektnivå och på användarnivå. Mer information om vilka timtyper som är tillgängliga för användarna finns i <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Definiera timtyper och tillgänglighet för tidrapporter</a>.</li> 
       <li><b>Inloggningstid:</b> Välj om användaren ska logga tid på arbetsobjekt i timmar eller dagar. Mer information finns i <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">Konfigurera om tid är inloggad i timmar eller dagar</a>.</li>

   <li> <b>FTE</b>: Det här är heltidsmotsvarigheten för användaren. Workfront använder det här numret för att beräkna användarens tillgänglighet baserat på standardschemat endast när inställningarna för resurshantering på systemnivå är inställda på standardschemat.

   <p>FTE anger hur lång tid användaren kan tillbringa på jobbet. Detta inkluderar overheadkostnader och tid för projektarbete. Till exempel ingår även tid som används i möten eller utbildning i heltidsanställda.</p>

   FTE måste vara ett decimaltal upp till 1 och det får inte vara 0. Om till exempel FTE-värdet är 0,5 och standardschemat i Workfront är 40 timmar är användaren tillgänglig för 20 timmar i veckan.

   Fältets standardvärde är 1.

   Schemalägg undantag, avbrottstid kan <span class="preview">och värdet för Arbetstid</span> kan påverka användarens tillgänglighet.

   Workfront beräknar en användares tillgänglighet beroende på inställningarna för resurshantering i inställningsområdet.

   Om inställningarna för resurshantering på systemnivå är inställda på Användarens schema, ignoreras det värde du anger här och användaren anses vara tillgänglig enligt det som anges i deras schema.

   Mer information finns i <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Konfigurera inställningar för resurshantering</a>.

   Mer information om hur du skapar scheman i Workfront finns i <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Skapa ett schema</a>.
   </li>

   <li><b>Resurspooler</b>: Associera användaren med Resurspooler. Mer information finns i <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Associera resurspooler med användare </a>.</li> 
        <li><b>Kostnad per timme</b>: Kostnadsbeloppet per timme för användaren. </li> 
        <li><b>Fakturering per timme</b>: Beloppet för fakturering per timme för användaren.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anpassad Forms</td> 
      <td>Koppla ett befintligt anpassat formulär till den här användaren. Du måste skapa ett anpassat formulär innan du kan koppla det till en användare. Endast aktiva anpassade formulär visas i listan. Mer information om hur du skapar anpassade formulär finns i <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Skapa eller redigera ett anpassat formulär</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kommentar</td> 
      <td> <p>Skriv den kommentar du vill skicka till användarna och till uppdateringsområdet för deras användarprofiler.</p> </td> 
     </tr> 
    </tbody> 
   </table>

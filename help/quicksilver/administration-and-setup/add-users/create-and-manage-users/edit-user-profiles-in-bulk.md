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
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '2213'
ht-degree: 0%

---

# Redigera användarprofiler gruppvis

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

1. Markera mer än en användare och klicka sedan på ikonen Redigera ![](assets/edit-icon.png).

1. I rutan **Redigera användare** som visas ändrar du något av följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Inställningar</td> 
      <td> 
       <ul> 
        <li><b>Tidszon:</b> Användarens tidszon.</li> 
        <li><b>Språk</b>: Användarens språkområde rekommenderas. Detta påverkar formatet för siffror och datum i e-postmeddelanden som kommer från Workfront.</li> 
        <li><b>Skicka material som jag själv har tilldelat till fliken Arbeta med</b>: Den här inställningen hänvisar till en borttagen funktion från Workfront.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Meddelanden</td> 
      <td>Välj de e-postmeddelanden som ska aktiveras för den nya användaren.<p>Du kan välja både snabbmeddelanden och dagliga sammanfattningsmeddelanden. Alla dagliga sammandragsmeddelanden levereras någon gång efter samma tid för alla valda användare. Mer information finns i <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Konfigurera händelsemeddelanden för alla i systemet</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Åtkomst</td> 
      <td> 
       <ul> 
        <li><b>Är aktiv:</b> Markera det här fältet för att ange om användarna är aktiva. Aktiva användare använder en Workfront-licens. Om du avmarkerar fältet inaktiveras användarna.</li> 
        <li> 
        <p><b>Åtkomstnivå:</b> Välj den åtkomstnivå som ska tilldelas dessa användare. Alla markerade användare får samma åtkomstnivå.
        </p> 
        <p>När du tilldelar en åtkomstnivå till användare kan du tilldela en nivå som är lika med eller mindre än din egen åtkomstnivå. (Om din åtkomstnivå till exempel är Planering kan du inte tilldela administratörsåtkomstnivån.) </p>
        <p>Du kan dock inte tilldela en åtkomstnivå som är lägre än din egen om Workfront-administratören har aktiverat behörigheter på åtkomstnivån som inte är aktiverad i din egen (via finjusteringsinställningarna, som beskrivs i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>).</p> 
        <p>Mer information om åtkomstnivåer finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Konfigurera åtkomst till Adobe Workfront</a>.</p> 
         </li> 
        <li> 
        <p><b>Layoutmall</b>: Välj en layoutmall för användarna. Den layoutmall som tilldelats användarna har företräde framför alla layoutmallar som tilldelats deras hemgrupp, hemteam eller primära jobbroll. Mer information om tilldelningsprioriteten för layoutmallar finns i <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Skapa och hantera layoutmallar</a>.</p> 
        <p><b>Obs!</b> Listan över layoutmallar som är tillgängliga i det här fältet beror på din åtkomst:
          <ul>
           <li>Som Workfront-administratör kan du se alla layoutmallar på system- och gruppnivå.</li>
           <li>Som gruppadministratör kan du se layoutmallar på systemnivå, samt mallar som är kopplade till de grupper som du hanterar.</li>
           <li><p>Som användare med en planerarlicens och möjlighet att redigera användare, kan du bara se layoutmallar på systemnivå. </p>
           <p>Mer information om layoutmallar på gruppnivå finns i <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Skapa och hantera layoutmallar</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organisation</td> 
      <td> 
       <ul> 
        <li><b>Företag</b>: Användarnas företag. Användare kan bara associeras med ett företag. Du måste skapa ett företag innan du kan associera det med en användare. Endast aktiva företag visas i listan. Mer information om hur du skapar företag finns i Förstå och hantera företag.</li> 
        <li><b>Hemteam</b>: Ange hemteamet för användarna. Användare kan bara ha ett hemteam. </li> 
        <li><b>Andra team</b>: Användare kan tillhöra flera team. </li> 
        <li> <p><b>Hemgrupp:</b> Välj en lämplig grupp att tilldela användarna som hemgrupp. Detta ger användaren möjlighet att komma åt objekt som delas med gruppen.</p> <p><b>OBS!</b> Detta är ett obligatoriskt fält. Du kan inte ha användare som inte är associerade med en hemgrupp.</p> <p>Du kan bara tilldela en grupp till användare i följande situationer:</p> 
         <ul> 
          <li>Du är Workfront-administratör.</li> 
          <li>Du är administratör för den gruppen.</li> 
          <li>Gruppen är offentlig.</li> 
         </ul> </li> 
        <li> <p><b>Andra grupper</b>: Användare kan tillhöra flera grupper. Du kan bara tilldela en grupp till en användare i följande situationer:</p> 
         <ul> 
          <li>Du är Workfront-administratör.</li> 
          <li>Du är administratör för den gruppen.</li> 
          <li> <p>Gruppen är offentlig. </p> 
          <p>Mer information om publika grupper finns i <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Skapa en grupp</a>.</p> 
          <p>Mer information om grupper finns i <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Översikt över grupper</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resursplanering</td> 
      <td> 
       <ul>

   <li>
       <b>Arbetstid</b>: Representerar den procentandel av heltidsekvivalenttiden (FTE) som användaren är tillgänglig för det faktiska arbetet, exklusive extrakostnader. Arbetstiden måste vara ett decimaltal upp till 1 och får inte vara 0. Exempel: 20 % tillgänglighet för faktiskt arbete är 0,2.

   Fältets standardvärde är 1, vilket anger att en användare tillbringar hela sitt heltidsanställda på faktiskt, projektrelaterat arbete.

   Systemet använder det här talet för att beräkna användarens tillgänglighet för faktiskt, projektrelaterat arbete.

   Mer information om hur du skapar scheman i Workfront finns i <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Skapa ett schema</a>.

   Schemalagda undantag och ledig tid kan också påverka användarkapaciteten.

   Workfront beräknar en användares tillgänglighet beroende på inställningarna för resurshantering i inställningsområdet. Mer information finns i <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Konfigurera inställningar för resurshantering</a>.

   <b>TIPS</b>

   Ange värdet 1 för Arbetstid för att ange att användaren är tillgänglig för projektrelaterat arbete och hela heltidsekvivalenten.
   </li>

   <li><b>Schemalägg inaktivering</b>: Markera den här kryssrutan om du vill schemalägga att användare ska inaktiveras efter en tidsperiod.</li> 
       <li><b>Schemalagt inaktiveringsdatum</b>: Det datum efter vilket användarna inaktiverades. Mer information om schemaläggning av användare för inaktivering finns i avsnittet <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Schemalägg användare för inaktivering</a> i <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Inaktivera eller återaktivera en användare</a>.</li> 
       <li> <p><b>Primär roll</b>: Detta är den primära jobbrollen som en användare har i Workfront. Alla uppgifter och utgåvor som användarna tilldelas till tilldelas som standard även den här jobbrollen. Jobbroller är viktiga i resurshanteringen. Mer information om jobbroller finns i <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Skapa och hantera jobbroller</a></p> <p>Du kan bara uppdatera det här fältet om du har en planlicens med administratörsåtkomst eller om du är Workfront-administratör. Mer information om hur du konfigurerar användare med administrativ användaråtkomst finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst till användare</a>.</p> </li> 
       <li>(Villkorligt) Om du valde en <b>primär roll</b> visas fältet <b>Procent av FTE-tillgänglighet</b> . Ange hur många procent av tiden för användarens scheman som ska tilldelas den här jobbrollen. Standardvärdet för procentandelen FTE-tillgänglighet för den primära rollen är 100 %.</li> 
       <li> <p><b>Andra roller</b>: Användare kan ha flera jobbroller i Workfront. Jobbroller är viktiga i resurshanteringen. Det finns ingen gräns för hur många jobbroller en användare kan utföra. Vi rekommenderar dock att du inte tilldelar en användare till ett för stort antal jobbroller eftersom resurshanteringen kan bli alltför komplex för dessa användare.</p> <p>Mer information om jobbroller finns i <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Skapa och hantera jobbroller</a>.</p> <p>Du kan bara uppdatera det här fältet om du har en planlicens med administratörsåtkomst eller om du är Workfront-administratör. Mer information om hur du konfigurerar användare med administrativ användaråtkomst finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst till användare</a>.</p> </li> 
       <li> <p>(Villkorligt) Om du markerade en eller flera <b>andra roller</b> visas fältet <b>Procent av FTE-tillgänglighet</b> för varje roll. Ange hur stor procentandel av tiden för användarens scheman som ska tilldelas varje jobbroll. Standardvärdet för procentandelen FTE-tillgänglighet för andra roller är 0 %.</p> <p><b>OBS</b>:  
       <ul> 
       <li>Om andra roller har 0 % FTE-tillgänglighet visas de inte i resursplaneraren, såvida inte användarna har tilldelats till uppgifter i de här rollerna.</li> 
       <li> <p>Summan av alla procent av FTE-tillgänglighet för alla roller måste vara lika med 100 %. Varje procentandel av FTE-tillgänglighet beräknar tillgängliga timmar för varje roll per användare i resursplaneraren. Tillgängliga timmar för varje roll per användare beror på användarens tillgängliga tid.</p> <p>Den tillgängliga tiden för användaren beräknas av Workfront utifrån den metod som Workfront-administratören har valt för att beräkna FTE i Inställningar för resurshantering.</p> <p>Mer information om hur du beräknar tillgängligheten för användaren finns i <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Översikt över beräkning av timmar och FTE för användare och roller i resursplaneraren</a>.</p> <p>Mer information om hur du konfigurerar inställningar för resurshantering finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Konfigurera inställningar för resurshantering</a>.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>Schema</b>: Associera ett schema med användarna. Schemat för användarna beräknar tidslinjen för de uppgifter som användarna är tilldelade till.</p> <p>En Workfront-administratör eller en gruppadministratör måste skapa ett schema innan det kan kopplas till användare.</p> <p>Välj en systemnivå eller ett gruppschema för att tilldela det till de valda användarna.</p> <p>Mer information om scheman på systemnivå och gruppnivå finns i <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Skapa ett schema</a>.</p> <p><b>VIKTIGT</b>: Workfront använder schemat för en användare endast när inställningen Beräkna resurstillgänglighet med är inställd på användarens schema. Mer information om hur inställningen Beräkna resurstillgänglighet med påverkar vilket schema som används för resurshantering finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Konfigurera inställningar för resurshantering</a>.</p> </li> 
       <li> <p><b>Tidrapportprofil</b>: Associera en tidrapportprofil med användarna. Detta garanterar att tidrapporterna genereras automatiskt för användarna.</p> 
       <p><b>OBS</b>:  
       <ul> 
       <li>Listan med tidrapportprofiler som du har tillgängliga i det här fältet beror på din åtkomst:
       <ul>
       <li>Som Workfront-administratör kan du se alla tidrapportprofiler på system- och gruppnivå.</li>
       <li><p>Som gruppadministratör kan du se tidrapportprofiler på systemnivå, samt de som är kopplade till de grupper som du hanterar.</p></li>
       <li><p>Som användare med en planerarlicens och möjlighet att redigera användare kan du bara se tidrapportprofiler på systemnivå.</p></li>
       </ul></li> 
       <li>Om du är gruppadministratör måste alla användare som du redigerar vara medlemmar i en grupp som du administrerar.</li> 
       </ul> </p> </li> 
       <li><b>Standardtimtyp</b>: Välj standardtimtyp för användarna. Det här är timtypen som används som standard när användaren loggar tid.</li> 
       <li> <p><b>Tillgängliga timtyper</b>: Välj de timtyper som ska vara tillgängliga för användaren. De här timtyperna visas överallt i Workfront där användarna kan logga tid. En användare kan bara se timtyperna som är aktiverade på projektnivå och på användarnivå.</p> 
       <p>Mer information om vilka timtyper som är tillgängliga för användare finns i <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Definiera timtyper och tillgänglighet</a>.</p> 
       </li> 
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
       <li> <p><b>Resurspooler</b>: Associera användarna med resurspooler.</p> <p><b>Obs!</b> Endast resurspooler som är gemensamma för alla användare visas i det här fältet. Om de valda användarna inte har några delade resurspooler är det här fältet tomt. Om det här fältet är tomt skrivs de resurspooler som du anger här över sina enskilda resurspooler.</p> 
       <p>Mer information om resurspooler finns i <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Översikt över resurspooler </a>.</p> </li> 
       <li><b>Kostnad per timme</b>: Kostnaden per timme för användaren. </li> 
       <li><b>Fakturering per timme</b>: Användarens faktureringsbelopp per timme.</li> 
       <li><b>Anpassad Forms</b>: Associera ett befintligt anpassat formulär med användarna. Du måste skapa ett anpassat formulär innan du kan koppla det till en användare. Endast aktiva anpassade formulär visas i listan. Mer information om hur du skapar anpassade formulär finns i <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Designa ett formulär med formulärdesignern</a>.</li> 
       <li><b>Kommentar</b>: Ange en kommentar i fältet. Alla valda användare får ett meddelande i appen samt ett e-postmeddelande med din kommentar. Kommentaren visas på fliken Uppdateringar i användarens profil.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) I avsnittet **Anpassad Forms** markerar du alternativet **Beräkna om anpassade uttryck** för att se till att alla beräknade anpassade fält i anpassade formulär som är kopplade till de valda användarna är uppdaterade.

1. Klicka på **Spara ändringar**.

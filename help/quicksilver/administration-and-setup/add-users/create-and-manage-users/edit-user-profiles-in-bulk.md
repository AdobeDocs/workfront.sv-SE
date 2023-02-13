---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Redigera användarprofiler gruppvis
description: Som Adobe Workfront-administratör kan du redigera flera användarkonton samtidigt.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: cb709b2f-659e-4110-81ac-a1ef967d534c
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '2194'
ht-degree: 0%

---

# Redigera användarprofiler gruppvis

>[!IMPORTANT]
>
>Det förfarande som beskrivs på denna sida gäller endast organisationer som ännu inte har anslutit sig till Admin Console. Om du har anslutit dig till Adobe Admin Console måste du utföra den här åtgärden via Adobe Admin Console.
>
>Instruktioner om hur du redigerar en användarprofil i Adobe Admin Console finns i avsnittet Redigera användarinformation i artikeln [Överför användare gruppvis](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) eller kontakta din Adobe Admin Console-administratör.
>
>En lista över procedurer som skiljer sig åt beroende på om din organisation har anslutit sig till Adobe Admin Console finns på [Plattformsbaserade administrationsskillnader (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Du kan redigera flera användarkonton samtidigt. När användare gruppredigeras uppdateras endast de fält som du specifikt markerar med samma information för alla markerade användare. Alla andra fält som du lämnar omarkerade förblir desamma för varje enskild användare, även om de är olika för varje användare.

>[!NOTE]
>
>* Du kan inte redigera personlig information i användarprofilerna gruppvis eftersom informationen måste vara unik för varje användare.
>* För att säkerställa att data är korrekta och att prestanda är optimala rekommenderar vi att du inte väljer fler än 2 000 användare åt gången för en massredigering.
>


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

## Redigera flera användarkonton samtidigt

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Användare** ![](assets/users-icon-in-main-menu.png).

1. Markera flera användare och klicka sedan på ikonen Redigera ![](assets/edit-icon.png).

1. I **Redigera användare** som visas ändrar du något av följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Inställningar</td> 
      <td> 
       <ul> 
        <li><b>Tidszon:</b> Användarens tidszon.</li> 
        <li><b>Språk</b>: Användarens språkområde. Detta påverkar formatet för siffror och datum i e-postmeddelanden som kommer från Workfront.</li> 
        <li><b>Visa procent färdigt vid uppdateringsstatus</b>: Markera det här alternativet om du vill att ett procentfält ska visas i uppdateringsflödet för uppgifter för alla användare.</li> 
        <li><b>Skicka jobb som jag har tilldelat mig själv till fliken Arbeta med</b>: Markera det här alternativet om du vill att allt som användarna tilldelar sig själva ska visas direkt på fliken Arbeta med. Som standard visas allt som tilldelats en användare på fliken Arbetsbegäran.</li> 
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
        <p>Du kan dock inte tilldela en åtkomstnivå som är lägre än din egen om Workfront-administratören har aktiverat behörigheter på åtkomstnivån som inte är aktiverad i din egen (via finjusteringsinställningarna som beskrivs i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>).</p> 
        <p>Mer information om åtkomstnivåer finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Konfigurera åtkomst till Adobe Workfront</a>.</p> 
         </li> 
        <li> 
        <p><b>Layoutmall</b>: Välj en layoutmall för användarna. Layoutmallen som tilldelats användarna har företräde framför alla layoutmallar som tilldelats deras hemgrupp, hemteam eller primära jobbroll. Mer information om tilldelningsprioriteten för layoutmallen finns i <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Skapa och hantera layoutmallar</a>.</p> 
        <p><b>ANMÄRKNING</b>: Listan med layoutmallar som är tillgängliga i det här fältet beror på din åtkomst:
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
        <li> <p><b>Hemgrupp:</b> Välj en lämplig grupp för att tilldela användarna som hemgrupp. Detta ger användaren möjlighet att komma åt objekt som delas med gruppen.</p> <p><b>ANMÄRKNING</b>: Detta är ett obligatoriskt fält. Du kan inte ha användare som inte är associerade med en hemgrupp.</p> <p>Du kan bara tilldela en grupp till användare i följande situationer:</p> 
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
        <li><b>Schemalägg inaktivering</b>: Markera den här rutan om du vill att användare ska inaktiveras efter en viss tid.</li> 
        <li><b>Schemalagt inaktiveringsdatum</b>: Datumet efter vilket användarna inaktiveras. Mer information om schemaläggning av användare för inaktivering finns i avsnittet <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Schemalägg användare för inaktivering</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Inaktivera eller återaktivera en användare</a>.</li> 
        <li> <p><b>Primär roll</b>: Detta är den primära rollen som en användare har i Workfront. Alla uppgifter och utgåvor som användarna tilldelas till tilldelas som standard även den här jobbrollen. Jobbroller är viktiga i resurshanteringen. Mer information om jobbroller finns i <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Skapa och hantera jobbroller</a></p> <p>Du kan bara uppdatera det här fältet om du har en planlicens med administratörsåtkomst eller om du är Workfront-administratör. Mer information om hur du konfigurerar användare med administrativ användaråtkomst finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst för användare</a>.</p> </li> 
        <li>(Villkorligt) Om du markerade en <b>Primär roll</b>, <b>Procent tillgängliga heltidsanställda</b> visas. Ange hur många procent av tiden för användarens scheman som ska tilldelas den här jobbrollen. Standardvärdet för procentandelen FTE-tillgänglighet för den primära rollen är 100 %.</li> 
        <li> <p><b>Andra roller</b>: Användare kan ha flera jobbroller i Workfront. Jobbroller är viktiga i resurshanteringen. Det finns ingen gräns för hur många jobbroller en användare kan utföra. Vi rekommenderar dock att du inte tilldelar en användare till ett för stort antal jobbroller eftersom resurshanteringen kan bli alltför komplex för dessa användare.</p> <p>Mer information om jobbroller finns i <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Skapa och hantera jobbroller</a>.</p> <p>Du kan bara uppdatera det här fältet om du har en planlicens med administratörsåtkomst eller om du är Workfront-administratör. Mer information om hur du konfigurerar användare med administrativ användaråtkomst finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst för användare</a>.</p> </li> 
        <li> <p>(Villkorligt) Om du markerade en eller flera <b>Andra roller</b>, <b>Procent tillgängliga heltidsanställda</b> visas för varje roll. Ange hur stor procentandel av tiden för användarens scheman som ska tilldelas varje jobbroll. Standardvärdet för procentandelen FTE-tillgänglighet för andra roller är 0 %.</p> <p><b>ANMÄRKNING</b>:  
          <ul> 
           <li>Om andra roller har 0 % FTE-tillgänglighet visas de inte i resursplaneraren, såvida inte användarna har tilldelats till uppgifter i de här rollerna.</li> 
           <li> <p>Summan av alla procent av FTE-tillgänglighet för alla roller måste vara lika med 100 %. Varje procentandel av FTE-tillgänglighet beräknar tillgängliga timmar för varje roll per användare i resursplaneraren. Tillgängliga timmar för varje roll per användare beror på användarens tillgängliga tid.</p> <p>Den tillgängliga tiden för användaren beräknas av Workfront utifrån den metod som Workfront-administratören har valt för att beräkna FTE i Inställningar för resurshantering.</p> <p>Mer information om hur du beräknar tillgänglighet för användaren finns i <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Översikt över beräkning av timmar och heltidsekvivalent för användare och roller i resursplaneraren</a>.</p> <p>Mer information om hur du konfigurerar inställningar för resurshantering finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Konfigurera inställningar för resurshantering</a>.</p> </li> 
          </ul> </p> </li> 
        <li> <p><b>Schema</b>: Associera ett schema med användarna. Schemat för användarna beräknar tidslinjen för de uppgifter som användarna har tilldelats.</p> <p>En Workfront-administratör eller en gruppadministratör måste skapa ett schema innan det kan kopplas till användare.</p> <p>Välj en systemnivå eller ett gruppschema för att tilldela det till de valda användarna.</p> <p>Mer information om scheman på systemnivå och gruppnivå finns i <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Skapa ett schema</a>.</p> <p><b>VIKTIGT</b>: Workfront använder schemat för en användare endast när inställningen Beräkna resurstillgänglighet med är inställd på Användarens schema. Mer information om hur inställningen Beräkna resurstillgänglighet med påverkar vilket schema som används för resurshantering finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Konfigurera inställningar för resurshantering</a>.</p> </li> 
        <li> <p><b>Tidrapportprofil</b>: Associera en tidrapportprofil med användarna. Detta garanterar att tidrapporterna genereras automatiskt för användarna.</p> 
        <p><b>ANMÄRKNING</b>:  
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
        <p>Mer information om vilka timtyper som är tillgängliga för användarna finns i <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Definiera timtyper och tillgänglighet för tidrapporter</a>.</p> 
        </li> 
        <li> <p><b>FTE</b>: Det nummer som du anger här tas endast med i beräkningen av användarens tillgänglighet baserat på standardschemat när inställningarna för resurshantering på systemnivå är inställda på <b>Standardschema</b>.</p> 
        <p>Om till exempel FTE-värdet är 0,5 och standardschemat är 40 timmar är användaren tillgänglig för arbete 20 timmar i veckan. Mer information om hur schemaundantag och -tid kan påverka användarens tillgänglighet när Standardschema väljs finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Konfigurera inställningar för resurshantering</a>. </p> 
        <p>Om inställningarna för resurshantering på systemnivå är inställda på <b>Användarens schema</b>, ignoreras värdet som du anger här och användaren anses vara tillgänglig enligt vad som anges i schemat. I det här fallet beräknas FTE för användaren för resursplaneraren enligt följande formel:</p>
        <p><code style="font-style: normal;">User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours</code> </p> <p>Mer information om hur du beräknar användarens FTE finns i <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Översikt över beräkning av timmar och heltidsekvivalent för användare och roller i resursplaneraren</a>.</p> <p>Mer information om hur du skapar scheman i Workfront finns i <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Skapa ett schema</a>.</p> <p>Mer information om hur du konfigurerar inställningar för resurshantering finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Konfigurera inställningar för resurshantering</a>.</p> 
        </li> 
        <li> <p><b>Resurspooler</b>: Associera användarna med resurspooler.</p> <p><b>ANMÄRKNING</b>: Endast de resurspooler som är gemensamma för alla markerade användare visas i det här fältet. Om de valda användarna inte har några delade resurspooler är det här fältet tomt. Om det här fältet är tomt skrivs de resurspooler som du anger här över sina enskilda resurspooler.</p> 
        <p>Mer information om resurspooler finns i <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Översikt över resurspooler </a>.</p> </li> 
        <li><b>Kostnad per timme</b>: Kostnadsbeloppet per timme för användaren. </li> 
        <li><b>Fakturering per timme</b>: Beloppet för fakturering per timme för användaren.</li> 
        <li><b>Anpassad Forms</b>: Koppla ett befintligt anpassat formulär till användarna. Du måste skapa ett anpassat formulär innan du kan koppla det till en användare. Endast aktiva anpassade formulär visas i listan. Mer information om hur du skapar anpassade formulär finns i <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Skapa eller redigera ett anpassat formulär</a>.</li> 
        <li><b>Kommentar</b>: Skriv en kommentar i fältet. Alla valda användare får ett meddelande i appen samt ett e-postmeddelande med din kommentar. Kommentaren visas på fliken Uppdateringar i användarens profil.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) I dialogrutan **Anpassad Forms** väljer du **Beräkna om anpassade uttryck** för att se till att alla beräknade anpassade fält i anpassade formulär som är kopplade till de valda användarna är uppdaterade.

1. Klicka **Spara ändringar**.

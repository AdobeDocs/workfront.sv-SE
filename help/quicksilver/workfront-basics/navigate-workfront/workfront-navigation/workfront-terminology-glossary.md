---
content-type: reference
navigation-topic: workfront-navigation
title: Ordlista för  [!DNL Adobe Workfront] terminologi
description: I  [!DNL Adobe Workfront] ordlistan visas termer som används ofta i  [!DNL Adobe Workfront]. You can use the glossary when you want to find the definition of concepts you see in the [!UICONTROL Workfront] gränssnittet, rapporter eller så försöker du förstå innebörden av  [!DNL Workfront] begrepp som definieras i  [!DNL Workfront] dokumentationen.
author: Alina
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: bfaf566e556882078875649549c0dfadacd800b8
workflow-type: tm+mt
source-wordcount: '16726'
ht-degree: 0%

---


# Ordlista för [!DNL Adobe Workfront]-terminologi

<!--Audited: 12/2023-->

>[!IMPORTANT]
>
>Den här artikeln bör användas som referens för att förstå de termer som du kan stöta på i programmet [!DNL Adobe Workfront], i [!DNL Workfront]-dokumentationen eller när du vanligtvis pratar om att planera och hantera arbete. Vi uppdaterar den här informationen och därför kanske inte tabellen är fullständig. Vi kommer att ta bort denna ansvarsfriskrivning när vi anser denna information vara uttömmande.

Följande tabell är en lista över vanliga termer i Adobe Workfront:

## A - C

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Objektnamn</strong></th> 
   <th><strong>Beskrivning</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Access Level]</td> 
   <td>En användarprofil som avgör hur en användare kan interagera med olika objekt och verktyg i Workfront.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Active Task]</td> 
   <td>En ofullständig aktivitet i ett aktuellt projekt som inte hindras från att bearbetas av en föregående aktivitet och som inte har någon aktivitetsbegränsning med ett framtida planerat startdatum. Med andra ord, det kan vi jobba med idag.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Activity]</td> 
   <td>I [!DNL Workfront Goals] är en aktivitet en förloppsindikator för ett mål. Det kan vara en förloppsindikator som du uppdaterar manuellt eller ett projekt som är associerat med målet. Du kan inte visa aktiviteter i en rapport och du kan inte komma åt dem via API:t [!DNL Workfront]. Mer information om aktiviteter finns i <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Kom igång med resultat och aktiviteter i Adobe Workfront-mål</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Cost]</td> 
   <td> <p>För uppgifter och ärenden är detta kostnaden associerat med de faktiska timmarna som loggats i relation till kostnaden per timme för den resurs som tilldelats uppgiften eller utgåvan. För projekt är detta det totala antalet [!UICONTROL Actual Costs] från aktiviteter och ärenden i projektet. Mer information finns i <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Spåra kostnader</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Expense Cost]</td> 
   <td> <p>Summan av [!UICONTROL Actual Amounts] för alla utgifter som loggats för ett projekt eller en uppgift.</p> <b>EXEMPEL </b>
   <p>Om du skapar en utgift för Uppgift 1 och anger 600,00 USD i fältet [!UICONTROL Actual Amount], är [!UICONTROL Actual Expense Cost] för den här aktiviteten 600,00 USD. </p> 
   <p>För ett projekt använder [!DNL Workfront] följande formel för att beräkna [!UICONTROL Actual Expense Cost]:</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Actual Hours]</td> 
   <td> <p>I ett projekt, en aktivitet eller en utleveransrapport är [!UICONTROL Actual Hours] summan av alla timmar som är inloggade på projektet, aktiviteten eller utgåvan.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span> Om du klickar på Loggtid på fliken [!UICONTROL Updates] för Aktivitet 1 och anger 25 timmar, motsvarar Faktiskt antal timmar i Aktivitet 1 25 timmar. </p> <p>[!DNL Workfront] beräknar [!UICONTROL Actual Hours] för överordnade aktiviteter eller projekt med följande formler:</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project</code> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Labor Cost]</td> 
   <td> <p>[!UICONTROL Actual Cost] som är associerad med det arbete som har investerats i en aktivitet eller ett projekt. </p> <p>För en uppgift beräknar [!DNL Workfront] [!UICONTROL Actual Labor Cost] med följande formel:</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>Om aktiviteten har [!UICONTROL Cost Type] av [!UICONTROL User Hourly] använder [!DNL Workfront] användarfrekvensen. Om aktiviteten har [!UICONTROL Cost Type] av [!UICONTROL Role Hourly] använder [!DNL Workfront] jobbrollens hastighet för att beräkna [!UICONTROL Actual Labor Cost]. </p> <p>För ett projekt använder [!DNL Workfront] följande formel för att beräkna [!UICONTROL Actual Labor Cost]:</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>Mer information finns i <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Spåra kostnader</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span>Om en användare till exempel loggar 5 timmar för en aktivitet med en [!UICONTROL User Hourly] [!UICONTROL Cost Type] och timtaxan är $100, är [!UICONTROL Actual Labor Cost] $500.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Revenue] </td> 
   <td> <p>[!UICONTROL Actual Revenue] för ett projekt eller en aktivitet är summan som är associerad med [!UICONTROL Actual Hours] för projektet eller aktiviteten. </p> <p>Mer information om att spåra intäkter i [!DNL Workfront] finns i <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Översikt över fakturering och intäkter</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Actual Start]</td> 
   <td>Tidsstämpeln när en användare ändrar ett pågående objekt för arbete som tilldelats användaren.</td> 
  </tr> 
  <!--<tr> 
 <td>A type of work process that is unplanned.</td> 
 -->
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Additional Schedules</td> 
    <td>An additional preset to be used for a new user group.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Agile] Metod</td> 
   <td>En typ av metod som bygger på den samverkansbaserade utvecklingen av behov och lösningar med tvärfunktionella team. Det uppmuntrar till flexibilitet och förändring baserat på en fast tidslinje.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Agile Team]</td> 
   <td>Skiljer sig från ett traditionellt team eftersom de tar sitt potentiella arbete från en eftersläpning och arbetar med det inom en angiven tidsperiod som kallas [!UICONTROL Iteration].</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL All My Teams]</td> 
   <td> <p>När det refereras till detta i [!UICONTROL filters] visar det här fältet antingen användare som tillhör någon av de team som den inloggade användaren tillhör, eller arbetsobjekt som tilldelats någon av de team som den inloggade användaren tillhör. </p> <p>Vi rekommenderar att du använder det här fältet i ett filter för att göra rapporter mer allmänna när du delar dem med andra användare. På så sätt kan du bara skapa en rapport som visar olika information beroende på vem som loggar in för att visa den, eftersom informationen alltid anpassas för den inloggade användaren. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Allocation Date]</td> 
   <td> <p>Du hittar det här fältet i följande typer av rapporter:</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[!UICONTROL Project] (Finansiella uppgifter)</li> 
     <li>[!UICONTROL Budgeted Hour]</li> 
    </ul> <p>För en <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->[!UICONTROL Project (Financial Data)]-rapport: </p> 
    <ul> 
     <li>Bygg den här rapporten när du försöker förstå <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> mängden [!UICONTROL Planned Hours] som är tilldelad dina resurser.</li> 
     <li> <p>[!UICONTROL Allocation Date] är den första dagen (söndag) i en vecka där allokeringen av [!UICONTROL Job Role] till en aktivitet startar. En resurs ([!UICONTROL Job Role]) kan ha så många [!UICONTROL Allocation Dates] som den har veckor under [!UICONTROL Duration] av de uppgifter som den är tilldelad till. Om uppgifter sträcker sig över flera månader kan den första dagen i en månad också bli [!UICONTROL Allocation Date], om den ligger inom [!UICONTROL Duration] för uppgiften.</p> <p>Du kan till exempel ha en [!UICONTROL Job Role] tilldelad till en aktivitet som sträcker sig över 3 veckor och har 90 [!UICONTROL Planned Hours]. De här timmarna fördelas jämnt under aktivitetens varaktighet, vilket gör att du tilldelar 6 [!UICONTROL Planned Hours] till din jobbroll varje dag:</p> <p><em> [!UICONTROL Daily Planned Hours] = [!UICONTROL Total Planned Hours]/ Antal [!UICONTROL Work Days] under [!UICONTROL Duration] för aktiviteten </em> </p> <p>Det innebär att det finns tre [!UICONTROL Allocation Dates], en för varje söndag varje vecka under [!UICONTROL Duration] för aktiviteten, där vart och ett har ett visst antal [!UICONTROL Planned Hours] associerade.<br>Om aktiviteten startar i mitten av den sista veckan i en månad och slutar två veckor efter början av en ny månad har aktiviteten fyra [!UICONTROL Allocation Dates] : en för varje söndag i varje vecka under [!UICONTROL Duration] för aktiviteten och en för den första dagen i den nya månaden.</p> <p>För att få ut så mycket som möjligt av den här informationen rekommenderar vi att du skapar en <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       -->-projektrapport (ekonomiska data) och lägger till en matrisgruppering för [!UICONTROL Allocation Date], och sedan grupperar du resultaten varje vecka, månad, kvartal eller år för att få de mest korrekta uppgifterna.<br>Mer information om hur du skapar en matrisgruppering finns i artikeln <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">Skapa en matrisrapport</a>.</p> </li> 
    </ul> <p>Den ekonomiska informationen fylls i i [!UICONTROL Project (Financial Data)] rapporter endast när de data som är associerade med den är mindre än 5 år gamla. Om en jobbroll till exempel allokerades till en aktivitet i januari 2015 och idag är september 2021, fylls inte ett ekonomiskt fält som [!UICONTROL Allocation Date] för jobbrollen i rapporten [!UICONTROL Project (Financial Data)]. </p> 
    <div> 
     <p>För en [!UICONTROL Budgeted Hour]-rapport:</p> 
     <ul> 
      <li>Bygg den här rapporten när du försöker förstå mängden [!UICONTROL Budgeted Hours] som allokeras till dina resurser eller till dina projekt i resursplaneraren.</li> 
      <li> <p>[!UICONTROL Allocation Date] är den första dagen (en söndag) i veckan som du budgeterade timmarna för [!UICONTROL Resource Planner]. </p> <p><b>TIPS</b></p> <p>Om en vecka sträcker sig över två månader genereras två rader i rapporten: en som motsvarar den första dagen i veckan (söndag i den första veckan som infaller under den första månaden) och den andra raden visar den första dagen i den andra månaden. </p> <p>Om du till exempel budgeterar 8 timmar för en användare för veckan 30 juni (söndag) - 6 juli (lördag) visar de två raderna [!UICONTROL Allocation Date] 30 juni och 1 juli. </p> </p> <p>Mer information om budgeteringsresurser i [!DNL Resource Planner] finns i artikeln <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budgetresurser i [!DNL Resource Planner] med [!UICONTROL Project]- och [!UICONTROL Role]-vyerna</a>.</p> <p>Mer information om hur du skapar en [!UICONTROL Budgeted Hour]-rapport finns i <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Rapport: Budgeterad timme</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Announcements]</td> 
   <td> <p>Ett sätt att kommunicera information till användarna i systemet. Den här informationen kommer ofta från [!DNL Workfront] till administratören eller från administratören till användaren. </p> <p>Mer information finns i <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Skicka meddelanden</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL App Integration]</td> 
   <td>En app representerar oftast en koppling till ett programvaruprogram, men kan också representera specialfunktioner som hanterar data.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approver Decision]</td> 
   <td> <p>I rapporten [!UICONTROL Proof Approval] visar det här fältet bevis för godkännandebeslut för korrektur som inte längre är aktiva.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approver stage]</td> 
   <td>I [!UICONTROL Proof Approval report] visar det här fältet information om ett korrektur på det aktuella stadiet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approval]</td> 
   <td> <p>En viss arbetsuppgift, till exempel en uppgift, ett dokument eller en tidrapport, kan kräva att en ansvarig eller annan användare signerar arbetsposten. Den här processen med att signera kallas för godkännande. </p> <p>Mer information finns i <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Översikt över godkännandeprocessen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approval date]</td> 
   <td>I rapporten [!UICONTROL Proof Approval] visar det här fältet det datum då ett bevis godkändes.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approver]</td> 
   <td>En användare eller jobbroll som måste signera för en viss arbetsuppgift, eller den användare som godkänner timposter på tidrapporter.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assigned To]</td> 
   <td> <p>I en [!UICONTROL Task or Issue]-rapport visar det här fältet aktivitetens eller problemets ägare eller [!UICONTROL Primary Assignee]. Du kan även filtrera eller gruppera efter det här fältet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment]</td> 
   <td>En användare, en jobbroll eller ett team som har tilldelats ett ärende eller en uppgift. Projekt, portföljer eller program kan inte ha tilldelningar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignments]</td> 
   <td> <p>I en [!UICONTROL Task]- eller [!UICONTROL Issue]-rapport visar det här fältet en lista över alla entiteter (användare, jobbroller, team) som är tilldelade till uppgiften eller utgåvan. Du kan filtrera efter det här fältet med fälten [!UICONTROL Assignment Users] och [!UICONTROL Assignment Roles]. Du kan filtrera efter det team som tilldelats uppgiften eller utgåvan med hjälp av fältet Team. Du kan inte gruppera en rapport efter det här fältet.</p> <p>Arbetsobjekt som har placerats i [!UICONTROL Recycle Bin] visas fortfarande i vissa rapporter som refererar till [!UICONTROL Assignment]-objektet där en [!DNL OR]-filtermodifierare används.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Roles]</td> 
   <td>
   <p>I en [!UICONTROL Task]- eller [!UICONTROL Issue]-rapport visar det här fältet information om de jobbroller som tilldelats för aktiviteterna eller problemen. Det här fältet visar [!UICONTROL Primary Owners] samt andra jobbroller som tilldelats aktiviteter eller ärenden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Status]</td> 
   <td> <p>I en uppdrags-, uppgifts- eller utgivningsrapport visar [!UICONTROL Assignment Status] om användarna som är tilldelade till ett arbetsobjekt har klickat på knappen [!UICONTROL Work On It] eller [!UICONTROL Done] för att acceptera eller slutföra arbetet. Följande [!UICONTROL Assignment Statuses] finns:</p> 
    <ul> 
     <li><b>[!UICONTROL Requested]</b>: användaren har tilldelats uppgiften eller utgåvan, men har inte klickat på knappen [!UICONTROL Work On It] för att börja arbeta med den än.</li> 
     <li><b>[!UICONTROL Working]</b>: användaren har klickat på knappen [!UICONTROL Work On It] och arbetar för närvarande med objektet. </li> 
     <li><b>[!UICONTROL Done]</b>: användaren har klickat på knappen [!UICONTROL Done] och har slutfört sitt arbete med objektet. </li> 
    </ul> <p>Mer information finns i <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">[!UICONTROL Work On It] och [!UICONTROL Done] knappöversikt</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Teams]</td> 
   <td>
   <p>I en [!UICONTROL task]- eller [!UICONTROL issue]-rapport visar det här fältet information om de team som har tilldelats till aktiviteterna eller problemen. Fältet visar [!UICONTROL Primary Owners] samt andra team som har tilldelats aktiviteter eller problem. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Users]</td> 
   <td>
   <p>I en [!UICONTROL Task]- eller [!UICONTROL Issue]-rapport visar det här fältet information om de användare som har tilldelats till aktiviteterna eller problemen. I det här fältet visas [!UICONTROL Primary Owners] samt andra användare som är tilldelade till uppgifter eller ärenden. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attribute]</td> 
   <td>Ett attribut är ett egenskap för ett [!DNL Workfront]-objekt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Audit Area]</td> 
   <td> <p>Granskningar är systemmeddelanden som registrerar en åtgärd som har utförts i Workfront. Följande granskningstyper registreras:</p> 
    <ul> 
     <li>[!UICONTROL Scope Change]</li> 
     <li>[!UICONTROL Attachment Action]</li> 
     <li>[!UICONTROL General Edit]</li> 
     <li>[!UICONTROL Status Change]</li> 
     <li>[!UICONTROL Note]</li> 
     <li>[!UICONTROL Combined Entry]</li> 
     <li>[!UICONTROL Error Entry]</li> 
     <li>[!UICONTROL Status Change]</li> 
     <li>[!UICONTROL Subscription Change]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Audit Trail]</td> 
   <td>Samlingen av anteckningar som automatiskt genereras av händelser som spåras via de registrerade ändringarna ([!UICONTROL Audit Areas]). Varje anteckning registrerar vem som gjorde åtgärden, vad de gjorde och när de gjorde det.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Automatic And On Change]</td> 
   <td> <p>En av [!UICONTROL Project Update]-typerna. Detta beräknar om projektets planerade och planerade tidslinjer när den nattliga omberäkningen körs och när någon uppdatering görs av projektet eller aktiviteterna i projektet. </p> <p>Mer information finns i <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Välj projekttypens uppdateringstyp </a>.</p> </td> 
  </tr>

<tr> 
   <td><p>Tillgänglighet</p></td> 
   <td> <p>Den här termen används i relation till "användartillgänglighet" eller "resurstillgänglighet" och visar hur lång tid resursen (användaren eller jobbrollen) är tillgänglig för arbete. </p> 
   <p>Workfront beräknar användartillgänglighet i flera fält och beroende på vilka inställningar som finns i systemet för resurshanteringsinställningar. Mer information finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Konfigurera inställningar för resurshantering</a>. </p>
   <p>Mer information om resurstillgänglighet finns i <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Kom igång med resurshantering</a></p>
   Alternativt används"kapacitet" även för att hänvisa till resurstillgänglighet. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Automatic Only]</td> 
   <td> <p>En av [!UICONTROL Project Update]-typerna. Detta beräknar om planerade och planerade tidslinjer när nattomberäkningen körs.</p> <p>Mer information finns i <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Välj typ av projektuppdatering</a>.</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>Arbeta som vanligt och få det att fungera som vanligt.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Backlog]</td> 
   <td>Området i en flexibel miljö där nya problem behålls tills de är klara att behandlas.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Baseline]</td> 
   <td>En datakälla för att mäta iterationer mot i en flexibel miljö.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Billable Expense]</td> 
   <td> <p>En utgift som är markerad som fakturerbar för kunden. Detta kan vara antingen en planerad utgift eller en faktisk utgift.</p> <p>Fälten Planerad fakturerbar utgift och Faktisk fakturerbar utgiftskostnad är tillgängliga så att du kan lägga till i vyer och rapporter. De visas inte på projekt- eller uppgiftsinformationssidorna.</p>
   <p>Du hittar dessa fält i följande typer av rapporter:</p>
   <ul>
   <li>Baslinje</li>
   <li>Mall</li>
   <li>Projekt (ekonomiska data)</li>
   </ul>
   <p>Mer information om hur du markerar en utgift som fakturerbar finns i <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">Hantera projektutgifter</a>.</p>
   </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Billing Record]</td> 
   <td> <p>Registrerar intäkter, timmar eller utgifter som kan faktureras. Den här informationen kan användas för att skapa fakturor i ett externt redovisningssystem.</p> <p>Mer information finns i <a href="../../../manage-work/projects/project-finances/create-billing-records.md">Skapa faktureringsposter</a>. </p> 
   </td> 
  </tr>

<tr> 
   <td>Faktureringspoststatus</td> 
   <td> <p>I en faktureringspost- eller timrapport visar status för en faktureringspost om faktureringsposten har fakturerats eller inte. Du kan inte ta bort ett projekt eller redigera tid som är associerad med en faktureringspost. Mer information finns i <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Skapa faktureringsposter</a>.</p>  
   </td> 
  </tr>


<tr> 
   <td>[!UICONTROL Branding]</td> 
   <td><p>Processen att anpassa [!DNL Workfront] för att ge gränssnittet ett utseende som speglar ditt företag genom att använda dina färger och logotyper.</p><p><strong>Obs!</strong><br>Om din organisation har anslutit till [!DNL Adobe Experience Cloud] är varumärkning inte tillgängligt.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Breadcrumbs]</td> 
   <td> <p>Det område högst upp på sidan som visar den hierarkiska platsen där användaren befinner sig i programmet.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Mer information finns i <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Översikt över vägbeskrivningar</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budget Status]</td> 
   <td> <p>Detta är ett inaktuellt fält. All information som det här fältet kan visa är relaterad till en funktion som [!DNL Workfront] har tagit bort och fältet kan inte uppdateras. </p> <p>Det här fältet visar om projektet lades till i [!UICONTROL Capacity Planner] och om budgetberäkningen har slutförts för det. [!UICONTROL Capacity Planner] har tagits bort från [!DNL Workfront]. </p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is&nbsp;not added to the capacity planner, its value is <i>Not Included</i>.&nbsp;</li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is&nbsp;added to the Capacity Planner but is excluded from the budget calculation,&nbsp;the value is <i>Included but not Calculated</i>.&nbsp;</li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> If the project is&nbsp;added to the Capacity Planner and included in the budget calculation, the value is <i>Included and Calculated</i>. </li>
     --> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budgeted Completion Date]</td> 
   <td> <p>Detta är ett inaktuellt fält. All information som det här fältet kan visa är relaterad till en funktion som [!DNL Workfront] har tagit bort. Det går inte att uppdatera det här fältet. </p>
   <p> Det här fältet är fortfarande synligt i [!UICONTROL project] och [!UICONTROL tasks] rapporter och listor.</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budgeted Cost]</td>

<td> <p>Detta är kostnaden som är associerad med budgeteringsresurser för ett projekt. </p>
   <p>Fältet visas i följande områden i [!DNL Workfront] under följande namn:</p>
   <ul>
   <li><strong>[!UICONTROL Budgeted Cost]</strong>: på panelen [!UICONTROL Business Case Summary]</li>
   <li><strong>[!UICONTROL Cost]</strong>: i [!UICONTROL Utilization]-områdena när information visas av [!UICONTROL Cost]</li>
   <li><strong>[!UICONTROL Project Budgeted Cost]</strong>: i listor och rapporter</li>
   </ul>   
    <p>[!UICONTROL Budgeted Cost] för projektet beräknas med följande formel:</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>Mer information om hur du beräknar [!UICONTROL Budgeted Cost] och om du vill förstå olika namn på det här konceptet i [!DNL Workfront] finns i <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Beräkna projektbudgeterad kostnad</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Budgeted Hours]</td> 
   <td> <p>Budgeterade timmar för resurser för det arbete de behöver för att slutföra projekt. Det här fältet refererar till de timmar som har budgeterats i området [!UICONTROL Resource Budgeting] i [!UICONTROL Business Case] (eller i [!UICONTROL Resource Planner]) för projektet eller för projektresurserna.</p> <p>Mer information finns i <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Förstå [!UICONTROL Budgeted Labor Cost] och [!UICONTROL Budgeted Hours] för projekt</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> Mer information om att budgetera användare i [!DNL Resource Planner] finns i artikeln <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budgetresurser i [!DNL Resource Planner] med [!UICONTROL Project]- och [!UICONTROL Role]-vyerna</a>. </p> 
    <p>De timmar som har budgeterats i området [!UICONTROL Resource Budgeting] i [!UICONTROL Business Case] eller [!UICONTROL Resource Planner] visas i följande områden i [!DNL Workfront] och under följande namn:</p> 
     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td><strong>[!UICONTROL Budgeted Hours] visningsnamn</strong></td> 
        <td><strong>Områden i [!DNL Workfront]</strong></td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Hours]</td> 
        <td>[!UICONTROL Resource Budgeting] området på [!UICONTROL Business Case]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BDG]</td> 
        <td>[!UICONTROL Resource Planner] visas av [!UICONTROL Hours]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Budgeted Hours]</td> 
        <td> <p>Vy för användningsrapport [!UICONTROL Hours]</p> <p>Mer information om rapporten [!UICONTROL Utilization] finns i artikeln <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Översikt över rapporten [!UICONTROL Resource Utilization]</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Bud. Hours]</td> 
        <td> <p>[!UICONTROL Budgeted Hour] rapport</p><p>Objektet [!UICONTROL Budgeted Hour] i rapporten Budgeterad timme refererar till information som relaterar till ett ersatt resurshanteringsverktyg. Endast fältet [!UICONTROL Bud. Hours] i den här rapporten refererar till de timmar som har budgeterats i området [!UICONTROL Resource Planner] eller [!UICONTROL Resource Budgeting] i projektets [!UICONTROL Business Case]. </p> <p>Mer information om hur du skapar en rapport finns i artikeln <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Skapa en anpassad rapport</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Resource Planner Budgeted Hours] </td> 
        <td> <p>Finns i följande rapporter:</p>
        <ul>
        <li>[!UICONTROL Project] rapport
        <li>[!UICONTROL Project (Financial Data)] rapport
        <li>[!UICONTROL Task] rapport
        <li>[!UICONTROL Issue] rapport
        <li>[!UICONTROL Budgeted Hour] rapport</li>
        </ul>
         <p>Mer information om hur du skapar en rapport finns i artikeln <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Skapa en anpassad rapport</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>Alla andra omnämnanden av [!UICONTROL Budgeted Hours] i [!DNL Adobe Workfront] avser timmar som budgeterats med borttagna funktioner från Workfront. Dessa är skrivskyddade fält och uppdateras inte med aktuell information när du använder aktuella resursbudgeteringsverktyg. </p>
    <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Hours from theResource Planner in the areas and reports listed below. </p>
     <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Hours view (in the BDG column)</li>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Hours view</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (the Bud. Hours field refers to hours budgeted for users; the Pln. Bud. Hours field refers to hours budgeted for roles or projects)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Project: Budgeted Hours field) </li>
        </ul>
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The fields listed below display in the reports listed and are hours formerly budgeted in the&nbsp;Capacity Planner or the Legacy Resource Estimates area of the Business Case.</p>
         <p>Important: The Capacity Planner and Legacy&nbsp;Resource Estimates have been removed from Workfront. You cannot update any information that might display in these fields.</p>
        <ul>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Capacity Planner</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Legacy&nbsp;Resource Estimates area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Bud. Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project (Financial&nbsp;Data) report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report (in the Project: Budgeted Hours field)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report (in the Project: Budgeted Hours field)</li>
      </ul> --> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budgeted Labor Cost]</td> 
   <td> <p>Detta är kostnaden som är associerad med de timmar som du, som resurshanterare, budgeterar för dina jobbroller för det arbete de behöver för att slutföra projekt. </p> <p>[!UICONTROL Budgeted Labor Cost] i en projektrapport beräknas med följande formel:</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>Detta fält kan avse följande:</p> 
    <ul> 
     <li> <p>Arbetskostnader som visas i området [!UICONTROL Resource Budgeting] i [!UICONTROL Business Case] eller i [!UICONTROL Resource Planner] som är associerade med kostnaden för jobbroller i ett projekt. Mer information om hur du beräknar [!UICONTROL Budgeted Labor Cost] finns i artikeln <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">[!UICONTROL Understand Budgeted Labor Cost] och [!UICONTROL Budgeted Hours] för projekt </a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Arbetskostnader som visas i området [!UICONTROL Resource Budgeting] i [!UICONTROL Business Case] som återspeglar den [!UICONTROL People Costs] som uppskattats i ett projekt som är länkat till projektet från [!DNL Scenario Planner] när du använder scenarioplanen för att budgetera dina projektresurser. Mer information om initiativ finns i <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">Översikt över initiativ i Scenarioplanen</a>. </p> <p>[!DNL Scenario Planner] kräver ytterligare en licens. Mer information om [!DNL Workfront Scenario Planner] finns i <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Översikt [!DNL Scenario Planner]</a>. </p> </li> 
     <p>Den visas i följande områden under följande namn:</p>
   <ul>
   <li><strong>[!UICONTROL Budgeted Labor Cost]</strong>: i området [!UICONTROL Resource Budgeting] i [!UICONTROL Business Case].
   <li><strong>[!UICONTROL Budgeted Cost]</strong>: i vyn [!UICONTROL Utilization] rapport [!UICONTROL Cost]
   <p>Mer information finns i <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Visa information om resursutnyttjande </a>.</p>
   <li><strong>[!UICONTROL BDG]</strong>: i [!DNL Resource Planner]-projekt eller [!DNL Role]-vyer, vid visning efter kostnad
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>: i följande rapporter: 
   <ul>
    <li>[!UICONTROL Project] rapport</li>
    <li>[!UICONTROL Project (Financial Data)] rapport</li>
    <li>[!UICONTROL Task] rapport</li>
    <li>[!UICONTROL Issue] rapport</li>
    <li>[!UICONTROL Budgeted Hour] rapport</li> 
    </ul>
    <p>Mer information om hur du skapar en rapport finns i artikeln <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Skapa en anpassad rapport</a>.</p>
    <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Labor costs for hours budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner). This was available only in Adobe Workfront Classic. </p>
           <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
       </li> 
    </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost field based on the hours budgeted in the Resource Planner in the following areas and reports in&nbsp;Workfront: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Cost view (in the BDG column)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Cost view (in the Budgeted Cost column)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case </li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost associated with resources budgeted in the Resource Planner in the Resource Planner Resource Budgeted Cost field in the following reports: </p>
       <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate a Budgeted Labor Cost field that contains information from a tool that has been deprecated in the reports listed below. You can no longer update the fields displayed in these reports and budgeting your resources on the projects does not update them: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul>      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating the Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>&nbsp;.&nbsp;</p>
    --> 
    </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Budgeted Start Date]</td> 
  <td> <p>Detta är ett inaktuellt fält. All information som det här fältet kan visa är relaterad till en funktion som [!DNL Workfront] har tagit bort. Det går inte att uppdatera det här fältet.</p>
  <p>De här områdena har tagits bort från [!DNL Workfront]. </p> 
  <p>Fältet är fortfarande synligt i [!UICONTROL project] och [!UICONTROL task] rapporter och listor.</p>
   <!--
   <p>This field shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.</p>
   -->   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Burndown Chart]</td> 
   <td>Ett linjediagram som ger en visuell representation av slutfört och återstående arbete.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Business Case]</td> 
   <td> <p>Ett verktyg som används för att utvärdera om ett projekt ska flyttas framåt från statusen [!UICONTROL Idea] till statusen [!UICONTROL Planning]. Med andra ord hjälper en [!UICONTROL business case] organisationen att avgöra om det är värt besväret att starta och slutföra projektet eller inte, särskilt när man jämför projekt med andra i en portfölj.</p> <p>Mer information finns i <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Skapa en [!UICONTROL Business Case] för ett projekt </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Business Case Budgeted Hours]</td> 
   <td> <p>Detta är ett inaktuellt fält. All information som det här fältet kan visa är relaterad till en funktion som [!DNL Workfront] har tagit bort. Det går inte att uppdatera det här fältet.</p> <p>Det här fältet är fortfarande synligt i projekt och [!UICONTROL task] listor och rapporter. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calculated Assignment]</td> 
   <td> <p>En av uppgifterna [!UICONTROL Duration Types]. Detta beräknar procentandelen av en 8-timmars arbetsdag som användaren som är tilldelad uppgiften tilldelas till uppgiften, baserat på [!UICONTROL Duration] för uppgiften och [!UICONTROL Work Required].</p> <p>Mer information finns i <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Översikt över aktiviteten [!UICONTROL Duration] och [!UICONTROL Duration Type]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calculated Work]</td> 
   <td> <p>En av uppgifterna [!UICONTROL Duration Types]. Detta beräknar [!UICONTROL Work Required] för en aktivitet utifrån procentsatserna [!UICONTROL Duration] och användaren [!UICONTROL Assignment] (som baseras på en arbetsdag på 8 timmar).</p> <p>Mer information finns i <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Översikt över aktiviteten [!UICONTROL Duration] och [!UICONTROL Duration Type]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar]</td> 
   <td> <p>Det finns två typer av kalendrar i [!DNL Workfront]: [!UICONTROL Home Calendar]- och kalenderrapporter.</p> <p>[!UICONTROL Home Calendar] är en personlig kalender som gör att en användare kan hantera sin arbetsbelastning mot sina tillgängliga timmar i [!DNL Workfront]. Användarna kan även integrera sina [!UICONTROL Home Calendar] med [!DNL Outlook] ([!DNL Google] och [!DNL Microsoft]-integrering som kommer). </p> <p>Mer information om [!UICONTROL Home Calendar] finns i <a href="../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md" class="MCXref xref">[!UICONTROL Home Calendar] view </a>.</p> <p>En kalenderrapport är en dynamisk rapport där användare kan visa datum och annan viktig information om en händelse, inklusive förfallodatum, arbetsstatus och användaren som händelsen är tilldelad till.</p> <p> Mer information om kalenderrapporter finns i <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">Översikt över kalenderrapporter</a>.</p> </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL Can Start]</td> 
   <td> <p>Det här fältet anger om en uppgift är klar att börja bearbetas. Om starten är klar att bearbetas i fältet [!UICONTROL Can Start] för aktiviteten är inställd på [!UICONTROL True]. </p> <p>Mer information finns i Översikt över <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref"> [!UICONTROL Can Start] för uppgifter </a>.</p> 
   <!--
     <p>(NOTE: everything below is drafted because I created a new article linked above with all this information - it was getting kind of too big for just a table cell)</p>
    --> <!--
     <p>Workfront checks for the following things before it marks a task as True for the Can Start field:<br></p>
    --> 
    <!--
     <ul> 
      <li> If the task has a parent, it checks to see if the value of Can Start for the parent it set to True. If the value for the parent is False, then all the subtasks have the value of Can Start set to False, as well.&nbsp;</li> 
      <li> It also checks to see if the predecessors of the task as well as the predecessors of their parents are complete. If they are complete, the Can Start value for the task is set to True. If any of the task predecessors or their parents' predecessors are not complete, or have a status of Complete-Pending Approval, then the Can Start value for the task is set to False.&nbsp;</li> 
     </ul>
    --> 
    <!--
     <p>For information about task predecessors, see <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p>
    --> <!--
     <p>Tip: If the Dependency Type between a task and its predecessors is Start-Start, the predecessor must start before the predecessor relationship is considered resolved and the successor tasks can start. For information about dependency types, see <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Overview of task dependency types</a>. </p>
    --> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Capacity</td> 
    <td>The total availability (measure in either hours or FTE) of a designated user, resource pool, team, rob role, or company.</td> 
   </tr>
  -->

<tr> 
   <td> <p>Kapacitet</p> </td> 
   <td> <p>En resurs tillgängliga tid när de kan allokeras till arbete. Se Tillgänglighet. </p></td> 
  </tr>

<tr> 
   <td> <p>[!UICONTROL Category]</p> </td> 
   <td> <p>En kategori är ett anpassat formulär. Du kan skapa rapporter för det här objektet och du kan även visa det i andra objektrapporter. Alla objekt kan inte ha ett eget formulär eller en egen kategori. Följande objekt kan ha ett eget formulär: <br></p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Task]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Document]</li> 
     <li>[!UICONTROL Expense]</li> 
     <li>[!UICONTROL Program]</li> 
     <li>[!UICONTROL User]</li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteration]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Category Name]</td> 
   <td> <p>När den läggs till som en kolumn i vyn för något av följande objekt visas en lista med alla anpassade formulär som är kopplade till dessa objekt:</p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Task]<br></li> 
     <li>[!UICONTROL Issue]<br></li> 
     <li>[!UICONTROL Portfolio]<br></li> 
     <li>[!UICONTROL Document]<br></li> 
     <li>[!UICONTROL Expense]<br></li> 
     <li>[!UICONTROL Program]<br></li> 
     <li>[!UICONTROL User]<br></li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteration]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Change Management]</td> 
   <td>Ett verksamhetsområde som är inriktat på att definiera, förstå och anpassa planerade arbeten till förändringar i omfång, schema, kostnad och resursfaktorer.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Change Order]</td> 
   <td>En typ av problem som uppstår mot ett projekt som anger en begärd ändring av det överenskomna omfånget.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Change Only]</td> 
   <td>Ett av projekten [!UICONTROL Update Types]. Det uppdaterar bara tidslinjer för [!UICONTROL Project Projected] och [!UICONTROL Planned] när uppdateringar görs av aktiviteter eller redigeringar utförs på projektet eller aktiviteterna.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Change Order]</td> 
   <td> <p>En av [!UICONTROL Issue]-typerna, som vanligtvis anger att ett oplanerat arbetsflöde måste utföras innan projektet kan slutföras.</p> <p>Mer information om [!UICONTROL Issue]-typer finns i avsnittet Standardproblemtyper i artikeln <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">Anpassa standardproblemtyper</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Child Task]</td> 
   <td>En aktivitet som är en [!UICONTROL Subtask] av en [!UICONTROL Parent Task] ([!UICONTROL Summary Task]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Children]</td> 
   <td>Samlingen av [!UICONTROL Subtasks] till en [!UICONTROL Parent Task] ([!UICONTROL Summary Task]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coaching] och [!UICONTROL Training]</td> 
   <td>Utbildningsmoduler, certifieringar, standarder eller en community med övningar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commit]</td> 
   <td>Ett kommunikationsverktyg som användare kan använda för att ställa in förväntningar på uppgiftsleveranser.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commit Date]</td> 
   <td>Ett kommunikationsverktyg som användaren kan använda för att ställa in förväntningarna kring uppgiftsleveranser.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Communication] och [!UICONTROL Reporting]</td> 
   <td>Standarder för att granska undantag och hälsa för ett projekt, program eller en portfölj</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Company]</td> 
   <td> <p>En [!UICONTROL Company] är en organisationsenhet i [!DNL Workfront]. </p> 
   <p> Du kan associera en användare eller ett projekt med ett företag. Mer information finns i <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">Skapa och redigera företag</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion date]</td> 
   <td> <p>Det datum då ett projekt, en uppgift eller ett ärende är inställt att slutföras. Det finns flera typer av [!UICONTROL Completion dates] i [!DNL Workfront]:</p> 
    <ul> 
     <li>[!UICONTROL Actual Completion Date]. Mer information finns i <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Översikt över projektet [!UICONTROL Actual Completion Date] </a>.</li> 
     <li>[!UICONTROL Planned Completion Date]. Mer information finns i <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Ange projektet [!UICONTROL Planned Completion Date]</a> och <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Översikt över aktiviteten [!UICONTROL Planned Completion Date]</a>.</li> 
     <li>[!UICONTROL Projected Completion Date]. Mer information finns i <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Översikt över [!UICONTROL Projected Completion Date] för projekt, uppgifter och problem</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion Day]</td> 
   <td>Den dag, i förhållande till början av [!UICONTROL Template], som en [!UICONTROL Template Task] eller en [!UICONTROL Template] ska vara slutförd.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion Mode]</td> 
   <td> <p>Detta visar hur ett projekt markeras som [!UICONTROL Complete]. Den kan ha två värden:</p> 
    <ul> 
     <li>[!UICONTROL Manual]: En användare måste ändra projektstatus till [!UICONTROL Complete].</li> 
     <li>[!UICONTROL Automatic]: Projektstatusen ändras automatiskt till [!UICONTROL Complete] när alla aktiviteter i projektet är 100 % slutförda och alla utgåvor stängs.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condition]</td> 
   <td> <p>Detta är en visuell representation av förloppet för en uppgift, ett problem eller ett projekt.</p> <p>För projekt kan villkoret ställas in manuellt av projektägaren eller automatiskt av [!DNL Workfront], baserat på projektets förloppsstatus. </p> <p>Möjliga värden för projektvillkoret är:</p> 
    <ul> 
     <li>[!UICONTROL On Target]</li> 
     <li>[!UICONTROL At Risk]</li> 
     <li>[!UICONTROL In Trouble]</li> 
    </ul> <p>Mer information om projektvillkor finns i artikeln <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Översikt över [!UICONTROL Project Condition] och [!UICONTROL Condition Type]</a>.</p>
     <p>Du kan koppla uppgifts- och utgivningsvillkor till ett tal som kan visas i rapporter. I listorna nedan visas standardnamn och standardnummer för uppgifts- och utgivningsvillkor. Systemadministratören kan uppdatera namnen på villkoren och lägga till nya villkor med olika nummer. När ett tal har associerats med ett villkor kan det inte redigeras.  </p> 
     <p>För uppgifter anges villkoret manuellt av uppgiftsägaren. Möjliga värden för aktivitetsvillkoret är:</p> 
    <ul> 
     <li>[!UICONTROL Going Smoothly] (0)<br></li> 
     <li> [!UICONTROL Some Concerns] (1)<br></li> 
     <li>[!UICONTROL Major Roadblocks] (2)</li> 
    </ul> <p>Mer information om aktivitetsvillkor finns i artikeln <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Uppdatera [!UICONTROL Condition] för uppgifter och problem</a>.</p> <p>För problem ställs villkoret in manuellt av utfärdaren. Möjliga värden för problemvillkoret är:<br></p> 
    <ul> 
     <li>[!UICONTROL Going Smoothly] (0)<br></li> 
     <li>[!UICONTROL Some Concerns] (1)<br></li> 
     <li>[!UICONTROL Major Roadblocks] (2)</li> 
    </ul> 
   <p><b>ANMÄRKNING</b></p>
    <p>När fältet [!UICONTROL Condition] spåras i [!UICONTROL Journal Entry] rapporter visar [!UICONTROL New] och [!UICONTROL Old Number Values] numret som är associerat med villkoret i stället för dess namn. Om ett villkor ursprungligen inte är definierat för en aktivitet eller ett problem och du senare uppdaterar det, kommer journalposten som hämtar uppdateringen att visa [!UICONTROL Old Number Value] för [!UICONTROL Condition]-fältet som -2 147 483 648. Se även [!UICONTROL New Number Value], [!UICONTROL Old Number Value] och [!UICONTROL Journal Entry] i den här artikeln. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condition Update]</td> 
   <td> <p>I det här fältet visas det aktuella tillståndet för uppgifter, projekt eller utgåvor. Det här alternativet visar de senaste uppdateringarna som ägare av aktiviteter, projekt eller utgåvor har tillhandahållit i fältet [!UICONTROL Update Status], tillsammans med det nya villkoret.</p> <p>Kommentarer som gjorts för villkorsuppdateringar visas inte i kolumnen [!UICONTROL Condition Update]. Endast huvuduppdateringen visas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Date]</td> 
   <td> <p>Om du använder en [!UICONTROL Task Constraint] som är knuten till ett specifikt datum, till exempel [!UICONTROL Must Start On], blir det datumet [!UICONTROL Constraint Date] för uppgiften.</p> <p>Följande uppgiftsbegränsningar uppdaterar fältet [!UICONTROL Constraint Date]:</p> 
    <ul> 
     <li>[!UICONTROL Must Start On]</li> 
     <li>[!UICONTROL Must Finish On]</li> 
     <li>[!UICONTROL Start No Later Than]</li> 
     <li>[!UICONTROL Start No Earlier Than]</li> 
    </ul> <p><b>TIPS</b></p>   
     <ul> 
      <li> <p>En aktivitet med [!UICONTROL Constraint] av [!UICONTROL Fixed Dates] saknar [!UICONTROL Constraint Date]. </p> </li> 
      <li> <p> [!UICONTROL Constraint Date] kan bara visas i en rapport eller anpassad vy.</p> </li> 
     </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Day]</td> 
   <td> <p>Om du använder en uppgiftsbegränsning i en malluppgift som är kopplad till en viss dag, till exempel Måste starta på, blir den dagen malluppgiftens begränsningsdag.</p> <p>Följande uppgiftsbegränsningar uppdaterar fältet [!UICONTROL Constraint Day]:</p> 
    <ul> 
     <li>[!UICONTROL Must Start On]</li> 
     <li>[!UICONTROL Must Finish On]</li> 
     <li>[!UICONTROL Start No Later Than]</li> 
     <li>[!UICONTROL Start No Earlier Than]</li> 
    </ul> <p><b>TIPS</b></p> <p>  [!UICONTROL Constraint Day] kan bara visas i en rapport eller anpassad vy. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Type]</td> 
   <td> <p>En uppgifts tidsplaneringstrend. [!UICONTROL As Soon as Possible] schemalägger till exempel en aktivitet som börjar så snart som möjligt och [!UICONTROL Finish No Later Than] schemalägger en aktivitet som ska slutföras av [!UICONTROL Constraint Date] och inte senare.</p> <p>Mer information finns i <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">[!UICONTROL Task Constraint] - översikt</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contextual Menu]</td> 
   <td>En meny, som finns till vänster på skärmen, där alternativen ändras för att korrelera med det aktiva innehållet. När en användare till exempel visar ett projekt visar [!UICONTROL Contextual Menu] länkar till projektrelaterad information och verktyg.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converted Issue Originator]</td> 
   <td>Ett fält i ett projekt eller en aktivitetsrapport som visar information om användaren som är [!UICONTROL Primary Contact] för ett problem när problemet konverteras till ett projekt eller en uppgift. Fältet visas också i avsnittet [!UICONTROL Project Details] där namnet på [!UICONTROL Primary Contact] för den konverterade utgåvan visas. Se även [!UICONTROL Primary Contact] i den här artikeln.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Cost]</td> 
   <td> <p>Det penningbelopp som du måste spendera när du slutför ett projekt, en uppgift eller en utgåva. </p> <p>Du kan spåra olika typer av kostnader för arbete, utgifter och risker som relaterar till projektet. Mer information om att spåra kostnader i [!DNL Workfront] finns i <a href="../../../manage-work/projects/project-finances/track-costs.md">Spåra kostnader</a>.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cost Type]</td> 
   <td>För en uppgift avgör [!UICONTROL Cost Type] hur aktiviteten kommer att öka kostnaderna. Några exempel är [!UICONTROL Fixed Hourly], [!UICONTROL User Hourly] och [!UICONTROL User Hourly plus Fixed]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cross-Project Dependencies]</td> 
   <td> <p>En aktivitet i ett projekt är beroende av en aktivitet från ett annat projekt.</p> <p>Mer information finns i <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Skapa föregående projekt mellan projekt</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Custom Data]</td> 
   <td> <p>Data som är unika för en organisation. Organisationer kan anpassa programmet [!DNL Workfront] genom att skapa anpassade formulär och anpassade fält. Denna anpassade information kan leda till rapporter för nyckeltal, revision och efterfrågeblandning. </p> <p>[!UICONTROL Custom Data] kan länkas till:</p> 
    <ul> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Users]</li> 
     <li>[!UICONTROL Companies]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Expenses]</li> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programs]</li> 
     <li>[!UICONTROL Iterations]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Data Type]</td> 
   <td>Alternativet som anger om ett [!UICONTROL Custom Data]-fält lagras i databasen som Text, Datum, Nummer eller Valuta.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Display Type]</td> 
   <td>Fälttypen för ett anpassat fält. Exempel är [!UICONTROL Drop-Down], [!UICONTROL Text Field], [!UICONTROL Text Area], [!UICONTROL Radio Buttons] osv.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Field]</td> 
   <td>För anpassade data som gör det möjligt för användaren att välja mellan flera alternativ är dessa värden de värden som användaren kan välja från. Anpassade alternativ är bara giltiga för [!UICONTROL Drop-Down], [!UICONTROL Multi-Select Drop-Down], [!UICONTROL Radio Buttons] och [!UICONTROL Checkboxes].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Form Label]</td> 
   <td>När du använder en anpassad visningstyp med anpassade alternativ är det den text i användargränssnittet som visas i listrutan, kryssrutorna eller alternativknapparna för det anpassade alternativet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Value]</td> 
   <td>När du använder ett anpassat fält med anpassade alternativ är det här värdet som kommer att lagras i databasen för ett visst alternativ.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom View]</td> 
   <td>En definition av de datafält, eller kolumner som visas för varje objekt i en lista.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Customer]</td> 
   <td>En organisation som använder en instans av Workfront.</td> 
  </tr> 
 </tbody> 
</table>

## D - F

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objektnamn</th> 
   <th>Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Dashboards]</td> 
   <td> <p> Du kan lägga till det här fältet i en rapport eller en vy av rapportobjektet för att visa de instrumentpaneler som rapporten finns på i en lista. </p> <p> Du kan även använda det här fältet för att filtrera efter rapporter som visas på en specifik kontrollpanel. </p> <p> Mer information om hur du tar med instrumentpanelsinformation om rapportobjektrapporter finns i avsnittet Om vilka rapporter som visas på instrumentpaneler i artikeln <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">Åtkomst till och ordna rapporter</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data Type]</td> 
   <td>Se [!UICONTROL Custom Data Type].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Days Late]</td> 
   <td> <p>Det här fältet visar en datumskillnad mellan [!UICONTROL Planned Start] och [!UICONTROL Today] om [!UICONTROL Actual Completion Date] saknas.</p> <p>Visar också en datumskillnad mellan [!UICONTROL Actual Completion] och [!UICONTROL Planned Completion] när det finns en [!UICONTROL Actual Completion Date].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Default Schedule]</td> 
   <td> <p>Anpassningsbara standardarbetstider som ska tilldelas användare och projekt inom en organisation. </p> <p>Scheman används för att beräkna datum för planerade, start och slutförande av uppgifter som har tilldelats användare.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Deliverable]</td> 
   <td>Kvantifierbara varor eller tjänster som måste tillhandahållas när ett projekt har slutförts.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Demand Management]</td> 
   <td>Värdering och prioritering av intag.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Department Goals]</td> 
   <td>Mål som är unika för en viss avdelning och som fokuserar på att förbättra driftsstatistik inom avdelningen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependency]</td> 
   <td>Länken mellan två uppgifter som kräver att en aktivitet ändrar status innan den andra aktiviteten kan också ändra status.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependency Type]</td> 
   <td> <p>Typen av schemaläggningsrelation mellan en aktivitet och dess föregångare. Ett exempel är [!UICONTROL Finish-Start], vilket kräver att den första aktiviteten måste avslutas innan den andra aktiviteten kan starta.</p> <p>Mer information finns i <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Översikt över typer av uppgiftsberoenden</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document]</td> 
   <td>Alla filer som är kopplade till ett objekt inom [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document Version]</td> 
   <td> <p>Varje gång samma dokument överförs till samma objekt tilldelas det ett versionsnummer. Användare kan visa och ändra flera alternativ för en tidigare version av ett dokument.</p> <p>Mer information finns i <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">Hantera dokumentversioner</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duration]</td> 
   <td> <p>Fönstret med den tid som tilldelats för slutförande av ett aktivitetsproblem, eller projekt (som bestäms av antalet dagar mellan [!UICONTROL Planned Start] och det planerade slutförandet).</p> 
    <ul> 
     <li>För uppgifter är Varaktighet ett redigerbart fält om uppgiftens varaktighetstyp inte är Enkel. Om varaktighetstypen för aktiviteten är Enkel, eller om aktivitetsbegränsningen är Fasta datum, är Varaktighet en beräkning som utförs av Workfront.</li> 
     <li>För problem är fältet Varaktighet alltid ett redigerbart fält och det bör representera en uppskattning av antalet dagar som skulle kräva att problemet löstes.</li> 
     <li>För projekt är Varaktighet en beräkning som utförs av [!DNL Workfront] och representerar skillnaden i dagar mellan planerad start för den första aktiviteten och [!UICONTROL Planned Completion] för den senaste aktiviteten i projektet.</li> 
    </ul> <p>Mer information om skillnaden mellan [!UICONTROL Duration] och [!UICONTROL Planned Duration] för uppgifter finns i artikeln <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md"> Skillnad mellan [!UICONTROL Planned Duration] och [!UICONTROL Duration] för uppgifter </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duration in Minutes]</td> 
   <td>Det här fältet visar samma information som fältet [!UICONTROL Duration] på några minuter i stället för dagar. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Duration per Occurrence]</td> 
   <td> <p>Detta visas i rutorna [!UICONTROL Task Details] och [!UICONTROL Edit Task] för en överordnad för återkommande uppgifter. Den visar varaktigheten för varje återkommande uppgift. Mer information om hur du skapar återkommande aktiviteter finns i <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Skapa återkommande aktiviteter</a>. </p> <p> <span>Varaktigheter som ändras i enskilda återkommande aktiviteter visar inte det värde som anges i det här fältet.</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Duration Type]</td> 
   <td> <p>Ett aktivitetsfält som anger hur det arbete som krävs för att slutföra uppgiften fördelas mellan de tilldelade under uppgiftens varaktighet. Det representerar relationen mellan [!UICONTROL Duration] för aktiviteten, [!UICONTROL Work Required] och tiden, eller [!UICONTROL Allocation], de tilldelade resurserna ska användas för aktiviteten för att slutföra den. </p> <p>Det här fältet visas på fliken [!UICONTROL Details] för en uppgift. </p> <p>Alternativen för varaktighetstypen för en uppgift är:</p> 
    <ul> 
     <li>[!UICONTROL Calculated assignment]</li> 
     <li>[!UICONTROL Calculated Work]</li> 
     <li>[!UICONTROL Effort Driven]</li> 
     <li>[!UICONTROL Simple]</li> 
    </ul> <p>Mer information finns i <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Översikt över aktiviteten [!UICONTROL Duration] och [!UICONTROL Duration Type]</a>.</p> 
    —&gt; </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Duration Unit]</td> 
   <td>Den enhet som används för att mäta tiden i en strömsökning.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Effort Driven]</td> 
   <td>Relationen mellan antalet användare och den tid det tar att slutföra uppgiften. När du lägger till fler användare minskar den totala schemalagda tiden för att slutföra uppgiften, men varaktigheten för aktiviteten ändras inte. Om en uppgift t.ex. är att skryta med ett par jordnötter, kommer den schemalagda tiden att minska om fler personer läggs till, men varaktigheten i persondagar kommer att vara densamma.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Elapsed Time]</td> 
   <td> <p>[!UICONTROL Elapsed time] är en tidsenhet för en uppgifts [!UICONTROL Duration]. Det är tiden mellan [!UICONTROL Planned Start Date] och [!UICONTROL Planned Completion Date] för en aktivitet som omfattar helger, helger och ledig tid. Med andra ord är förfluten tid en del av kalenderdagarna. </p> <p>[!DNL Workfront] har stöd för följande enheter för förfluten tid för uppgiftens varaktighet:</p> 
    <ul> 
     <li> <p>[!UICONTROL Elapsed Minutes]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Hours]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Days]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Weeks]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Months]</p> </li> 
    </ul> <p>Mer information om aktivitetens varaktighet, inklusive förfluten tid, finns i <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Översikt över aktiviteten [!UICONTROL Duration] och [!UICONTROL Duration Type]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL End Date]</td> 
   <td> <p> I en [!UICONTROL Rate]-rapport är detta det datum då en ny faktureringsfrekvens för en jobbroll på projektnivå avslutas. De timmar som är associerade med projektet som är före detta datum multipliceras med den här faktureringstakten för att beräkna projektets intäkter. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Engagement]</td> 
   <td>[!UICONTROL Work Performance Indicator] (WPI) som anger när engagemang och tro på uppgiften, projektet, teamet eller organisationen avtar. Detta visar att ni måste agera för att återförverkliga den tron och det engagemang ni har. WPI mäts genom att ställa de enkla frågorna: "Förstår du vad du förväntade dig? Gjorde det du fick göra någon skillnad för organisationen? Gjorde du ett bra jobb?"</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Enterprise Goals]</td> 
   <td>Korsfunktionella mål som bidrar till mätvärdena för företagets mål.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event]</td> 
   <td>Ändringar i ett projekt eller en uppgift.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event Handler]</td> 
   <td>Automatiska uppgifter som inträffar när händelser inträffar. Ett vanligt exempel är ett automatiskt e-postmeddelande.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event notification]</td> 
   <td>E-post som genereras från en händelsehanterare.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Expenses]</td> 
   <td>En icke-arbetskostnad för uppgifter eller projekt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL External]</td> 
   <td> <p>Vanligtvis är detta en licenstyp, eller en användare med en sådan licens. En användare med en sådan licenstyp har bara möjlighet att granska information i systemet. De kan inte aktivt delta i arbetet.</p> <p>Mer information finns i <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] licensöversikt</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL External System]</td> 
   <td>Tjänster eller programvara som lagras och styrs utanför det angivna arkivsystemet.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Field]</td> 
   <td><p>Alla Workfront-objekt eller den information som är kopplad till dem, så som de visas i databasen. </p>
   <p>Till exempel är "project", "user", "hour" både Workfront-objekt och fält. "Namn", "status", "ägare", "startdatum" är Workfront-fält som är associerade med ovanstående objekt. </p>

<p>När du refererar till objekt kan termerna "objekt" och "fält" användas på ett sätt som inte kan ändras.</p>
   <p>När det gäller rapportering avser"fälten" objekten eller informationen om objektet som du vill hämta i rapporten.</p>

<p><b>ANMÄRKNING</b></p>

<p>I textrapporter hänvisar fälten till objekten eller deras information så som den visas i databasen.</p>
   <p>Ibland skiljer sig namnet som visas i användargränssnittet från namnet på fältet i databasen. "issue" är till exempel namnet på objektet i Workfront-gränssnittet, men "opTask" är namnet på objektet (eller fältet) i Workfront-databasen. </p> 
   <p> Det är viktigt att du använder fältet så som det visas i databasen när du skriver en textlägesrapport, vy, filter eller gruppering, eller när du skapar ett beräkningsfält.</p>

<p>Mer information finns i <a href="../../../wf-api/general/api-explorer.md">API-utforskaren</a> och <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md">Textläge - översikt</a>.</p>

<p>Som standard innehåller Workfront en uppsättning fält som definierar både objekt och deras information. Du kan också skapa anpassade fält för att definiera objekt, men du kan inte skapa anpassade objekt.</p> 
   </td> 
  </tr>

<tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Filter]</td> 
   <td> <p>Ett av huvudbyggstenarna i en rapport eller ett listelement som definierar vilken information som visas på skärmen. Mer information om rapportelement finns i <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Rapportera element: filter, vyer och grupperingar</a>.</p> <p>Filtret avgör vilka resultat som visas i en rapport eller på en [!DNL Workfront]-panel, som projekt, uppgifter eller problem.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Financial Work Management]</td> 
   <td>Process för att hantera arbetskostnader, utgifter och intäktsdata i [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fixed Cost]</td> 
   <td>Du kan definiera ett fast kostnadsbelopp för ett projekt. Detta är en del av [!UICONTROL Planned Cost] av projektet som representerar den summa pengar som du behöver för att slutföra projektet. Mer information om kostnader finns i <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Spåra kostnader</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fixed Revenue]</td> 
   <td>Du kan definiera ett fast intäktsbelopp för ett projekt. Detta är en del av [!UICONTROL Planned Revenue] i projektet som representerar den summa pengar som du kan få om du slutför projektet. Mer information om intäkter finns i <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Översikt över fakturering och intäkter</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Flags]</td> 
   <td> <p> Detta är samma fält som [!UICONTROL Status Icons], men det är bara tillgängligt för följande vyer: </p> 
    <ul> 
     <li> [!UICONTROL Templates] </li> 
     <li> [!UICONTROL Expenses] </li> 
    </ul> <p> Mer information finns i artikeln <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Inbyggda statusikoner i vyer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder]</td> 
   <td>Mappar används för att ordna dokument eller rapporter som är kopplade till ett objekt.</td> </tr>
  <tr>
  <td>[!UICONTROL FTE] (heltidsekvivalent)</td> 
   <td>Det här är heltidsmotsvarigheten som anger hur lång tid en resurs är tillgänglig för arbete. 
   Fältet [!UICONTROL FTE] visas i följande områden: 
  <ul>
   <li> Användarprofil, när användaren redigerar eller skapar </li>
   <li> [!UICONTROL Resource Planner] </li>
   <li> [!UICONTROL Scenario Planner] (ytterligare licens krävs för Workfront Scenario Planner) </li>
   <li> Användarlistor och rapporter </li> </ul>

<p>[!UICONTROL FTE] måste vara ett decimaltal upp till 1 och det får inte vara 0. </p>
   <p> En [!UICONTROL FTE] av 1 (som är standard för en användares [!UICONTROL FTE]-fält, enligt definitionen i användarens profil) betyder att en resurs (användare eller roll) arbetar hela antalet timmar, baserat på det schema som beräknar tillgängligheten. </p>
   <p>Din Workfront-administratör bestämmer vilket schema som ska användas för att fastställa användarens tillgänglighet.  </p>
   <ul>
   <li> När [!UICONTROL Default Schedule] används använder Workfront [!UICONTROL FTE] för användaren som finns i deras profil för att beräkna tillgängligheten. </li>
   <li> När användarens schema används används användarens tid av, [!UICONTROL Work Time]-värde och [!UICONTROL Default Schedule]-timmar för att beräkna användarens [!UICONTROL FTE]. </li> </ul>

<p>Mer information finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Konfigurera inställningar för resurshantering</a>.  </p>
   <p>Mer information om hur du skapar scheman i [!DNL Workfront] finns i <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Skapa ett schema</a>. </p>

<p><b>ANMÄRKNING</b></p>
   <p>För alla beräkningar i [!UICONTROL Scenario Planner] använder Workfront följande värde: 1 [!UICONTROL FTE] = 8 timmar.</p>
   <p>Mer information finns i <a href="../../../scenario-planner/get-started-with-scenario-planning.md">Kom igång med [!UICONTROL Scenario Planner]</a>. </p>
   </td> </tr> 
   </tbody> 
   </table>

<!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Task field used by the planner to set how the work required is allocated to the assignees across the duration.</p>
<!--
FTE
The designated full time equivalency for users. A full-time user should have 100% FTE and part-time user should have a percentage that equals their working hours. 
-->

## G - I

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objektnamn</th> 
   <th>Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Gantt Chart]</td> 
   <td> <p>En visuell tidslinje för projektdatum i en kalendervy baserat på planerade eller planerade datum när aktiviteterna för projektet är schemalagda.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal]</td> 
   <td><p>Det finns två koncept för mål i [!DNL Workfront]: </p> 
    <ul> 
     <li> <p><b>Projektmål</b>: En uppsättning affärsmål som har överenskommits med relevanta intressenter i ett projekt. Projektmål ingår i ett projekts affärsfall. </p> <p>Du kan inte visa projektmål i listor eller rapporter, men du kan komma åt dem via API:t. </p> <p>Mer information om projektmål för affärsärenden finns i <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">Skapa mål för affärsärenden </a>. </p> </li> 
     <li> <p><b>Strategiska mål</b>: Ett strategiskt mål är ett mål som du skapar för att planera din arbetsstrategi för en viss tidsperiod. Du kan skapa de här typerna av mål med [!DNL Workfront Goals]. Din organisation måste köpa ytterligare en licens och du måste ha tillgång till den här funktionen för att kunna skapa strategiska mål. [!DNL Workfront Goals] är bara tillgängliga med ytterligare en licens.</p> 
     <p>Mer information finns i <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] översikt </a>. </p> 
     <p>Du kan visa strategiska mål i ett mål eller en projektrapport och få tillgång till dem via API:t. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal Hierarchy]</td> 
   <td> <p>I [!UICONTROL Goal]- och [!UICONTROL Project]-rapporter är detta ett samlingsfält som visar målen i hierarkin som ett strategiskt mål tillhör när det justeras mot andra mål. Målen avgränsas med en ▸. </p> <p>Endast målets överordnade och målet visas i det här fältet. Barnens mål visas inte. </p> <p>Mer information om att justera mål i [!DNL Workfront Goals] finns i <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">Översikt över måljustering i [!DNL Workfront Goals]</a>. </p> 
   <p>Det här fältet visas bara om din organisation har köpt [!DNL Workfront Goals]. Mer information om hur du hanterar strategiska mål med [!DNL Workfront Goals] finns i <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] översikt </a>. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal Success Score]</td> 
   <td> I en [!UICONTROL Project report] refererade det här fältet till projektnivåmål som är kopplade till [!UICONTROL Business] -ärendet. För närvarande är detta ett föråldrat fält och är inte kopplat till någon funktion.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Goals] </td> 
   <td> <p>I en [!UICONTROL Project]-rapport är detta ett samlingsfält som visar alla strategiska mål som är kopplade till ett projekt. Målen avgränsas med kommatecken.</p> <p>Det här fältet visas bara om din organisation har köpt [!DNL Workfront Goals]. Mer information om hur du hanterar strategiska mål med [!DNL Workfront Goals] finns i <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] översikt</a>. Mer information om strategiska mål och projektmål i [!DNL Workfront] finns i [!UICONTROL Goal] i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global Interface Preferences]</td> 
   <td>Gränssnittsinställningar som påverkar alla användare. [!UICONTROL Global Interface Preferences] kan skrivas över av [!UICONTROL User Interface Preferences].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Group]</td> 
   <td> <p>En samling användare (eventuellt från samma avdelning eller affärsenhet) som har åtkomst till samma objekt. Förutom användare kan grupper associeras med portföljer, program, projekt, <span> projektmallar, </span> företag, team, scheman, layoutmallar och tidrapportprofiler.</p> <p>Du kan också tilldela behörigheter till objekt per grupp. Mer information finns i <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Översikt över grupper</a>.</p> <p>I en lista eller rapport över objekt av någon av följande typer kan du använda fältet [!UICONTROL Group] för att lista vilka objekt av den typen som är associerade med en viss grupp: användare, portfölj, program, projekt, <span>projektmall</span>, företag, team, schema, layoutmall eller tidrapportprofil.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Group Administrator]</td> 
   <td> <p>Användare som hanterar objekt, åtkomst och användare för angivna användargrupper.</p> <p> I en [!UICONTROL Group]-rapport visar det här fältet namnen på de användare som har angetts som [!UICONTROL Group Administrators] i gruppen. Mer information om gruppadministratörer finns i <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppadministratörer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Group with Administration Access]</td> 
   <td> <p> I ett [!UICONTROL Layout Template], [!UICONTROL Timesheet Profile] eller [!UICONTROL Schedule report] visar det här fältet de grupper vars gruppadministratörer har behörighet att ändra mallen. Du kan även filtrera den här rapporten efter det här fältet. </p> <p> Mer information finns i <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Skapa och hantera layoutmallar</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Grouping]</td> 
   <td> <p>Ett rapportelement som används för att kategorisera information i en lista enligt ett gemensamt kriterium.</p> <p>Mer information finns i avsnittet [!UICONTROL Groupings] i artikeln <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Rapportera element: filter, vyer och grupperingar</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Handoff Date]</td> 
   <td> <p>Det datum då en uppgift blir tillgänglig för arbete. [!UICONTROL Handoff Date] är en beräkning och kan inte anges manuellt. <br>Mer information om [!UICONTROL Handoff Date] finns i artikeln <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">[!UICONTROL Task Handoff Date] översikt</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Help Desk]</td> 
   <td>Ett alternativt namn som beskriver [!UICONTROL Requests]-området för [!DNL Workfront]. Du kan använda området [!UICONTROL Requests] för att bearbeta kundsupportärenden, projektförfrågningar, helpdesk-biljetter osv.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Owner]</td> 
   <td>I en [!UICONTROL Hour]-rapport är [!UICONTROL Owner] den användare som timmarna har tilldelats. Detta skiljer sig från användaren som faktiskt loggar tiden. Dessa två enheter kan ibland vara två olika användare. <br>Mer information om loggningstid för en annan användare finns i artikeln <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Loggtid</a>.</td> 
  </tr>

<tr> 
   <td>Timstatus</td> 
   <td> <p>Ett attribut som anges av Workfront för de faktiska timmar som användare loggar efter uppgifter, ärenden eller projekt. </p>

Timposter kan ha någon av följande statusvärden i Workfront:
<ul>
   <li><b>Skickat</b>: Timmarna har loggats på ett projekt, en uppgift eller ett problem. De ingår antingen i en faktureringspost eller har inte lagts till i en faktureringspost än.</li>
   <li><b>Godkänd</b>: Timmarna har loggats och de har godkänts av projektägaren. De ingår antingen i en faktureringspost eller har inte lagts till i en faktureringspost än.</li> 
   <li><b>Inte godkänt</b>: Timmarna har loggats och avvisats av projektägaren. De ingår antingen i en faktureringspost eller har inte lagts till i en faktureringspost än.</li>
   <li><b>Fakturerad</b>: timmarna har loggats, lagts till i en faktureringspost och faktureringspostens status har markerats som Fakturerad. De behövde inte godkännas av projektägaren.</li>
   <li><b>Fakturerad och godkänd</b>: timmarna har loggats, godkänts av projektägaren och faktureringspostens status har markerats som Fakturerad.</li>
   </ul>


<p>När timmar är en del av en faktureringspost visar timstatusen om timarna har godkänts eller om faktureringsposten de tillhör har fakturerats. Timstatus för en timpost visas bara i en timlista eller rapport. </p>

<p>Mer information om hur du lägger till timmar i faktureringsposter finns i avsnittet Lägg till timmar i faktureringsposter i artikeln <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Skapa faktureringsposter</a>.</p>

<p>Mer information om att godkänna tid för projekt finns i <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >Kräv tid för att godkännas för ett projekt</a>.</p>

<p><b>TIPS</b></p>

<p>Allmänna timmar som inte loggas direkt på arbetsobjekt visar inte timstatus. </p> </td> 
  </tr>



<tr> 
   <td>[!UICONTROL Hour Type]</td> 
   <td> <p>An attribute that can be set for Actual Hours that users log for tasks, issues, or projects. Det här är också ett attribut för loggade timmar som inte är direkt länkade till arbetet, till exempel [!UICONTROL Vacation] och [!UICONTROL Time Off].</p> <p>Mer information finns i <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">Hantera timtyper</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>ID:t är en alfanumerisk indikator som är associerad med alla objekt i [!DNL Workfront]. Det identifierar varje objekt i databasen [!DNL Workfront] unikt. Du kan visa ID:t för alla objekt i en rapport eller en lista för varje objekt. </p> <p><b>TIPS</b></p>   <p>Du kan även visa ID:t i URL:en för objektets sida. Ett projekts-ID kan till exempel se ut ungefär som det nummer som anges på följande URL när du öppnar sidan [!UICONTROL Project Details]:</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Individual Goals]</td> 
   <td>Individuella mål som bidrar till mätvärdena för teamets mål, men som inte är relaterade till personlig utveckling eller karriärutveckling.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Inherited Access]</td> 
   <td>Delningsfunktion som tillåter åtkomst att sprida objekt från objekt till andra. Projektanvändarens ärvda åtkomst som definierats i program- och portföljposter.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Initiative]</td> 
   <td> <p>I [!DNL Workfront Scenario Planner] kan du dela in en plan i flera initiativ för att göra det enklare att hantera planen. <span>Du kan skapa en [!UICONTROL Initiative]-rapport och du kan komma åt [!UICONTROL Initiative] information i en [!UICONTROL Project]-rapport.</span></p> <p>[!DNL Scenario Planner] kräver ytterligare en licens. Mer information om [!DNL Workfront Scenario Planner] finns i <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Översikt [!DNL Scenario Planner]</a>. </p> <p>[!DNL Initiative]-rapporten visas inte i din [!DNL Workfront]-instans om inte ditt företag har köpt en [!DNL Workfront Scenario Planner]-licens. Du kan inte komma åt [!UICONTROL Initiatives] via API:t.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role]</span> </td> 
   <td> <p><span>Rapporttypen [!UICONTROL Initiative Job Role] visar information om de jobbroller som är associerade med ett planinitiativ i [!DNL Workfront Scenario Planner].</span> </p> <p>[!DNL Scenario Planner] kräver ytterligare en licens. Mer information om [!DNL Workfront Scenario Planner] finns i <a href="../../../scenario-planner/scenario-planner-overview.md">Översikt [!DNL Scenario Planner]</a>. </p> <p><span>Den här rapporttypen visas inte i din [!DNL Workfront]-instans om inte företaget har köpt en [!DNL Workfront Scenario Planner]-licens.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role Hours]</span> </td> 
   <td> <p><span> I en [!UICONTROL Initiative Job Role]-rapport visar detta antalet timmar som är associerade med en jobbroll i ett initiativ.</span> </p> <p>[!DNL Scenario Planner] kräver ytterligare en licens. Mer information om [!DNL Workfront Scenario Planner] finns i <a href="../../../scenario-planner/scenario-planner-overview.md">Översikt [!DNL Scenario Planner]</a>. </p> <p>Det här fältet och rapporttypen [!UICONTROL Initiative Job Role] visas inte i din [!DNL Workfront]-instans om inte företaget har köpt en [!DNL Workfront Scenario Planner]-licens.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Job Role Count]</td> 
   <td> <p>I en [!UICONTROL Initiative Job Role]-rapport visas antalet specifika jobbroller som är associerade med ett initiativ.</p> <p>[!DNL Scenario Planner] kräver ytterligare en licens. Mer information om [!DNL Workfront Scenario Planner] finns i <a href="../../../scenario-planner/scenario-planner-overview.md">Översikt [!DNL Scenario Planner]</a>. </p> <p>Det här fältet och rapporttypen [!UICONTROL Initiative Job Role] visas inte i din [!DNL Workfront]-instans om inte företaget har köpt en [!DNL Workfront Scenario Planner]-licens.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Last Published Date]</td> 
   <td> <p>Ett fält i en [!UICONTROL Initiative]-, [!UICONTROL Initiative Job Role]- och [!UICONTROL Project]-rapport som visar datumet då ett planinitiativ senast publicerades i ett projekt. Du kan publicera initiativ för att skapa projekt eller för att uppdatera projekt som är kopplade till initiativen.</p> <p>[!DNL Scenario Planner] kräver ytterligare en licens. Mer information om [!DNL Workfront Scenario Planner] finns i <a href="../../../scenario-planner/scenario-planner-overview.md">Översikt [!DNL Scenario Planner]</a>. </p> <p><span>Mer information om publiceringsinitiativ finns i </span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">Publish-scenarier för att skapa och uppdatera projekt i [!DNL Workfront Scenario Planner]</a>. Det här fältet visas inte i din [!DNL Workfront]-instans om inte företaget har köpt en [!DNL Workfront Scenario Planner]-licens.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Inline Search]</td> 
   <td>En sökning som utförs när ett formulär fylls i för att hitta möjliga poster för ett specifikt fält.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interface Setup]</td> 
   <td>Det område i programmet där du kan definiera anpassade vyer, filter, grupperingar, listkontroller osv.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Is Company Goal]</p></td> 
   <td> <p>I [!DNL goal reports] visas värdet [!UICONTROL True]/ [!UICONTROL False] för varje strategiskt mål för att ange om din organisation har tilldelats målet som ägare. </p> 
   <p>Det här fältet visas bara om din organisation har köpt [!DNL Workfront Goals]. Mer information om hur du hanterar strategiska mål med [!DNL Workfront Goals] finns i <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] översikt </a>.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue]</td> 
   <td> <p>En oplanerad arbetsuppgift som vanligtvis anger att det finns ett problem som förhindrar slutförande av en uppgift eller ett projekt. Planen har trimmats och utvärderats för vidare arbetsinsats</p> <p>En [!UICONTROL Issue] kan också vara en [!UICONTROL Help Desk]-begäran. [!UICONTROL Change Orders], [!UICONTROL Requests] och [!UICONTROL Bugs] är också [!UICONTROL Issues].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue Management]</td> 
   <td> <p>Processen och reglerna som styr definitionen av problemtyp och den routnings-, resage- eller trafikprocess som är kopplad till varje typ.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue Owner]</td> 
   <td>Det eller de team som ansvarar för att testa och slutföra ett problem.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Iteration]</td> 
   <td>En tidsperiod under vilken ett team producerar en fördefinierad uppsättning slutprodukter.</td> 
  </tr> 
 </tbody> 
</table>

## J - L

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objektnamn</th> 
   <th>Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Job Role]</td> 
   <td> <p>Används för att identifiera en användares dagliga arbetsuppgifter. Jobbroller kan tilldelas till arbetsuppgifter för att identifiera den kompetens som krävs för att slutföra en arbetsprocess utan att tilldela den till en viss användare. </p> <p>En användare kan ha mer än en roll. Exempel är Graphic Designer eller Consultant.</p> <p>Mer information finns i <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Skapa och hantera jobbroller</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Journal Entry]</p> </td> 
   <td> <p>Ett objekt som kan rapporteras och som ger dig information om systemuppdateringar för spårade fält som visas i området [!UICONTROL Updates] med projekt, uppgifter, problem och andra objekt.</p> <p>Mer information finns i <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">Rapport om [!UICONTROL Updates]-området</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kanban Flag]</td> 
   <td> <p>I en [!UICONTROL Task]-rapport eller [!UICONTROL Issue]-rapport visar fältet [!UICONTROL Kanban Flag] flaggstatusen som angetts för artikeln på [!UICONTROL Kanban board]. Möjliga värden är [!UICONTROL On Track], [!UICONTROL Ready to Pull] och [!UICONTROL Is Blocked].</p> <p>Mer information om hur du anger flaggstatus för artiklar på [!UICONTROL Kanban story board] finns i  artikeln <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref"> Använd flaggor på artiklar på [!UICONTROL Kanban board]</a> .</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPI:er</td> 
   <td>Ett mätbart värde som visar hur effektivt ett företag uppnår viktiga affärsmål.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag]</td> 
   <td>Den tid som måste gå efter att föregående uppgifts [!UICONTROL Planned Completion Date] har passerat tills den beroende aktiviteten kan börja.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag Types]</td> 
   <td> <p>Metoden för att beräkna [!UICONTROL Lag]. Den kan vara:</p> 
    <ul> 
     <li>[!UICONTROL Days] (arbetsdagar)</li> 
     <li>[!UICONTROL Calendar Days] (ignorera helger)</li> 
     <li>[!UICONTROL Percent]</li> 
     <li>[!UICONTROL Day of Week]</li> 
    </ul> <p>Mer information finns i <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">Översikt över fördröjda typer</a>.</p> </td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Large Thumbnail]</td> 
   <td> <p> I en [!UICONTROL Document]-lista eller -rapport visas en förhandsgranskning av dokumentet i en miniatyrbild. </p> <p>Välj <strong>[!UICONTROL Large Thumbnail]</strong> om du vill visa en miniatyrbild som är 400 pixlar bred i rapporten.</p> <p>Storleken på miniatyrbilden justeras när du ändrar bredden på kolumnen i en lista eller rapport.</p> <p>Se även [!UICONTROL Thumbnail] i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last 10 Viewers]</td> 
   <td> <p>I en rapportlista visar det här fältet namnen på upp till 10 användare som har visat rapporten senast.<br>Mer information om användningsinformation i rapportlistor finns i artikeln <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visa rapportanvändning</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Condition Note]</td> 
   <td> <p>I det här fältet visas den uppdatering som senast angavs för ett objekt av objektets ägare. Detta är ägarens senaste aktivitet eller interaktion för ett objekt.</p> <p>Kolumnen [!DNL Last Condition Note] är tom om anteckningstexten för den sista anteckningen i ett objekt har tagits bort. När en ny anteckning läggs in på objektet blir den sista anteckningen och visas igen i kolumnen. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Finance Update Date]</td> 
   <td>I en [!UICONTROL project]-rapport hämtar det här fältet datum och tid när projektets ekonomi senast beräknades och uppdaterades. Mer information om projektets ekonomi finns i <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">Översikt över projektets ekonomi</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Note]</td> 
   <td> <p>I det här fältet visas den senaste uppdateringen som en användare har angett för ett objekt. Detta är den senaste aktiviteten eller interaktionen för ett objekt.</p> <p>Kolumnen [!UICONTROL Last Note] är tom om texten i den sista anteckningen i ett objekt har tagits bort. När en ny anteckning läggs in på objektet blir den sista anteckningen och visas igen i kolumnen.</p>
   <p>När det här fältet läggs till i en [!UICONTROL Task]-rapport finns det eventuella uppdateringar kvar på underordnade objekt, till exempel problem, underaktiviteter, dokument osv. — av uppgiften visas inte i den här kolumnen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Viewed By]</td> 
   <td> <p>I en rapportlista visar det här fältet information om användaren som senast visade rapporten.<br>Mer information om användningsinformation i rapportlistor finns i artikeln <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visa rapportanvändning</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Viewed Date]</td> 
   <td> <p>I en rapportlista visar det här fältet det datum då rapporten senast visades.<br>Mer information om användningsinformation i rapportlistor finns i artikeln <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visa rapportanvändning</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Layout Template]</td> 
   <td>Definieras av systemadministratören eller gruppadministratören för att identifiera flikarna och rapporterna som visas på en viss användares arbetsyta.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Layout Type]</td> 
   <td>I kombination med [!UICONTROL Custom Views] anger [!UICONTROL Layout Type] typen av [!UICONTROL Custom View]. För närvarande är bara List tillgängligt. I framtiden kan [!UICONTROL Detail] (vyn [!UICONTROL Detail] för ett objekt) bli tillgänglig.</td> 
  </tr> 
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Cost</i>. </p> </td> 
  </tr>
  --> 
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Hours</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Hours</i>. </p> <p>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        This field shows the number of hours budgeted for the project in the Legacy Resource Estimates area of the Business Case or in the Capacity Planner. 
       <br>If there&nbsp;are multiple job roles, this is a summary of the budgeted hours for all job roles. The Legacy Budgeted Hours are calculated after you have used the "Set budget to schedule" feature, or after you have defined how many of the Planned Hours should be budgeted, in the Resource Estimates area of the Business Case of the project or in the Capacity Planner.&nbsp; 
     </p> </td> </tr> -->
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Labor Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> <p>The field is still visible in some reports and lists. </p> <p>See <i>Budgeted Labor Cost</i>. </p> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In a project report, this field shows the labor cost associated with the project, taking into account the Cost per Hour rate of every job role and the amount of Legacy Budgeted Hours estimated in the Legacy Resource Estimates area of the Business Case that is needed for each role to complete the project.&nbsp;</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Legacy Budgeted Labor Cost in a project report is calculated using the following formula:</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code style="font-style: normal;">Legacy Budgeted Labor Cost = SUM(Job Role Cost per Hour * Legacy Budgeted Hours per Job Role)</code> </p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating Legacy Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>&nbsp;&nbsp;</p>
    --> </td> 
  </tr> 
  <tr> 
   <!-- <td>Legacy Resource Pool</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> 
   <p>Although not recommended, you may update the information in this report using the API.</p> 
   <p>See <i>Resource Pools</i> for updated fields. </p> 
   <p>The Legacy Resource Pool is a collection&nbsp;of job roles associated with a project or a user. The functionality of the Legacy Resource Pools is displayed in the tools available in the Legacy Resource Planning tab of the People area. This is a deprecated field.</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Library Task]</td> 
   <td>En mall för en enskild aktivitet som används för att ge konsekvent namngivning av [!UICONTROL Tasks] och [!UICONTROL Template Tasks] i hela programmet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Type]</td> 
   <td>Den typ av licens som tilldelats en [!UICONTROL Access Level]. Det är antingen [!UICONTROL Full User], [!UICONTROL Limited User] eller [!UICONTROL Requester].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Limit Plan]</td> 
   <td> <p>I en [!UICONTROL Group]-vy eller rapport visar det här fältet det maximala antalet [!UICONTROL Plan] licenser som kan tilldelas användare som har respektive grupp angiven som [!UICONTROL Home Group].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Limit Work]</td> 
   <td> <p>I en [!UICONTROL Group]-vy eller rapport visar det här fältet det maximala antalet [!UICONTROL Work] licenser som kan tilldelas användare som har respektive grupp angiven som [!UICONTROL Home Group].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limited User]</td> 
   <td>En licenstyp som gör att du kan skapa en [!DNL Access Level] som innehåller skrivskyddade behörigheter, med möjlighet att skicka utgåvor, göra anteckningar och överföra dokument.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL List Controls]</td> 
   <td> <p>En del av [!UICONTROL Interface Setup] som tillåter länkning av anpassade filter, vyer och grupperingar till enskilda användare eller globalt till alla användare.</p> </td> 
  </tr> 
 </tbody> 
</table>

## M - O

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objektnamn</th> 
   <th>Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Manual Only]</td> 
   <td> <p>En av [!UICONTROL Update Types] för [!UICONTROL Project]. Med den här inställningen kan [!UICONTROL Project Projected]- och [!UICONTROL Planned]-tidslinjer bara uppdateras när användaren klickar på [!UICONTROL Recalculated Timelines]. Projekt som har konfigurerats på det här sättet ignoreras under den nattliga omberäkningen och när projektet eller aktiviteterna i projektet uppdateras.</p> <p>Mer information finns i <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Markera projektet [!UICONTROL Update Type] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Me]</td> 
   <td> <p>Detta avser den inloggade användaren. </p> <p>Vi rekommenderar att du använder det här fältet i ett filter för att göra rapporter mer allmänna när du delar dem med andra användare. På så sätt kan du bara skapa en rapport som visar olika information beroende på vem som loggar in för att visa den, eftersom informationen alltid anpassas för den inloggade användaren. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Max Users]</td> 
   <td> <p>Detta är ett inaktuellt fält. All information som det här fältet kan visa är relaterad till en funktion som [!DNL Workfront] har tagit bort och fältet kan inte uppdateras. </p> <p>I tidigare versioner av [!DNL Workfront] kunde du uppdatera det här fältet när du skapade eller redigerade en jobbroll. Det visade det totala antalet användare som kan associeras med en roll i varje projekt. Värdet noll tillåts för ett obegränsat antal användare som kan tilldelas i ett projekt. </p>Fältet är fortfarande synligt i vissa rapporter och listor, men den information som visas kan inte uppdateras. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Milestone]</td> 
   <td> <p>En markör som du kan associera med en uppgift för att ange att en nyckelpunkt i projektet har uppnåtts när uppgiften har slutförts. Vanligtvis kan du använda milstolpar för att visa en viktig händelse, som slutförandet av en fas i projektet eller en uppsättning kritiska aktiviteter. [!UICONTROL Milestones] är vanligtvis associerade med överordnade uppgifter. Du måste skapa milstolparna innan du kan koppla dem till uppgifter. Mer information om milstolpar finns i <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">Skapa en milstolpe-sökväg</a> och <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">Associera milstolpar med aktiviteter</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Milestone Path]</td> 
   <td>En samling med [!UICONTROL milestones]. [!UICONTROL Milestone Paths] används i projekt för att skilja projekt med vissa typer av [!UICONTROL Milestones] från projekt med en annan uppsättning [!UICONTROL Milestones].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Milestone Task]</td> 
   <td>En aktivitet som flaggats för att indikera en rapporterbar händelse att mäta.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Module]</td> 
   <td>Ett steg i ett scenario i [!DNL Workfront Fusion] som utför en funktion baserat på den associerade appen.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL My Primary Role]</td> 
   <td> <p>När det refereras till detta i filter visas antingen användare som har samma [!UICONTROL Primary Role] som den inloggade användaren, eller arbetsobjekt som tilldelats [!UICONTROL Primary Role] för den inloggade användaren.</p> <p>Vi rekommenderar att du använder det här fältet i ett filter för att göra rapporter mer allmänna när du delar dem med andra användare. På så sätt kan du bara skapa en rapport som visar olika information beroende på vem som loggar in för att visa den, eftersom informationen alltid anpassas för den inloggade användaren. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL My Home Team]</td> 
   <td> <p>När det refereras till detta i filter, visas antingen användare som tillhör [!UICONTROL Home Team] för den inloggade användaren, eller arbetsobjekt som tilldelats [!UICONTROL Home Team] för den inloggade användaren. </p> <p>Vi rekommenderar att du använder det här fältet i ett filter för att göra rapporter mer allmänna när du delar dem med andra användare. På så sätt kan du bara skapa en rapport som visar olika information beroende på vem som loggar in för att visa den, eftersom informationen alltid anpassas för den inloggade användaren. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Naming convention]</td> 
   <td>En uppsättning regler för hela organisationen som använder data för att skapa namn på projekt, uppgifter och slutprodukter.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Native Integration]</td> 
   <td>En integrering som inte kräver någon manuell kodning eller API-konfiguration. Kallas även"färdig" integrering.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Navigation Menu]</td> 
   <td>Den översta mittenpanelen i programmet som har länkar till huvudområden i [!UICONTROL Workfront].</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[!UICONTROL New Number Value]</td> 
   <td>I en [!UICONTROL Journal Entry]-rapport visas det uppdaterade värdet för ett fält som ersätter [!UICONTROL Old Number Value].
   Mer information finns i [!UICONTROL Old Number Value] i den här artikeln.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Non-Billable Expense]</td> 
   <td> <p>En utgift som inte är markerad som fakturerbar för kunden. Detta kan vara antingen en planerad utgift eller en faktisk utgift.</p> <p>Fälten Planerad icke-fakturerbar kostnad och Faktisk icke-fakturerbar kostnad är tillgängliga så att du kan lägga till i vyer och rapporter. De visas inte på projekt- eller uppgiftsinformationssidorna.</p>
   <p>Du hittar dessa fält i följande typer av rapporter:</p>
   <ul>
   <li>Baslinje</li>
   <li>Mall</li>
   <li>Projekt (ekonomiska data)</li>
   </ul>
   <p>Mer information om hur du markerar en utgift som fakturerbar finns i <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">Hantera projektutgifter</a>.</p>
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Non Work Day]</td> 
   <td>En dag som inte har allokerats till slutförande av tilldelningar. Det här är vanligtvis en semesterdag, semester eller helg. Termen visas i API-utforskaren. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Note]</td> 
   <td>En kommentar eller uppdatering har gjorts för ett [!DNL Workfront]-objekt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Note Text]</td> 
   <td> <p>Här visas texten för en uppdatering som har angetts av en användare för ett objekt. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Number of Linked Goals]</td> 
   <td> <p>I en [!UICONTROL Project]-rapport är detta antalet strategiska mål som är associerade med projektet. Mer information om hur du associerar projekt med strategiska mål finns i <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Lägg till projekt i mål i [!DNL Adobe Workfront Goals]</a>.</p> 
   <p>Mer information om strategiska mål finns i [!UICONTROL Goal] i den här artikeln.</p> 
   <p>Det här fältet visas bara om din organisation har köpt [!DNL Workfront Goals]. Mer information om hur du hanterar strategiska mål med [!DNL Workfront Goals] finns i <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Lägg till projekt i mål i [!UICONTROL Adobe Workfront Goals]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Object]</td> 
   <td> <p>Den information du visar i [!DNL Adobe Workfront] representeras av objekt som lagras i databasen [!DNL Workfront]. Objekten är vad som driver informationen i Workfront. Några exempel på objekt är:</p> 
    <ul> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programs]</li> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>[!UICONTROL Reports]</li> 
     <li>[!UICONTROL Groups]</li> 
     <li>[!UICONTROL Teams]</li> 
     <li>[!UICONTROL Users]</li> 
     <li>[!UICONTROL Companies]</li> 
     <li>[!UICONTROL Custom forms]</li>
     <li>[!UICONTROL Custom fields]</li>  
     <li>[!UICONTROL Hours]</li> 
     <li>[!UICONTROL Billing Rates]</li> 
     <li>[!UICONTROL Templates]</li> 
     <li>[!UICONTROL Template tasks]</li>

<p><b>ANMÄRKNING</b></p>
  <p>Det här är inte en omfattande lista. </p>

</ul> <p>Mer information finns i <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Förstå objekt i [!UICONTROL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Object Types]</td> 
   <td>Om du skapar en rapport eller lista som innehåller alla dina anpassade formulär kan du använda det här fältet som en vy eller ett filter för att se vilka objekttyper som är kopplade till respektive formulär. </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL Old Number Value]</td> 
   <td>I en [!UICONTROL Journal Entry]-rapport visar detta det ursprungliga värdet för ett fält innan det uppdaterades. När ett fälts värde har uppdaterats visas det som [!UICONTROL New Number Value] i en [!UICONTROL Journal Entry]-rapport. Mer information finns också i [!UICONTROL New Number Value].</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL On Change Only]</td> 
   <td> <p>En av [!UICONTROL Project Update]-typerna. När det här alternativet är markerat uppdateras tidslinjerna [!UICONTROL Project Projected] och [!UICONTROL Planned] endast när en uppdatering eller ändring görs i projektet eller i en aktivitet i projektet. Det uppdaterar inte projektet varje kväll.</p> <p>Mer information finns i <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Välj projekttypens uppdateringstyp </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Op Task]</td> 
   <td> <p>Namnet på [!UICONTROL Issue] i databasen [!DNL Workfront], som används i textlägesrapporter eller beräknade anpassade data.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Open]</td> 
   <td>Ett problem eller en uppgift som inte är fullständig, men som du arbetar med.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Org Chart]</td> 
   <td>Kort för organisationsschemat. Det här är ett diagram som visar hierarkin i en organisation. Det finns också på fliken på [!UICONTROL User]-detaljskärmen som visar och tillåter inställning av [!UICONTROL Company]- och [!UICONTROL Reporting]-relationer för [!UICONTROL User].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Organizational Setup]</td> 
   <td>Detta definierar [!UICONTROL Companies], [!UICONTROL Groups] och [!UICONTROL Security Profiles] för din organisation.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Other Groups]</td> 
   <td> <p>I en rapport eller vy som listar användare, visar det här fältet alla grupper där varje användare är medlem. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency]</span> </td> 
   <td> 
    <div> 
     <p>I en [!UICONTROL Job Role]-rapport är detta den valuta som är associerad med en jobbroll. Det är en åsidosättning av [!UICONTROL Base Currency] som upprättats i området [!UICONTROL Setup] av administratören [!DNL Workfront]. </p> 
     <p>Mer information finns i <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Skapa och hantera jobbroller</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency Billing/ Hour]</span> </td> 
   <td> 
    <div> 
     <p>I en [!UICONTROL Job Role]-rapport är det här faktureringshastigheten per timme för jobbrollen som använder den valda [!UICONTROL Override Currency] för jobbrollen.</p> 
     <p> Mer information finns i <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Skapa och hantera jobbroller</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency Cost/ Hour]</span> </td> 
   <td> 
    <div> 
     <p>I en [!UICONTROL Job Role]-rapport är detta kostnaden per timma för jobbrollen med den valda [!UICONTROL Override Currency] för jobbrollen. </p> 
     <p>Mer information finns i <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Skapa och hantera jobbroller</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Owner]</td> 
   <td>Den användare som ansvarar för slutförandet av det angivna objektet.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Owner Type]</span> </td> 
   <td> 
    <div> 
     <p>I en [!UICONTROL Goal]-rapport visas den typ av ägare som har tilldelats ett strategiskt mål. Följande typer är målägare:</p> 
     <ul> 
      <li> <p>[!UICONTROL User]</p> </li> 
      <li> <p>[!UICONTROL Team] </p> </li> 
      <li> <p>[!UICONTROL Group]</p> </li> 
     </ul> 
     <p>Inget värde visas i det här fältet när målägaren är din organisation. </p> 
     <p>Detta kräver ytterligare en licens. Mer information om [!DNL Workfront Goals] finns i <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] översikt</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## P - R

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objektnamn</th> 
   <th>Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Parameter]</td> 
   <td> <p>Ett [!UICONTROL parameter] är ett anpassat fält. Du kan skapa en rapport för alla parametrar eller anpassade fält i systemet. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent]</td> 
   <td>I en rapport visar det här fältet information om objektets överordnade objekt. I till exempel en [!UICONTROL issue]-rapport kan den visa information om aktiviteten eller projektet som problemet är loggat under. I en aktivitetsrapport kan den visa information om den direkta överordnade aktiviteten eller om projektet. Mer information om vilka objekt som kan ha överordnade objekt i [!DNL Workfront] finns i avsnittet"Objektens inbördes beroende och hierarki" i artikeln <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Förstå objekt i [!DNL Adobe Workfront]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent Lag]</td> 
   <td>Den tid som måste gå mellan [!UICONTROL Parent Task]-starten och [!UICONTROL Subtask]-starten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent Task]</td> 
   <td>Kallas även [!UICONTROL Summary Task]. Det här är en aktivitet som har underaktiviteter (kallas även [!UICONTROL Children Tasks]). [!UICONTROL Duration], [!UICONTROL Work Required] och [!UICONTROL Percent Complete] för den överordnade aktiviteten beräknas från underaktiviteterna.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Part-Time Resources]</td> 
   <td>En licensierad användare som har mindre kapacitet än standardschemat som definierats i systemet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Percent Complete]</td> 
   <td> <p>Ett projekt-, uppgifts- eller utleveransfält som visar hur stor procentandel av arbetet som är associerat med uppgiften, projektet eller utgåvan som har slutförts.</p> <p>Du kan uppdatera det här fältet manuellt för problem och arbetsuppgifter. </p> <p>För projekt och överordnade uppgifter är det här fältet en sammanslagning av alla arbetsuppgifter och du kan inte uppdatera det manuellt. </p> <p>Mer information finns i <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">Projekt [!UICONTROL Percent Complete] - översikt</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permission]</td> 
   <td> <p>Rättigheter som ges till en användare på ett objekt, vanligtvis givna så att de kan slutföra arbetet med objektet eller visa objektet. Du kan ge behörighet till:</p> 
    <ul> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programs]</li> 
     <li>[!UICONTROL Reports]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Custom Forms]</li> 
     <li>[!UICONTROL Views]</li> 
     <li>[!UICONTROL Filters]</li> 
     <li>[!UICONTROL Groupings]</li> 
    </ul> <p>Mer information finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Översikt över delningsbehörigheter för objekt</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan]</td> 
   <td> <p>Det här är en fullständig licenstyp i systemet [!DNL Workfront]. Användarna måste ha den här för att få tillgång till alla funktioner i [!DNL Workfront].</p> <p>Mer information finns i <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] licensöversikt</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan] (i [!DNL Scenario Planner])</td> 
   <td> <p>En plan är huvudobjektet när du arbetar med [!DNL Workfront]-scenarioplanen. Du kan ange strategin för ditt företags närmaste och långsiktiga framtid och identifiera varje resultat på hög nivå och lägga till den som en plan i [!DNL Workfront]-scenarioplanen. </p> <p>Du kan inte visa [!DNL Scenario Planner]-planer i en rapport och du kan inte komma åt dem via API:t [!DNL Workfront]. </p> <p>[!DNL Scenario Planner] kräver ytterligare en licens. Mer information om [!DNL Workfront Scenario Planner] finns i <a href="../../../scenario-planner/scenario-planner-overview.md">Översikt [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned]</td> 
   <td> <p>Den tidsperiod inom vilken något är planerat att inträffa. När du skapar projekt, aktiviteter eller utgåvor i [!DNL Workfront] måste du fastställa de planerade start- och slutdatumen samt den planerade tidsram under vilken de inträffar. Dessa värden representerar din ursprungliga avsikt eller uppskattning av hur lång tid det tar att slutföra en artikel. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Benefit]</td> 
   <td>Det här är en manuell inmatning som projektledaren kan göra för att bedöma om ett projekt skulle medföra någon ekonomisk fördel för organisationen. Att ange det här värdet kan vara en del av att sätta ihop en [!UICONTROL Business Case] för projektet. Du måste ha [!UICONTROL Manage] behörigheter för projektet för att uppdatera det här värdet.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Planned Budgeted Hours]</td> 
   <td> <p>I en [!UICONTROL Budgeted Hour]-rapport visar detta antalet timmar som budgeterats för projekt eller [!UICONTROL Job Roles] i [!UICONTROL Resource Planner]. </p> <p>Mer information om budgeteringsprojekt eller roller i [!UICONTROL Resource Planner] finns i artikeln <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budgetresurser i [!UICONTROL Resource Planner] med hjälp av vyerna [!UICONTROL Project] och [!UICONTROL Role]</a>. Mer information om rapporten [!UICONTROL Budgeted Hours] finns i artikeln <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Rapport: Budgeterad timme</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Completion Date]</td> 
   <td> <p>Du kan ställa in [!UICONTROL Planned Completion Date] manuellt till ett valfritt datum. Om du inte anger [!UICONTROL Planned Completion Date] anges den automatiskt i [!DNL Workfront]. När den anges automatiskt är [!UICONTROL Planned Completion Date]: [!UICONTROL Planned Start Date] + [!UICONTROL Duration]</p> <p>Mer information finns i följande artiklar:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Översikt över aktiviteten [!UICONTROL Planned Completion Date]</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Ange projektet [!UICONTROL Planned Completion Date]</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Cost]</td> 
   <td> <p>Totalt för [!UICONTROL Planned Labor Cost] och [!UICONTROL Planned Expense Cost] för projektet. Detta inkluderar inte [!UICONTROL Planned Risk Cost] i projektet.  </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Duration]</td> 
   <td> <p>En uppgifts [!UICONTROL Planned Duration] är vanligtvis densamma som aktivitetens [!UICONTROL Duration]. Det representerar skillnaden i dagar mellan [!UICONTROL Planned Start] och [!UICONTROL Planned Completion Dates] för aktiviteten. </p> <p>När aktiviteten har typen [!UICONTROL Duration] av [!UICONTROL Effort Driven] kan [!UICONTROL Planned Duration] skilja sig från [!UICONTROL Duration] för aktiviteten, baserat på hur många resurser du tilldelar uppgiften. </p> <p>Om en aktivitet med typen [!UICONTROL Duration] av [!UICONTROL Effort Driven] till exempel har [!UICONTROL Duration] på 3 dagar och du tilldelar en resurs med ett heltidsschema till aktiviteten, är även [!UICONTROL Planned Duration] 3 dagar. Om du tilldelar tre resurser med ett heltidsschema till samma uppgift stannar [!UICONTROL Duration] kvar i tre dagar, men [!UICONTROL Planned Duration] blir en dag. [!UICONTROL Planned Duration] ändrar också [!UICONTROL Planned Start]- och [!UICONTROL Planned Completion]-datumen för aktiviteten så att de återspeglar den nya [!UICONTROL Planned Duration]. Därför påverkas även tidslinjen i projektet. </p> <p>Mer information om skillnaden mellan [!UICONTROL Duration] och [!UICONTROL Planned Duration] för uppgifter finns i artikeln <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref"> Skillnad mellan [!UICONTROL Planned Duration] och [!UICONTROL Duration] för uppgifter </a>.</p> <p>Projekt och ärenden har inte en [!UICONTROL Planned Duration]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Duration Minutes]</td> 
   <td> <p>[!UICONTROL Planned Duration Minutes] för ett projekt eller en utgåva är [!UICONTROL Duration] för projektet eller utgåvan på några minuter. </p> <p>Aktiviteter har inget [!UICONTROL Planned Duration Minutes]-fält. </p> <p>[!UICONTROL Template Tasks] har ett [!UICONTROL Planned Duration Minutes]-fält som visar [!UICONTROL Planned Duration] för aktiviteten i minuter. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Expense Cost]</td> 
   <td> <p>Summan av [!UICONTROL Planned Amounts] för alla utgifter som loggats för ett projekt eller en uppgift.</p> <p><b>EXEMPEL</b></p>
   <p>Om du skapar en utgift för Uppgift 1 och anger 600,00 USD i fältet [!UICONTROL Planned Amount], är [!UICONTROL Planned Expense Cost] för den här aktiviteten 600,00 USD. </p> 
   <p>För ett projekt använder [!DNL Workfront] följande formel för att beräkna [!UICONTROL Planned Expense Cost]:</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Hours]</td> 
   <td> <p>Det här fältet visas i [!UICONTROL projects]-, [!UICONTROL tasks]- och problemområdena, rapporter för projekt, uppgifter eller problem samt resurshanteringsverktyg som [!UICONTROL Resource Planner]-, [!UICONTROL Workload Balancer]- och [!UICONTROL Utilization]-rapporten. </p> <p>Den visar hur många timmar projektägaren uppskattar att varje uppgift eller problem ska ta att slutföra. För projekt är det vanligtvis en sammanslagning av [!UICONTROL Planned Hours] från aktiviteterna i projektet. </p> <p>Fältet [!UICONTROL Planned Hours] kan visa olika information beroende på varifrån du visar den. Mer information om planerade timmar finns i <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Översikt över planerade timmar</a>.</p> <p>Planerade timmar lagras i minuter i databasen [!DNL Workfront]. När du skriver beräkningar med det här fältet måste du ta hänsyn till att timmarna visas som minuter.<br></p> <p>Som standard fördelas Planerade timmar jämnt till alla dagar under en arbetsuppgifts varaktighet och även till alla resurser som tilldelats uppgiften. Användare kan uppdatera det dagliga antalet planerade timmar för en arbetsuppgift eller de enskilda planerade timmarna för varje tilldelad.</p> <p>Det här fältet uppdateras inte för projekt, uppgifter och problem: </p> 
    <ul> 
     <li> <p>För problem kan du uppdatera det här fältet manuellt. Planerade timmar för utleverans läggs inte till i projektplanerade timmar. </p> <p><b>TIPS</b></p> <p>I en problemrapport ersätts ett av [!UICONTROL Planned Hours]-fälten med fältet [!UICONTROL Work]. I fältet visas antalet planerade timmar för problemet. Mer information finns i fälten "work" och "[!UICONTROL Work]" i den här tabellen. </p> </li> 
    </ul> 
    <ul> 
     <li> <p>För uppgifter kan du uppdatera det här fältet manuellt när [!UICONTROL Duration Type] för uppgiften är [!UICONTROL Calculated Assignment] eller [!UICONTROL Simple]. Det här fältet beräknas av [!DNL Workfront] när [!UICONTROL Duration Type] för aktiviteten är [!UICONTROL Calculated Work] eller [!UICONTROL Effort Driven].<br>Mer information om [!UICONTROL Task Duration] finns i artikeln <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Översikt över aktiviteten [!UICONTROL Duration] och [!UICONTROL Duration Type]</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>För projekt beräknar [!DNL Workfront] de planerade timmarna genom att lägga till alla planerade timmar från alla aktiviteter i projektet. </p> </li> 
    </ul> <p><b>TIPS</b></p> <p>Du kan även visa [!UICONTROL Planned Hours] i [!UICONTROL project]-, [!UICONTROL task]- eller [!UICONTROL issues]-rapporter genom att använda textläge och referera till ytterligare fält. Mer information finns i fälten <code>work</code>, [!UICONTROL Work] och <code>workRequiredExpression</code> i den här tabellen. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Labor Cost]</td> 
   <td> 
    <p>För en uppgift, timpriset för användaren eller rollen multiplicerat med antalet timmar som tilldelats användaren eller rollen.</p> <p>För ett projekt är det totalt [!UICONTROL Planned Labor Costs] av alla aktiviteter.</p> <p>Huruvida användarfrekvensen eller rollen används beror på vilken kostnadstyp som har valts för den angivna uppgiften. </p> <p>Mer information finns i <a href="../../../manage-work/projects/project-finances/track-costs.md">Spåra kostnader</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Revenue]</td> 
   <td> <p>Uppgifter och projekt kan visa ett värde för [!UICONTROL Planned Revenue] i [!DNL Workfront]. [!UICONTROL Planned Revenue] representerar summan som är associerad med [!UICONTROL Planned Hours] för aktiviteterna i projektet. För projekt kan den även innehålla [!UICONTROL Fixed Revenue] av projektet. </p> <p>För uppgifter är detta den intäkt som är associerad med [!UICONTROL Planned Hours] av aktiviteter. Planerade timmar från alla aktiviteter räknas upp till projektets planerade timmar för att bidra till beräkningen av projektet [!UICONTROL Planned Hours]. </p> 
   <p>[!DNL Workfront] beräknar [!UICONTROL Planned Revenue] för aktiviteter och projekt med följande formler:</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>Projektet [!UICONTROL Planned Revenue] som visas i området [!UICONTROL Project Details] och i projektrapporter skiljer sig från den planerade intäkten som visas i rapporten [!UICONTROL Utilization]. </p> <p>[!UICONTROL Planned Revenue] i området [!UICONTROL Project Details] visar aktivitetsintäkten samt projektets fasta intäkt. [!UICONTROL Planned Revenue] i [!UICONTROL Utilization Report] visar [!UICONTROL Planned Revenue] som bara är associerad med aktiviteterna i projektet. </p> 
     <p><b>EXEMPEL</b></p>  
      <p>Om projektet har en aktivitet med 10 timmar, som tilldelats en konsult med en timtaxa på 20 USD och projektet har $100 [!UICONTROL Fixed Revenue], visar [!UICONTROL Utilization]-rapporten [!UICONTROL Planned Revenue] $200 för [!UICONTROL Planned Revenue] (den  som är associerad med timmarna för aktiviteten). I avsnittet [!UICONTROL Project Details] visas $300 ([!UICONTROL Planned Revenue] från aktiviteten och Fast intäkt för projektet). </p> 
    <p>Mer information om att spåra intäkter i [!DNL Workfront] finns i <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">Översikt över fakturering och intäkter</a>. </p> 
    <p>Mer information om [!UICONTROL Planned Revenue]-beräkningar i [!UICONTROL Utilization report] finns i <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Visa information om resursutnyttjande </a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Risk Cost]</td> 
   <td> <p>Summan av [!UICONTROL Potential Cost] av alla risker för projektfactoring i Sannolikheten för att de ska uppstå. Detta belopp ingår inte i [!UICONTROL Planned Cost] för projektet.</p> <p>[!UICONTROL Planned Risk Cost] för ett projekt beräknas med följande formel:</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Profile]</td> 
   <td>En administratörsdefinierad samling flikar och portalavsnitt som visas i [!DNL Workfront]-programmet [!UICONTROL Home] och andra instrumentpaneler.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Section]</td> 
   <td>En komponent på en flik på en Dashboard- eller portalsida. Vanligtvis en enda rapport, diagram, kalender eller lista med nyckelinformation.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Tab]</td> 
   <td>En flik på en portal eller kontrollpanel som innehåller upp till tre portalsektioner.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Portfolio]</td> 
   <td> <p>En samling projekt som har enhetliga egenskaper. Dessa projekt konkurrerar vanligtvis om samma resurser, budget eller tidskortplats. Du kan dela upp Portfolio i Program och associera projekten med Program innan de läggs till i Portfolio.</p> <p>Mer information om portföljer finns i <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">Översikt över Portfolio i [!DNL Adobe Workfront]</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Management]</td> 
   <td>Ett område som är inriktat på att hantera en samling eller relaterade program och projektsatsningar.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Optimizer]</td> 
   <td>Ett [!DNL Workfront]-verktyg som kan användas för att utvärdera och prioritera projekt i en portfölj.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Owner]</td> 
   <td>Den berörda part som ansvarar för prioriteringen och budgeten för en portfölj.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Potential Risk Cost]</td> 
   <td>Det här är ett projektfält som du kan hitta i listor och rapporter. Det visar den potentiella kostnaden för de risker som är förknippade med projektet, om de skulle inträffa. Mer information finns i <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Beräkna potentiella riskkostnader </a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Predecessor]</td> 
   <td> <p>En uppgift som måste slutföras innan en beroende uppgift kan slutföras. En aktivitet som är markerad som [!UICONTROL Dependency] för en annan aktivitet. Föregångare låter planeraren ange sekvensberoendelogik, till exempel att starta en aktivitet när en annan uppgift har slutförts.</p> <p>Mer information finns i <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Översikt över föregående aktiviteter</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Primary Company]</td> 
   <td>Det företag som användaren tillhör enligt sina användarinställningar. Företag kan också associeras med projekt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Primary Contact]</td> 
   <td><p>[!UICONTROL Primary Contact] är skapare av ett problem och identifieras automatiskt av [!DNL Workfront] när någon skapar problemet. Du kan uppdatera det här fältet manuellt om du har [!DNL Manage] behörigheter för problemet. Ett problem kan bara ha en primär kontakt.</p> 
   <p>Om du ändrar den primära kontakten har den användare som ursprungligen utsågs till primär kontakt fortfarande [!UICONTROL Manage] åtkomst till problemet.</p>
   <p>När du konverterar ett problem till en aktivitet eller ett projekt blir den användare som är angiven som [!UICONTROL Primary Contact] för problemet [!UICONTROL Converted Issue Originator] för projektet eller aktiviteten. Om [!UICONTROL Primary Contact] av utgåvan uppdateras efter att utgåvan konverterades, kommer [!UICONTROL Converted Issue Originator] att bevaras som [!UICONTROL Primary Contact] för utgåvan när konverteringen inträffade. Se även [!UICONTROL Converted Issue Originator] i den här artikeln.</p> 
   </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Priority]</td> 
   <td>Ett värde som kan tilldelas till en aktivitet, ett ärende eller ett projekt för att ange hur viktig den är. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Private]</td> 
   <td>På en [!UICONTROL Note] eller [!UICONTROL Document] gör det här alternativet det objektet dolt för de flesta visningsprogram. För en kö med privata hjälpförfrågningar kan bara användare i projektgruppen skicka utgåvor till den kön (eller projektet) via området [!UICONTROL Requests].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Profile]</td> 
   <td>All information om ett användarkonto.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Program]</td> 
   <td> <p>En delmängd inom en portfölj, där liknande projekt kan grupperas tillsammans för att uppnå en väldefinierad fördel.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Program Management]</td> 
   <td>Hantering av projektövergripande beroenden, risker, problem, krav och lösningar för att hålla programmet felfritt och uppnå de definierade fördelarna.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Program Owner]</td> 
   <td>Den berörda part som ansvarar för att övervaka och organisera verksamheter för att se till att projektmålen överensstämmer med företagets mål.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Progress]</span> </td> 
   <td> <p>I en [!UICONTROL Goal]-rapport visas procentandelen av hur nära ett strategiskt mål är att slutföra. Procentandelen av förloppet visas som ett tal. Mer information om strategiska mål finns också i [!UICONTROL Goal] i den här tabellen.</p> <p>Det här fältet är bara synligt om din organisation har köpt [!DNL Workfront] mål. Mer information om hur du hanterar strategiska mål med [!DNL Workfront Goals] finns i <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> Lägga till projekt i mål i [!DNL Adobe Workfront Goals] </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Progress Status]</td> 
   <td> <p>I en rapport om projekt, aktivitet och mål visas statusvärdet för projekt, uppgifter eller strategiska mål i det här fältet. Mer information finns i följande artiklar:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">Översikt över status för projektförlopp</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Översikt över status för aktivitetsstatus</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">Översikt över målförlopp och villkor i [!DNL Adobe Workfront Goals]</a> </p>
     <p>Rapporten [!UICONTROL Goal] och fältet [!UICONTROL Progress Status] for [!DNL goals] visas bara om din organisation har köpt [!DNL Workfront Goals]. Mer information om strategiska mål i [!DNL Workfront Goals] finns i <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] översikt</a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>[!UICONTROL Project]</td> 
   <td> <p>En stor mängd arbete som måste slutföras inom en viss tidsram och som måste använda en viss budget och ett visst antal resurser. För att projektet ska bli hanterbart delar du upp det i en serie uppgifter. När du slutför alla uppgifter slutförs projektet. Mer information om hur du planerar ett projekt finns i <a href="../../../manage-work/projects/planning-a-project/plan-project.md">Planera en projektöversikt</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Assignment Planned Hours]</td> 
   <td> <p>I en [!UICONTROL Initiative Job Role]-rapport visar det här antalet [!UICONTROL Planned Hours] som är associerade med en jobbroll som är tilldelad aktiviteter eller ärenden i projektet. Det här fältet och rapporttypen [!UICONTROL Initiative Job Role] visas inte i din [!DNL Workfront]-instans om inte företaget har köpt en [!DNL Workfront Scenario Planner]-licens. Mer information om [!DNL Workfront Scenario Planner] finns i <a href="../../../scenario-planner/scenario-planner-overview.md">Översikt [!DNL Workfront Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Details]</td> 
   <td>Information om aktuell status för ett projekt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Budgeted Cost]</td> 
   <td> <p> Detta är [!UICONTROL Budgeted Cost] för ett projekt så som det visas i listor och rapporter.</p><p>Se även [!UICONTROL Budgeted Cost] i den här artikeln.</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Project Management]</td> 
   <td>En uppsättning profiler som styr tröskelvärdena för när projekt ska skapas, kategoriseras och namnges.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Project Overhead]</td> 
   <td>I en [!UICONTROL Hour]-rapport är det här fältet reserverat för ekonomisk information som är knuten till de timmar som loggas med timtypen [!UICONTROL Project Time]. Projekt kan ha egna faktureringstariffer och om en timme loggas direkt i ett projekt används dessa i beräkningar. Baserat på projektinställningarna kan projekt också ha olika valutor och det kan finnas en valutakonvertering för dessa timmar. Objektet [!UICONTROL Project Overhead] tillåter [!DNL Workfront] att hämta den informationen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Owner]</td> 
   <td>Användaren som ansvarar för att hantera omfång, tidslinje och tilldelningar för ett projekt. Standardgodkännaren för ändringsorder, ekonomiska ändringar och slutprodukter.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Planning]</td> 
   <td>Processer för att utveckla och underhålla projektschemat.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Sponsor]</td> 
   <td>En utsedd intressentprofil som var och en av dina användare ska relatera till. I [!DNL Workfront] är de angivna som [!UICONTROL Access Levels]</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Teams]</td> 
   <td> <p>Samlingen användare eller roller som tilldelats ett projekt</p> <p>Mer information finns i <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">Översikt över projektgruppen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project tracking]</td> 
   <td>Data som används för att mäta ett projekts hälsa och omfattning</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projected]</td> 
   <td> <p>En uppskattning av tidsstämpeln för när arbetet ska slutföras baserat på planerade timmar och procent slutfört för en uppgift, utleverans eller projekt.</p> <p>Det här refererar till datum eller [!UICONTROL Duration] för aktiviteter, utgåvor eller projekt. Vanligtvis anger det datum och tidslängd som stämmer bättre med arbetsobjektens livslängd, efter att en del arbete redan har slutförts eller någon tid har gått. </p> <p>[!UICONTROL Projected Completion Date] för en aktivitet är till exempel det datum då [!DNL Workfront] uppskattar att aktiviteten kommer att slutföras, baserat på hur mycket arbete som har utförts hittills, hur många som har tilldelats den och hur lång tid som har gått sedan startdatumet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Deadline]</td> 
   <td> <p>I rapporter som innehåller objektet [!UICONTROL Document Version] (t.ex. en [!UICONTROL Document Version]-rapport och en [!UICONTROL Proof Approval]-rapport), visas veckodag, datum, tid och år för korrekturdeadline.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Decision]</td> 
   <td> <p>I rapporter som innehåller objektet [!UICONTROL Document Version] (till exempel en [!UICONTROL Document Version]-rapport)  och [!UICONTROL Proof Approval] rapport) visar det här fältet bevisets beslutsstatus (väntande, ändringar krävs eller godkänt)</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Name]</td> 
   <td> <p>I rapporter som innehåller [!UICONTROL Document Version]-objektet (till exempel en [!UICONTROL Document Version]-rapport och en [!UICONTROL Proof Approval]-rapport) visas korrekturnamnet i det här fältet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Pages]</td> 
   <td> <p>I rapporter som innehåller objektet [!UICONTROL Document Version] (till exempel en [!UICONTROL Document Version]-rapport och en [!UICONTROL Proof Approval]-rapport), visar det här fältet antalet sidor som ingår i korrekturet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Progress]</td> 
   <td> <p>I rapporter som innehåller [!UICONTROL Document Version]-objektet (till exempel en [!UICONTROL Document Version]-rapport och en [!UICONTROL Proof Approval]-rapport) visas korrekturens förloppsstatus ([!UICONTROL Sent], [!UICONTROL Opened], [!UICONTROL Commented], [!UICONTROL Decision Made]).</p> <p>Mer information finns i <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">Översikt över korrekturförloppet</a> i <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">Översikt över korrekturförlopp och status</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proofing]</td> 
   <td>En granskningsprocess där en eller flera användare markerar och kommenterar innehåll som ska ändras i en bild, ett textdokument, en video eller interaktivt webbinnehåll.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Public]</td> 
   <td>På en [!UICONTROL Note] eller [!UICONTROL Document] gör det här alternativet objektet tillgängligt för andra användare, eller till och med personer utanför [!DNL Workfront]. För [!UICONTROL Help Request Queue] betyder [!UICONTROL Public] att alla användare som kan skicka problem till ett projekt kan skicka problem via området [!UICONTROL Requests].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Quality]</td> 
   <td>Uppfattningen om arbetskvalitet inom organisationen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue]</td> 
   <td>Kallas även Help Desk Queue eller [!UICONTROL Help Request Queue]. Det här är ett projekt som har publicerats i området [!UICONTROL Requests] så att användare kan skicka utgåvor till det. Vanligtvis skapas köer för särskilda ämnen, som [!UICONTROL Bugs], [!UICONTROL Project Requests] osv.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue Properties]</td> 
   <td>De här inställningarna definierar regler för att skicka utgåvor för ett projekt som publiceras till [!UICONTROL Requests]-området.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue Topic]</td> 
   <td> <p>En egenskap på en [!UICONTROL Help Request Queue] som tillåter användare som skickar ett problem att välja ett ämne. Ämnen kan:</p> 
    <ul> 
     <li>Kopplas till ett anpassat dataformulär.</li> 
     <li>Tilldela automatiskt utgåvan till en användare, roll eller team genom att ange routningsregeln för det valda ämnet.</li> 
     <li>Flytta utgåvan till ett annat projekt eller en annan kö via uppsättningen med routningsregler för det valda ämnet.</li> 
    </ul> <p>Mer information finns i <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Skapa köämnen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rank]</td> 
   <td> <p>I en [!UICONTROL Access Level]-rapport kan du manuellt ange en [!UICONTROL Rank] av [!UICONTROL Access Level]. Detta hjälper dig som [!DNL Workfront]-administratör att visuellt identifiera den komplexitetsnivå som är kopplad till varje åtkomstnivå. Du kan till exempel ge lägre tal för mer komplexa ([!UICONTROL Plan]-nivå) åtkomstnivåer och högre tal för mindre komplexa ([!UICONTROL Requester]-nivå) åtkomstnivåer. Du kan inte rangordna standardåtkomstnivåer. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ready]</td> 
   <td> <p>Det här fältet i en aktivitetsrapport anger om en [!UICONTROL Agile]-aktivitet har markerats som [!UICONTROL Ready] i efterloggen. Den här flaggan gäller bara för [!UICONTROL Agile] aktiviteter, som är uppgifter som tilldelats ett [!UICONTROL Agile]-team. </p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Recurrence Frequency]</td> 
   <td> <p>Ett fält som visas i rutan [!UICONTROL Task Details] eller [!UICONTROL Edit Task] för en överordnad för återkommande uppgifter. Det är den frekvens med vilken uppgifterna i återgivningen inträffar. Mer information om hur du skapar återkommande aktiviteter finns i <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Skapa återkommande aktiviteter</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reference Number]</td> 
   <td> <p>Projekt, uppgifter och ärenden kopplas automatiskt till ett unikt referensnummer när de skapas. Du kan visa [!UICONTROL Reference Number] på sidan [!UICONTROL Details] med projekt, uppgifter eller problem, eller i en lista eller rapport. </p> <p><b>TIPS</b><p><br>Du kan använda referensnummer när två objekt har samma namn, eftersom referensnummer alltid är unika. </p> <p>[!DNL Workfront] genererar automatiskt sekventiella referensnummer på systemnivå. Varje projekt, uppgift eller utgåva får nästa tillgängliga nummer i sekvensen. <br></p> <p>Om till exempel Användare A skapar en uppgift kan [!DNL Workfront] automatiskt tilldela uppgiften referensnumret 100. Om Användare B skapar ett problem direkt efter detta tilldelar [!DNL Workfront] numret 101 till utgåvan. Du kan inte redigera referensnummer manuellt. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rejection Issue]</td> 
   <td>I ett projekt eller en aktivitetsrapport är det här problemet som skapas när godkännandet för projektet eller uppgiften avvisas. Mer information om refuseringsproblem finns i artikeln <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Skapa en godkännandeprocess för arbetsobjekt</a>. </td> 
  </tr>

<tr>
  <td>Relationstyper</td>
  <td><p>Workfront-objekt är alltid kopplade till varandra med någon av följande relationstyper:</p>

<ul><li> <b>Ett till många</b>: I den här relationen kan ett objekt anslutas till flera andra objekt av olika typer. Ett projekt kan t.ex. ha flera uppgifter. Relationen projekt-uppgifter är en relation som är en för många. Du kan inte visa den här relationen i en rapport med hjälp av standardgränssnittet. Du måste använda textlägesrapportering för att visa en till flera relationer.</li>
  <li><b>Ett till ett</b>: I den här relationen kan ett objekt bara vara anslutet till ett annat objekt av en annan typ. Ett projekt kan t.ex. bara ha en grupp. Projekt-grupprelationen är en relation som skiljer sig från en. Du kan visa en till en relation mellan objekt i en standardrapport.</li>
  <li><b>Många till ett</b>: I den här relationen kan flera objekt bara vara kopplade till ett annat objekt av en annan typ. Flera uppgifter kan till exempel vara anslutna till samma projekt. Relationen Aktiviteter och projekt är många till en relation. Du kan visa många till en relation mellan objekt i en standardrapport. </li>
  <li><b>Många till många</b>: I den här relationen kan flera objekt av samma typ kopplas till flera objekt av en annan typ. Flera användare kan till exempel tillhöra flera andra team, och teamen kan tillhöra flera användare. Du kan inte visa den här relationen i en rapport med hjälp av standardgränssnittet. Du måste använda textlägesrapportering för att visa många till många relationer. </li> </ul>
  </td></tr>
<tr> 
   <td>[!UICONTROL Remaining Risk Cost]</td> 
   <td> <p>Ett projektfält som visar skillnaden mellan [!UICONTROL Planned Risk Cost] för ett projekt och summan av alla [!UICONTROL Actual Costs] risker i projektet. </p> <p>[!UICONTROL Remaining Risk Cost] för ett projekt beräknas med följande formel:</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Replanning]</td> 
   <td>Ändra datum för ett projekt för att reparera eller lösa problem. Ett projekt som har varit parkerat i flera månader måste till exempel planeras om för att återspegla korrekta datum. Detta är en manuell åtgärd som innebär att du justerar antingen datum för projektet eller datum för uppgifterna. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Report]</td> 
   <td>Ett diagram eller en tabell som innehåller information om ett givet [!DNL Workfront]-objekt och dess relaterade attribut.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Request]</td> 
   <td> <p>En typ av problem som har trimmats i en central kö och som inte har något samband med pågående arbetsinsatser.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Request Queue]</td> 
   <td>Eftersläpning av problem som hanteras av en trafik- och triageprocess.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Request velocity]</td> 
   <td>Total arbetscykeltid för att ta emot och slutföra en begäran.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Requester]</td> 
   <td>Vanligtvis en licenstyp. En användare med en beställarlicens kan skicka begäranden om nytt arbete i systemet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reserved Time]</td> 
   <td>Dagar som anges på användarens personliga tid, vilket anger att användaren inte kommer att vara tillgänglig för arbete. Se [!UICONTROL Non Work Days].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Issue]</td> 
   <td> <p>I en problemrapport använder du det här fältet i vyer eller filter för att hänvisa till problemet som löser problemet. </p> <p>Mer information om hur du visar upplösta objekt i rapporter finns i <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Visa information om upplösta och upplösta objekt i en rapport</a> i <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Översikt över upplösta och upplösta objekt </a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Project]</td> 
   <td> <p>I en problemrapport använder du det här fältet i vyer eller filter för att hänvisa till projektet som löser problemet. </p> <p>Mer information om hur du visar upplösta objekt i rapporter finns i <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Visa information om upplösta och upplösta objekt i en rapport</a> i <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Översikt över upplösta och upplösta objekt </a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Task]</td> 
   <td> <p>I en problemrapport använder du det här fältet i vyer eller filter för att hänvisa till den uppgift som löser problemet. </p> <p>Mer information om hur du visar upplösta objekt i rapporter finns i <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Visa information om upplösta och upplösta objekt i en rapport</a> i <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Översikt över upplösta och upplösta objekt </a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource]</td> 
   <td>Användare eller roller som finns i [!DNL Workfront] och som har tilldelats projektteam, uppgifter och ärenden. De ansvarar för att slutföra arbetet som är kopplat till projekt, uppgifter eller problem. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in&nbsp;Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>[!UICONTROL Resource Management]</td> 
   <td> <p>[!UICONTROL Resource Management] är en företagsverktygsuppsättning som gör att du kan göra en exakt prognos över användningen av dina resurser utifrån deras tillgänglighet, så att det arbete som måste utföras i tid och budget slutförs. </p> <p>Med verktygen för resurshantering kan ni planera långsiktig kapacitet och kortsiktiga planeringsbehov för era resurser. </p> <p>Mer information om resurshantering i [!DNL Workfront] finns i <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Kom igång med resurshantering</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Manager IDs]</td> 
   <td><p>I en projektrapport kan du använda det här alternativet när du skapar ett filter för att hitta en specifik resurshanterare. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Managers]</td> 
   <td> <p>I en projektrapport eller listvy är detta ett informationsfält som visar användare som är avsedda att utföra resurshanteringsaktiviteter i projektet.  När du använder [!UICONTROL Resource Managers] i en rapport visas en lista med resurshanterare, där varje resurshanterare i projektet avgränsas med kommatecken. Du kan utse upp till 30 resurshanterare för ett visst projekt.</p> <p>Mer information finns i artikeln <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">Ange resurshanterare för ett projekt eller en mall </a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Resource Planner Budgeted Hours] </td> 
   <td>Budgeterade timmar för projektet och de resurser som är associerade med det i [!UICONTROL Resource Planner]. Se även [!UICONTROL Budgeted Hours] i den här artikeln. </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL Resource Planner] </td> 
   <td>Ett avancerat [!DNL Workfront]-verktyg som gör att du kan visa och hantera resurser i projekt, jobbroller eller användare. Mer information finns i <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Översikt över resursplanering</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Planner Budgeted Labor Cost]</td> 
   <td> <p>Detta är kostnaden som är associerad med timarna som budgeterats för projektjobbroller med hjälp av resursplaneraren. </p> <p>Se även"Budgeterad arbetskostnad" i den här artikeln. </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL Resource Pools]</td> 
   <td> <p>Resurspooler är samlingar med användare som kan kopplas till ett projekt. Användarna i samma resurspool tillhör vanligtvis samma avdelning, har liknande eller kompletterande färdigheter eller finansieras via samma budget. Du kan associera flera resurspooler till ett projekt eller till en användare. En resurspool kan tilldelas exklusivt till ett projekt eller delas av flera projekt.</p> 
   <p>Mer information om resurspooler finns i <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Översikt över resurspooler </a>.</p> 
   <p>I projektrapporter visar Resurspooler alla pooler som är associerade med ett projekt. Det här objektet kan inte användas i en gruppering.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Utilization]</td> 
   <td>En rapport som visar antalet tillgängliga timmar under en viss tidsperiod och antalet schemalagda timmar för varje användare i rapporten. Detta beräknas också till [!UICONTROL Average Hours Per Day] och en allokeringsprocent.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Result]</td> 
   <td>I [!DNL Workfront Goals] är ett resultat en förloppsindikator för ett mål. Det kan vara ett tal, ett procentvärde eller ett valutabelopp som du uppdaterar manuellt. Du kan inte visa resultat i en rapport och du kan inte komma åt dem via API:t [!DNL Workfront]. Mer information om aktiviteter finns i <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Kom igång med resultat och aktiviteter i Adobe Workfront-mål</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Revenue]</td> 
   <td>Ett fakturerbart belopp för uppgiften eller projektet. Beloppet kan vara timvis, fast eller en kombination av båda.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Revenue Type]</td> 
   <td>Inkomsttypen bestämmer hur aktiviteten ska generera intäkter. Några exempel är [!UICONTROL Fixed Hourly], [!UICONTROL Role Hourly] och [!UICONTROL Role Hourly w/Cap]. Mer information om att spåra intäkter i [!DNL Workfront] finns i <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Översikt över fakturering och intäkter</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reviewer]</td> 
   <td>Vanligtvis en licenstyp. En användare med en [!UICONTROL Reviewer]-licens kan granska och godkänna arbetsobjekt i systemet.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk]</td> 
   <td> <p>Detta kan referera till följande koncept i [!DNL Workfront]:</p> 
    <ul> 
     <li> <p>Ett fält i ett projekt som anger hur riskabelt ett projekt kan vara. Du kan prioritera genomförandet av dina projekt baserat på risknivån. Projekt kan ha följande risknivåer:</p> <p>- [!UICONTROL Very Low]</p> <p>- [!UICONTROL Low]</p> <p>- [!UICONTROL Medium]</p> <p>- [!UICONTROL High]</p> <p>- [!UICONTROL Very High]</p> <p>De risknivåer du anger för ett projekt kan inte anpassas. </p> <p> Mer information om hur du uppdaterar risken för ett projekt finns i avsnittet Projektinställningar i artikeln <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Redigera projekt</a>. Du kan visa riskfältet för ett projekt i rapporter. </p> </li> 
     <li> <p>En händelse som kan inträffa under ett projekts livslängd och som identifierar en potentiell inverkan på projektets kostnad, omfattning eller schema. Du definierar potentiella risker för ett projekt och associerar en sannolikhet för att de ska inträffa eller en kostnad när du skapar projektets affärsärende. Mer information om hur du lägger till risker i projektets affärsmodell finns i"Skapa och redigera risker i projekt". </p> <p>Du kan inte visa risker som definierats i [!UICONTROL Business Case] i rapporter. Du kan bara visa flera typer av riskkostnader i rapporter och listor. </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk Cost]</td> 
   <td> <p>Kostnaden för riskerna i ett projekt. Följande är riskkostnader för projekt som du kan visa i rapporter:</p> 
    <ul> 
     <li> <p>[!UICONTROL Actual Cost]: ett fält på en risk som visar den faktiska kostnaden för den risk som har inträffat. Förutom rapporter och listor kan du hitta dem i rutan [!UICONTROL Edit Risk] när du redigerar eller skapar en risk. </p> <p>Information om kostnader för projekt, aktiviteter eller utgåvor finns i [!UICONTROL Actual Cost] i den här artikeln. </p> </li> 
     <li> <p>[!UICONTROL Planned Risk Cost]: ett fält i projektet som visar totalt [!UICONTROL Potential Risk Costs] för projektet. Se även [!UICONTROL Planned Risk Cost] i den här artikeln. </p> <p>Information om möjliga riskkostnader finns i <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Beräkna potentiella riskkostnader </a>. </p> </li> 
     <li> <p>[!UICONTROL Remaining Risk Cost]: ett fält i projektet som visar skillnaden mellan det totala antalet [!UICONTROL Actual Costs] av alla risker och [!UICONTROL Planned Risk Cost]. Se även"Återstående riskkostnad" i den här artikeln. </p> </li>
    </ul> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk Management]</td> 
   <td>Processer för att identifiera, minska och övervaka risker.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td>Se [!UICONTROL Job Role] i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing]</td> 
   <td>Tilldela eller flytta ett problem automatiskt, vanligtvis på grund av ett köämne eller genom att vara standardväg (routningsregel) för kön.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing Rule]</td> 
   <td>En inställning för projekt och köämnen som automatiskt tilldelar en utgåva till en användare, en roll eller ett team, eller flyttar utgåvan till ett annat projekt eller köämne. Routningsregler används vanligtvis med hjälpfrågeköer för att automatiskt tilldela inkommande ärenden.</td> 
  </tr> 
 </tbody> 
</table>

## S - U

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objektnamn</th> 
   <th>Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Saved Search]</td> 
   <td>En sökning som sökvillkoren har sparats för. Sparade sökningar gör det enkelt att köra samma sökningar igen utan att behöva ange sökvillkoren igen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Scenario] (i [!DNL Workfront Fusion]) </td> 
   <td> <p>Ett scenario består av en serie steg (moduler) som anger hur data ska överföras och transformeras mellan program/tjänster.</p> <p>Mer information om scenarier i [!DNL Workfront Fusion] finns i <a href="../../../workfront-fusion/scenarios/scenario-overview.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] scenarioöversikt </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scenario] (i [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>I [!DNL Scenario Planner] är ett scenario en kopia av en plan. </p> <p>[!DNL Scenario Planner] kräver ytterligare en licens. Mer information om [!DNL Workfront Scenario Planner] finns i <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Översikt [!DNL Scenario Planner]</a>. </p> <p>Mer information om att skapa scenarier finns i <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">Skapa och jämföra planscenarier i [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schedule]</td> 
   <td>Arbetsschemat för veckan, inklusive arbetstider, kombinerat med lediga dagar (t.ex. helgdagar) och undantagsdagar (t.ex. en arbetsdag på lördag). Du kan associera scheman med projekt och användare.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schedule Exemption]</td> 
   <td>Kallas även [!UICONTROL Modified Shift]. Dagar som schemaläggs i motsats till de vanliga veckoarbetstiderna enligt schemat. En lördag som schemalagts till att fungera, när schemat är inställt på att endast fungera måndag till fredag, skulle till exempel vara [!UICONTROL Schedule Exemption].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scheduled Report]</td> 
   <td> <p>När du skapar en rapportrapport kan du visa information om rapportens scheman, om rapporten är schemalagd för leverans med hjälp av fältet [!UICONTROL Scheduled Report]. I det här fältet visas flera värden, ett för varje schema i varje rapport, i en punktlista. Mer information om schemaläggning av rapporter finns i artikeln <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">Översikt över rapportleverans</a>.</p> <p>Eftersom det här fältet innehåller flera värden kan det inte användas i en gruppering. Du kan bara komma åt den i ett filter eller en vy. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scope Change]</td> 
   <td>En [!UICONTROL Audit Trail] som, om den är aktiv, genererar en anteckning varje gång en ändring görs i omfattningen för ett projekt eller en uppgift, till exempel om en [!UICONTROL Task Duration] eller [!UICONTROL Predecessors] ändras.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Section]</td> 
   <td>Ett område på skärmen, med ett eget huvud, som skapats för att ordna anpassade data för visning.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Section Break]</td> 
   <td>Ett mellanrum eller en kant mellan avsnitt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Security]</td> 
   <td>De inställningar som gör att en användare kan interagera med vissa objekt i systemet och inte med andra. Se även [!UICONTROL Access Levels] i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Setup]</td> 
   <td>Det område där administratörer kan konfigurera systemkonfigurationer och inställningar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severity]</td> 
   <td> <p>[!UICONTROL Severity] är en indikation på hur sannolikt det är att ett objekt påverkar slutförandet av arbetet. Ett problem med hög [!UICONTROL Severity] kan till exempel helt blockera en uppgifts slutförande, men ett problem med låg [!UICONTROL Severity] kan vara enbart kosmetiskt.</p> <p>Mer information finns i <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref"> Uppdatera allvarlighetsgrad</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severities]</td> 
   <td>Se [!UICONTROL Severity] i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sharing]</td> 
   <td>Åtgärden som tillåter andra användare att visa eller redigera ett visst objekt i [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Slack Date]</td> 
   <td>I en uppgiftsvy eller rapport visar [!UICONTROL Slack Date] det exakta datumet när en aktivitet definitivt kan påverka [!UICONTROL Completion Date] för projektet. Mer information om [!UICONTROL Slack Date] för en aktivitet finns i <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">Översikt över aktivitetsdatum i Slack </a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Smart Assignments]</td> 
   <td> <p>När du tilldelar användare uppgifter eller utgåvor till användare, ger [!DNL Workfront] rekommendationer ([!UICONTROL Smart Assignments]) om vilka som är bäst på att slutföra arbetet, baserat på den tid de har till hands för att slutföra det och deras relation till projektet.</p> <p>Mer information finns i <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">Översikt över smarta uppdrag</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source]</td> 
   <td> <p>Anger det överordnade objektet för ett annat objekt. Ett dokument som är kopplat till en aktivitet har till exempel namnet på uppgiften i fältet [!UICONTROL Source] i en [!UICONTROL Document] -rapport eller vy. Ett problem som loggas under ett projekt har namnet på projektet i fältet [!UICONTROL Source] i en problemrapport eller vy. </p> 
   <p>I följande rapporter visas en Source-kolumn där du kan visa information om det överordnade objektet:</p>
  <ul><li>Utfallsrapporter</li>
    <li>Timrapporter</li>
    <li>Dokumentrapporter </li>
    </ul>
   <p>Om användare inte har behörighet till det överordnade objektet för ett problem, en timme eller ett dokument visas kolumnen Source i rapporten tom, även om rapporten är konfigurerad att visas eller levereras med en annan användares åtkomstbehörighet. </p>
   <p> Om du vill visa information om det överordnade objektet i rapporten rekommenderar vi att du lägger till en kolumn för det överordnade objektet där du kan visa namnet på det överordnade objektet. </p>
    <p>Du kan till exempel lägga till något av följande i en rapport med en Source-kolumn: </p>
    <ul><li>Kolumnerna Projektnamn, Aktivitetsnamn eller Utleveransnamn till ett dokument eller en timrapport.</li>
    <li>Kolumnerna Projektnamn eller Aktivitetsnamn i en problemrapport. </li> </ul>
    Mer information finns i <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md">Kör och leverera en rapport med åtkomsträttigheter för en annan användare</a>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Start Date]</td> 
   <td> <p>Det datum då arbetet i ett objekt är inställt på att starta. Det finns flera startdatum i [!DNL Workfront]: </p> 
    <ul> 
     <li>[!UICONTROL Planned]</li> 
     <li>[!UICONTROL Actual]</li> 
     <li>[!UICONTROL Projected] </li> 
    </ul> <p>I en [!UICONTROL Rate report] är detta det datum då en ny faktureringsfrekvens för en jobbroll på projektnivå startar. De timmar som är associerade med projektet som ligger efter detta datum multipliceras med den här faktureringstakten för att beräkna projektets intäkter. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status]</td> 
   <td> <p>En indikator som används för att signalera en arbetsflödesposition för en arbetsuppgift eller ett strategiskt mål.</p> <p>För projekt är [!UICONTROL Status] en inställning i projektet som anger om projektet är:</p> 
    <ul> 
     <li>[!UICONTROL Current]</li> 
     <li>[!UICONTROL On Hold] </li> 
     <li>[!UICONTROL Complete] </li> 
     <li>[!UICONTROL Dead]</li> 
    </ul> <p>Mer information om ett projekts status finns i <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">Åtkomst till listan över systemprojektstatus</a>.</p>
    <p>För uppgifter är [!UICONTROL Status] en inställning för aktiviteten som anger om aktiviteten är:</p> 
    <ul> 
     <li>[!UICONTROL New]</li> 
     <li>[!UICONTROL In Progress]</li> 
     <li>[!UICONTROL Complete]</li> 
    </ul> <p>Mer information om aktivitetsstatus finns i <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">Åtkomst till listan över aktivitetsstatus</a></p> <p>För problem är [!UICONTROL Status] en inställning för problemet som anger om problemet är:</p> 
    <ul> 
     <li>[!UICONTROL New]</li> 
     <li>[!UICONTROL In Progress]</li> 
     <li>[!UICONTROL Awaiting Feedback]</li> 
     <li>[!UICONTROL On Hold]</li> 
     <li>[!UICONTROL Resolved]</li> 
     <li>[!UICONTROL Won't Resolve]</li> 
     <li>[!UICONTROL Cannot Duplicate]</li> 
     <li>[!UICONTROL Verified Complete]</li> 
     <li>[!UICONTROL Reopened]</li> 
    </ul> <p>Mer information om status för systemproblem finns i <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Åtkomst till listan över status för systemproblem</a>.</p> 
    <p>För strategiska mål är [!UICONTROL Status] en inställning för målet som anger om målet är:</p> 
     <ul> 
      <li>[!UICONTROL Active]</li> 
      <li>[!UICONTROL Draft]</li> 
      <li>[!UICONTROL Inactive]</li> 
      <li>[!UICONTROL Closed]</li> 
     </ul> 
     <p>Mer information om strategiska mål finns också i [!UICONTROL Goal] eller [!UICONTROL Goals] i den här artikeln. </p> 
     <p>För strategiska mål visas det här fältet bara om din organisation har köpt [!DNL Workfront Goals]. Mer information om hur du hanterar strategiska mål med [!DNL Workfront Goals] finns i <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] översikt</a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status Change]</td> 
   <td>En [!UICONTROL Audit Trail]. En anteckning skapas när en användare ändrar status för projektet, aktiviteten eller utgåvan.</td> 
  </tr> 
  <tr> 
   <td>Statusikoner</td> 
   <td> <p>Du kan lägga till det inbyggda [!UICONTROL Status Icons]-fältet som en kolumn i vyerna för att förbättra synligheten i viktiga punkter om objekten, som:</p> 
    <ul> 
     <li>Ett objekt har bifogade dokument</li> 
     <li>Ett objekt är associerat med en godkännandeprocess</li> 
     <li>Ett objekt har ytterligare anteckningar kopplade till sig</li> 
     <li>En utgift är fakturerbar eller återbetalningsbar </li> 
     <li>En uppgift är på en kritisk väg</li> 
     <li>En användare tillhör ett företag, ett team eller finns i en annan tidszon </li> 
    </ul> <p>Du kan lägga till fältet [!UICONTROL Status Icons] i vyerna för följande objekt: </p> 
    <ul> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Template Tasks]</li> 
     <li>[!UICONTROL Templates]</li> 
     <li>[!UICONTROL Expenses]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Users]</li> 
    </ul> <p>Mer information finns i <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Inbyggda statusikoner i vyer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status Update]</td> 
   <td> <p>I ett projekt-, aktivitets- eller problemrapport visar det här fältet den senaste statusuppdateringen som objektägare har tillhandahållit i området [!UICONTROL Updates]. För projekt innebär detta att kommentarer som gjorts av projektägaren och för uppgifter och ärenden innebär detta att de som tilldelats kommenterar.</p> 
   <p> Kommentarer som görs när statusen för ett objekt uppdateras visas inte i kolumnen [!UICONTROL Status Update].</p> <p>Om du vill visa statusarna [!UICONTROL New], [!UICONTROL In Process] och [!UICONTROL Complete] använder du kolumnen [!UICONTROL Status].</p> <p>Mer information om status finns i artikeln <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Uppdatera aktivitetsstatus</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Statuses]</td> 
   <td>Se [!UICONTROL Status] i den här artikeln.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Storyboard]</td> 
   <td>Ett diagram som visar status för artiklar (uppgifter i den flexibla metoden) och hur de fortskrider mot slutförande.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Hours]</td> 
   <td>Ett mått som används för att mäta svårigheten eller komplexiteten i en artikel. Agile-team kan välja om de vill använda timmar eller punkter.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Points]</td> 
   <td>Ett mått som används för att mäta svårigheten eller komplexiteten i en artikel. Agile-team kan välja om de vill använda timmar eller punkter.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Strategic]</td> 
   <td>Långsiktigt arbete som förändrar organisationen eller hur organisationen fungerar.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Strategic Alignment]</td> 
   <td>Mäta och anpassa företagsmål mellan portföljer och program.</td> 
  </tr>

<tr> 
   <td><code>[!UICONTROL stretch]</code></td> 
   <td><p>Detta används i rapportkolumner när du använder gränssnittet för textläge. </p>
   <p><code>[!UICONTROL stretch]</code> används för att identifiera vilka kolumner som upptar extra utrymme som inte behövs för vyn. Användargränssnittets bredd för en vanlig användare är cirka 850 pixlar. Det innebär att om du har en vy med fyra
   kolumner (150 pixlar vardera) som vyn upptar 600 av 850 pixlar. Det finns 250 extra pixlar i gränssnittet som läggs till i kolumner som har en sträckningsprocent. </p>
   <p>En kolumns sträckning används när du använder den extra kodraden <code>[!UICONTROL usewidths=true]</code> för minst en av kolumnerna i vyn. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Subscribers]</td> 
   <td> <p>Användare som prenumererar på projekt, uppgifter eller utgåvor.</p> <p>När du använder det här fältet i en rapport visas en lista med prenumeranter, där varje prenumerant avgränsas med kommatecken.</p> <p>Mer information finns i artikeln <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Prenumerera på objekt i [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Summary Task]</td> 
   <td>Se [!UICONTROL Parent Task] i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subtask]</td> 
   <td>En underordnad aktivitet som finns under en överordnad aktivitet.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL System Governance]</td> 
   <td>En uppsättning profiler som styr ändringar och underhåll av ett system.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL System Integration]</td> 
   <td>Att knyta samman olika datorsystem och program fysiskt eller funktionellt för att fungera som en samordnad helhet.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task]</td> 
   <td> <p>En aktivitet som måste utföras som ett steg mot att uppnå ett slutligt mål (att slutföra projektet).</p> <p>Mer information finns i <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">Översikt över uppgifter</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Task Attribute]</td> 
   <td>Andra fält eller objekt som är kopplade till en uppgift och som anger viss information om uppgiften. Några exempel är [!UICONTROL Planned Completion Date] och [!UICONTROL Status].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Task Constraint]</td> 
   <td>Se [!UICONTROL Constraint Type] och [!UICONTROL Constraint Date].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task Management]</td> 
   <td>En uppsättning profiler som styr tröskelvärdena för skapande, tilldelning, avslutande och synlighet av uppgifter.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task Owner]</td> 
   <td>Det team eller den användare som ansvarar för beräkningen av arbetsinsatsen och slutförandet av uppgiften</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Team]</td> 
   <td> <p>En samling användare som arbetar för liknande mål eller affärsmål. De här användarna kan tilldelas till ett arbetsobjekt genom att tilldela teamet till arbetsobjektet.</p> <p>Mer information om team finns i <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Teams overview</a>.</p> <p>Projekt kan ha en [!UICONTROL Project Team], som innehåller alla användare eller roller som är associerade med arbetet i projektet.</p> <p>Mer information om projektteam finns i <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Översikt över projektgruppen</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Template]</td> 
   <td> <p>Projektmallar är allmänna konturer för dina mest repeterbara projekt. Du kan definiera uppgifter, köämnen, anpassade formulär, bifoga dokument eller godkännanden när du skapar en projektmall för att spara tid när du måste skapa ett nytt projekt. </p> <p>Du kan bifoga mallar till befintliga projekt eller använda dem för att skapa nya projekt. All information som anges i mallen överförs till de projekt som skapas med den. </p> <p>Mer information om mallar finns i <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">Översikt över projektmallar</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Template Task]</td> 
   <td>En uppgift som är en del av en mall. Malluppgifter blir uppgifter i projektet som skapas med hjälp av mallen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thread]</td> 
   <td>A [!UICONTROL Note] och dess samling svar som relaterar till ett visst ämne.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thumbnail]</td> 
   <td> <p> I en [!UICONTROL Document]-lista eller -rapport visas en förhandsgranskning av dokumentet i en miniatyrbild. </p> <p> Välj <strong>[!UICONTROL Thumbnail]</strong>  om du vill visa en 33-66 pixlar bred miniatyrbild i rapporten. </p> <p>Storleken på miniatyrbilden justeras när du ändrar bredden på kolumnen i en lista eller rapport.</p> <p>Se även [!UICONTROL Large Thumbnail] i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Time Off]</td> 
   <td>Du kan skapa en [!UICONTROL Time Off]-rapport för att visa när användare har angett att de är lediga i sin profil. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Timesheet]</td> 
   <td> <p>Ett tidkort där användarna kan ange faktiska timmar som de har arbetat med projekt, uppgifter eller ärenden, eller timmar som de har spenderat på andra aktiviteter som inte har med arbetet att göra, som möten eller utbildning. Förutom att ange hur lång tid du tillbringat arbetet kan du även ange om tiden är arbetsrelaterad eller om den motsvarar overheadtid genom att använda timtyper för att definiera tidsangivelserna. Mer information om tidrapporter finns i <a href="../../../timesheets/timesheets/timesheets-overview.md">Översikt över tidrapporter</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Timesheet Profile]</td> 
   <td> <p>En [!UICONTROL Timesheet Profile] är en mall som [!DNL Workfront] använder för att automatiskt skapa tidrapporter för de användare som är associerade med dem. </p> <p>Du kan konfigurera ett antal inställningar som ska gälla för varje tidrapport när den skapas. Vissa av dessa inställningar är: hur ofta tidrapporten ska skapas (varje vecka, varannan vecka, två gånger i månaden eller varje månad), startdagen för tidrapporten, tidrapportgodkännare och tillgängliga [!UICONTROL Hour Types] som användare kan associera med inspelade timmar.</p> </td> 
  </tr> 
  <tr > 
   <td>[!UICONTROL Top Parent ID] </td> 
   <td> <p>I det här fältet kan du identifiera och filtrera data om en grupp på den översta nivån och dess undergrupper i en lista eller rapport.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Top Parent Name] </td> 
   <td> <p>I det här fältet kan du identifiera data om en grupp på den översta nivån och dess undergrupper i en [!UICONTROL View] för en lista eller rapport.</p> <p>Du kan också göra detta med fältet [!UICONTROL Top Parent ID].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Total Hours]</td> 
   <td> <p>I ett [!UICONTROL project report] visar det här fältet den avrundade summan av alla timmar i projektet, den senaste gången som projektets ekonomi beräknades. [!UICONTROL Actual Hours] återspeglar de exakta timmarna som är loggade i projektet. Vanligtvis måste [!UICONTROL Actual Hours] matcha [!UICONTROL Total Hours]. Om [!UICONTROL Total Hours] verkar skilja sig avsevärt från fältet [!UICONTROL Actual Hours] måste du beräkna om ekonomi för projektet.</p> <p>Mer information om hur du beräknar om projektekonomi finns i artikeln <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">Beräkna om projektekonomi</a>.</p> <p>I en tidrapportvy [!UICONTROL Standard] refererar det här fältet till det totala antalet timmar som loggats för objekt för de datum som visas på en tidrapport. Fältet [!UICONTROL Total Hours] för tidrapporter i den här inbyggda vyn refererar till fältet [!UICONTROL hoursDuration], som dynamiskt beräknar skillnaden i timmar mellan tidrapportets start- och slutdatum. Detta används för att visa kolumnen [!UICONTROL Total Hours] i rött om användaren loggar mer tid än de tillgängliga timmarna i tidrapporternas tidsram. Mer information finns i <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">Visa totalt antal timmar på tidrapporten</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tracking Mode]</td> 
   <td> <p>Ett attribut för en uppgift. Detta avgör hur och när de planerade tidslinjerna uppdateras för en aktivitet. Exempel:</p> 
    <ul> 
     <li>[!UICONTROL User Must Update] kräver att en uppgift uppdateras manuellt. Annars blir det [!UICONTROL Behind Schedule] och sedan [!UICONTROL Late].</li> 
     <li>[!UICONTROL Auto Complete] kommer automatiskt att slutföra en uppgift när förfallodatumet, eller [!UICONTROL Planned Completion Date], har passerat.</li> 
    </ul> <p>Mer information finns i <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Översikt över läget Uppgiftsspårning</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Trigger]</td> 
   <td>En händelse som startar ett scenario.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trouble Task]</td> 
   <td>En ofullständig aktivitet med villkoret [!UICONTROL Late], [!UICONTROL Behind Schedule] eller [!UICONTROL At Risk].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unassigned Task]</td> 
   <td>En uppgift som inte har tilldelats någon användare, roll eller team.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Update Type]</td> 
   <td> <p>En inställning för ett projekt som avgör när projektets planerade tidslinje beräknas om. [!UICONTROL Update Type] kan ha följande värden:</p> 
    <ul> 
     <li>[!UICONTROL Automatic and On Change]</li> 
     <li>[!UICONTROL Automatic Only]</li> 
     <li>[!UICONTROL Manual Only] </li> 
    </ul> <p>Mer information finns i <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Välj projekttypens uppdateringstyp </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User]</td> 
   <td>Ett konto som skapats i [!DNL Workfront] för att tillåta en person att logga in och interagera med systemet.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL User Delegation]</p> </td> 
   <td> <p>Ett objekt som kan rapporteras och som anger:</p> 
    <ul> 
     <li>Vilka användare som har delegerat uppgifter, utgåvor och projektgodkännanden</li> 
     <li>Vilka användare som har fått uppgifter, utgåvor och projektgodkännanden delegerade till sig</li> 
     <li>När dessa delegeringar börjar och slutar</li> 
    </ul> <p>Mer information finns i <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">Skapa en användardelegeringsrapport</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Interface]</td> 
   <td>Alla visuella och interaktiva aspekter av programmet [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Interface Preferences]</td> 
   <td>[!UICONTROL User Interface Setup]. [!DNL Workfront]-administratörer kan ändra de här inställningarna för att anpassa olika aspekter av användargränssnittet.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Utilization]</td> 
   <td>Tillgängligheten för en användare eller roll baserat på tilldelat schema, PTO och aktuell arbetsbelastning.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Utilization]</td> 
   <td> <p>En sökning kombinerat med en rapport som visar hur användare (resurser) tilldelas eller överfördelas. Se [!UICONTROL Resource Utilization] i den här artikeln.</p> </td> 
  </tr> 
 </tbody> 
</table>

## V - Z

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objektnamn</th> 
   <th>Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Velocity]</td> 
   <td>Ett mått på den totala arbetscykeltiden (hur lång tid det tar att slutföra en del av arbetet) och hur ofta arbete utförs i den tid som ursprungligen verkställdes (förhållandet mellan arbete och slutförande).</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL View]</td> 
   <td> <p>Vyer refererar till ett rapportelement som gör att du kan ändra kolumnerna i en rapport eller i en lista med objekt.</p> 
   <p> Vyn hänvisar också till en användares rätt att endast visa information om ett objekt, beroende på åtkomstnivå eller behörighetsdelningsnivå för det objektet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL View Icons]</td> 
   <td> <p> Detta är samma fält som statusikoner, men det är bara tillgängligt för följande vyer: </p> 
    <ul> 
     <li> [!UICONTROL Documents] </li> 
    </ul> <p> Mer information finns i artikeln <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Inbyggda statusikoner i vyer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Month]</td> 
   <td> <p>I en rapportlista visas antalet gånger som rapporten har visats under den senaste månaden.<br>Mer information om användningsinformation i rapportlistor finns i artikeln <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visa rapportanvändning</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Quarter]</td> 
   <td>I en rapportlista visas antalet gånger som rapporten har visats under det senaste kvartalet.<br>Mer information om användningsinformation i rapportlistor finns i artikeln <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >Visa rapportanvändning</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Year]</td> 
   <td>I en rapportlista visas antalet gånger som rapporten har visats under det senaste året.<br>Mer information om användningsinformation i rapportlistor finns i artikeln <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visa rapportanvändning</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views This Month]</td> 
   <td> <p>I en rapportlista visas antalet gånger som rapporten har visats under den här månaden.<br>Mer information om användningsinformation i rapportlistor finns i artikeln <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visa rapportanvändning</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views This Quarter]</td> 
   <td>I en rapportlista visas antalet gånger som rapporten har visats under det här kvartalet.<br>Mer information om användningsinformation i rapportlistor finns i artikeln <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visa rapportanvändning</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views This Year]</td> 
   <td>I en rapportlista visas antalet gånger som rapporten har visats under det här året.<br>Mer information om användningsinformation i rapportlistor finns i artikeln <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">Visa rapportanvändning</a>.</td> 
  </tr>

<tr>
  <td> <code>[!UICONTROL width]</code>
  </td>
<td> I en rapport, när du använder [!UICONTROL Text Mode]-gränssnittet, den kodrad där du kan ange bredden på varje kolumn i pixlar. Workfront tillhandahåller en föreslagen bredd för varje fält,
men beroende på fälttyp och format kan du behöva göra justeringar.
Du måste använda den extra <code>[!UICONTROL usewidths=true]</code>-kodraden för att framtvinga den bredd som anges för kolumnen. 
  </td>

</tr>

<tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>I en projekt-, uppgifts- eller problemrapport visas de planerade timmarna för projektet, aktiviteten eller utgåvan med följande programsats i textläge:</p>
   <code><p>valuefield=work</p>
   <p>valueformat=HTML</p></code> 
   <p>Mer information om hur du använder textläge finns i <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Översikt över syntaxen i textläge</a>. </p> 
   <p><b>TIPS</b> 
   <p>Om du lägger till ett av [!UICONTROL Planned Hours]-fälten i en problemrapport läggs fältet <code>work </code> till i rapporten. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work]</td> 
   <td> <p>En av två primära licenstyper. Detta har mindre åtkomst än [!UICONTROL Plan], men kan skapa och göra uppdateringar i systemet. En användare med en Work-licens har fler funktioner än en [!UICONTROL External]-, [!UICONTROL Reviewer]- eller [!UICONTROL Requester]-licensinnehavare.</p> <p>Mer information finns i <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] licensöversikt</a>.</p> <p>Arbetet kan referera till antalet [!UICONTROL Planned Hours] för ett projekt, en aktivitet eller ett problem. Mer information finns i fältet [!UICONTROL work] i den här tabellen. </p> <p><b>TIPS</b></p> <p> Om du lägger till ett av [!UICONTROL Planned Hours]-fälten i en problemrapport läggs fältet <code>work </code> till i rapporten. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Breakdown Structure]</td> 
   <td>En hierarkisk struktur för de uppgifter som ska utföras av projektteamet baserat på den överordnade/underordnade relationen.</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Work Effort] </td> 
   <td> 
    <p>En projektledare kan bestämma sig för att använda det här fältet i stället för [!UICONTROL Planned Hours] för att uppskatta hur mycket arbete som krävs för att slutföra en uppgift. Det här fältet är bara synligt när följande villkor är uppfyllda:</p> 
     <ul> 
      <li> <p>Aktiviteten har en [!UICONTROL Simple Duration Type]. </p> <p><b>TIPS</b></p> <p> Om du uppdaterar aktiviteten [!UICONTROL Duration Type] till någon annan typ döljs det här fältet. </p> </li> 
      <li>Projekthanteraren har aktiverat [!UICONTROL Use Work Effort] att automatiskt beräkna aktivitetsfältet [!UICONTROL Planned Hours] i projektet. </li> 
     </ul> 
     <p>Mer information om hur du använder [!UICONTROL Work Effort] i stället för [!UICONTROL Planned Hours] för att beräkna aktivitetsinsatsen finns i <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Översikt över arbetsinsats</a>. </p> 
     <p>Du kan visa det här fältet i uppgiftsrapporter och listor.</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Work Item]</td> 
   <td> <p>Det här fältet refererar till aktiviteter eller problem i [!DNL Workfront]. </p> <p>Rapporten [!UICONTROL Work Item] visar information om både uppgifter och problem. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work management mix]</td> 
   <td>En [!UICONTROL Work Performance Indicator] (WPI) av den andel arbete som har allokerats för att köra ditt företag jämfört med att ändra ditt företag. Mix WPI hjälper er att på organisationsnivå förstå om er strategi har någon verklig arbetstilldelning.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Resource]</td> 
   <td>En beteckning för en person i systemet som är berättigad till arbete eller spårtid.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Role and Responsibilities]</td> 
   <td>Definiera ägare och intressenter för att hantera omfattningen, genomförandet och godkännandena av den avsedda utgåvan, uppgiften, projektet, programmet eller portföljen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work management SLA]</td> 
   <td>En kvantifierbar mätmetod som alla intressenter har kommit överens om.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Stakeholder]</td> 
   <td>En samling användare med ett starkt intresse för resultatet av en arbetsbegäran.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work management touchpoints]</td> 
   <td>Digitaliserade register över kommunikation mellan intressenter.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Performance Indicators] </td> 
   <td> <p>Blandningsgrad, kapacitet, hastighet, kvalitet och engagemang.</p> <p>WPI är en vanlig akronym för [!UICONTROL Work Performance Indicator].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Process]</td> 
   <td> <p>Den metod som används för att ta emot, prioritera och köra arbete. Det sätt du utför arbetet på kallas vanligtvis"arbetsflöde" eller"projektplan" (en lista med uppgifter med datum, föregående relationer osv.). </p> <p>Exempel på en arbetsprocess kan vara produktion av en enda resurs eller leverans av en kampanj med flera resurser. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Workflow template]</td> 
   <td>I rapporten [!UICONTROL Proof Approval] visar det här fältet alla arbetsflödesmallar som är kopplade till ett korrektur. Om det inte finns några bifogade mallar är kolumnen tom.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Work Time]</td> 
   <td>

<p>Representerar procentandelen av heltidsekvivalent ([!UICONTROL FTE]) tid som användaren är tillgänglig för faktiskt arbete, exklusive overhead. [!UICONTROL Work Time] måste vara ett decimaltal upp till 1 och det får inte vara 0. Exempel: 20 % tillgänglighet för faktiskt arbete är 0,2.</p>
   </p>Fältets standardvärde är 1, vilket anger att en användare tillbringar hela [!UICONTROL FTE] på faktiskt, projektrelaterat arbete.  </p>
   <p>Systemet använder det här talet för att beräkna användarens tillgänglighet för faktiskt, projektrelaterat arbete. </p>
   <p> Schemalagda undantag och ledig tid kan också påverka användarkapaciteten. </p>
   <p>Mer information om hur du skapar scheman i Workfront finns i <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Skapa ett schema</a>. </p>
    <p>Workfront beräknar en användares tillgänglighet beroende på inställningarna för resurshantering i området [!UICONTROL Setup]. Mer information finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">Konfigurera inställningar för resurshantering</a>. </p> 
   <p>Du kan uppdatera [!UICONTROL Work Time] för en användare när du redigerar eller skapar användaren. Mer information finns i <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Redigera en användares profil</a></p> 
   <b>TIPS</b> 
   <p>Ange värdet [!UICONTROL Work Time] till 1 för att ange att användaren är tillgänglig för projektrelaterat arbete och hela heltidsekvivalenten.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Working time]</td> 
   <td>I Workfront-dokumentationen används den här termen för att beskriva den tid som tilldelats till arbetet enligt ett schema.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>I en projekt-, uppgifts- eller problemrapport visas antalet planerade timmar för projektet, aktiviteten eller utgåvan med följande programsats i textläge följt av ordet"Timmar":</p>
   <code>
   <p>valuefield=workRequiredExpression</p>
   <p>valueformat=HTML</p>
   </code>
    <p>Mer information om hur du använder textläge finns i <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Översikt över syntaxen i textläge</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

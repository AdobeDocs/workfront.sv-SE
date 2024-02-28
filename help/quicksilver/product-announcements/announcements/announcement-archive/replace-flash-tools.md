---
title: Ersättning av verktyg baserade på Flash i Adobe Workfront
description: Ersättning av verktyg baserade på Flash i Adobe Workfront
author: Luke
draft: Probably
feature: Product Announcements
exl-id: a0ca824d-aab8-4da2-97ed-0913a7f76d55
source-git-commit: c80d9b0b7eb2a638af9e0a11ca3038ed99ecf1ee
workflow-type: tm+mt
source-wordcount: '2701'
ht-degree: 0%

---

# Ersättning av verktyg baserade på Flash i Adobe Workfront

Vi har tagit bort alla Flash-baserade verktyg från Adobe Workfront Classic.

Nu finns ersättningsverktyg som bygger på aktuella standarder i Workfront. Ändringarna är anpassade till att stödet för Flash upphör enligt Adobe.

## Viktiga datum

Följande datum är viktiga för borttagningen av alla Flash-baserade verktyg i Workfront:

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>July 1, 2020</strong>: All Flash-based tools will be removed from all Workfront products for those customers who are not using them currently. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">All customers who are currently using the Flash-based tools will continue to have access after this date. If you are still using these products, report all blocking issues or concerns that you see which prevent you from fully transitioning all your users to the new replacement tools by this date. Work with your account manager or our support team to report these concerns. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about contacting our support team, see <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>. </p>
  -->

* **19 november 2020**: Alla Flash-baserade verktyg har tagits bort från alla Workfront-produkter.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  We recommend that you start using the new tools and retire the Flash tools before then, to increase the security of your instance. We will also gradually disable the tools that have not been used for at least 3 months. If you would like us to disable the Flash tools before November, you can contact
  <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>.
  </MadCap:conditionalText>
  -->

## Äldre Flash-baserade verktyg

Verktygen som anges i följande avsnitt har tagits bort från Workfront och ersatts med nya lösningar.

Mer information om ersättningsverktyg finns i [Äldre verktyg för Flash och ersättningar av dessa](#legacy-flash-based-tools-and-their-replacements) i den här artikeln.

### Resurshantering

* Fliken Äldre resursplanering i området Personer och alla verktyg som finns på fliken, som innehåller följande:

   * Resursbudgethanteraren
   * Kapacitetsplanering
   * Resursuppskattningar
   * Resursrutnät\
     Mer information finns i [Resursplanering: artikelindex](../../../resource-mgmt/resource-planning/resource-planning-overview.md).

* Området för beräkning av äldre resurser i ett projekts affärsfall

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  is displayed in view-only mode
  </MadCap:conditionalText>
  -->

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  For more information, see
  <a href="../../../resource-mgmt/resource-mgmt-overview/migrate-resource-estimates-to-budgeting.md" class="MCXref xref">Migrate from Legacy Resource Estimates to Resource Budgeting </a>
  </MadCap:conditionalText>
  -->

  .

* Underfliken Resursstödraster på fliken Anställning i ett projekt
* Alternativet Använd nytt schemaläggningsområde på underfliken Schemaläggning på fliken Personal i ett projekt som tar bort det tidigare schemaläggningsområdet eller Team Builder. I det här fallet visas tidslinjen för schemaläggning nu som standard.
* Fliken Allokering under användarprofilen

### Rapporter

Följande rapportfunktioner och rapporter har tagits bort:

* Borttagna rapporteringsfunktioner:

   * Alternativet Resursstödraster i en användarrapport
   * Alternativet Äldre Gantt i ett projekt eller en aktivitetsrapport\
     Mer information finns i [Visa information i Gantt-schemat](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

* Borttagna rapporter:

   * Rapporten Äldre resurspool
   * Resursuppskattningsrapporten

  >[!NOTE]
  >
  >Alla äldre fält som öppnas via rapporter eller via API:t (äldre resurspool, äldre budgeterad kostnad, äldre kostnad, äldre budgeterade timmar, äldre budgeterad arbetskostnad osv.) visas i olika rapporter, men innehåller ingen ny information.

### Äldre Gantt

* Alla äldre Gantt-vyer från projekt- och uppgiftslistor samt rapporter och rapportalternativ
* Underflikarna Äldre Gantt i Portfolio och Program
* Underfliken Äldre Gantt i en lista över malluppgifter i en mall, vyn Äldre Gantt på fliken Underaktiviteter i en malluppgift och i en malluppgiftsrapport

### Korrektur

Det äldre korrekturläsaren har ersatts med det nya visningsprogrammet för webbkorrektur och skrivbordsgranskning för de flesta kunder och har tagits bort för alla kunder i november 2020.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">With the 2018.2 release, the Legacy proofing viewer was removed as the default viewer.</p>
-->

Mer information finns i följande resurser:

* [Granska korrektur i webbkorrekturläsaren](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proofs-in-wpv.md)
* [Granska korrektur i Desktop Proofing Viewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/review-proofs-in-desktop-proofing-viewer.md)

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="../../../workfront-proof/wp-work-proofsfiles/review-proofs-lpv/lpv-removed-2018.md" class="MCXref xref">Legacy proofing viewer removed in 2018.3</a> </li>
  -->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Additional features to be removed</h3>
<ul>
<li>The Legacy Portfolio Optimizer<br>For more information, see <a href="../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md" class="MCXref xref">Portfolio Optimizer overview</a>.<br></li>
<li>The Legacy financial fields in the Business Case of the project and the Portfolio Optimizer</li>
<li>The dialog boxes used when sharing reports, calendars, and documents no longer rely on Flash-based technology</li>
</ul>
</div>
-->

## Äldre verktyg för Flash och ersättningar av dessa {#legacy-flash-based-tools-and-their-replacements}

Om inget annat anges har alla äldre funktioner ersatts med nya, vilket visas i följande tabell.

>[!CAUTION]
>
>De gamla Flasharna har tagits bort från alla miljöer.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Äldre verktyg</strong> </p> </th> 
   <th> <p><strong>Nya verktyg</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Äldre resurspooler</strong> </p> <p>Äldre resurspooler var grupper eller samlingar av jobbroller som behövdes samtidigt för att slutföra ett projekt. Äldre resurspooler hade ett antal brister:</p> 
    <ul> 
     <li> Du kunde associera en användare med en äldre resurspool, men den användes endast för rapportering. Eftersom äldre resurspooler arbetade med abstrakta rollentiteter för jobb, beaktades inga av användarens schemaundantag och ledig tid, vilket resulterade i felaktiga data om resurstillgänglighet. </li> 
    </ul> 
    <ul> 
     <li>Du kan bara ange en äldre resurspool per projekt, vilket resulterade i att flera äldre resurspooler endast stöder flödet av separata grupper som arbetar oberoende av varandra och aldrig delar resurser. I alla andra fall rekommenderades en äldre resurspool som innehöll alla resurser i systemet, vilket ledde till prestandaproblem med stora mängder projekt och data.</li> 
    </ul> </td> 
   <td> <p><strong>Resurspool</strong> </p> <p>Nya resurspooler är en samling användare som behövs samtidigt för att slutföra projektet. Workfront inser också att det finns tillfällen då specialiserade användare måste tilldela dem arbete separat. Därför kan du nu budgetera användare istället för jobbroller. </p> Fördelar med resurspoolen jämfört med äldre resurspooler är bland annat följande: 
    <ul>
     <li>Eftersom resurspooler baseras på användarna beaktas redan deras tids- och schemaundantag för beräkningarna av användar- och rolltillgänglighet. Detta resulterar i exakta och aktuella data, vilket gör det möjligt att fatta korrekta budgetbeslut och minimera sannolikheten för ändringar när projektet körs.</li>
     <li>Eftersom det nu finns större kontroll över tillgängligheten av resurser och exaktheten i data kan du koppla flera resurspooler till ett projekt med Workfront. En användare kan också tillhöra mer än en resurspool om de har flera kunskaper som kan användas i flera projekt samtidigt. </li>
    </ul><p>Om du har sådan kontroll över data behöver du inte längre ha en resurspool som innehåller alla resurser för att distribuera den tillgängliga budgeten. Vi rekommenderar faktiskt inte det här. Vi rekommenderar i stället att du diversifierar dina resurspooler och endast associerar relevanta resurspooler med projekt.</p><p> Mer information om resurspooler finns i <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Översikt över resurspooler </a></p></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Resursbudgethanteraren</strong> </p> <p>Du kan använda Resursbudgethanteraren för att ange tillgängligheten för jobbrollresurser i flera resurspooler. På grund av bristerna i den äldre resurspoolen användes denna funktion sällan. När den användes tvingades användare att manuellt ange tillgänglighet för jobbroller för att göra budgeteringen mer korrekt. Schemaundantagen och användarens ledig tid har inte beaktats.</p> </td> 
   <td> <p>Med automatisk beräkning av tillgänglighet baserad på användarna i resurspoolerna behövs inte längre Resource Budget Manager. Verktyget har tagits bort, tillsammans med allt manuellt arbete för att beräkna tillgänglighet.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Resursuppskattningar</strong> </p> <p>Fliken Resursberäkning under varje äldre resurspool har samma syfte som Resursbudgethanteraren, endast i samband med en äldre resurspool. Det här verktyget har samma begränsningar som Resursbudgethanteraren och de äldre resurspoolerna: felaktiga data och manuell inmatning av tillgänglighet. </p> </td> 
   <td> <p>Med automatisk beräkning av användartillgänglighet har resursuppskattningar blivit föråldrade och tagits bort.</p> <p>Verktyget tas bort från de äldre resurspoolerna och de äldre resursberäkningarna i ett projekts affärsfall. <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The Legacy Resource Estimates area on the Business Case of the project remains there in View-only mode at this time. 
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Kapacitetsplanering</strong> </p> <p>Kapacitetsplaneraren var ett Workfront-verktyg för att budgetera resurser och prioritera projekt i en äldre resurspool utifrån tillgängliga resurser. Eftersom uppgifterna från resursuppskattningar och resursbudgetförvaltaren som tillhandahöll informationen för kapacitetsplaneraren var ofullständiga, måste projektprioriteringen dubbelkontrolleras mot användarnas tillgänglighet.</p> <p>Att använda en enda äldre resurspool som innehöll alla jobbroller i systemet var det vanligaste scenariot, vilket ledde till prestandaproblem när kapacitetsplaneraren försökte läsa in ett stort antal projekt.</p> </td> 
   <td> <p><strong>Resursplaneringens projektvy</strong> </p> <p>I den projektbaserade vyn i resursplaneraren kan du budgetera resurser och prioritera projekt på samma sätt som du gjorde i den gamla kapacitetsplaneraren. Till skillnad från det gamla verktyget stöds nu mer data, med mer exakt information eftersom både användarens tid och schemaundantag har beaktats.</p> <p>Tillgänglig, planerad och budgeterad information visas i en översikt så att resurshanterarna kan se både om det finns tillräckligt med personer för att utföra arbetet och om projektplanerna överskrider de ursprungliga budgetuppskattningarna.</p> <p> Mer information om hur du använder projektvyn i resursplaneraren finns i <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Översikt över resursplanering</a></p> <p><strong>Scenarioplanen</strong> </p> <p>För långsiktig kapacitetsplanering, scenariomodellering och prioritering har vi också infört Workfront Scenario Planner. </p> <p>Scenarioplaneraren finns endast i den nya Adobe Workfront-upplevelsen och kräver ytterligare en licens. Mer information om Workfront Scenario Planner finns i <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Översikt över scenarioplanen</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Uppskattningar av äldre resurser (affärsärende)</strong> </p> <p>Du kan använda området Legacy Resource Estimates i affärsärendet för att budgetera ett visst antal arbetstimmar och kostnader som en del av projektplaneringen och begäran om resurser. Den här vyn gav ingen insyn i tillgängligheten för resurser, vilket resulterade i ungefärliga begäranden om resurser och en ökad risk för avvisat projektarbete.</p> </td> 
   <td> <p><strong>Resursbudgetering (affärsärende)</strong> </p> <p>Avsnittet Resursbudgetering under Affärsärende ger möjlighet att planera resurser till affärsärendet, vilket ger insyn i användar- och rolltillgänglighet samt möjlighet att budgetera på användarnivå. </p> <p> Mer information om resursbudgeteringsområdet för affärsärendet finns i <a href="../../../manage-work/projects/define-a-business-case/areas-of-business-case.md" class="MCXref xref">Översikt över affärsområdet</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Resursuppskattningsrapporter</strong> </p> <p>När du använder de äldre verktygen för resurshantering kan du rapportera om budgeterade och planerade timmar från affärsärendet. På så sätt kan du skapa matrisrapporter som visar det totala budgeterade och planerade arbetet för varje jobbroll inom en viss tidsram. Rapporten kunde inte redigeras och du kunde inte ändra budgeten för dina resurser baserat på rapportresultatet. </p> </td> 
   <td> <p><strong>Användningsrapport</strong> </p> <p>Den inbyggda användningsrapporten visar Planerade, Budgeterade och Faktiska timmar, Kostnad och Inkomster sida vid sida. </p> <p>Mer information om hur du använder användningsrapporten finns i <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Visa information om resursutnyttjande </a>. </p> 
    <div> 
     <p><strong>Rapporteringsskyldiga budgeterade timmar</strong> </p> 
     <p>Skapa en rapport för budgeterade timmar för att granska timmar som budgeterats i resursplaneraren i ett rapportformulär. </p> 
     <p>Mer information om budgeterade timmar finns i <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Ordlista för Adobe Workfront-terminologi</a>.</p> 
     <p>Mer information om hur du skapar en rapport finns i <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Skapa en anpassad rapport</a>.</p> 
    </div> <p><strong>Resursplaneringens rollvy</strong> </p> <p>De budgeterade och planerade timmarna från affärsärendet i de äldre resurshanteringsverktygen är nu tillgängliga i en ny intern vy - rollbaserad vy av resursplaneraren. I den här vyn finns tillgänglig, planerad och budgeterad timinformation i korthet så att du kan kontrollera och ändra budgeteringen på samma plats. Detta ger bättre beslutsunderlag vid högnivåplanering av arbetsuppgifter. </p> <p> Mer information om budgeteringsresurser i rollvyn i resursplaneraren finns i <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using2" class="MCXref xref">Använd projekt- och rollvyer för att budgetera resurser </a> avsnitt i <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Översikt över resursplanering</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Resursrutnät</strong> </p> <p>Resursstödrastret gav dig synlighet i allokeringen av specifika användare när ett projekt fortskrider mot slutförande. </p> <p>Du kan till exempel enkelt se när någon i projektteamet fick sitt arbete gjort tidigt och när någon blev försenad samt om de var överallokerade eller underallokerade under en viss tidsperiod. </p> <p>Tyvärr kunde ni inte agera på informationen i samma vy. För att åtgärda överallokeringsproblem var du tvungen att gå till projekten och manuellt justera informationen där utan att synas i resultatet av åtgärderna.</p> </td> 
   <td> <p>Resursstödrastret har ersatts av två nya verktyg. Du kan använda följande verktyg, beroende på vilken fas av resursplaneringen du befinner dig i:</p> 
    <ul> 
     <li> <p><strong>För analysfasen:</strong> </p> 
      <ul> 
       <li> <p><strong>Utjämning av arbetsbelastning</strong>: Använd arbetsbelastningsutjämnaren för att visa användarnas arbetsbelastning på en mer detaljerad nivå. När du använder Utjämning av arbetsbelastning kan du visa vilka användare som har tillgänglighet i sin arbetsbelastning för att slutföra uppgiften i tid. Detta inkluderar deras ledig tid och information om schemaläggningsundantag. </p> <p>Mer information om belastningsutjämnaren finns i <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Översikt över belastningsutjämnare</a>.</p> </li> 
       <li> <p><strong>Resursplaneringens användarvy</strong><strong>:</strong> När du försöker förstå på en högre nivå vilka projekt dina användare har tilldelats använder du användarvyn i resursplaneraren. På så sätt kan du se vad användarna arbetar med samt deras över- och underallokering för en viss tidsram. Resursplaneraren innehåller även en visualisering av den övergripande allokeringen av användare i sin helhet samt synlighet i loggade faktiska timmar, vilket är praktiskt när du vill analysera förloppet av det arbete som har utförts. </p> <p>Information om hur du använder användarvyn i resursplaneraren finns i <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using" class="MCXref xref">Använd användarvyn för att visa tillgängliga, planerade och faktiska timmar eller heltidsanställda </a> avsnitt i <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Översikt över resursplanering</a></p> </li> 
      </ul> </li> 
     <li><strong>För den taktiska fasen:</strong> 
      <ul> 
       <li><strong>Utjämning av arbetsbelastning</strong> Du kan göra följande med hjälp av Utjämning av arbetsbelastning: 
        <ul>
         <li>Tilldela användare arbete.</li>
         <li>Hantera användarnas allokeringar till arbetsobjekt. </li>
         <li>Dela belastningsutjämnaren med andra användare som kanske inte har synlighet i området Personer. Använd funktionen Delningsbar länk för att dela en länk till Utjämning av arbetsbelastning och bädda in den i anpassade instrumentpaneler. Alla användare som har åtkomst till Visa användare kan visa de här instrumentpanelerna när du delar dem.</li>
        </ul><p>Utjämning av arbetsbelastning är tillgängligt i området Personer. </p><p>Mer information om belastningsutjämnaren finns i <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Översikt över belastningsutjämnare</a>.</p></li> 
      </ul> <!--
       <ul data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
        <li><strong>The Resource Scheduling Areas</strong><strong>:</strong> When assigning your resources to the actual work that must be completed, use the Resource Scheduling areas in the People or Team areas, or at the project level. These areas allow you to visualize and manage the users' workload by day and rectify any problems from one view using the following actions: 
         <ul>
          <li> manual dragging and dropping of tasks to the correct assignee </li>
          <li> automatic assigning of tasks </li>
          <li> bulk swapping assignments </li>
          <li><p>adjusting Planned Hours according to the true availability of users. </p></li>
         </ul><p>These actions provide even more control over managing workload. </p><p> For information about managing user assignments and allocations in the Resource Scheduling areas, see <a href="../../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md" class="MCXref xref">Get started with Resource Scheduling</a>.</p><p>With this new functionality, the Resource Grid is replaced by the User View of the Resource Planner and the Resource Scheduling areas in the following areas of the application: </p>
         <ul>
          <li>People - the Resource Grid is eliminated along with the Legacy Resource Planning tab.</li>
          <li>Project - the Scheduling area under the Staffing tab of the project is available to Work and Plan license users. They do not have to have Manage access to the project to view this area. </li>
          <li>Reporting - the ability to view User reports in the Resource Grid view is removed. Instead, there is an option to share a URL for the User View of the Resource Planner and embed it in custom dashboards, providing visibility into user utilization to virtually anyone in the system. Any users with access to View users are able to view these dashboards when you share them. </li>
          <li>User - the Allocation tab is eliminated as the same information can be accessed in the User View of the Resource Planner.</li>
         </ul></li> 
       </ul>
      --> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Gantt-schema, aktivitetslista</strong> </p> <p> Det äldre Gantt-schemat i uppgiftslistan gav användarna möjlighet att se tidslinjen i projektet och utföra konsekvensscenarioplanering utan att implementera ändringar i databasen. Det gamla Gantt-schemat baserades på Flash-teknik, som innebar säkerhetsrisker. </p> </td> 
   <td> <p><strong>Gantt-schema,</strong> <strong>Uppgiftslista</strong></p> <p> Det nya HTML-baserade Gantt-schemat har samma syfte som det gamla Gantt-schemat. Användarna kan visualisera tidslinjen i projektet och utföra konsekvensscenarioplanering utan att implementera ändringar i databasen genom att ändra till alternativet Spara manuellt i verktygsfältet i uppgiftslistan. </p> <p>Det nya Gantt-schemat är interaktivt när du använder alternativet Spara automatiskt, som du kan använda när du vill spara ändringarna automatiskt när de inträffar. </p> <p>Det nya Gantt-schemat för uppgiftslistor bygger på den senaste tekniken och är tillförlitligt. Det nya Gantt-schemat finns direkt i uppgiftslistan och är enkelt att komma åt när du arbetar med uppgiftslistan utan att behöva byta flikar eller ändra vyn. </p> <p>Även om det nya Gantt-diagrammet har samma funktioner som det föregående diagrammet, finns det vissa skillnader i funktioner jämfört med det gamla Gantt-diagrammet. </p> <p> Underfliken Äldre Gantt i en lista över malluppgifter i en mall, vyn Äldre Gantt på fliken Underaktiviteter i en mallaktivitet och det äldre Gantt-schemat i en mallaktivitetsrapport har också ersatts med det HTML-baserade Gantt-schemat. </p> <p>Om du använder det äldre Gantt-schemat mest för enkla vyer och snabbredigeringar och inte använder det faktiska diagrammet, kan du med det nya alternativet Tidslinjeplanering göra snabba ändringar i viktiga planeringsfält. Du kan välja Planera tidslinje i stället för Spara automatiskt i verktygsfältet i uppgiftslistan.</p> <p>Mer information om hur du sparar en uppgiftslista med alternativet Tidslinjeplanering finns i avsnittet Spara ändringar i en uppgiftslista manuellt när du väljer alternativet Tidslinjeplanering i artikeln <a href="../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">Redigera uppgifter i en lista</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Äldre Gantt-schema för en projektlista</strong> </p> <p>Det äldre Gantt-schemat i projektlistan ger användarna möjlighet att se projekt och deras uppgifter i en vy. Utan att lämna projektlistans sammanhang kan användarna se information om aktiviteterna i ett projekt samt beroendena mellan projekten. Det äldre Gantt-schemat i projektlistan baserades på Flash-teknik, som innebär säkerhetsrisker. </p> </td> 
   <td> <p><strong>Gantt-schema, projektlista</strong> </p> <p>Det HTML-baserade Gantt-diagrammet har samma syfte som det gamla Gantt-diagrammet. Användare kan visa projekt och deras uppgifter i en vy för att visuellt identifiera beroenden mellan projekt och uppgifter. Gantt-schemat för projektlistan finns direkt i projektlistan. Det nya Gantt-schemat har ett modernt gränssnitt och bygger på den senaste tekniken.</p> <p>Mer information om Gantt-schemat för projektlistor finns i <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">Visa information i Gantt-schemat </a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Dialogrutor för delning av rapporter, kalendrar och dokument</strong> </p> <p>När du delar rapporter, kalendrar och dokument baserades dialogrutorna på Flash.</p> </td> 
   <td> <p>Erfarenheten när du delar rapporter, kalendrar och dokument i Workfront har inte ändrats. Men upplevelsen är inte längre beroende av Flash.</p> <p>Mer information om hur du delar dessa objekt finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Översikt över delningsbehörigheter för objekt</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Språkkontroll för äldre användare</strong> </p> <p>Det äldre korrekturläsaren var ett webbaserat korrekturläsare med funktioner för korrektur av statisk text, video och interaktiva korrektur.</p> </td> 
   <td> <p><strong>Språkkontroll för webben för visningsprogram och skrivbordet</strong> </p> <p>I Web Proofing Viewer finns funktioner för korrektur av statisk text och video.</p> <p>Desktop Proofing Viewer har funktioner för korrektur av interaktiva korrektur och ger dessutom fullt stöd för statiskt material och videoklipp.</p> <p>Filformatet SWF stöds inte längre av någon av de största leverantörerna och har ersatts med HTML5 banners för korrektur. </p> <p>Mer information om skillnaderna mellan de tillgängliga korrekturläsarna finns i <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Skillnader mellan Web Proofing Viewer och Desktop Proofing Viewer - översikt</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

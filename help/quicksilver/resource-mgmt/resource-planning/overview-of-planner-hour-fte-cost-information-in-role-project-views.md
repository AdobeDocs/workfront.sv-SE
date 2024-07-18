---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: Översikt över timmar, heltidsanställda och kostnadsinformation i projekt- och rollvyerna i resursplaneraren
description: Översikt över timmar, heltidsanställda och kostnadsinformation i projekt- och rollvyerna i resursplaneraren
author: Alina
feature: Resource Management
exl-id: 76de1945-3f19-4c91-801c-07dc79e646ad
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: tm+mt
source-wordcount: '2977'
ht-degree: 0%

---

# Översikt över timmar, heltidsanställda och kostnadsinformation i projekt- och rollvyerna i resursplaneraren

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this came from the budget-resources-project-role-views-resource-planner article)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: relink all articles pointing to this section to the new article)</p>
-->

Resursplaneringens huvudfunktion är att budgetera dina resurser för det arbete de måste utföra i ett projekt. Du kan visa resursernas tillgängliga tid och tilldela deras tid till de projekt där de har tilldelats.

Mer information om budgeteringsresurser i resursplaneraren finns i [Budgetresurser i resursplaneraren med projekt- och rollvyerna](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)

I den här artikeln beskrivs några av de nyckelbegrepp som du behöver känna till innan du börjar budgetera dina resurser i Resursplaneraren.

## Översikt över budgetresurser

Tänk på följande när du budgeterar resurser med hjälp av resursplaneraren:

* Du kan budgetera allokeringen av dina resurser genom att ange ett antal timmar, heltidsekvivalenter eller kostnader som dina resurser kan använda för att slutföra arbetet med projekt. När du budgeterar tid eller kostnad för en resurs minskar antalet tillgängliga timmar, heltidsekvivalenter eller kostnaden för resursen med det budgeterade beloppet. Detta resulterar i att beloppen Tillgängliga timmar, Heltidsekvivalenter eller Kostnad för de projekt som följer efter projektet som du budgeterar för minskar för de användarna och rollerna i dessa projekt.

  >[!IMPORTANT]
  >
  >Du kan budgetera dina resurser för en period på 15 år. Om du budgeterar resurser för ett projekt med en varaktighet på mer än 15 år kanske budgetinformationen inte är korrekt.

* Du kan budgetera timmar, heltidsekvivalenter eller kostnad för dina resurser för alla tidsbildrutor som visas i resursplaneraren, oberoende av tidslinjen i projektet. Om du till exempel vill ange att dina resurser kanske inte är tillgängliga under tidslinjen för projektet (där de är kopplade till Planerade timmar), men de kan vara tillgängliga under en annan tid, kan du göra det genom att budgetera dem för tidsramar där Planerade timmar är noll, om det är när de blir tillgängliga för arbete. Du kan ändra tidslinjen för projektet manuellt så att den matchar resurstillgängligheten när du har gjort detta.

  >[!NOTE]
  >
  >Vi rekommenderar att du budgeterar timmar, heltidsekvivalenter eller kostnad manuellt för jobbroller eller för användare först. Du kan bara använda de automatiska alternativen för att budgetera tid för dina projekt och resurser när du är säker på att beloppet för Planerade timmar, FTE eller Kostnad alltid ska matcha dina budgeterade timmar, FTE eller Kostnad.\
  >Mer information om hur du använder de automatiska alternativen för budgetering i Resursplanering finns i avsnittet Budgetprojekt och roller automatiskt i artikeln [Granska resurstillgänglighet och allokering med Adobe Workfront Resursplanering](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

* FTE eller kostnader för budgetering är identiska med budgeteringstimmar, där Adobe Workfront använder FTE och kostnadsvärden i stället för timmar för de resurser du budgeterar.

  Mer information om hur kostnader beräknas i resursplaneraren finns i [Beräkna kostnader i resursplaneraren](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

* Budgeteringsallokeringar för dina resurser i resursplaneraren görs på följande sätt:

   * Manuellt

     eller

   * Automatiskt, genom att använda projekt- och rollalternativen i vyerna **Visa efter projekt** och **Visa efter roll**.

  Mer information finns i [Budgetresurser i resursplaneraren med projekt- och rollvyerna](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

* När en användare ändrar jobbroller, tas bort, inaktiveras eller tas bort från en resurspool ändras inte timmarna som har budgeterats för rollen och de omfördelas till de återstående användarna i rollen. Om ingen användare längre är associerad med jobbrollen blir de budgeterade timmarna för rollen noll.

Mer information om projekt- och rollalternativen finns i avsnittet [Förstå värdena för Timmar, FTE och Kostnad i resursplaneraren](#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner) i den här artikeln.

## Förstå värdena för timmar, heltidsekvivalenter och kostnad i resursplaneraren {#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this needs to be broken into its own article and leave here just the how-to: see this article: overview-of-planner-hour-fte-cost-information-in-role-project-views)</p>
-->

Innan du budgeterar dina resurser och uppdaterar informationen om budgeterade timmar i resursplaneraren måste du känna till följande koncept

* **Planerade timmar, FTE eller kostnad**: Det arbete som måste utföras enligt definition för aktiviteter och problem.
* **Tillgängliga timmar, FTE eller kostnad**: Den tid som användare eller jobbroller är tillgängliga för arbete, enligt scheman som är associerade med användarna.

Den här informationen visas i resursplaneraren för varje resurs (användare eller roll) och för varje projekt.

Mer information om vad som visas i projekt- och rollvyerna för projektet finns i artikeln [Resursplaneringsöversikt](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Mer information om hur kostnader beräknas i resursplaneraren finns i artikeln [Beräkna kostnader i resursplaneraren](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

>[!NOTE]
>
>Budgetering efter kostnad är identiskt med budgetering per timme eller heltidsekvivalent, men du måste förstå hur Workfront beräknar kostnad för resursplaneraren.
>
>Mer information om hur kostnader beräknas i resursplaneraren finns i artikeln [Beräkna kostnader i resursplaneraren](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

I följande tabeller visas information om tilldelning och tillgänglighet som visas i resursplaneraren när du använder antingen projektet eller rollvyn. Du kan visa den här informationen via Timmar, FTE eller Kostnad:

* [AVL (tillgänglig) kolumn](#the-avl-available-column)
* [PLN-kolumnen (planerad)](#the-pln-planned-column)
* [BDG-kolumnen (budgeterad)](#the-bdg-budgeted-column)
* [VAR-kolumnen (varians)](#the-var-variance-column)
* [NET-kolumnen](#the-net-column)

### Kolumnen AVL (tillgänglig) {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Visas av</strong> </td> 
   <td><strong>Beskrivning</strong> </td> 
  </tr> 
  <tr> 
   <td>Projekt </td> 
   <td> <p>Det totala antalet timmar, heltidsekvivalenter eller kostnader för vilka alla användare i projektet är tillgängliga att arbeta enligt sitt schema för den valda tidsramen. </p> </td> 
  </tr> 
  <tr> 
   <td>Roll</td> 
   <td> <p>Totalt antal timmar, heltidsanställda eller kostnader som alla användare som är associerade med den här rollen är tillgängliga att arbeta för enligt sitt schema och deras <strong>procentandel FTE-tillgänglighet</strong> för den specifika rollen, för den valda tidsramen. </p> <p>Tänk på följande: </p> 
    <ul> 
     <li>Om ingen användare är associerad med en jobbroll är värdet för Tillgängliga timmar för jobbrollen noll. </li> 
     <li>Om en användare är associerad med en primär jobbroll, men <strong>procentandelen FTE-tillgänglighet</strong> för rollen är 0 %, är värdet för tillgängliga timmar för jobbrollen noll.</li> 
     <li>Om användaren är associerad med andra roller och <strong>procentandelen FTE-tillgänglighet</strong> för rollerna är 0 %, visas inte de andra rollerna i resursplaneraren och användaren visas bara under sin primära roll.</li> 
    </ul> <p>Mer information om <strong>procentandelen FTE-tillgänglighet</strong> för en jobbroll finns i artikeln <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Redigera en användares profil</a>.</p> <p>Mer information om hur tillgängligheten för jobbroller beräknas i resursplaneraren finns i avsnittet Beräkna tillgängliga timmar och FTE för en jobbroll i resursplaneraren i artikeln <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Översikt över beräkning av timmar och FTE för användare och roller i resursplaneraren</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Användare</td> 
   <td> <p>Timmar, heltidsanställda eller kostnad som användaren kan arbeta enligt sitt schema för den valda tidsramen. Det här numret subtraherar timmarna som är associerade med följande:</p> 
    <ul> 
     <li>schemaläggningsundantag</li> 
     <li>användarens lediga tid</li> 
     <li>timmar budgeterade för andra projekt. </li> 
    </ul> <p>Tillgängliga timmar, heltidsanställda eller kostnader för en användare ändras enligt följande: </p> 
    <ul> 
     <li>hur deras schema och FTE beräknas baserat på inställningarna för resurshantering på systemnivå.<br><p>Mer information om hur du beräknar tillgängligheten för användare och jobbroller finns i artikeln <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Översikt över beräkning av timmar och FTE för användare och roller i resursplaneraren</a>.</p>
     Mer information om hur du konfigurerar inställningar för resurshantering i Workfront finns i <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Konfigurera inställningar för resurshantering</a></li> 
    </ul> 
    <ul> 
     <li><strong>Projektplaneringsprioritet</strong>, om användaren har budgeterats för arbete.<br>Mer information om hur Project Planning Priority påverkar användarens tillgängliga timmar finns i <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">Navigeringsöversikt för resursplanering </a>. </li> 
    </ul> <p>Om användaren är schemalagd för inaktivering är tillgängliga timmar, heltidsekvivalenter eller kostnad för dagar efter inaktiveringsdatumet noll. <br>Mer information om hur du inaktiverar användare finns i artikeln <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Inaktivera eller återaktivera en användare</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Kolumnen PLN (planerad) {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Visas av</strong> </td> 
   <td><strong>Beskrivning</strong> </td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td> <p>Totalt antal planerade timmar, heltidsekvivalenter eller kostnader från alla jobbroller eller användare som listas under projektet, inklusive i avsnitten <strong>Ingen roll</strong> eller <strong>Ingen användare</strong>, för den valda tidsramen och som visas på fliken Projektinformation för projektet. </p> <p><b>ANMÄRKNING</b>

Manuella justeringar av dagliga användartilldelningar kan ändra värdet för planerade timmar varje vecka, månad eller kvartal i resursplaneraren. Du kan justera dagliga användarallokeringar för uppgifter och ärenden manuellt med hjälp av Utjämning av arbetsbelastning. Mer information finns i <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Hantera användartilldelningar i Utjämning av arbetsbelastning</a>.</p> </td>
</tr> 
  <tr> 
   <td>Roll</td> 
   <td> <p>Totalt antal planerade timmar från alla uppgifter som tilldelats rollen, under den valda tidsramen. </p> <p>Avsnittet <strong>Ingen roll</strong> visar de planerade timmarna som är kopplade till aktiviteter som antingen inte har tilldelats, har tilldelats till team (vars timmar anges i avsnittet <strong>Ingen användare</strong>) eller har tilldelats till användare som inte är kopplade till en jobbroll. </p> </td> 
  </tr> 
  <tr> 
   <td>Användare</td> 
   <td> <p>Planerade timmar från alla uppgifter som tilldelats användaren i en viss roll, under den valda tidsramen. </p> <p>Avsnittet <strong>Ingen användare</strong> visar de planerade timmarna som är kopplade till aktiviteter som är antingen ej tilldelade eller tilldelade till team. </p> </td> 
  </tr> 
 </tbody> 
</table>

Tänk på följande när du visar Planerade timmar:

* Även om du inte kan se information om uppgiftsallokeringar i resursplaneraren i projekt- och rollvyerna, kommer antalet planerade timmar från de planerade timmarna för aktiviteterna i projekten.
* Planerade timmar fördelas jämnt till varje dag under aktiviteternas varaktighet, för varje resurs som tilldelats dem. Aktivitetens varaktighet baseras på planerade start- och slutförandedatum för aktiviteten och omfattar alla kalenderdagar inom den tidsperioden.\
  Workfront tar hänsyn till schemat för användare eller projekt när Planerade timmar distribueras till användare eller projekt. I det här fallet fördelas planerade timmar jämnt till varje dag under aktiviteternas längd, exklusive helger, lediga dagar och schemaläggningsundantag.\
  Om du till exempel visar resursplaneraren efter vecka och du har uppgifter som sträcker sig över flera veckor i projekt, beror antalet planerade timmar per vecka på hur många dagar inom den veckan som ingår i aktivitetens varaktighet. Detta fungerar på liknande sätt när resursplaneraren visas efter månad eller kvartal och när uppgifterna sträcker sig över flera månader eller kvartal.\
  Veckoslutsdagar, schemaundantag och lediga dagar exkluderas från denna distribution.
* Följande kategorier av uppgifter ingår i beräkningen av planerade timmar för varje resurs:

   * uppgifter som tilldelats användare i Resurspooler, jobbroller eller team i projektet\
     Om uppgifter tilldelas team visas deras allokering under avsnitten **Ingen roll** och **Ingen användare**. Du kan se de planerade timmar som är kopplade till team, men du kan inte budgetera timmarna eftersom inga roller eller användare är kopplade till uppgifterna.

   * ej tilldelade uppgifter

* Planerade timmar i resursplaneraren inkluderar inte Planerade timmar som är associerade med följande:

   * överordnade uppgifter
   * uppgifter som tilldelats användare utan resurspooler
   * problem när inställningen **Inkludera timmar från problem** är inaktiverad.

* Planerade timmar visas inte i resursplaneraren om aktivitetens varaktighet är noll.
* Planerade timmar som är associerade med inaktiverade användare visas inte.

### Kolumnen BDG (budgeterad) {#the-bdg-budgeted-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Visas av</strong> </td> 
   <td><strong>Beskrivning</strong> </td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td> <p>En manuell inmatning som beräknar hur många timmar, heltidsekvivalenter eller kostnad du budgeterar för ett projekt för en vald tidsram. </p> <p>I projektvyn fördelas de timmar du budgeterar för projektet till de jobbroller som listas under projektet. Det planerade timbeloppet för varje roll avgör hur budgeterade timmar fördelas till rollerna. Budgeterade timmar fördelas till roller med högre värden för Planerade timmar. </p> <p>I rollvyn fördelas inte de timmar du budgeterar för projektet till roller eller användare i projektet. </p> </td> 
  </tr> 
  <tr> 
   <td>Roll</td> 
   <td> <p>En manuell inmatning som beräknar hur många timmar du budgeterar för en roll, för en vald tidsram. </p> <p>Om ingen användare är associerad med jobbrollen kan du inte beräkna budgeterade timmar för jobbrollen. </p> <p>I rollvyn fördelas de timmar du budgeterar för rollen till de projekt som listas under rollen. Det planerade timbeloppet för varje projekt avgör hur budgeterade timmar fördelas till projekten. Budgeterade timmar fördelas till projekt med högre värden för Planerade timmar.</p> <p>I projektvyn fördelas inte de timmar du budgeterar för rollen till projekten eller användarna som är associerade med rollen. </p> </td> 
  </tr> 
  <tr> 
   <td>Användare</td> 
   <td> <p>En manuell inmatning som beräknar hur många timmar du budgeterar för en användare för en vald tidsram. </p> <p> <p><b>OBS!</b>   Du kan beräkna budgeterade timmar för användare som inte är tilldelade till aktiviteter, men som är kopplade till en resurspool i ett projekt, eftersom dessa användare också visas i resursplaneraren. De planerade timmarna ska dock vara noll om de inte har tilldelats aktiviteter. </p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Tänk på följande när du arbetar med budgeterade timmar:

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(Duplicated below ??)
</MadCap:conditionalText>
-->

* Du kan bara budgetera resurser när du har behörigheten Redigera för Resurshantering och Ekonomi och Hantera ekonomi för projekten.

  Mer information om åtkomsten som krävs för budgetresurser finns i artikeln [Åtkomst krävs för att budgetera resurser i Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* Som standard är budgeterade timmar i resursplaneraren noll för alla resurser och för alla projekt.
* Du kan beräkna budgeterade timmar manuellt för användare och roller, eller så kan du använda en av länkarna i projekt- eller jobbrollens **Fler**-menyer för att uppdatera dem enligt antalet planerade timmar.\
  Mer information om projekt- och rollalternativ finns i avsnittet [Översikt över timmar, heltidsekvivalenter och kostnadsinformation i projekt- och rollvyerna för resursplaneraren](#Budget) i den här artikeln.

* Den minsta tidsperioden du kan budgetera timmar, heltidsekvivalenter eller Kostnad för är en vecka. Du kan inte budgetera timmar, heltidsekvivalenter eller kostnad för en dag.
* Budgeterade timmar fördelas jämnt till varje dag under varaktigheten för uppgifter, för varje resurs som tilldelats dem. Aktivitetens varaktighet baseras på planerade start- och slutförandedatum för aktiviteten och omfattar alla kalenderdagar inom den tidsperioden.\
  Workfront tar hänsyn till schemat för användaren eller projektet när budgeterade timmar fördelas till användare eller projekt. I det här fallet fördelas budgeterade timmar jämnt till varje dag under varaktigheten för uppgifter exklusive helger, men inklusive undantag för tid och schema.\
  Om du till exempel visar resursplaneraren efter vecka och har uppgifter som sträcker sig över flera veckor, beror antalet budgeterade timmar per vecka på hur många dagar inom den veckan som ingår i aktivitetens varaktighet. Veckoslutsdagar exkluderas från denna distribution. Detta fungerar på liknande sätt när resursplaneraren visas efter månad eller kvartal och när uppgifterna sträcker sig över flera månader eller kvartal.

* Du kan rapportera om budgeterade timmar genom att välja Budgeterad timme som rapportobjekt för en ny rapport.\
  Mer information om vilka objekt du kan rapportera om i Workfront finns i avsnittet&quot;Rapport om objekt&quot; i artikeln [Förstå objekt i Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
  Mer information om hur du skapar en budgeterad timrapport finns i artikeln [Rapport: Budgeterad timme](../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md).

* Timmar som tidigare budgeterats för användare som senare inaktiverades visas inte.

### Kolumnen VAR (varians) {#the-var-variance-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Visas av</strong> </td> 
   <td><strong>Beskrivning</strong> </td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td> <p>Timme, FTE eller Kostnadsvarians visar om du har tillräckligt många budgeterade timmar för projektet för att kunna utföra alla planerade timmar för projektet. </p> <p>Projekttimmen, heltidsekvivalenten eller kostnadsvariansen beräknas med följande formel:</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Roll</td> 
   <td> <p>Timme, FTE eller Kostnadsvarians visar om du har tillräckligt med budgeterade timmar, FTE eller kostnad för att rollen ska kunna utföra de planerade timmar som tilldelats den. </p> <p>Rolltimmen, FTE eller kostnadsvariansen beräknas med följande formel:</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Användare</td> 
   <td> <p>Timmar, FTE eller Kostnadsvariant visar om du har tillräckligt många budgeterade timmar för att användaren ska kunna genomföra de planerade timmarna som tilldelats dem. </p> <p>Användartimmar, FTE eller Kostnadsvarians beräknas med följande formel:</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>När Timmar, heltidsekvivalenter eller kostnadsvarianter visas i rött har du uppskattat färre budgeterade timmar än de planerade timmarna för det faktiska arbete som behöver slutföras. I det här fallet kanske inte de budgeterade timmarna räcker till för att slutföra arbetet.

### NET-kolumnen  {#the-net-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Visas av</strong> </td> 
   <td><strong>Beskrivning</strong> </td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td> 
    <div> 
     <p>I projektet Nettotimmar, FTE eller Kostnad kan något av följande visas: </p> 
     <ul> 
      <li> <p>Skillnaden mellan tillgänglig tid eller kostnad och budgeterad tid eller kostnad för projektet:</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p>Skillnaden mellan tillgänglig tid eller kostnad och planerad tid eller kostnad för projektet när värdena för Använd planerad (PLN) i NETTOberäkningar är aktiverade: </p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code>
      </p>

<p><b>TIPS</b></p>        
  <p>Det här alternativet används bara när du anpassar vyn i avsnittet Visa markerade objekt.</p>
  <p>Mer information finns i <a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" >Granska resurstillgänglighet och allokering med Adobe Workfront resursplanerare</a> </p> 
      </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>Roll</td> 
   <td> 
    <div> 
     <p>Rollen Nettotimmar, FTE eller Kostnad kan visa något av följande: </p> 
     <ul> 
      <li> <p>Skillnaden mellan tillgänglig tid eller kostnad och budgeterad tid eller kostnad för rollen:</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>Skillnaden mellan tillgänglig tid eller kostnad och planerad tid eller kostnad för rollen när värdet för Använd planerad (PLN) i NETTOberäkningar är aktiverat:</span> </p> <p><span><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <p><b>TIPS</b> <span>

Det här alternativet används bara när du anpassar vyn i avsnittet Visa markerade objekt.</span> </p> <p><span>Mer information finns i </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Granska resurstillgänglighet och allokering med Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr> 
  <tr> 
   <td>Användare</td> 
   <td> 
    <div> 
     <p>Användaren kan visa följande Net Hours, FTE eller Cost: </p> 
     <ul> 
      <li> <p>Skillnaden mellan Tillgänglig tid eller kostnad och Budgeterad tid eller kostnad för användaren:</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>Skillnaden mellan Tillgänglig tid eller kostnad och Planerad tid eller kostnad för användaren när värdet för Använd planerad (PLN) i NET-beräkningar är aktiverat:</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <p><b>TIPS</b> <span>

Det här alternativet används bara när du anpassar vyn i avsnittet Visa markerade objekt.</span> </p> <p><span>Mer information finns i </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Granska resurstillgänglighet och allokering med Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**När NET-timmar, FTE eller Kostnad visas i rött finns det inte tillräckligt med tillgänglig tid eller budget för att täcka antingen budgeterad** eller planerad tid eller kostnad som är associerad med arbetet. I det här fallet är resurserna överallokerade.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the table below is ideal but it does not transfer to Markdown)</p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Column Name (Hours, FTE, or Cost)</strong> </td>
<td><strong>Displayed by</strong> </td>
<td><strong>Description</strong> </td>
</tr>
<tr>
<td rowspan="3">AVL <br>(Available Hours, FTE, or Cost)</td>
<td>Project </td>
<td> <p>The total of Hours, FTEs, or Cost for which all the users on the project are available to work according to their schedule, for the time frame selected. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Hours, FTEs, or Cost for which all the users associated with this role are available to work according to their schedule and their <strong>Percentage of FTE Availability</strong> for that specific role, for the time frame selected. </p> <p>Consider the following: </p>
<ul>
<li>If no user is associated with a job role, then the value for the Available Hours for the job role is zero. </li>
<li>If a user is associated with a Primary Job Role, but the <strong>Percentage of FTE Availability</strong> for the role is 0%, the job role Available Hours value is zero.</li>
<li>If the user is associated with Other Roles and the <strong>Percentage of FTE Availability</strong> for the roles is 0%, the Other Roles are not listed in the Resource Planner and the user displays only under their Primary Role.</li>
</ul> <p>For more information about the <strong>Percentage of FTE Availability</strong> for a job role, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> <p>For more information about how the job role availability is calculated in the Resource Planner, see the section "Calculate the Available Hours and FTE for a job role in the Resource Planner" in the article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>Hours, FTEs, or Cost that the user is available to work, according to their schedule, for the time frame selected. This number subtracts the hours associated with the following:</p>
<ul>
<li>schedule exceptions</li>
<li>time off of the user</li>
<li>hours budgeted for other projects. </li>
</ul> <p>The Available Hours, FTEs, or Cost for a user change according the following: </p>
<ul>
<li>how their schedule and FTE are calculated based on the Resource Management Preferences at the system level.<br>For more information about calculating user and job role availability, see the article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</li>
</ul>
<ul>
<li>the <strong>Project Planning Priority</strong>, if the user is budgeted for work.<br>For more information about how Project Planning Priority affects the Available Hours of a user, see <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">Resource Planner navigation overview </a>. </li>
</ul> <p>If the user is scheduled for deactivation, the Available Hours, FTEs, or Cost for the days after the deactivation date are zero. <br>For more information about deactivating users, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</p> </td>
</tr>
<tr>
<td rowspan="4">PLN <br>(Planned Hours, FTE, or Cost)</td>
<td>Project</td>
<td> <p>The total of the Planned Hours, FTEs, or Cost from all the job roles or users listed under the project, including in the <strong>No Role</strong> or <strong>No User</strong> sections, for the time frame selected, and as displayed in the Project Details tab of the project. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of the Planned Hours from all the tasks assigned to the role, during the time frame selected. </p> <p>The <strong>No Role</strong> section will show the Planned Hours associated with tasks that are either unassigned, assigned to teams (whose hours are listed in the <strong>No User</strong> section), or assigned to users who are not associated with a job role. </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>The Planned Hours from all the tasks assigned to the user in a specific role, during the time frame selected. </p> <p>The <strong>No User</strong> section will show the Planned Hours associated with tasks that are either unassigned or assigned to teams. </p> </td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when viewing Planned Hours:</p>
<ul>
<li>Although you cannot see information about task allocations in the Resource Planner in the Project and Role views, the amount of Planned Hours comes from the Planned Hours on the tasks in the projects. </li>
<li> <p>Planned Hours are equally distributed to each day within the Duration of tasks, for each resource assigned to them. The task Duration is based on the task Planned Start and Completion Dates and includes every calendar day within that period of time.<br>Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks excluding weekends, time-off days, and schedule exceptions.<br>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li>
<li> The following categories of tasks are included in calculating the Planned Hours for each resource:
<ul>
<li> tasks assigned to users in Resource Pools, job roles, or teams on the project<br>If tasks are assigned to teams, their allocation will appear under <strong>No Role</strong> and <strong>No User</strong> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks. </li>
<li> unassigned tasks </li>
</ul></li>
<li> Planned Hours in the Resource Planner do not include Planned Hours associated with the following:
<ul>
<li>parent tasks</li>
<li>tasks assigned to users with no Resource Pools</li>
<li>issues, when the <strong>Include hours from Issues</strong> setting is disabled.</li>
</ul></li>
<li>Planned Hours do not display in the Resource Planner if the task Duration is zero.</li>
<li>Planned Hours associated with deactivated users do not display. </li>
</ul> </td>
</tr>
<tr>
<td rowspan="4"> BDG <br>(BudgetedHours, FTE, or Cost) </td>
<td>Project</td>
<td> <p>A manual entry to estimate how many hours, FTE, or Cost you budget for a project, for a selected time frame. </p> <p>In the Project view, the hours you budget for the project are distributed to the job roles listed under the project. The amount of Planned Hours for each role determines how the Budgeted Hours are distributed to the roles. The Budgeted Hours are distributed to the roles with higher Planned Hours values. </p> <p>In the Role view, the hours you budget for the project are not distributed to the roles or the users on the project. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>A manual entry to estimate how many hours you budget for a role, for a selected time frame. </p> <p>If no user is associated with the job role, you cannot estimate the Budgeted Hours for the job role. </p> <p>In the Role view, the hours you budget for the role are distributed to the projects listed under the role. The amount of Planned Hours for each project determines how the Budgeted Hours are distributed to the projects. The Budgeted Hours are distributed to the projects with higher Planned Hours values.</p> <p>In the Project view, the hours you budget for the role are not distributed to the projects or the users associated with the role. </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>A manual entry to estimate how many hours you budget for a user, for a selected time frame. </p> <p> <note type="note">  You can estimate the Budgeted Hours for users who are not assigned to tasks, but are associated with a Resource Pool on a project because these users also appear in the Resource Planner. Their Planned Hours should be zero, however, if they are not assigned to tasks.
</note> </p> </td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when working with Budgeted Hours:</p> <li>
<ul>
<li> <p>You can budget resources only when you have Edit access to Resource Management and Financial Data and Manage Finance permissions on the projects.</p> <p>For information about the access needed for budgeting resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this bullet: Duplicated below)</p>
</li>
</ul> </li>
<ul>
<li>By default, the Budgeted Hours in the Resource Planner are zero for all resources and for all the projects.</li>
<li>You can manually estimate the Budgeted Hours for users and roles, or you can use one of the links in the Project or Job Role <strong>More</strong> menus to update them according to the number of Planned Hours.<br>For more information about project and role options, see the section <a href="#Budget" class="MCXref xref">Overview of hours, FTE, and cost information in the Project and&nbsp;Role views of the Resource Planner</a> in this article.</li>
<li> The smallest period of time you can budget hours, FTE, or Cost for is a week. You cannot budget hours, FTE, or Cost for a day. </li>
<li> Budgeted Hours are equally distributed to each day within the Duration of tasks, for each resource assigned to them. The task Duration is based on the task Planned Start and Completion Dates and includes every calendar day within that period of time. <br>Workfront takes into account the schedule of the user or of the project when distributing Budgeted Hours to users or projects. In this case, Budgeted Hours are equally distributed to each day within the Duration of tasks excluding weekends, but including time-off and schedule exceptions. <br>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks, the number of Budgeted Hours per week depends on how many days within that week are part of the task Duration. Weekend days are excluded from this distribution. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters. </li>
<li>You can report on Budgeted Hours, by selecting Budgeted Hour as your report object for a new report.<br>For information about what objects you can report on in Workfront, see the section "Report on objects" in the article <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. <br>For information about building a Budgeted Hour report, see the article <a href="../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Report: Budgeted Hour</a>.</li>
<li>Hours previously budgeted for users who were later deactivated do not display. <br></li>
</ul> </td>
</tr>
<tr>
<td rowspan="4">VAR <br>(Hour, FTE, or ,Cost Variance)</td>
<td>Project</td>
<td> <p>The Hour, FTE, or Cost Variance shows whether you have enough Budgeted Hours for the project to accomplish all the Planned Hours for the project. </p> <p>The Project Hour, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The Hour, FTE, or Cost Variance shows whether you have enough Budgeted Hours, FTE, or Cost for the role to accomplish the Planned Hours assigned to it. </p> <p>The Role Hour, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>The Hours, FTE, or Cost Variance shows whether you have enough Budgeted Hours for the user to accomplish the Planned Hours assigned to them. </p> <p>The User Hours, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td colspan="2"> <note type="note">
When the Hours, FTE, or Cost Variance displays in red, you have estimated less Budgeted Hours than the Planned Hours of the actual work that needs to be completed. In this case, the Budgeted Hours might not be enough to complete the work.
</note> </td>
</tr>
<tr>
<td rowspan="4"> NET <br>(Net Hours, FTEs, or Cost) </td>
<td>Project</td>
<td>
<div>
<p>The project Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the project:</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the project, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td>Role</td>
<td>
<div>
<p>The role Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the role:</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the role, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span class="preview"><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td>User</td>
<td>
<div>
<p>The user Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the user:</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the user, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td colspan="2"> <note type="note">
<span>When the NET Hours,&nbsp;FTE, or Cost display in red, there is not enough Available time or budget to cover either the Budgeted</span> or the Planned time or cost associated with the work. In this case, the resources are overallocated.
</note> </td>
</tr>
</tbody>
</table>
-->

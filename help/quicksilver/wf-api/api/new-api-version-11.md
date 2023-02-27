---
content-type: api
navigation-topic: api-navigation-topic
title: Nyheter i API-version 11
description: ReportableBudgedHour har lagts till i Adobe Workfront API som en resurs för rapportering. Den innehåller referensfält, kärnfält och standardfält som inte finns i BudgetHour.
author: Becky
feature: Workfront API
exl-id: b8826dc6-9791-49f6-923d-5a0c5392a8b0
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '3600'
ht-degree: 0%

---

# Nyheter i API-version 11

* [Tillagda resurser](#added-resources)
* [Borttagna resurser](#removed-resources)
* [Ändrade resurser](#modified-resources)

## Tillagda resurser {#added-resources}

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasaccessrule" class="MCXref xref">LoginAsAccessRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasadditionalrule" class="MCXref xref">LoginAsAdditionalRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginassettings" class="MCXref xref">LoginAsSettings</a> </li>
  -->

* [RapporterbarBudgeteradTimme](#reportablebudgetedhour)

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginasaccessrule">LoginAsAccessRule</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">accessExpirationDate</li> 
     <li style="font-weight: bold;">accessorID</li> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">userID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referensfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">accessor</li> 
     <li style="font-weight: bold;">kund</li> 
     <li style="font-weight: bold;">användare  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Kärnfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginasadditionalrule">LoginAsAdditionalRule</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">loginAsSettingsID</li> 
     <li style="font-weight: bold;">objID</li> 
     <li style="font-weight: bold;">objObjCode  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referensfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">kund  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Kärnfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginassettings">LoginAsSettings</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">licenseTypes</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">restrictedLoginAs  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referensfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">kund  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Samlingsfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">additionalRules</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Kärnfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### RapporterbarBudgeteradTimme {#reportablebudgetedhour}

ReportableBudgedHour har lagts till i Adobe Workfront API som en resurs för rapportering. Den innehåller referensfält, kärnfält och standardfält som inte finns i BudgetHour.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">allokeringsdatum </p> <p>Tilldelningsdatumet är den första dagen (en söndag) i veckan som du budgeterade timmarna för i resursplaneraren.</p> </li> 
     <li> <p style="font-weight: bold;">BudgeteradTimme </p> <p>Budgeterade timmar är timmar som resurshanteraren budgeterar för det arbete som resurser måste slutföra i projekt</p> </li> 
     <li> <p style="font-weight: bold;">ID </p> <p>Det unika Workfront-ID som tilldelats ett specifikt Rapporteringsbart timobjekt.</p> </li> 
     <li style="font-weight: bold;">planeradeBudgeteradeTimmar </li> 
     <li> <p style="font-weight: bold;">projectID </p> <p>Det unika Workfront-id som tilldelats ett specifikt projekt.</p> </li> 
     <li> <p style="font-weight: bold;">roleID</p> <p>Det unika Workfront-ID som tilldelats en specifik jobbroll.</p> </li> 
     <li> <p style="font-weight: bold;">userID</p> <p>Det unika Workfront-ID som tilldelats en viss användare.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referensfält</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">projekt</p> <p>Det projekt som en ReportableBudgetedHour är associerad med.</p> </li> 
     <li> <p style="font-weight: bold;">roll</p> <p>Jobbrollen som en ReportableBudgetedHour är associerad med.</p> </li> 
     <li> <p style="font-weight: bold;">användare</p> <p>Användaren som en ReportableBudgetedHour är associerad med.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Kärnfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">name</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standardfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">name</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Operationer</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">COUNT</li> 
     <li style="font-weight: bold;">GET</li> 
     <li style="font-weight: bold;">RAPPORT </li> 
     <li style="font-weight: bold;">SÖK</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Borttagna resurser {#removed-resources}

Inga resurser togs bort för API v11.

## Ändrade resurser {#modified-resources}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li><a href="#accesslevelpermissions" class="MCXref xref">AccessLevelPermissions</a> </li> 
     <li><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </li> 
     <li><a href="#accessrule" class="MCXref xref">AccessRule</a> </li> 
     <li><a href="#approval" class="MCXref xref">Godkännande</a> </li> 
     <li><a href="#approvalpath" class="MCXref xref">ApprovalPath</a> </li> 
     <li><a href="#approvalprocess" class="MCXref xref">ApprovalProcess</a> </li> 
     <li><a href="#assignment" class="MCXref xref">Tilldelning</a> </li> 
     <li><a href="#baselinetask" class="MCXref xref">OriginalplanAktivitet</a> </li> 
     <li><a href="#category" class="MCXref xref">Kategori</a> </li> 
     <li><a href="#company" class="MCXref xref">Företag</a> </li> 
     <li><a href="#customenum" class="MCXref xref">CustomEnum</a> </li> 
     <li><a href="#customer" class="MCXref xref">Kund</a> </li> 
     <li><a href="#customerpreferences" class="MCXref xref">CustomerPreferences</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#docmetadatalinkgroup" class="MCXref xref">DocMetadataLinkGroup</a> </li> 
     <li><a href="#document" class="MCXref xref">Dokument</a> </li> 
     <li><a href="#iteration" class="MCXref xref">Upprepning</a> </li> 
     <li><a href="#layout-template" class="MCXref xref">Layoutmall</a> </li> 
     <li><a href="#milestonepath" class="MCXref xref">MilstolpePath</a> </li> 
     <li><a href="#note" class="MCXref xref">Anteckning</a> </li> 
     <li><a href="#optask" class="MCXref xref">OpTask</a> </li> 
     <li><a href="#parameter" class="MCXref xref">Parameter</a> </li> 
     <li><a href="#portfolio" class="MCXref xref">Portfolio</a> </li> 
     <li><a href="#program" class="MCXref xref">Program</a> </li> 
     <li><a href="#project" class="MCXref xref">Projekt</a> </li> 
     <li><a href="#proofapproval" class="MCXref xref">KorrekturGodkännande</a> </li> 
     <li><a href="#queuedef" class="MCXref xref">QueueDef</a> </li> 
     <li><a href="#reservedtime" class="MCXref xref">ReservedTime</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#resourceplannerfilter" class="MCXref xref">Resursplaneringsfilter</a> </li> 
     <li><a href="#risk" class="MCXref xref">risk</a> </li> 
     <li><a href="#scheduledreport" class="MCXref xref">SchemalagdRapport</a> </li> 
     <li><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </li> 
     <li><a href="#task" class="MCXref xref">Uppgift</a> </li> 
     <li><a href="#team" class="MCXref xref">Team</a> </li> 
     <li><a href="#template" class="MCXref xref">Mall</a> </li> 
     <li><a href="#templateassignment" class="MCXref xref">TemplateAssignment</a> </li> 
     <li><a href="#templatetask" class="MCXref xref">TemplateTask</a> </li> 
     <li><a href="#timesheet" class="MCXref xref">Tidrapport</a> </li> 
     <li><a href="#update" class="MCXref xref">Uppdatera</a> </li> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#user" class="MCXref xref">User</a> </li>
     --> 
     <li><a href="#usernote" class="MCXref xref">UserNote</a> </li> 
     <li><a href="#work" class="MCXref xref">Arbete </a> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### AccessLevelPermissions {#accesslevelpermissions}

Ett AccessLevelPermissions-objekt representerar en uppsättning behörigheter. Den här behörighetsuppsättningen kan sedan kopplas till en åtkomstnivå.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> <p>Följande fält har lagt till det möjliga värdet BUDGETING_INFORMATION. Detta gör att användare med behörighet kan redigera prioriteringar och budgettimmar i planeraren.</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRequest {#accessrequest}

Om en användare inte har åtkomst till ett objekt i Workfront som de behöver kan de begära åtkomst till det objektet. AccessRequest-objektet representerar denna begäran.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">åtgärd</p> <p>Det möjliga värdet BUDGETING_INFORMATION har lagts till. Detta gör att användare med behörighet kan redigera prioriteringar och budgettimmar i planeraren.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRule {#accessrule}

Ett AccessRule-objekt representerar en regeluppsättning med anpassade åtkomstnivåer som avgör hur användare kan dela projekt som de skapar.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> <p>Följande fält har lagt till det möjliga värdet BUDGETING_INFORMATION. Detta gör att användare med behörighet kan redigera prioriteringar och budgettimmar i planeraren.</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Godkännande {#approval}

En viss arbetsuppgift, till exempel en uppgift, ett dokument eller en tidrapport, kan kräva att en ansvarig eller annan användare signerar arbetsposten. Ett Approval-objekt representerar åtgärden för signering av en arbetsuppgift.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Direktfält<p style="font-weight: normal;">Följande fält lade till validerarna AT_DATE_BEFORE_YEAR och AT_DATE_AFTER_YEAR. Dessa validerare anger att datum för associerade objekt inte kan anges före år 1900 eller efter 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">planeratSlutförandedatum</li>
     <li style="font-weight: bold;">planeratStartdatum</li>
    </ul><p style="font-weight: normal;">Följande fält har lagts till i det offentliga API:t för genomskinlighet vid beräkning av EAC (uppskattning vid slutförande).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">BCWP (Budgeted Cost of Work Performed) kallas även för Earned Value och är ett projektresultatmått som representerar den budgeterade kostnaden för det belopp av uppgiften som faktiskt har slutförts vid den tidpunkt då mätvärdet beräknas. BCWP = Faktisk procent slutfört x aktivitetsbudget för uppgifter. För projekt är BCWP = SUM(BCWP-värden för alla överordnade och enskilda uppgifter).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">BCWS (Budgeted Cost of Work Scheduled) kallas även för Planerat värde och är ett projektresultatmått som representerar den budgeterade kostnaden för det belopp av aktiviteten som skulle ha slutförts vid den tidpunkt då mätvärdet beräknas. För uppgifter, BCWS = planerad procent färdig x aktivitetsbudget. För projekt är BCWS = SUM(BCWS-värden för alla överordnade och enskilda uppgifter).</p></li>
    </ul><p style="font-weight: normal;">I följande fält lades det möjliga värdet ET till. Det här värdet representerar tidsenheten Förflutna månader, som refererar till månader utan hänsyn till helger eller helger.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">Följande fält har lagt till flaggans VALUTA</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">Följande fält har tagits bort från godkännandeobjektet.</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul><p style="font-weight: normal;">Följande fält har lagts till i Approval-objektet.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Referensfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">Borttagen från godkännandeobjektet  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Samlingsfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Tillagd i Godkännandeobjektet.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalPath {#approvalpath}

Ett ApprovalPath-objekt är en gren i en godkännandeprocess. Godkännandesökvägar baseras på statusen för objektet som godkännandeprocessen är kopplad till.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">Tillagt det möjliga värdet ET. Det här värdet representerar tidsenheten Förflutna månader, som refererar till månader utan hänsyn till helger eller helger.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalProcess {#approvalprocess}

Ett ApprovalProcess-objekt är ett godkännande i flera steg som kan kopplas till ett projekt, en aktivitet eller ett problem.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Det här fältet lades till och är en boolesk parameter som har värdet true om ett objekt är aktivt och false om det inte är det. Objekt som är inställda på Aktiv visas i rullgardinsmenyer och textbaserade fält och kan kopplas till andra objekt. Objekt som inte är inställda på Aktiv visas inte i rullgardinsmenyer och textframåt-fält som ska kopplas till andra objekt.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standardfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Tilldelning {#assignment}

Ett uppdragsobjekt representerar anslutningen mellan en arbetsuppgift och användaren, teamet eller gruppen som är tilldelad att arbeta med den.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit </p> <p style="font-weight: normal;">Tillagt det möjliga värdet ET. Det här värdet representerar tidsenheten Förflutna månader, som refererar till månader utan hänsyn till helger eller helger.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OriginalplanAktivitet {#baselinetask}

Baslinjer är bilder på hur ett projekts prestanda ser ut vid en viss tidpunkt. De lagrar viktig information om projektet, t.ex. nyckeldatum, förlopp, kostnad och intäktsvärden. När du skapar en baslinje hämtas uppgiftsinformationen också till baslinjeuppgifterna för den baslinjen.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">Tillagt det möjliga värdet ET. Det här värdet representerar tidsenheten Förflutna månader, som refererar till månader utan hänsyn till helger eller helger.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Kategori {#category}

Ett kategoriobjekt är ett anpassat formulär. Du kan skapa rapporter för det här objektet och du kan även visa det i andra objektrapporter.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Det här fältet lades till och är en boolesk parameter som har värdet true om ett objekt är aktivt och false om det inte är det. Objekt som är inställda på Aktiv visas i rullgardinsmenyer och textbaserade fält och kan kopplas till andra objekt. Objekt som inte är inställda på Aktiv visas inte i rullgardinsmenyer och textframåt-fält som ska kopplas till andra objekt.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standardfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Företag {#company}

Ett företagsobjekt representerar en organisation som består av en samling personer. Företag är associerade med en användare eller ett projekt.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Det här fältet lades till och är en boolesk parameter som har värdet true om ett objekt är aktivt och false om det inte är det. Objekt som är inställda på Aktiv visas i rullgardinsmenyer och textbaserade fält och kan kopplas till andra objekt. Objekt som inte är inställda på Aktiv visas inte i rullgardinsmenyer och textframåt-fält som ska kopplas till andra objekt.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standardfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum {#customenum}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A CustomEnum object is an enumeration that is created in Workfront to be used in objects and fields throughout Workfront.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Åtgärder</td> 
   <td> <p style="font-weight: normal;">Följande åtgärder har lagts till i CustomEnum-objektet</p> 
    <ul> 
     <li style="font-weight: bold;">getDefaultOpTaskConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultProjectConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultTaskConditionEnum</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Frågor</td> 
   <td> <p>Följande frågor har lagts till i CustomEnum-objektet</p> 
    <ul> 
     <li style="font-weight: bold;">opTaskConditions</li> 
     <li style="font-weight: bold;">projectConditions</li> 
     <li style="font-weight: bold;">taskConditions</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Kund {#customer}

Ett kundobjekt representerar en organisation som använder en instans av Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>customEnumTypes</p> <p style="font-weight: normal;">Möjliga värden har lagts till: </p> 
      <ul> 
       <li style="font-weight: normal;">CONDITION_PROJ (projektvillkor)</li> 
       <li style="font-weight: normal;">CONDITION_TASK (aktivitetsvillkor)</li> 
       <li style="font-weight: normal;">CONDITION_OPTASK (Utgivningsvillkor)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Reference Fields</td> 
    <td> 
     <ul> 
      <li style="font-weight: bold;"> <p>loginAsSettings</p> <p style="font-weight: normal;">Added. &nbsp;</p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td>Åtgärder</td> 
   <td> <p style="font-weight: normal;">Följande åtgärder har lagts till i kundobjektet</p> 
    <ul> 
     <li style="font-weight: bold;">målEnabled</li> 
     <li style="font-weight: bold;">updateLoginAsSettings</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomerPreferences {#customerpreferences}

Ett CustomerPreferences-objekt representerar den uppsättning inställningar som en kund har ställt in för sin instans av Workfront.

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">Möjliga värden har lagts till:</p> 
      <ul> 
       <li style="font-weight: normal;">password:password.uthPolicy (Krav för lösenordskomplexitet)</li> 
       <li style="font-weight: normal;"> password:password.minimumLength (Minimum Password Length)</li> 
       <li style="font-weight: normal;">lösenord:mobileSessionTimeout (tidsgräns för mobilsession)</li> 
       <li style="font-weight: normal;"> project.mgmt:default.project.usertimeoff (användartid av)</li> 
       <li style="font-weight: normal;">tidrapport:default.tidrapport.manualrole (rollen för manuell kontroll)</li> 
       <li style="font-weight: normal;">korrektur:defaultNonRecipientRole (config.proofhq.defaultnonmottagarrole) </li> 
       <li style="font-weight: normal;">korrektur:defaultNonRecipientGuestRole (config.proofhq.defaultnonmottagarguestrole)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocMetadataLinkGroup {#docmetadatalinkgroup}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Åtgärder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>getMetadataDetailsForDocument</p> <p style="font-weight: normal;">Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Dokument {#document}

Ett Document-objekt representerar en fil (t.ex. skrivet material, bilder eller andra typer av information).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Åtgärder</td> 
   <td> <p>Följande åtgärder har lagts till i Document-objektet.</p> 
    <ul> 
     <li style="font-weight: bold;">completeLargeDocument</li> 
     <li style="font-weight: bold;">createLargeDocument</li> 
     <li style="font-weight: bold;">createProofRest</li> 
     <li style="font-weight: bold;">getDocumentProofTemplate</li> 
     <li style="font-weight: bold;">getProofRecipients</li> 
     <li style="font-weight: bold;">getProofStages</li> 
     <li style="font-weight: bold;">getProofTemplate</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Upprepning {#iteration}

Ett Iteration-objekt representerar en enkel Agile Iteration. Iterationer är diskreta tidsperioder som används för att planera och slutföra Agile-berättelser.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> <p>Följande fält har lagts till i Iteration-objektet.</p> 
    <ul> 
     <li style="font-weight: bold;">originalTotalPoints</li> 
     <li style="font-weight: bold;">punkter slutförda</li> 
     <li style="font-weight: bold;">totalPoints  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Layoutmall {#layout-template}

Ett objekt av typen Layoutmall representerar en särskild disposition av layoutelement, till exempel huvudmenyn, navigeringspanelen eller Hem-området. Layoutmallar kan tilldelas användare, team, grupper eller jobbroller.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamp </p> <p style="font-weight: normal;">Det här fältet lades till och är en boolesk parameter med värdet true om en layoutmall är inställd på att visa tidsstämplar för förfallodatum i Arbetslista och Kalender, och false om den är inställd på att dölja tidsstämplar.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standardfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamp</p> <p style="font-weight: normal;">Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### MilstolpePath {#milestonepath}

En milstolpe är en markör för en uppgift som anger att den är en huvudpunkt i projektet. I allmänhet används för att beteckna en viktig händelse, t.ex. slutförande av en fas i projektet eller en uppsättning kritiska aktiviteter. Ett MlestonePath-objekt är en samling milstolpar.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Det här fältet lades till och är en boolesk parameter som har värdet true om ett objekt är aktivt och false om det inte är det. Objekt som är inställda på Aktiv visas i rullgardinsmenyer och textbaserade fält och kan kopplas till andra objekt. Objekt som inte är inställda på Aktiv visas inte i rullgardinsmenyer och textframåt-fält som ska kopplas till andra objekt.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standardfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Anteckning {#note}

Ett Note-objekt är en kommentar eller en uppdatering som görs på ett Workfront-objekt.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> <p>Följande fält har lagts till i anteckningsobjektet.</p> 
    <ul> 
     <li style="font-weight: bold;">proofID  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Samlingsfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>gillar</p> <p style="font-weight: normal;">Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

Ett OpTask-objekt kallas vanligtvis för ett problem. Ett problem är en arbetsuppgift som vanligtvis anger att det finns ett problem som förhindrar att en uppgift eller ett projekt slutförs. Ett problem kan också vara en Help Desk-begäran. Ändringsorder, begäranden och buggar är också problem.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Direktfält<p style="font-weight: normal;">Följande fält lade till validerarna AT_DATE_BEFORE_YEAR och AT_DATE_AFTER_YEAR. Dessa värden anger att datum för associerade objekt inte kan anges före år 1900 eller efter 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">planeratSlutförandedatum</li>
     <li style="font-weight: bold;">planeratStartdatum</li>
    </ul><p style="font-weight: normal;">Följande fält har lagts till i OpTask.</p>
    <ul>
     <li style="font-weight: bold;"><p>kanbanBoardID </p><p style="font-weight: normal;">Unikt Workfront-ID för ett Kanban-styrelsobjekt.</p></li>
     <li style="font-weight: bold;"><p>percentComplete</p><p style="font-weight: normal;">Procent färdigt är en parameter som returnerar det ifyllda beloppet för en utgåva, i procent.</p></li>
     <li style="font-weight: bold;">storyPoints</li>
     <li style="font-weight: bold;">arbete  </li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Samlingsfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Sökfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>arbete</p> <p style="font-weight: normal;">Borttagen</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standardfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>percentComplete</p> <p style="font-weight: normal;">Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Åtgärder</td> 
   <td> <p>Följande åtgärder har lagts till i OpTask-objektet</p> 
    <ul> 
     <li style="font-weight: bold;">bulkMove</li> 
     <li style="font-weight: bold;">copyIssue</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Parameter {#parameter}

Ett Parameter-objekt är ett anpassat fält.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Det möjliga värdet TYAH (Typeahead) har lagts till.</p> </li> 
     <li style="font-weight: bold;"> <p>refObjCode </p> <p style="font-weight: normal;">Det här fältet lades till och refererar till objektkoden för ett refererat objekt. Objektkoder för alla objekt finns i <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Portfolio {#portfolio}

Ett Portfolio-objekt är en samling projekt som konkurrerar om samma resurser, vanligtvis pengar eller personer som ska slutföra dem.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>description</p> <p style="font-weight: normal;">Valideraren MAX_LENGTH har lagts till, vilket anger att längden på beskrivningen inte är längre än 4 000 tecken.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Program {#program}

Ett Program-objekt är en delmängd i en portfölj, där liknande projekt kan grupperas tillsammans.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>description</p> <p style="font-weight: normal;">Valideraren MAX_LENGTH har lagts till, vilket anger att längden på beskrivningen inte är längre än 4 000 tecken.</p> </li> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Det här fältet lades till och är en boolesk parameter som har värdet true om ett objekt är aktivt och false om det inte är det. Objekt som är inställda på Aktiv visas i rullgardinsmenyer och textbaserade fält och kan kopplas till andra objekt. Objekt som inte är inställda på Aktiv visas inte i rullgardinsmenyer och textframåt-fält som ska kopplas till andra objekt.  </p> </li> 
     <li style="font-weight: bold;"> <p>name </p> <p style="font-weight: normal;">Valideraren MAX_LENGTH har lagts till, vilket anger att namnet inte är längre än 255 tecken.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standardfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Projekt {#project}

Projekt är arbetsuppgifter inom Workfront och är en viktig byggsten i det sätt på vilket Workfront hjälper människor att arbeta. Ett Project-objekt representerar en grupp med uppgifter med ett gemensamt, specifikt mål.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Direktfält<p style="font-weight: normal;">Följande fält lade till validerarna AT_DATE_BEFORE_YEAR och AT_DATE_AFTER_YEAR. Dessa värden anger att datum för associerade objekt inte kan anges före år 1900 eller efter 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">planeratSlutförandedatum</li>
     <li style="font-weight: bold;">planeratStartdatum</li>
    </ul><p style="font-weight: normal;">Följande fält har lagts till i det offentliga API:t för genomskinlighet vid beräkning av EAC (uppskattning vid slutförande).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">BCWP (Budgeted Cost of Work Performed) kallas även för Earned Value och är ett projektresultatmått som representerar den budgeterade kostnaden för det belopp av uppgiften som faktiskt har slutförts vid den tidpunkt då mätvärdet beräknas. BCWP = Faktisk procent slutfört x aktivitetsbudget för uppgifter. För projekt är BCWP = SUM(BCWP-värden för alla överordnade och enskilda uppgifter).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">BCWS (Budgeted Cost of Work Scheduled) kallas även för Planerat värde och är ett projektresultatmått som representerar den budgeterade kostnaden för det belopp av aktiviteten som skulle ha slutförts vid den tidpunkt då mätvärdet beräknas. För uppgifter, BCWS = planerad procent färdig x aktivitetsbudget. För projekt är BCWS = SUM(BCWS-värden för alla överordnade och enskilda uppgifter).</p></li>
    </ul><p style="font-weight: normal;">Följande fält har lagt till flaggans VALUTA</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">Följande fält har tagits bort från Project-objektet.</p>
    <ul>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Samlingsfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### KorrekturGodkännande {#proofapproval}

Ett ProofApproval-objekt representerar ett godkännande som är direkt kopplat till ett korrektur.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isAwaitingDecision</p> <p style="font-weight: normal;">Det här fältet har lagts till och är en boolesk parameter som har värdet true om ett bevis väntar på ett beslut och false om det inte gör det.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

Ett QueueDef-objekt representerar en kö, vilket är ett projekt som har publicerats till Help Desk-området där användarna kan skicka problem till den.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> <p>Följande fält har lagt till det möjliga värdet BUDGETING_INFORMATION. Detta gör att användare med behörighet kan redigera prioriteringar och budgettimmar i planeraren.</p> 
    <ul> 
     <li style="font-weight: bold;">requestCoreAction</li> 
     <li style="font-weight: bold;">requestForbiddenActions</li> 
    </ul>  </td> 
  </tr> 
 </tbody> 
</table>

### ReservedTime {#reservedtime}

Ett ReservedTime-objekt representerar dagar som anges på användarens personliga tid, vilket anger att användaren inte kommer att vara tillgänglig för arbete.

ReservedTime-resursen lade till flaggan REPORTABLE.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> <p>Följande fält tog bort flaggan NOT_GROUPABLE.</p> 
    <ul> 
     <li style="font-weight: bold;">endDate</li> 
     <li style="font-weight: bold;">extRefID</li> 
     <li style="font-weight: bold;">startDate </li> 
    </ul> <p>Följande fält har tagits bort från objektet ReservedTime.</p> 
    <ul> 
     <li style="font-weight: bold;">taskID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referensfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>uppgift</p> <p style="font-weight: normal;">Borttagen  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Operationer</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>REDIGERA</p> <p style="font-weight: normal;">Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Resursplaneringsfilter {#resourceplannerfilter}

Ett ResourcePlannerFilter-objekt är en uppsättning regler som bestämmer vilka objekt som ska visas i resursplaneraren.

ResourcePlannerFilter-resursen lade till flaggan SHARABLE. Det fanns inga andra ändringar av objektet.

### risk {#risk}

Ett Risk-objekt representerar en möjlig händelse som kan hindra ett projekt från att avslutas i tid eller inom budgeten. Risker läggs till projekt i planeringsfasen för att identifiera potentiella hinder innan något arbete godkänns.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> <p>Följande fält har lagts till i riskobjektet:</p> 
    <ul> 
     <li style="font-weight: bold;"> <p>enteredByID</p> <p style="font-weight: normal;">ID för den användare som ursprungligen skapade objektet.</p> </li> 
     <li> <p style="font-weight: bold;">entryDate</p> <p>Datumet då ett objekt skickades av en användare i Workfront.</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdateDate</p> <p>Parametern Senaste uppdateringsdatum returnerar det datum då den senaste uppdateringen gjordes för ett objekt,</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdatedByID </p> <p>Senast uppdaterad med ID är en parameter som returnerar användar-ID:t för den senaste användaren som uppdaterade objektet.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referensfält</td> 
   <td> <p style="font-weight: normal;">Följande referensfält har lagts till i RIsk-objektet.</p> 
    <ul> 
     <li style="font-weight: bold;">enteredBy</li> 
     <li style="font-weight: bold;">lastUpdatedBy  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### SchemalagdRapport {#scheduledreport}

Ett ScheduledReport-objekt representerar en rapport som har konfigurerats att schemaläggas för leverans.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>pageSize</p> <p style="font-weight: normal;">Följande möjliga värden har lagts till:</p> 
      <ul> 
       <li style="font-weight: normal;">A2</li> 
       <li style="font-weight: normal;">A1</li> 
       <li style="font-weight: normal;">A0  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

Ett ScoreCardQuestion-objekt representerar en fråga som har lagts till i ett styrkort. Dessa frågor avgörs vanligtvis av Portfolio-förvaltaren och deras svar gör det möjligt för förvaltaren att förstå hur väl ett projekt passar ihop med portföljens mål.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Tillagt möjligt värde TYAH (Typeahead)  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Uppgift {#task}

Ett Task-objekt representerar en arbetsuppgift som måste utföras som ett steg mot att uppnå ett slutligt mål (slutföra ett projekt).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Direktfält<p style="font-weight: normal;">Följande fält lade till validerarna AT_DATE_BEFORE_YEAR och AT_DATE_AFTER_YEAR. Dessa värden anger att datum för associerade objekt inte kan anges före år 1900 eller efter 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">planeratSlutförandedatum</li>
     <li style="font-weight: bold;">planeratStartdatum</li>
    </ul><p style="font-weight: normal;">Följande fält har lagts till i det offentliga API:t för genomskinlighet vid beräkning av EAC (uppskattning vid slutförande).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">BCWP (Budgeted Cost of Work Performed) kallas även för Earned Value och är ett projektresultatmått som representerar den budgeterade kostnaden för det belopp av uppgiften som faktiskt har slutförts vid den tidpunkt då mätvärdet beräknas. BCWP = Faktisk procent slutfört x aktivitetsbudget för uppgifter. För projekt är BCWP = SUM(BCWP-värden för alla överordnade och enskilda uppgifter).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">BCWS (Budgeted Cost of Work Scheduled) kallas även för Planerat värde och är ett projektresultatmått som representerar den budgeterade kostnaden för det belopp av aktiviteten som skulle ha slutförts vid den tidpunkt då mätvärdet beräknas. För uppgifter, BCWS = planerad procent färdig x aktivitetsbudget. För projekt är BCWS = SUM(BCWS-värden för alla överordnade och enskilda uppgifter).</p></li>
    </ul><p style="font-weight: normal;">I följande fält lades det möjliga värdet ET till. Det här värdet representerar tidsenheten Förflutna månader, som refererar till månader utan hänsyn till helger eller helger.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">Följande fält har tagits bort från Task-objektet.</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
    </ul><p style="font-weight: normal;">Följande fält har lagts till i Task-objektet.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Referensfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">Borttagen  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Samlingsfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Team {#team}

Ett Team-objekt är en samling användare som kan tilldelas till ett arbetsobjekt.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>agileEstimateType </p> <p style="font-weight: normal;">Det här fältet lades till i Team-objektet. Agile Estimate Type bestämmer hur arbetsbelastningen för en artikel beräknas. Om det beräknas i timmar är detta antalet planerade timmar som läggs till i artikeln. Om poängen är i punkter lägger varje punkt till ett antal planerade timmar i artikeln baserat på hur punkterna är inställda (standardvärdet är 8 timmar). Möjliga värden för Agile Estimate-typen är:</p> 
      <ul> 
       <li style="font-weight: normal;"> STORY_POINTS (artikelpunkter)</li> 
       <li style="font-weight: normal;">TIMMAR (timmar)</li> 
       <li style="font-weight: normal;">LEGACY_POINTS (Timmar som punkter)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Mall {#template}

Ett mallobjekt representerar ett mönster för ett projekt. Projekt kan skapas från mallar för att spara tid. En mall innehåller ett team och uppgifter som kopieras till ett projekt när mallen används.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Det här fältet lades till och är en boolesk parameter som har värdet true om ett objekt är aktivt och false om det inte är det. Objekt som är inställda på Aktiv visas i rullgardinsmenyer och textbaserade fält och kan kopplas till andra objekt. Objekt som inte är inställda på Aktiv visas inte i rullgardinsmenyer och textframåt-fält som ska kopplas till andra objekt.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Samlingsfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriority</p> <p style="font-weight: normal;">Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standardfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateAssignment {#templateassignment}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A TemplateAssignment object represents the connection between a Template and the User, Team, or Group it is assigned to.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit</p> <p style="font-weight: normal;">Tillagt det möjliga värdet ET. Det här värdet representerar tidsenheten Förflutna månader, som refererar till månader utan hänsyn till helger eller helger.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateTask {#templatetask}

Ett TemplateTask-objekt representerar en aktivitet som är en del av en Template. Malluppgifter blir uppgifter i det projekt där mallen används.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> <p style="font-weight: normal;">I följande fält lades det möjliga värdet ET till. Det här värdet representerar tidsenheten Förflutna månader, som refererar till månader utan hänsyn till helger eller helger.</p> 
    <ul> 
     <li style="font-weight: bold;">durationUnit</li> 
     <li style="font-weight: bold;">workUnit</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Samlingsfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriority</p> <p style="font-weight: normal;">Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Tidrapport {#timesheet}

Ett Timesheet-objekt representerar ett virtuellt tidkort som gör att användare kan ange faktiskt antal arbetstimmar för uppgifter, projekt och obemannade timtyper.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Kärnfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>objCode</p> <p style="font-weight: normal;">Borttagen</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Uppdatera {#update}

Arbetsobjekt i Workfront kan uppdateras för att hålla användarna informerade om den aktuella statusen. Ett Update-objekt representerar en av dessa uppdateringar. Uppdateringar kan anges av användare eller skapas av Workfront-systemet.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>updateType</p> <p style="font-weight: normal;">Möjliga värden har lagts till som referenceObjectCustomData (enum.updatetypeenum.referenceObjectCustomData)  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Frågor</td> 
   <td> <p style="font-weight: normal;">Följande frågor har lagts till i Update-objektet.</p> 
    <ul> 
     <li style="font-weight: bold;">objectUpdatesMobile</li> 
     <li style="font-weight: bold;">updateThreadMobile</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="user">User</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A User object represents a person with an account in Workfront that can log in and interact with the system.</p>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Samlingsfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>loginAsAccessRules</p> <p style="font-weight: normal;">Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Åtgärder</td> 
   <td> <p style="font-weight: normal;">Följande åtgärder har lagts till i User-objektet.</p> 
    <ul> 
     <li style="font-weight: bold;">hasGrantLoginAsAccess</li> 
     <li style="font-weight: bold;">isUserAdmin</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Frågor</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>userAdmins</p> <p style="font-weight: normal;">Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UserNote {#usernote}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Åtgärder</td> 
   <td> <p style="font-weight: normal;">Följande åtgärder har lagts till i User-objektet.</p> 
    <ul> 
     <li style="font-weight: bold;">confirmMyNotifications</li> 
     <li style="font-weight: bold;">unrecognizedAllObjectsTypeCount  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Frågor</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>myAllObjectTypesUnreadNotifications</p> <p style="font-weight: normal;">Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Arbete  {#work}

Ett Work-objekt är ett vanligt gränssnitt som både Task och OpTask ärver och delar gemensam kod mellan de två.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Direktfält<p style="font-weight: normal;">Följande fält lade till validerarna AT_DATE_BEFORE_YEAR och AT_DATE_AFTER_YEAR. Dessa värden anger att datum för associerade objekt inte kan anges före år 1900 eller efter 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">planeratSlutförandedatum</li>
     <li style="font-weight: bold;">planeratStartdatum</li>
    </ul><p style="font-weight: normal;">Följande fält har lagts till i det offentliga API:t för genomskinlighet vid beräkning av EAC (uppskattning vid slutförande).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">BCWP (Budgeted Cost of Work Performed) kallas även för Earned Value och är ett projektresultatmått som representerar den budgeterade kostnaden för det belopp av uppgiften som faktiskt har slutförts vid den tidpunkt då mätvärdet beräknas. BCWP = Faktisk procent slutfört x aktivitetsbudget för uppgifter. För projekt är BCWP = SUM(BCWP-värden för alla överordnade och enskilda uppgifter).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">BCWS (Budgeted Cost of Work Scheduled) kallas även för Planerat värde och är ett projektresultatmått som representerar den budgeterade kostnaden för det belopp av aktiviteten som skulle ha slutförts vid den tidpunkt då mätvärdet beräknas. För uppgifter, BCWS = planerad procent färdig x aktivitetsbudget. För projekt är BCWS = SUM(BCWS-värden för alla överordnade och enskilda uppgifter).</p></li>
    </ul><p style="font-weight: normal;">I följande fält lades det möjliga värdet ET till. Det här värdet representerar tidsenheten Förflutna månader, som refererar till månader utan hänsyn till helger eller helger.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">Följande fält har tagits bort från Work-objektet.</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
    </ul><p style="font-weight: normal;">Följande fält har lagts till i Work-objektet.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Referensfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">Borttagen  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Samlingsfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

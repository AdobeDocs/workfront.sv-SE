---
content-type: api
navigation-topic: api-navigation-topic
title: Nyheter i API-version 13
description: Adobe Workfront släppte API-version 13 den 22 april 2021. API-version 13 innehåller följande ändringar från version 12.
author: Becky
feature: Workfront API
role: Developer
exl-id: afbc986e-8b5c-40bc-9120-e8d34e0f7004
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1072'
ht-degree: 0%

---

# Nyheter i API-version 13

Adobe Workfront släppte API-version 13 den 22 april 2021. API-version 13 innehåller följande ändringar från version 12.

## Tillagda resurser

Inga resurser har lagts till för API-version 13.

## Borttagna resurser

Inga resurser togs bort för API-version 13.

## Ändrade resurser

Följande resurser ändrades för API-version 13.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">AccessLevel</a> </p> </li> 
     <li> <p><a href="#breadcrumb" class="MCXref xref">BreadCrumb</a> </p> </li> 
     <li> <p><a href="#burndownevent" class="MCXref xref">BurndownEvent</a> </p> </li> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">CustomerPreferences</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">Dokumentversion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">Grupp </a> </p> </li> 
     <li> <p><a href="#journalentry" class="MCXref xref">JournalEntry</a> </p> </li> 
     <li> <p><a href="#layouttemplate" class="MCXref xref">LayoutTemplate</a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">OpTask</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#project" class="MCXref xref">Projekt</a> </p> </li> 
     <li> <p><a href="#proofapproval" class="MCXref xref">Korrektur för godkännande</a> </p> </li> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">Aktivitet</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">Team</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">Tidrapport</a> </p> </li> 
     <li> <p><a href="#timesheetprofile" class="MCXref xref">Tidrapportprofil</a> </p> </li> 
     <li> <p><a href="#uitemplate" class="MCXref xref">UITemplate</a> </p> </li> 
     <li> <p><a href="#userdelegation" class="MCXref xref">Användardelegering</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">Arbete </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessLevel {#accesslevel}

Ett AccessLevel-objekt är associerat med användare och beskriver uppsättningen AccessLevelPermissions som avgör vad användaren kan komma åt.

Mer information om åtkomstnivåer finns i [Hur åtkomstnivåer fungerar](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direktfält</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>Beskrivning</b> </p> <p>Valideraren MAX_LENGTH har lagts till, vilket anger att längden på beskrivningen inte är längre än 4 000 tecken.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BreadCrumb {#breadcrumb}

Ett BreadCrumb-objekt representerar ett element i hierarkin för överordnade/underordnade element för ett Workfront-arbetsobjekt. Brevbeskrivningar visar hur en arbetsuppgift passar in i den större strukturen för Portfolio, projekt, projekt och uppgifter.

Mer information om vägbeskrivningar finns i [Översikt över vägbeskrivningar i den nya Adobe Workfront-upplevelsen](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direktfält</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>Objektkoder finns i <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API-utforskaren</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BurndownEvent {#burndownevent}

Ett BurndownEvent-objekt representerar ett objekt som ändrar bundet för en iteration.

Mer information om nedladdning finns i [Nedladdning](../../agile/use-scrum-in-an-agile-team/burndown/burndown.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direktfält</p> </td> 
   <td> <p>Följande fält tog bort flaggan NOT_GROUPABLE </p> 
    <ul> 
     <li> <p>applyDate</p> </li> 
     <li> <p>entryDate</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomerPreferences {#customerpreferences}

Ett CustomerPreferences-objekt representerar den uppsättning inställningar som en kund har ställt in för sin instans av Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">Möjliga värden har lagts till:</p> 
      <ul> 
       <li style="font-weight: normal;">password:aemAPIKey (config.general.aem.apikey)</li> 
       <li style="font-weight: normal;"> lösenord:aemAADomain (config.general.aem.adomain) </li> 
       <li style="font-weight: normal;">password:aemIntegrationEnabled (config.general.aem.enabled)</li> 
       <li style="font-weight: normal;">password:aemHost (config.general.aem.host)</li> 
       <li style="font-weight: normal;">tidrapport:default.tidrapport.restrict.tidrapport.edit.owners.admins (config.tidrapport.restrict.tidrapport.edit.owners.admins)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Åtgärder</td> 
   <td> <p>Följande åtgärder har lagts till i CustomerPreferences-resursen.</p> 
    <ul> 
     <li> <p><b>getTimesheetPreferences</b> </p> </li> 
     <li> <p><b>setTimesheetPreferences</b> </p> <p>Tar argumentet:</p> 
      <ul> 
       <li> <p>inställningar (karta)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion {#documentversion}

Ett DocumentVersion-objekt representerar en specifik version av en fil (t.ex. skrivet material, bilder eller andra typer av information).

Mer information om dokumentversioner finns i [Överföra en ny version av ett dokument](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direktfält</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>Tillagt möjligt värde:</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><b>proofID</b> </p> <p>Flagga som lagts till NOT_FILTERABLE</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Grupp  {#group}

Ett Group-objekt representerar en uppsättning användare och team. Grupper representerar ofta avdelningsstruktur.

Mer information om grupper finns i [Grupper kontra team i Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Åtgärder</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>getParents</b> </p> <p>Den här åtgärden returnerar en array av gruppens överordnade grupper (grupper som den angivna gruppen är en undergrupp till).</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### JournalEntry {#journalentry}

JournalEntry-objektet kan ställas in för att logga information om specifika objektfält när som helst när dessa fält ändras. När ett fält har ställts in för att loggas som en del av journalpostobjektet, skapas en motsvarande journalpost varje gång fältet ändras.

JournalEntry-resursen lade till flaggan REPORTABLE.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direktfält</p> </td> 
   <td> <p>Följande fält tog bort flaggan NOT_GROUPABLE:</p> 
    <ul> 
     <li> <p><b>changeType</b> </p> </li> 
     <li> <p><b>entryDate</b> </p> </li> 
     <li> <p><b>fieldName</b> </p> </li> 
     <li> <p><b>objObjCode</b> </p> </li> 
    </ul> <p>I följande fält lades flaggan NOT_FILTERABLE till:</p> 
    <ul> 
     <li> <p><b>subObjCode</b> </p> </li> 
     <li> <p><b>subObjID</b> </p> </li> 
     <li> <p><b>topObjCode</b> </p> </li> 
     <li> <p><b>topObjID</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LayoutTemplate {#layouttemplate}

Adobe Workfront-administratörer och gruppadministratörer kan skapa mallar för att anpassa layoutelementen i Adobe Workfront. LayoutTemplate-objektet är specifikt för Adobe Workfront Classic.

Objektet som representerar layoutmallar i den nya Adobe Workfront-upplevelsen finns i [UITemplate](#uitemplate)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direktfält</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>Beskrivning</b> </p> <p>Valideraren MAX_LENGTH har lagts till, vilket anger att längden på beskrivningen inte är längre än 4 000 tecken.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LinkedFolder {#linkedfolder}

Ett LinkedFolder-objekt representerar en mapp som är länkad från en extern dokumentleverantör, till exempel Google Drive eller Dropbox.

Mer information om länkade mappar finns i [Länka dokument från externa program](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direktfält</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>Tillagt möjligt värde:</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
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
   <td> <p>Sökfält</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>FavitedByUsersMM</b> </p> </li> 
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
   <td> <p>Direktfält</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>convertOpTaskOriginatorID</b> </p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Removed flag NOT&nbsp;FILTERABLE</p>
      --> </li> 
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
   <td> <p>Direktfält</p> </td> 
   <td> <p>Följande fält har lagts till i resursen ProofApproval.</p> 
    <ul> 
     <li> <p><b>approverStage</b> </p> </li> 
     <li> <p><b>Beslutsdatum</b> </p> </li> 
     <li> <p><b>workflowTemplate</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

Ett QueueDef-objekt representerar en kö, vilket är ett projekt som har publicerats till Help Desk-området där användarna kan skicka problem till den.

Mer information om begärandeköer finns i [Skapa en begärandekö](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direktfält</td> 
   <td> 
    <ul> 
     <li> <p><b>documentPosition</b> </p> <p>Tillagd. Möjliga värden är:</p> 
      <ul> 
       <li> <p>0 (efter anpassade formulär)</p> </li> 
       <li> <p>1 (Före anpassade formulär)</p> </li> 
      </ul> </li> 
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
   <td> <p>Sökfält</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>FavitedByUsersMM</b> </p> </li> 
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

### Tidrapport {#timesheet}

Ett Timesheet-objekt representerar ett virtuellt tidkort som gör att användare kan ange faktiskt antal arbetstimmar för uppgifter, projekt och obemannade timtyper.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Kärnfält</td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>Borttagen</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Tidrapportprofil {#timesheetprofile}

Ett Timesheet-objekt representerar ett virtuellt tidkort som gör att användare kan ange faktiskt antal arbetstimmar för uppgifter, projekt och obemannade timtyper.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standardfält</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UITemplate {#uitemplate}

Adobe Workfront-administratörer och gruppadministratörer kan skapa mallar för att anpassa layoutelementen i Adobe Workfront. UITemplate-objektet är specifikt för den nya Adobe Workfront-upplevelsen.

Objektet som representerar layoutmallar i Adobe Workfront Classic finns i [LayoutTemplate](#layouttemplate).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Åtgärder</td> 
   <td> <p>Följande åtgärder har lagts till i UITemplate-resursen.</p> 
    <ul> 
     <li> <p><b>migrateCustomersAllLayoutTemplates</b> </p> <p>Tar argumentet:</p> 
      <ul> 
       <li> <p>overrideIfExists (boolesk)</p> </li> 
      </ul> </li> 
     <li> <p><b>migrateLayoutTemplates</b> </p> <p>Tar argumenten:</p> 
      <ul> 
       <li> <p>layoutTemplateIDs (string[])</p> </li> 
       <li> <p>overrideIfExists (boolesk)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UserDelegering {#userdelegation}

Ett UserDelegation-objekt representerar delegeringen av arbete från en användare till en annan för en viss tidsperiod.

UserDelegation-objektet lade till flaggan REPORTABLE.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direktfält</td> 
   <td> <p>Följande fält tog bort flaggan NOT_GROUPABLE</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Standardfält</td> 
   <td> <p>Följande fält har lagts till:</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
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
   <td> <p>Sökfält</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>FavitedByUsersMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

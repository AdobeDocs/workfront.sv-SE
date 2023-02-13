---
content-type: api
navigation-topic: api-navigation-topic
title: Nyheter i API-version 14
description: Adobe Workfront släppte API-version 14 den 9 september 2021. API-version 14 innehåller följande ändringar från version 14.
author: John
feature: Workfront API
exl-id: eca5d1cc-6348-445c-be84-c0a29f15980d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 0%

---

# Nyheter i API-version 14

Adobe Workfront släppte API-version 14 den 9 september 2021. API-version 14 innehåller följande ändringar från version 14.

## Tillagda resurser

Inga resurser har lagts till för API-version 14.

## Borttagna resurser

Inga resurser togs bort för API-version 14.

## Ändrade resurser

Följande resurser ändrades för API-version 14.

* [Faktureringspost (BILL)](#billingrecord-bill)
* [Kategori (CTGY)](#category-ctgy)
* [CustomEnum (CSTEM)](#customenum-cstem)
* [Kund (CUST)](#customer-cust)
* [CustomerPreferences (CUSTPR)](#customerpreferences-custpr)
* [DocumentVersion (DOCV)](#documentversion-docv)
* [Grupp (GRUPP)](#group-group)
* [NoteTag (NTAG)](#notetag-ntag)
* [Projekt (PROJ)](#project-proj)
* [QueueDef (QUED)](#queuedef-qued)
* [Resursallokering (RSALLO)](#resource-allocation-rsallo)
* [Roll (ROLE)](#role-role)
* [Mall (TMPL)](#template-tmpl)
* [Tidrapport (TSPEN)](#timesheet-tshet)

### Faktureringspost (BILL) {#billingrecord-bill}

Ett BillingRecord-objekt registrerar intäkter, timmar eller utgifter som kan faktureras. Den här informationen kan användas för att skapa fakturor i ett externt redovisningssystem.

Mer information om faktureringsposter finns i [Skapa faktureringsposter](../../manage-work/projects/project-finances/create-billing-records.md).

Faktureringsposten-objektet lade till flaggan **DATA_EXTENDIBLE**.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Direktfält</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>categoryID</b> </p> <p>Tillagd. En kategori är ett eget formulär. Den här parametern har lagts till för att ge stöd för möjligheten att lägga till anpassade Forms till BillingRecord-objekt.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Referensfält</td> 
   <td> 
    <ul> 
     <li> <p><b>kategori</b> </p> <p>Tillagd. En kategori är ett anpassat formulär. Den här parametern lades till för att ge stöd för möjligheten att lägga till anpassade formulär i BillingRecord-objekt.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Samlingsfält</td> 
   <td> 
    <ul> 
     <li> <p><b>objectCategories</b> </p> <p>Tillagd. Detta representerar en samling kategorier (anpassade formulär) som är associerade med objektet BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtgärder</td> 
   <td> 
    <ul> 
     <li> <p><b>calculateDataExtension</b> </p> <p>Tillagd. Den här åtgärden beräknar om uttrycken i anpassade formulärfält.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Kategori (CTGY) {#category-ctgy}

Ett kategoriobjekt är ett anpassat formulär.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direktfält</td> 
   <td> 
    <ul> 
     <li> <p><b>catObjCode</b> </p> <p>Tillagt möjligt värde:</p> 
      <ul> 
       <li> <p> FAKTURERING (Faktureringspost)</p> </li> 
      </ul> <p>Det här värdet har lagts till för att ge stöd för möjligheten att lägga till anpassade formulär i BillingRecord-objekt.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtgärder</td> 
   <td> 
    <ul> 
     <li> <p><b>isObjectFrozenInPendingApprovalStatus</b> </p> <p>Den här åtgärden tar parametrarna objID och objCode och returnerar ett booleskt värde.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum (CSTEM) {#customenum-cstem}

CustomEnum-objektet hjälper dig att konvertera statuskoder till läsbar text.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Frågor</td> 
   <td> 
    <ul> 
     <li> <p><b>getGroupStatuses</b> </p> <p>Tillagd. Den här frågan stöder möjligheten att skapa och hantera statusvärden för grupper och undergrupper. </p> <p>Mer information finns i <a href="../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md" class="MCXref xref">Hantera gruppstatus</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Kund (CUST) {#customer-cust}

Ett kundobjekt representerar en organisation som använder en instans av Workfront.

Detta är ett internt objekt.

### CustomerPreferences (CUSTPR) {#customerpreferences-custpr}

Ett CustomerPreferences-objekt representerar den uppsättning inställningar som en kund har ställt in för sin instans av Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direktfält</td> 
   <td> 
    <ul> 
     <li> <p><b>name</b> </p> <p>Tillagt möjligt värde:</p> 
      <ul> 
       <li> <p>Tillåt användare att lägga till bilder i uppdateringar (uppdateringar:images.toggle)</p> </li> 
      </ul> <p>Den här parametern stöder möjligheten att lägga till bilder i uppdateringar av arbetsobjekt. </p> <p>Mer information finns i <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Uppdatera arbete</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion (DOCV) {#documentversion-docv}

Ett DocumentVersion-objekt representerar en specifik version av en fil (t.ex. skrivet material, bilder eller andra typer av information).

Mer information om dokumentversioner finns i [Överföra en ny version av ett dokument](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direktfält</td> 
   <td> 
    <ul> 
     <li> <p><b>lastCallbackDate</b> </p> <p>Tillagd. I det här fältet registreras datum och tid för det senaste återanropet från Workfront Proof, om versionen är associerad med ett korrektur.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Grupp (GRUPP) {#group-group}

Ett Group-objekt representerar en uppsättning användare och team. Grupper representerar ofta avdelningsstruktur.

Mer information om grupper finns i [Grupper kontra team i Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Åtgärder</td> 
   <td> 
    <ul> 
     <li> <p><b>addSubgroups</b> </p> <p>Tillagd. Den här åtgärden tar en array med groupID:n och lägger till dessa grupper som undergrupper i den angivna gruppen.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### NoteTag (NTAG) {#notetag-ntag}

Ett NoteTag-objekt representerar taggen för en användare eller ett team i en uppdatering av ett arbetsobjekt.

Mer information om hur du taggar i uppdateringar finns i [Tagga andra för uppdateringar](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Operationer</td> 
   <td> <p>Följande åtgärder har lagts till i objektet NoteTag:</p> 
    <ul> 
     <li> <p><b>COUNT</b> </p> </li> 
     <li> <p><b>GET</b> </p> </li> 
     <li> <p><b>RAPPORT</b> </p> </li> 
     <li> <p><b>SÖK</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Projekt (PROJ) {#project-proj}

Projekt är arbetsuppgifter inom Workfront och är en viktig byggsten i det sätt på vilket Workfront hjälper människor att arbeta. Ett Project-objekt representerar en grupp med uppgifter med ett gemensamt, specifikt mål.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Åtgärder</td> 
   <td> 
    <ul> 
     <li> <p><b>updateBusinessCaseSource</b> </p> <p>Tillagd.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef (QUED) {#queuedef-qued}

Ett QueueDef-objekt representerar en kö, vilket är ett projekt som har publicerats i Help Desk-området där användarna kan skicka utgåvor till den.

Mer information om köer finns i [Skapa en begärandekö](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Åtgärder</td> 
   <td> 
    <ul> 
     <li> <p><b>searchByPath</b> </p> <p>Tillagd. Den här åtgärden stöder möjligheten att söka efter begäranden genom att använda sökvägen via begärandekön och ämnesgrupper.</p> <p>Mer information om hur du söker i begärandeköer efter sökväg finns i <a href="../../manage-work/requests/create-requests/create-submit-requests.md#create-requests-in-the-web-app" class="MCXref xref">Skapa förfrågningar och generera utkast i Workfront webbprogram</a> in <a href="../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Skapa och skicka Adobe Workfront-förfrågningar</a>.</p> </li> 
    </ul> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

### Resursallokering (RSALLO) {#resource-allocation-rsallo}

Ett resursallokeringsobjekt representerar uppskattningen av resurser som behövs för ett visst projekt. Det här objektet används endast i den äldre resursplaneraren. Använd BGHR (Budgeted Hour) för motsvarande fält i den nya resursplaneraren.

Objektet Resursallokering tog bort flaggan **RAPPORTERBART**.

### Roll (ROLE) {#role-role}

Ett rollobjekt (jobbroll) representerar en funktionskapacitet eller en kompetensuppsättning som en användare kan fylla, till exempel Designer eller Product Manager.

Mer information om jobbroller finns i [Översikt över jobbroll](../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Tillagd. Det här är en boolesk parameter som har värdet true om ett objekt är aktivt och false om det inte är det. Objekt som är inställda på Aktiv visas i rullgardinsmenyer och textbaserade fält och kan kopplas till andra objekt.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Standardfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Mall (TMPL) {#template-tmpl}

Ett Template-objekt representerar ett mönster för ett projekt. Projekt kan skapas från mallar för att spara tid. En mall innehåller ett team och uppgifter som kopieras till alla projekt som skapas från mallen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">Tillagd. Det här fältet lades till för att ge stöd för möjligheten att associera grupper med mallar.</p> <p style="font-weight: normal;">Mer information finns i <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Redigera projektmallar</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Referensfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>grupp</p> <p style="font-weight: normal;">Tillagd. Det här fältet lades till för att ge stöd för möjligheten att associera grupper med mallar.</p> <p style="font-weight: normal;">Mer information finns i <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Redigera projektmallar</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><strong>Timesheet (TSHET)</strong></p>
<p>A&nbsp;Timesheet object represents a virtual timecard that allows users to enter actual hours worked for tasks, projects, and overhead hour types.</p>
<p>For more information, see <a href="../../timesheets/timesheets/timesheets-overview.md" class="MCXref xref">Timesheets overview</a>.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Core Fields</td>
<td>
<ul>
<li> <p><b>objCode</b> </p> <p>Removed.</p> </li>
</ul> </td>
</tr>
</tbody>
</table>
</div>
-->

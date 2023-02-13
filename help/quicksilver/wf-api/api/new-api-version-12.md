---
content-type: api
navigation-topic: api-navigation-topic
title: Nyheter i API-version 12
description: Workfront släppte API version 12 den 12 november 2020. API-version 12 innehåller följande ändringar från version 11
author: John
feature: Workfront API
exl-id: 1ffba3b5-ab24-4ca2-a1ef-f7e5b77e776c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '2516'
ht-degree: 0%

---

# Nyheter i API-version 12

Workfront släppte API version 12 den 12 november 2020. API-version 12 innehåller följande ändringar från version 11

## Tillagda resurser

Följande resurser är nya i Workfront API version 12.

* [BreadCrumb](#breadcrumb)
* [RichTextParameterValue](#richtextparametervalue)

### BreadCrumb {#breadcrumb}

Ett BreadCrumb-objekt representerar ett element i hierarkin för överordnade/underordnade element för ett Adobe Workfront-arbetsobjekt. Brevbeskrivningar visar hur en arbetsuppgift passar in i den större strukturen för Portfolio, projekt, projekt och uppgifter.

Mer information om Breadcrumbs i Workfront finns i [En översikt över vägbeskrivningar i nya Adobe Workfront](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Åtgärd</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">getObjectHierarchy</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### RichTextParameterValue {#richtextparametervalue}

RTF-fält är nu tillgängliga för fler objekt. RichTextParameterValue-objektet lades till i Workfront för att stödja den här tillgängligheten.

Mer information finns i [RTF-fält i Adobe Workfront API](../../wf-api/general/rich-text-field-api.md).

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
     <li style="font-weight: bold;">ID</li> 
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

## Borttagna resurser

Inga resurser togs bort för API-version 12.

## Ändrade resurser

Följande resurser ändrades för Workfront API version 12.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">AccessLevel</a> </p> </li> 
     <li> <p><a href="#accesslevelpermissions" class="MCXref xref">AccessLevelPermissions</a> </p> </li> 
     <li> <p><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </p> </li> 
     <li> <p><a href="#accessrule" class="MCXref xref">AccessRule</a> </p> </li> 
     <li> <p><a href="#activitylog" class="MCXref xref">ActivityLog</a> </p> </li> 
     <li> <p><a href="#announcementattachment" class="MCXref xref">AnnouncementAttachment</a> </p> </li> 
     <li> <p><a href="#approval" class="MCXref xref">Godkännande</a> </p> </li> 
     <li> <p><a href="#calendarsection" class="MCXref xref">CalendarSection</a> </p> </li> 
     <li> <p><a href="#company" class="MCXref xref">Företag</a> </p> </li> 
     <li> <p><a href="#customer" class="MCXref xref">Kund</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">CustomerPreferences</a> </p> </li> 
     <li> <p><a href="#document" class="MCXref xref">Dokument</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">Grupp </a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">OpTask</a> </p> </li> 
     <li> <p><a href="#parameter" class="MCXref xref">Parameter</a> </p> </li> 
     <li> <p><a href="#portfolio" class="MCXref xref">Portfolio</a> </p> </li> 
     <li> <p><a href="#program" class="MCXref xref">Program</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#scheduledreport" class="MCXref xref">SchemalagdRapport</a> </p> </li> 
     <li> <p><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">Uppgift</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">Team</a> </p> </li> 
     <li> <p><a href="#templatetask" class="MCXref xref">TemplateTask</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">Tidrapport</a> </p> </li> 
     <li> <p><a href="#user" class="MCXref xref">Användare</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">Arbete </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### AccessLevel {#accesslevel}

Ett AccessLevel-objekt är associerat med användare och beskriver uppsättningen AccessLevelPermissions som avgör vad användaren kan komma åt.

Mer information om åtkomstnivåer finns i [Hur åtkomstnivåer fungerar](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Direct Fields</td>
   --> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">fieldAccessPrivileges</p>
      --> <!--
       <p style="font-weight: normal;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Added the possible value CPJ (Copy). This allows Users with Planner Access Level to copy Projects.</p>
      --> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessLevelPermissions {#accesslevelpermissions}

Ett AccessLevelPermissions-objekt representerar en specifik behörighet för att komma åt, skapa eller ändra ett Workfront-objekt. Dessa behörigheter kan sedan kopplas till en åtkomstnivå.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li> <p><strong>coreAction</strong> </p> <p>Följande possibleValues har lagts till:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>En användare med en åtkomstnivå som innehåller den här behörigheten kan uppdatera planerade timmar i Utjämning av arbetsbelastning.</p> <p>Mer information finns i <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Uppdatera planerade timmar för aktiviteter vid hantering av användarallokeringar</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Hantera användarallokeringar i Utjämning av arbetsbelastning</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>En användare med en åtkomstnivå som innehåller den här behörigheten kan lägga till fält i anpassade formulär.</p> <p>Mer information finns i <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Skapa eller redigera ett anpassat formulär</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>En användare med en åtkomstnivå som innehåller den här behörigheten kan dela ett anpassat fält i hela systemet med åtkomsten Ta bort.</p> <p>Mer information finns i <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Konfigurera delning för anpassade fält och widgetar</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>forbiddenActions</strong> </p> <p>Följande possibleValues har lagts till:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>secondaryActions</strong> </p> <p>Följande possibleValues har lagts till:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">OR</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value PLANNED_HOURS_CONTOURING, which allows a user to update planned hours in the Workload Balancer</p>
    --> 
    <ul> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">coreAction</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">forbiddenActions</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">secondaryActions</p>
      --> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value ADD_TO_CUSTOM_FORMS, which allows a user to add fields to custom forms.</p>
    --> 
    <ul> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">coreAction</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">forbiddenActions</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">secondaryActions</p>
      --> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value EDIT_SYSTEMWIDE, which allows a user to share a custom field system-wide with Delete access. </p>
    --> <!--
     <ul data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
      <li> <p>coreAction</p> </li> 
      <li> <p>forbiddenActions</p> </li> 
      <li> <p>secondaryActions</p> </li> 
     </ul>
    --> </td> 
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
     <li> <p style="font-weight: bold;">åtgärd</p> <p>Följande possibleValues har lagts till:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>En användare med en åtkomstnivå som innehåller den här behörigheten kan uppdatera planerade timmar i Utjämning av arbetsbelastning.</p> <p>Mer information finns i <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Uppdatera planerade timmar för aktiviteter vid hantering av användarallokeringar</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Hantera användarallokeringar i Utjämning av arbetsbelastning</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>En användare med en åtkomstnivå som innehåller den här behörigheten kan lägga till fält i anpassade formulär.</p> <p>Mer information finns i <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Skapa eller redigera ett anpassat formulär</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>En användare med en åtkomstnivå som innehåller den här behörigheten kan dela ett anpassat fält i hela systemet med åtkomsten Ta bort.</p> <p>Mer information finns i <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Konfigurera delning för anpassade fält och widgetar</a>.</p> </li> 
      </ul> </li> 
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
   <td> 
    <ul> 
     <li><strong>coreAction</strong> <p>Följande possibleValues har lagts till:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>En användare med en åtkomstnivå som innehåller den här behörigheten kan uppdatera planerade timmar i Utjämning av arbetsbelastning.</p> <p>Mer information finns i <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Uppdatera planerade timmar för aktiviteter vid hantering av användarallokeringar</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Hantera användarallokeringar i Utjämning av arbetsbelastning</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>En användare med en åtkomstnivå som innehåller den här behörigheten kan lägga till fält i anpassade formulär.</p> <p>Mer information finns i <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Skapa eller redigera ett anpassat formulär</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>En användare med en åtkomstnivå som innehåller den här behörigheten kan dela ett anpassat fält i hela systemet med åtkomsten Ta bort.</p> <p>Mer information finns i <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Konfigurera delning för anpassade fält och widgetar</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>forbiddenActions</strong> </p> <p>Följande possibleValues har lagts till:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>secondaryActions</strong> </p> <p>Följande possibleValues har lagts till:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ActivityLog {#activitylog}

Ett ActivityLog-objekt är en fullständig lista över alla aktiviteter som har utförts i ett visst Workfront-korrekturkonto.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Operationer</p> </td> 
   <td> <p>Följande åtgärd togs bort från ActivityLog-objektet:</p> 
    <ul> 
     <li> <p><strong>LÄGG TILL</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AnnouncementAttachment {#announcementattachment}

Ett AnnouncementAttachment-objekt representerar en fil som har bifogats till ett Workfront-meddelande.

Mer information om meddelandebilagor finns i [Skicka meddelanden](../../administration-and-setup/get-started-wf-administration/view-send-announcements.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direktfält</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>fileExtension</strong> </p> <p>Möjliga värden har lagts till:</p> 
      <ul> 
       <li> <p>qdoc (enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslides (enum.fileextension.qslides)</p> </li> 
       <li> <p>qsheet (enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
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
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>Följande flaggor har tagits bort:</p> 
      <ul> 
       <li> <p>DYNAMISK,</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>Följande flaggor har lagts till</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>DYNAMISK,</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>workEffort</strong> </p> <p>Det här fältet lades till och visar om det tar en användare en liten, medelstor eller stor del av den dagliga arbetsinsatsen att slutföra en uppgift. Möjliga värden är:</p> 
      <ul> 
       <li> <p>1 (liten)</p> </li> 
       <li> <p>2 (medel)</p> </li> 
       <li> <p>3 (stor)</p> </li> 
      </ul> <p>Mer information om hur du arbetar i Workfront finns i <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Översikt över arbetsinsats</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CalendarSection {#calendarsection}

Ett kalenderavsnitt är en kalenderrapport.

Mer information om kalenderrapporter finns i [Översikt över kalenderrapporter](../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> <p style="font-weight: normal;">Följande fält har lagts till i CalendarSection-objektet för att ge stöd för den nya funktionen att använda anpassade datum i kalenderrapporter. </p> <p style="font-weight: normal;">Mer information finns i <a href="../../reports-and-dashboards/reports/calendars/use-custom-dates.md" class="MCXref xref">Använd anpassade datumfält i en kalenderrapport</a>.</p> 
    <ul> 
     <li> <p style="font-weight: normal;">customDate</p> </li> 
     <li> <p style="font-weight: normal;">customEndDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">customStartDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">ignoreActualDates</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Företag {#company}

Ett företagsobjekt representerar en organisation som består av en samling personer.

Mer information om företag finns i [Skapa och redigera företag](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">ID för gruppen som företaget är associerat med.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referensfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>grupp</p> <p style="font-weight: normal;">Gruppen som företaget är associerat med. Genom att associera ett företag med en grupp kan gruppadministratören utöka gruppåtkomst och behörigheter till företaget.</p> </li> 
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
  <tr> 
   <td>Åtgärder</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>productEnabled</strong> </p> <p style="font-weight: normal;">Den här åtgärden tar ett CustomerProductTypeEnum-argument och returnerar ett booleskt värde som anger om kunden har ett konto för produkten. </p> </li> 
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
       <li style="font-weight: normal;">lösenord:zoomIntegrationEnabled (Aktivera zoomintegration i uppdateringsströmmen)</li> 
       <li style="font-weight: normal;"> password:quipIntegrationEnabled (config.general.quip.enabled)  </li> 
      </ul> </li> 
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
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>createLinkedProofVersion</p> <p style="font-weight: normal;">Tillagd</p> </li> 
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
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">Möjligt värde har tagits bort:</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>proofDecision</strong> </p> <p>Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Åtgärder</td> 
   <td> <p>Följande åtgärder har lagts till i Document-objektet.</p> 
    <ul> 
     <li> <p style="font-weight: bold;">getDocumentReviewerDecision</p> <p style="font-weight: normal;">Den här åtgärden tar argumentet documentVersonID (sträng) och returnerar en karta som anger granskarens beslut.</p> </li> 
     <li style="font-weight: bold;"> <p>setDocumentReviewerDecision</p> <p style="font-weight: normal;">Den här åtgärden har följande argument:</p> 
      <ul style="font-weight: normal;"> 
       <li> <p>documentVersionID (sträng)</p> </li> 
       <li> <p>reviewerDecision (sträng)</p> </li> 
       <li> <p>kommentar (sträng)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Grupp  {#group}

Ett Group-objekt representerar en uppsättning användare och team. Grupper representerar ofta avdelningsstruktur.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeaderID</p> <p style="font-weight: normal;">ID för den affärsledare som är tilldelad gruppen.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referensfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeader</p> <p style="font-weight: normal;">Den affärsledare som tilldelats gruppen. En företagsledare är någon som fattar affärsbeslut för gruppen.</p> <p style="font-weight: normal;">Mer information om företagsledare finns på <a href="../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Översikt över företagsledare</a>.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Åtgärder</td> 
   <td> 
    <ul> 
     <li> <p><strong>assignMultiple</strong> </p> <p>Den här åtgärden har följande argument:</p> 
      <ul> 
       <li> <p>userIDs (string[])</p> </li> 
       <li> <p>roleIDs (string[])</p> </li> 
       <li> <p>teamID (sträng)</p> </li> 
      </ul> </li> 
     <li> <p><strong>getGroupMembers</strong> </p> </li> 
     <li> <p><strong>updateMembersList</strong> </p> <p>Den här åtgärden har följande argument:</p> 
      <ul> 
       <li> <p>newMemberID (sträng[])</p> </li> 
       <li> <p>removedMemberDs (string[])</p> </li> 
      </ul> </li> 
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
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">Möjligt värde har tagits bort:</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

Ett OpTask-objekt kallas vanligtvis för ett problem. Ett problem är en arbetsuppgift som vanligtvis anger att det finns ett problem som förhindrar att en uppgift eller ett projekt slutförs. Ett problem kan också vara en Help Desk-begäran. Ändringsorder, begäranden och buggar är också problem.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Direktfält</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>Ordningen anger en uppgifts eller artikels position på Agile-eftersläpningen.</p> <p>Det här fältet tog bort följande flaggor:
       <ul>
        <li>DYNAMISK,</li>
        <li>LAZY_READ,</li>
        <li>NOT_GROUPABLE:</li>
       </ul></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtgärder</td> 
   <td> <p>De här åtgärderna har lagt till argumentstatusen för att stödja den nya Start-knappfunktionen, som ändrar statusen för en arbetsuppgift när en användare klickar på knappen för att ange att de har påbörjat arbetet med posten.</p> <p>Mer information finns i <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Ersätta knappen Work On It (Arbeta på) med en Start-knapp</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Parameter {#parameter}

Ett Parameter-objekt är ett anpassat fält.

Parameterresursen lade till flaggan SHARABLE.

Mer information om anpassade fält finns i [Skapa eller redigera ett anpassat formulär](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) in [Skapa eller redigera ett anpassat formulär](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direktfält</td> 
   <td> 
    <ul> 
     <li> <p><strong>dataType</strong> </p> <p>Tillagt möjligt värde:</p> 
      <ul> 
       <li> <p>RICH (RTF)</p> <p>Mer information finns i <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">RTF-fält i Adobe Workfront API</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>displayType</strong> </p> <p>Tillagt möjligt värde:</p> 
      <ul> 
       <li> <p>RICH (textfält med formatering)</p> <p>Mer information finns i <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">RTF-fält i Adobe Workfront API</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>label</strong> </p> <p>Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Samlingsfält</td> 
   <td> 
    <ul> 
     <li> <p><strong>accessRules</strong> </p> <p>Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Standardfält</td> 
   <td> 
    <ul> 
     <li> <p class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"><strong>label</strong> </p> <p>Tillagd</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Portfolio {#portfolio}

Ett Portfolio-objekt är en samling projekt som konkurrerar om samma resurser, vanligtvis pengar eller personer som ska slutföra dem.

Mer information om portföljer finns i [Översikt över Portfolio i Adobe Workfront](../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">ID för gruppen som portföljen är associerad med.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referensfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>grupp</p> <p style="font-weight: normal;">Gruppen som portföljen är associerad med. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Program {#program}

Ett programobjekt är en delmängd av projekt i en portfölj, där liknande projekt kan grupperas tillsammans.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">ID för gruppen som programmet är associerat med.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referensfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>grupp</p> <p style="font-weight: normal;">Gruppen som programmet är associerat med. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

Ett QueueDef-objekt representerar en kö, vilket är ett projekt som har publicerats till Help Desk-området där användarna kan skicka problem till den.

Mer information om köer finns i [Skapa en begärandekö](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direktfält</td> 
   <td> 
    <ul> 
     <li><strong>requestCoreAction</strong> <p>Följande possibleValues har lagts till:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>En användare med en åtkomstnivå som innehåller den här behörigheten kan uppdatera planerade timmar i Utjämning av arbetsbelastning.</p> <p>Mer information finns i <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Uppdatera planerade timmar för aktiviteter vid hantering av användarallokeringar</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Hantera användarallokeringar i Utjämning av arbetsbelastning</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>En användare med en åtkomstnivå som innehåller den här behörigheten kan lägga till fält i anpassade formulär.</p> <p>Mer information finns i <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Skapa eller redigera ett anpassat formulär</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>En användare med en åtkomstnivå som innehåller den här behörigheten kan dela ett anpassat fält i hela systemet med åtkomsten Ta bort.</p> <p>Mer information finns i <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Konfigurera delning för anpassade fält och widgetar</a></p> </li> 
      </ul> <li> <p><strong>requestForbiddenActions</strong> </p> <p>Följande possibleValues har lagts till:</p> 
       <ul> 
        <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
        <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
        <li> <p>EDIT_SYSTEMWIDE </p> </li> 
       </ul> </li> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### SchemalagdRapport {#scheduledreport}

Ett ScheduledReport-objekt representerar en rapport som har konfigurerats att schemaläggas för leverans.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direktfält</td> 
   <td> 
    <ul> 
     <li> <p><strong>format</strong> </p> <p>Möjliga värden har lagts till:</p> 
      <ul> 
       <li> <p>qdoc (enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslides (enum.fileextension.qslides)</p> </li> 
       <li> <p>qsheet (enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

Ett ScoreCardQuestion-objekt representerar en fråga som har lagts till i ett styrkort. Dessa frågor avgörs vanligtvis av Portfolio-förvaltaren och deras svar gör det möjligt för förvaltaren att förstå hur väl ett projekt passar ihop med portföljens mål.

Mer information om styrkortsfrågor finns i [Skapa ett styrkort](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Möjligt värde RICH (textfält med formatering) har lagts till </p> <p style="font-weight: normal;">Mer information finns i <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">RTF-fält i Adobe Workfront API</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Uppgift {#task}

Ett Task-objekt representerar en arbetsuppgift som måste utföras som ett steg mot att uppnå ett slutligt mål (slutföra ett projekt).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direktfält</td> 
   <td> 
    <ul> 
     <li> <p><strong>workEffort</strong> </p> <p>Det här fältet lades till och visar om det tar en användare en liten, medelstor eller stor del av den dagliga arbetsinsatsen att slutföra en uppgift. Möjliga värden är:</p> 
      <ul> 
       <li> <p>1 (liten)</p> </li> 
       <li> <p>2 (medel)</p> </li> 
       <li> <p>3 (stor)</p> </li> 
      </ul> <p>Mer information om hur du arbetar i Workfront finns i <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Översikt över arbetsinsats</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtgärder</td> 
   <td> <p>De här åtgärderna har lagt till argumentstatusen för att stödja den nya Start-knappfunktionen, som ändrar statusen för en arbetsuppgift när en användare klickar på knappen för att ange att de har påbörjat arbetet med posten.</p> <p>Mer information finns i <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Ersätta knappen Work On It (Arbeta på) med en Start-knapp</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Team {#team}

Ett Team-objekt är en samling användare som kan tilldelas till ett arbetsobjekt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direktfält</td> 
   <td> <p>Följande fält har lagts till i teamresursen:</p> 
    <ul> 
     <li> <p><strong>completeDaysOnKanbanBoard</strong> </p> <p>Det här fältet visar antalet dagar som ett ifyllt kort återstår på Kanban-tavlan.</p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../agile/get-started-with-agile-in-workfront/configure-kanban.md" class="MCXref xref">Configure Kanban</a>.</p>
      --> </li> 
     <li> <p><strong>groupID</strong> </p> <p>Det här fältet associerar ett team med en grupp. Detta identifierar teamet som en del av gruppen och ger gruppadministratören möjlighet att hantera teamen.</p> </li> 
     <li> <p><strong>workOnItStatusChange</strong> </p> <p>Det här är en boolesk parameter som anger om teamets Work on It-knapp har konfigurerats som en Start-knapp. När en teammedlem klickar på en Start-knapp för att börja arbeta med ett arbetsobjekt ändras objektets status från Nytt till en status som konfigurerats i gruppinställningarna.</p> </li> 
     <li> <p>I följande fält kan du ange anpassade statusvärden för Start-knappen för de enskilda arbetsobjekten.</p> 
      <ul> 
       <li> <p><strong>workOnItOpTaskBugReportStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskChangeOrderStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskIssueStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskRequestStatuses</strong> </p> <p><strong>workOnItTaskStatuses</strong> </p> </li> 
      </ul> <p>Mer information om knappen Start finns i <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Ersätta knappen Work On It (Arbeta på) med en Start-knapp</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Referensfält</td> 
   <td> <p>Följande fält har lagts till i teamresursen:</p> 
    <ul> 
     <li> <p><strong>grupp</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateTask {#templatetask}

Ett TemplateTask-objekt representerar en aktivitet som är en del av en Template. Malluppgifter blir uppgifter i det projekt där mallen används.

Mer information om malluppgifter finns i [Redigera en malluppgift](../../manage-work/projects/create-and-manage-templates/edit-template-task.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direktfält</td> 
   <td> 
    <ul> 
     <li> <p><strong>workEffort</strong> </p> <p>Det här fältet lades till och visar om det tar en användare en liten, medelstor eller stor del av den dagliga arbetsinsatsen att slutföra en uppgift. Möjliga värden är:</p> 
      <ul> 
       <li> <p>1 (liten)</p> </li> 
       <li> <p>2 (medel)</p> </li> 
       <li> <p>3 (stor)</p> </li> 
      </ul> <p>Mer information om hur du arbetar i Workfront finns i <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Översikt över arbetsinsats</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Tidrapport {#timesheet}

Ett Timesheet-objekt representerar ett virtuellt tidkort som gör att användare kan ange faktiskt antal arbetstimmar för uppgifter, projekt och obemannade timtyper.

Mer information om tidrapporter finns i [Översikt över tidrapporter](../../timesheets/timesheets/timesheets-overview.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Kärnfält</td> 
   <td> <p>Följande fält har tagits bort från tidrapportresursen:</p> 
    <ul> 
     <li> <p><strong>objcode</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Uppdatera

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direktfält</td> 
   <td> 
    <ul> 
     <li> <p><strong>updateType</strong> </p> <p>Följande möjliga värden har lagts till:</p> 
      <ul> 
       <li> <p>InitiativeAdd (enum.updatetypeenum.initiativeadd)</p> </li> 
       <li> <p>InitiativeEdit (enum.updatetypeenum.initiativeedit)</p> </li> 
      </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Mer information om initiativ finns i <a href="../../scenario-planner/initiatives-overview.md" class="MCXref xref">Översikt över initiativ i scenarioplaneraren</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Användare {#user}

Ett User-objekt representerar en person med ett konto i Workfront som kan logga in och interagera med systemet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direktfält</td> 
   <td> <p>Följande fält har lagts till i användarresursen:</p> 
    <ul> 
     <li> <p><strong>actualDeactivationDate</strong> </p> <p>Detta representerar datum och tid då en användare inaktiverades.</p> <p>Mer information om inaktiverade användare finns i <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Inaktivera eller återaktivera en användare</a>.</p> </li> 
     <li> <p><strong>alignAccessType</strong> </p> <p>I det här fältet visas användarens åtkomst till Workfront-mål. Möjliga värden är:</p> 
      <ul> 
       <li> <p>Ingen åtkomst</p> </li> 
       <li> <p>Visa</p> </li> 
       <li> <p>Redigera</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtgärder</td> 
   <td> <p>Följande åtgärd lades till i användarresursen:</p> 
    <ul> 
     <li> <p><strong>getUserAccessPermissionsByObjCode</strong> </p> <p>Den här åtgärden använder följande argument</p> 
      <ul> 
       <li> <p>ids (sträng)</p> </li> 
       <li> <p>objCode (sträng)</p> </li> 
      </ul> </li> 
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
   <td>Direktfält</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>Ordningen anger en uppgifts eller artikels position på Agile-eftersläpningen.</p> <p>Det här fältet tog bort följande flaggor:</p> 
      <ul> 
       <li> <p>DYNAMISK,</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>I det här fältet lades följande flaggor till:</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>DYNAMISK,</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>workEffort</strong> </p> <p>Det här fältet lades till och visar om det tar en användare en liten, medelstor eller stor del av den dagliga arbetsinsatsen att slutföra en uppgift. Möjliga värden är:</p> 
      <ul> 
       <li> <p>1 (liten)</p> </li> 
       <li> <p>2 (medel)</p> </li> 
       <li> <p>3 (stor)</p> </li> 
      </ul> <p>Mer information om hur du arbetar i Workfront finns i <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Översikt över arbetsinsats</a>.</p> </li> 
    </ul> <p style="font-weight: normal;">  </p> </td> 
  </tr> 
 </tbody> 
</table>

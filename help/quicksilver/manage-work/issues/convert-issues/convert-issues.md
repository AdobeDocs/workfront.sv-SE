---
product-area: projects
navigation-topic: convert-issues
title: Översikt över konverteringsproblem i Adobe Workfront
description: Om mer arbete behöver utföras för att slutföra ett problem efter att utgåvan har skickats kan du konvertera utgåvan till ett projekt eller till en uppgift.
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 97c83b65-208b-4e3f-b4cc-681237d82aa3
source-git-commit: 7c624eff8931d206285b6c4d91083f4bf09a88b0
workflow-type: tm+mt
source-wordcount: '1289'
ht-degree: 0%

---

# Översikt över konverteringsproblem i Adobe Workfront

Om mer arbete behöver utföras för att slutföra ett problem efter att utgåvan har skickats kan du konvertera utgåvan till ett projekt eller till en uppgift.

Mer information om hur du konverterar problem till uppgifter finns i [Konvertera ett problem till en uppgift i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md).

Mer information om hur du konverterar problem till projekt finns i [Konvertera ett problem till ett projekt i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Att tänka på vid konvertering av problem

* Din Workfront-administratör eller gruppadministratör har redan angett inställningar för vad som ska hända med ett problem, dess lösning och den primära kontaktens åtkomst när den konverteras till ett projekt eller en uppgift, enligt beskrivningen i [Konfigurera inställningar för uppgifter och problem i hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* Workfront tar bort alla godkännanden som är kopplade till problem under konverteringen.
* Workfront skriver över problemets objekt när du konverterar det till en uppgift eller ett projekt. Den nya aktiviteten eller problemet blir det nya objekt som löser problemet efter konvertering.
* Tänk på följande:

   * Under konverteringen kan du få frågan om du vill behålla problemet och dess lösning knuten till det projekt eller den uppgift du håller på att skapa.
   * Om du behåller problemet uppdateras status och procent färdigt för projektet eller uppgiften automatiskt, och procentandelen färdigt för problemet när något ändras i projektet, uppgiften eller utgåvan eller när Workfront beräknar om tidslinjen.

* När du konverterar ett problem till en uppgift eller ett projekt tas problemet bort från startdelen för den användare som är tilldelad problemet.

* När du konverterar en utgåva till ett projekt med hjälp av en mall överförs den mesta informationen från mallen till det nya projektet. Men viss information från problemet kan också överföras till det nya projektet. Mer information finns i [Översikt över projektfält vid konvertering av ett ärende till ett projekt med en mall](#overview-of-project-fields-when-converting-an-issue-to-a-project-using-a-template) i den här artikeln.
* När du konverterar ett problem flyttas inte alla dokument eller deras information till det nya objektet som problemet konverteras till. Följande objekt inkluderas när du konverterar ett ärende som har bifogade dokument eller dokumentlänkar:

   * Dokument
   * Dokumentlänkar till tredjepartstjänster som Google Drive eller SharePoint.
   * Versioner
   * Korrektur inkluderas endast när alternativet **Behåll det ursprungliga problemet och knyt lösningen till den här uppgiften** är omarkerad.
   * Dokumentgodkännanden inkluderas inte när du konverterar ett problem som har bifogade dokument och dokumentlänkar.

* Om du bestämmer dig för att behålla utgåvan vid konverteringen och har bifogade dokument, kopieras dokumentet och dess versioner till projektet eller uppgiften. Korrektur och dokumentgodkännanden kopieras inte till projektet eller uppgiften.
* Om du bestämde dig för att inte behålla utgåvan vid konverteringen och den har bifogade dokument, överförs dokumentet, dess versioner och korrekturet till projektet eller uppgiften. Dokumentgodkännandena överförs inte till projektet eller uppgiften.
* Om du har dokument och mappar länkade till originalutgåvan från tredjepartstjänster, som Google Drive, oavsett om du behåller utgåvan eller inte under konverteringen, kopieras dessa länkar till det nya objektet.
* Utskickskommentarer kopieras också till uppgiften eller projektet som konverteras från problemet, men taggade användare överförs inte.
* Om du vill överföra anpassad formulärinformation från utgåvan till projektet eller uppgiften som du konverterar den till måste du se till att du har ett anpassat projekt eller en anpassad uppgift som innehåller samma fält som du vill överföra från utgåvan. Mer information finns i [Överför anpassade formulärdata vid konvertering av ett objekt](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md).

## Översikt över projektfält vid konvertering av ett ärende till ett projekt med en mall {#overview-of-project-fields-when-converting-an-issue-to-a-project-using-a-template}

När du konverterar ett problem till ett projekt kan du antingen konvertera det till ett tomt projekt eller använda en mall.

Mer information finns i [Konvertera ett problem till ett projekt i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

När du använder en mall överförs vissa fält som fylls i i mallen till projektet som skapats från den konverterade utgåvan. Andra fält överförs till projektet från den konverterade utgåvan.

I följande tabell visas projektinformation och om den överförs från mallen eller från utgåvan:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Beskrivning</td> 
   <td> <p>Beskrivning av utleverans överförs till det nya projektet. </p> <p> Om det inte finns någon beskrivning av problemet överförs beskrivningen från mallen till projektet. </p> <p>Om fältet Beskrivning är tomt både för utgåvan och mallen är fältet tomt i projektet. </p> </td> 
  </tr> 
  <tr> 
   <td>Status</td> 
   <td>Standardstatus vald för gruppen i mallen. Om mallen inte är associerad med gruppen, ställs projektstatusen in på den standardstatus som anges av Workfront-administratören i området Projektinställningar i installationsprogrammet. Mer information finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Konfigurera systemomfattande projektinställningar</a>.</td> 
  </tr> 
  <tr> 
   <td>Prioritet</td> 
   <td>Överför från mallen. </td> 
  </tr> 
  <tr> 
   <td>URL</td> 
   <td> <p>URL:en från utgåvan överförs till det nya projektet. </p> <p> Om ingen URL har angetts för problemet överförs URL:en från mallen till projektet. </p> <p>Om URL-fältet är tomt både för utgåvan och mallen är fältet tomt i projektet. </p> </td> 
  </tr> 
  <tr> 
   <td>Typ av projektvillkor</td> 
   <td>Överför från mallen.</td> 
  </tr> 
  <tr> 
   <td>Projektvillkor</td> 
   <td>Matchar standardinställningen på systemnivå enligt vad som anges av Workfront-administratören i området Inställningar. Mer information finns i <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">Ange ett anpassat villkor som standard för projekt</a></td> 
  </tr> 
  <tr> 
   <td>Schemalägg från</td> 
   <td>Överför från mallen.</td> 
  </tr> 
  <tr> 
   <td>Projektdatum</td> 
   <td> 
    <ul> 
     <li> <p><b>Planerat startdatum</b>: Den närmaste arbetstiden baserat på mallschemats arbetstid bör vara förmarkerad, enligt tidszonen för mallens schema. Det här fältet är inaktiverat om fältet Schemalägg från är inställt på Från slutförande. </p> </li> 
     <li> <p><b>Planerat slutförandedatum</b>: Den närmaste arbetstiden baserat på mallschemats arbetstid bör vara förmarkerad, enligt tidszonen för mallens schema. Det här fältet är inaktiverat om fältet Schemalägg från är inställt på Från start. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>Överför från mallen. Annars är fältet tomt.</td> 
  </tr> 
  <tr> 
   <td>Program</td> 
   <td>Överför från mallen. Annars är fältet tomt.</td> 
  </tr> 
  <tr> 
   <td>Grupp</td> 
   <td>Överför från mallen. Om det inte finns någon grupp i mallen ställs den in på den projektgrupp som utgåvan tillhör.</td> 
  </tr> 
  <tr> 
   <td>Företag</td> 
   <td>Överför från mallen. Annars är fältet tomt.</td> 
  </tr> 
  <tr> 
   <td>Projektägare</td> 
   <td>Överför från fältet Mallägare i mallen. I annat fall anges den inloggade användaren som utför konverteringen. </td> 
  </tr> 
  <tr> 
   <td>Projektsponsorer</td> 
   <td>Överför från fältet Mallsponsor i mallen. Annars är fältet tomt.</td> 
  </tr> 
  <tr> 
   <td>Resurshanteraren</td> 
   <td>Överför från mallen. Annars är fältet tomt.</td> 
  </tr> 
  <tr> 
   <td>Uppgiftsinställningar</td> 
   <td>Överför från mallen.</td> 
  </tr> 
  <tr> 
   <td>Ärendeinställningar</td> 
   <td>Överför från mallen. </td> 
  </tr> 
  <tr> 
   <td>Åtkomst</td> 
   <td> <p>Överför från Access-avsnittet i mallen. </p> </td> 
  </tr> 
  <tr> 
   <td>Godkännanden</td> 
   <td>Överför från mallen. Godkännandena som är kopplade till problemet tas bort under konverteringen. </td> 
  </tr> 
 </tbody> 
</table>

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Convert an issue to a project</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;moved to its own article)</p>
-->
<!--
<ol>
<li value="1"> Click the <strong>Issues</strong> icon on a project. <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/qs-issues-icon-highlighted-on-project.png"> </p> </li>
<li value="2"> <p>Click the issue to be converted to access the issue.</p> </li>
<li value="3"> <p> Click the <strong>More</strong> menu, then click <strong>Convert to Project</strong>. </p> <p> <img src="assets/qs-issue-more-menu-highlighted-350x469.png" style="width: 350;height: 469;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="4"> <p>In the submenu that displays, do one of the following:</p>
<ul>
<li>Click <strong>New Project</strong></li>
<li>Under <strong>New from Template</strong>, click the name of a project template you want to use</li>
</ul> </li>
<li value="5"> <p>Specify a name for the project.</p> <p>The default name is the name of the issue you are converting.</p> </li>
<li value="6">(Optional and conditional) If you are creating this project from a template, update the available fields in the Convert to Project box.<br>For more information about editing fields on projects, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
<li value="7"> <p>(Optional and conditional) Under <strong>Options</strong>, select any of the available options:</p>
<ul>
<li> <p><strong>Keep the original issue and tie its resolution to the this project</strong>When deselected, the original issue is deleted.</p> <note type="note">
<p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p>
<ul>
<li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li>
<li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a> </p> </li>
</ul>
</note> </li>
<li><strong>Allow <User Name> to have access to this project</strong>If unselected, the user who entered the issue has no access to the new task.</li>
</ul> <note type="note">
<div>
<p>The options that are available here depend on how the Workfront administrator has configured them for everyone in the system or for your group. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p>
<p>Or, if the top-level groups in your organization configured them separately, the options available here depend on which group you selected for the new project in step 6. For more information, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md" class="MCXref xref">Configure task and issue preferences for a group</a><span class="preview">.</span></p>
</div>
</note> </li>
<li value="8">(Optional) In the <strong>Custom Forms</strong> section, attach any custom forms.<br>For more information about transferring information from the custom form of the issue to that of the new project, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md" class="MCXref xref">Transfer custom form data when converting an object</a>.</li>
<li value="9"> <p>Click <strong>Save Changes.</strong></p> <p> <img src="assets/qs-issue-convert-to-project-before-saving-ui-350x366.png" style="width: 350;height: 366;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> <p>The issue is now a project, if you decided to delete the original issue.<br>Or<br>The issue is now linked to the new project and it will complete when the project completes, if you decided to keep the original issue. </p> <p>Some issue fields transfer to the project. For information, see the <a href="#view-original-issue-information-on-projects-and-tasks" class="MCXref xref">View original issue information on projects and tasks</a> section in this article. </p> </li>
<li value="10"> <p>(Optional) Set any further project details ​(project owner, project dates) and tasks as necessary.</p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Convert an issue to a task</h2> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article)</p>
-->
<!--
<ol>
<li value="1"> Click the Issues icon on a project.  </li>
<li value="2"> <p>Click the issue you want to convert to go to the issue's landing page. </p> </li>
<li value="3"> <p> Click the <strong>More</strong> menu on the issue, then <strong>Convert to Task</strong>.  </p> <p> <img src="assets/qs-issue-more-menu-highlighted-350x469.png" style="width: 350;height: 469;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="4"> <p>Name the task.</p> </li>
<li value="5"> <p>Identify the project where the task will reside. </p> <p>You can select a different project from the project that the issue is on.</p> </li>
<li value="6"> <p>In the <strong>Project</strong> box, start typing the name of the project where you want to put the new task, then press <strong>Enter</strong> when it appears.</p> <p>By default, this box the name of the project containing the issue that you are converting.</p> </li>
<li value="7"> <p>(Optional and conditional) Under <strong>Options</strong>, select any of the following options. </p> <p>The Workfront administrator or group administrator must enable these preferences before they are visible during the conversion of issues: </p>
<ul>
<li> <p><strong>Keep the original issue and tie its resolution to the this task</strong> </p> <p>If unselected, the original issue is deleted.</p> <note type="note">
<p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p>
<ul>
<li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li>
<li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a> </p> </li>
</ul>
</note> </li>
<li> <p><strong>Allow <User Name> to have access to this task</strong> </p> <p>If unselected, the user who entered the issue has no access to the new task.</p> </li>
<li> <p><strong>Keep the planned completion date of the issue</strong> </p> <p>If unselected, the Planned Completion Date of the new task is calculated from the Planned Start Date of the task. The Planned Start Date of the new task is set according to the system preferences for new tasks.</p> </li>
</ul> <note type="note">
<div>
<p>The options that display here depend on how the Workfront administrator configured them for everyone in the system. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p>
<p>Or, if the top-level groups in your organization configured them separately, the options that display here depend on which group is associated with the project you selected in step 6. For more information, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md" class="MCXref xref">Configure task and issue preferences for a group</a>.</p>
</div>
</note> </li>
<li value="8">(Optional) Attach custom forms.<br>For more information about transferring information from the custom form of the issue to that of the new task, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md" class="MCXref xref">Transfer custom form data when converting an object</a>.<br><p><img src="assets/qs-issue-convert-to-task-before-saving-ui-350x367.png" style="width: 350;height: 367;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></p></li>
<li value="9"> <p>Click <strong>Save Changes</strong> when all task settings are set.</p> <p>The issue is now a task on the designated project, if you decided to delete the original issue.</p> <p>Or</p> <p>The issue is now linked to the new task on the project you chose, and it will complete once the task completes, if you decided to keep the original issue.</p> <p>Some issue fields transfer to the task. For information, see the <a href="#view-original-issue-information-on-projects-and-tasks" class="MCXref xref">View original issue information on projects and tasks</a> section in this article. <br></p> </li>
<li value="10"> <p>(Optional) Continue editing the task (assignments, dates) as necessary. </p> </li>
</ol>
</div>
-->

## Visa ursprunglig probleminformation om projekt och uppgifter {#view-original-issue-information-on-projects-and-tasks}

Du kan visa den ursprungliga utgivningsinformationen i projekt- och uppgiftslistor och rapporter eller i området Projektinformation. Mer information om hur du skapar rapporter finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Tabellen nedan visar vilka problemfält som visas i de konverterade projekten och uppgifterna.

| Ärendefält | Projekt eller aktivitetsfält | Projektlista eller rapport | Området Projektinformation | Uppgiftslista eller rapport | Området Uppgiftsinformation |
|---|---|---|---|---|---|
| Ärendenamn | Namn på konverterat ärende | ✔ | ✔ | ✔ | ✔ |
| Primär kontakt | Namn på den som skapat det konverterade problemet | ✔ | `✔` | ✔ |   |
| Anmälningsdatum | Konverterat utgivningsdatum | ✔ |   | ✔ |   |


>[!CAUTION]
>
>Om den primära kontakten för ett problem ändras eller om problemet inte längre är länkat till projektet eller aktiviteten efter att problemet har konverterats, uppdateras inte namnet på den konverterade utgåvan och den ursprungliga primära kontakten för problemet visas när problemet konverterades.

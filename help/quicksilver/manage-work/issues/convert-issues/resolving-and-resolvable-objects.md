---
content-type: reference
product-area: projects
navigation-topic: convert-issues
title: Översikt över upplösta och upplösta objekt
description: Ett upplösningsbart objekt är ett problem vars upplösning är knuten till ett upplösningsbart objekt. Ett objekt som åtgärdar problemet är ett projekt, en uppgift eller ett annat problem.
author: Alina
feature: Work Management
exl-id: 2ff034ec-6116-42af-a55f-1fb24fc12b2f
source-git-commit: cd0adf2bd44a5c9f093e005b5af54b54ad019e34
workflow-type: tm+mt
source-wordcount: '1732'
ht-degree: 0%

---

# Översikt över upplösta och upplösta objekt

Ett upplösningsbart objekt är ett problem vars upplösning är knuten till ett upplösningsbart objekt. Ett objekt som åtgärdar problemet är ett projekt, en uppgift eller ett annat problem.

När du konverterar ett problem till en aktivitet eller ett projekt blir problemet ett objekt som kan lösas i aktiviteten eller projektet.

Du kan också manuellt länka ett problem till ett löst objekt, som kan vara en uppgift, ett projekt eller ett problem. Mer information finns i [Koppla lösningen av ett problem manuellt till andra problem, uppgifter eller projekt](../../../manage-work/issues/convert-issues/manually-tie-resolution-of-issue-to-ptis.md).

Det ursprungliga problemet blir det löstagbara objektet för aktiviteten, projektet eller problemet i det här scenariot.

## Konfigurera Adobe Workfront för hantering av upplösta objekt {#set-up-adobe-workfront-to-handle-resolvable-objects}

Som Workfront-administratör eller gruppadministratör kan du bestämma hur du vill hantera de upplösta objekten i systemet eller gruppen.

Du kan välja att behålla det löstagbara objektet när du konverterar det till en uppgift eller ett projekt, eller att ta bort det när uppgiften eller projektet har skapats. Du kan välja att tillåta att dessa inställningar ändras under konverteringen av problem, vilket gör att användaren kan välja om utgåvorna ska behållas eller tas bort när de konverteras.

>[!NOTE]
>
>Lösbara objekt är alltid problem vars upplösning och status kan vara beroende av upplösningen och statusen för det upplösta objektet som de är kopplade till. Att lösa objekt kan vara problem, uppgifter eller projekt.

Mer information om hur du ställer in inställningar för hantering av upplösta objekt finns i [Konfigurera inställningar för uppgifter och problem i hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Note: drafted and just pointed the user to the article linked above)&nbsp;</p>
<p>To establish the system default for what happens to the issue as it is being converted to a task or a project:</p>
<ol>
<li value="1">Log in to Workfront as a Workfront administrator <span>or group administrator.</span></li>
<li value="2"> <p>  From the main menu, click <strong>Setup</strong>. </p> <p> <img src="assets/qs-main-menu-expanded-with-menu-highlight-350x521.png" style="width: 350;height: 521;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">Expand <strong>Project Preferences</strong>.</li>
<li value="4">Click <strong>Tasks & Issues</strong>.</li>
<li value="5">Go to the <strong>Issues</strong> area of the setup.<br><img src="assets/qs-setup-project-preferences-issues-area-350x214.png" style="width: 350;height: 214;"><br>Consider editing any of the following settings:
<ul>
<li><p><strong>Automatically update Resolvable Issue status when the status of the Resolving Object changes:</strong> Select this option to tie the resolution of the original issue to the resolution of its Resolving Object. In order for this setting to have any effect, the options to <strong>Keep the original issue and tie its resolution to the task</strong> or<strong>project</strong> must be selected.</p>
<ul>
<li>When this setting is enabled, you can create custom statuses with the same key for both issues and projects or tasks. When the project or task (as a resolvable object) turns into the custom status, the change also reflects on the status of the issue. The status key must be the same for the issue and project or task statuses.</li>
<li><p>When this setting is disabled, resolving object statuses are automatically set to the default status, instead of the custom ones. For more information about the default statuses, see <a href="#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object" class="MCXref xref">Synchronize the Status of the Resolvable Object with that of the Resolving Object</a>.</p><note type="note">
The default status of the issue is controlled by the status of the project or task, regardless of whether this option is selected or not.
</note></li>
</ul></li>
<li><strong>When converting an issue to a TASK...:</strong> The settings in this section determine what happens during the conversion process from issue to task:
<ul>
<li><strong>Keep the original issue and tie its resolution to the task:</strong> When converting the issue, it remains visible as an issue until the task is complete. The status of the issue automatically changes to Closed when the task completes.</li>
<li><strong>Allow Primary Contact to have access to the task:</strong> Gives the primary contact (issue creator) access to the task to review the task, make updates, and stay informed of its progress.</li>
<li><strong>Allow these settings to be changed during conversion:</strong> Allows the user who is converting the issue to change these options during the conversion of an issue to a task. </li>
</ul></li>
<li><strong>When converting an issue to a PROJECT...:</strong> The settings in this section determine what happens during the conversion process from issue to project:
<ul>
<li><strong>Keep the original issue and tie its resolution to the project:</strong> When converting the issue, it remains visible as an issue until the project is complete. The status of the issue automatically changes to Closed when the project completes.</li>
<li><strong>Allow Primary Contact to have access to the project:</strong> Gives the primary contact (issue creator) access to the project to review the project, make updates, and stay informed of its progress.</li>
<li><strong>Allow these settings to be changed during conversion:</strong> Allows the user who is converting the issue to change these options during the conversion of an issue to a project. </li>
</ul></li>
</ul></li>
<li value="6">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Hantera det upplösta objektet under konverteringen till ett projekt eller en uppgift

Beroende på hur Workfront eller gruppadministratören har konfigurerat inställningar för problem på system- eller gruppnivå kan du kanske hantera det lösta objektet när ett problem konverteras till ett projekt eller en uppgift.

Följande scenarier finns:

* Om Workfront- eller gruppadministratören har **Behåll det ursprungliga problemet och knyt lösningen till uppgiften** och **Behåll det ursprungliga problemet och knyt dess lösning till projektet** markerade och **Tillåt att de här inställningarna ändras under konverteringen** Om du inte markerar det här alternativet kan du inte ändra de här inställningarna eftersom du konverterar utgåvor till aktiviteter eller projekt.\
   ![](assets/qs-setup-project-preferences-issues-area-some-boxes-unselected-350x217.png)

* Om Workfront- eller gruppadministratören har **Behåll det ursprungliga problemet och knyt lösningen till uppgiften** och **Behåll det ursprungliga problemet och knyt dess lösning till projektet** antingen markerade eller omarkerade och **Tillåt att de här inställningarna ändras under konverteringen** Om du väljer det här alternativet kan du ändra de här inställningarna när du konverterar problem till aktiviteter eller projekt.\
   ![](assets/qs-options-to-keep-issue-when-coverting-it-inside-the-issue-350x113.png)

Mer information om hur du konverterar problem till aktiviteter och projekt finns i [Översikt över konverteringsproblem i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Tie the resolution of an issue to a project, task or </h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: created new article for this section; draft when the article is live and see if you need to make a link from this one to the new article) </p>
<div>
<p>You can manually tie the resolution of an issue to the resolution of a project, task, or issue without converting the issue. The issue becomes one of the Resolvable Objects of the project, task, or issue you select. When you do this, a change in the status of the project, task, or issue triggers a change in the status of the original issue, so you cannot manually edit the status of the original issue. <br>For more information about how the status of the Resolving Object affects the Resolvable Object, see <a href="#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object" class="MCXref xref">Synchronize the Status of the Resolvable Object with that of the Resolving Object</a>.</p>
<p>You must have Manage permissions on the original issue and View permissions on the project, task, or issue to do this. </p>
<p>To tie the resolution of an issue to the resolution of a project, task, or issue:</p>
<ol>
<li value="1">Navigate to an issue whose resolution you want to tie to a task or a project.</li>
<li value="2"> <p>  Click the <strong>Issue Details</strong> > <strong>Overview</strong> area. </p> <p> <img src="assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png" style="width: 350;height: 462;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Edit</strong> icon <img src="assets/edit-icon.png"> in the upper-right corner of the Issue Details section. </p> </li>
<li value="4">At the bottom of the form,  click in the <strong>Resolved By</strong> field,  and select from the following types of resolving objects:
<ul>
<li><strong>Project</strong></li>
<li><strong>Task</strong></li>
<li><p><strong>Issue</strong></p></li>
</ul><p>The field for the resolving object displays. </p></li>
<li value="5">After selecting the object, start typing the name of a specific project, task, or issue in the available field and select it when it appears in the drop-down list. </li>
<li value="6">Click <strong>Save</strong>&nbsp;<strong>Changes</strong>.<br>The original issue becomes the Resolvable Object for the project, task, or issue you selected in step 4 and 5.<br><note type="note">
One project, task, or issue may have multiple issues as Resolvable Objects.
</note></li>
</ol>
</div>
</div>
-->

## Synkronisera statusen för det upplösta objektet med statusen för det upplösta objektet {#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object}

* [Synkronisera statusar när det lösta objektet är problem](#synchronize-statuses-when-the-resolving-object-is-an-issue)
* [Synkronisera statusar när det upplösta objektet är en uppgift eller ett projekt](#synchronize-statuses-when-the-resolving-object-is-a-task-or-a-project)

### Synkronisera statusar när det lösta objektet är problem {#synchronize-statuses-when-the-resolving-object-is-an-issue}

Om en utgåva manuellt är kopplad till en annan utgåva, utlöser den andra utgåvans status (Resolving Object) en statusändring för den första utgåvan (Resolvable Object). Status för den första utgåvan matchar status som den andra utgåvan har ändrats till. Detta gäller både standardstatus och anpassad utgivningsstatus.

### Synkronisera statusar när det upplösta objektet är en uppgift eller ett projekt {#synchronize-statuses-when-the-resolving-object-is-a-task-or-a-project}

När ett problem är det löstagbara objektet för en aktivitet eller ett projekt, ändrar aktiviteternas status och projekten status på problemet. Standardstatusvärden aktiveras annorlunda än anpassade statusvärden, i det här fallet.

* [Synkronisera standardstatusen för det upplösta objektet med standardstatusen för det upplösta objektet](#synchronize-the-default-status-of-the-resolving-object-with-the-default-status-of-the-resolvable-object)
* [Synkronisera det upplösta objektets anpassade status med det upplösta objektets anpassade status](#synchronize-the-custom-status-of-the-resolving-object-with-the-custom-status-of-the-resolvable-object)

#### Synkronisera standardstatusen för det upplösta objektet med standardstatusen för det upplösta objektet {#synchronize-the-default-status-of-the-resolving-object-with-the-default-status-of-the-resolvable-object}

Oavsett om du har markerat alternativet &quot;Uppdatera automatiskt löst problem när statusen för det upplösta objektet ändras&quot; ändras statusen för det upplösta objektet varje gång standardstatusen ändras för de upplösta objekten (projekt eller uppgifter), ändras statusen för det upplösta objektet (utleveranser). Endast standardstatusvärden har redan mappats för att utlösa en sådan ändring.

Följande standardstatusvärden för uppgifter utlöser följande ändringar i standardstatusvärdena för problem när problemet ställs in som objekt för att lösa en uppgift:

| **AKTIVITETSSTATUS** | **UTFÄRDSSTATUS** |
|---|---|
| Nytt | Nytt |
| Pågår | Pågår |
| Slutförd | Stängd |

Följande standardstatusvärden för projekt utlöser följande ändringar i standardstatusvärdena för problem när problemet ställs in som ett lösligt objekt i ett projekt. Vissa projektstatusar utlöser inga ändringar av status för problemen. Problemen är fortfarande kvar i den status de hade innan projektet omvandlades till en av följande statusar:

| **PROJEKTSTATUS** | **UTFÄRDSSTATUS** |
|---|---|
| Planering | Nytt |
| Aktuell | Pågår |
| Parkerad | Parkerad |
| Begärd | Utlöser ingen ändring av utgivningsstatus |
| Godkänd | Utlöser ingen ändring av utgivningsstatus |
| Avvisad | Utlöser ingen ändring av utgivningsstatus |
| Idea | Utlöser ingen ändring av utgivningsstatus |
| Död | Stängd |
| Slutförd | Stängd |

>[!NOTE]
>
>När status för utgåvan har stängts (till följd av att aktiviteten eller projektet har stängts) förblir utgåvan stängd, oavsett vilken status aktiviteten eller projektet ändras till efter att de har stängts.

#### Synkronisera det upplösta objektets anpassade status med det upplösta objektets anpassade status {#synchronize-the-custom-status-of-the-resolving-object-with-the-custom-status-of-the-resolvable-object}

När du ändrar status för aktiviteten eller projektet till en anpassad status ändras statusen för utgåvan till en anpassad utgåvstatus endast om följande två villkor uppfylls:

* Alternativet&quot;Uppdatera automatiskt lösningsbart problem när statusen för det upplösta objektet ändras&quot; är markerat. Mer information om hur du aktiverar den här inställningen finns i [Konfigurera Adobe Workfront för hantering av upplösta objekt](#set-up-adobe-workfront-to-handle-resolvable-objects).

* Den anpassade statusen för projektet eller aktiviteten har samma kod med tre bokstäver som den anpassade statusen för utgåvan.

Du kan skapa anpassade statusvärden med samma nyckel för både utgåvor, projekt och uppgifter. När projektet eller aktiviteten (som ett löst objekt) ändras till anpassad status, återspeglar ändringen även problemets status. Statusnyckeln måste vara densamma för utleverans- och projekt- eller aktivitetsstatus.

Du kan till exempel skapa ett anpassat projekt med namnet&quot;Starta&quot; och koden&quot;LCD&quot; med tre bokstäver som är lika med&quot;Aktuell&quot;. Du kan även skapa ett eget ärende med namnet&quot;Project Launched&quot; och bokstaven code&quot;LCD&quot; som är lika med&quot;In Progress&quot;. När du markerar projektet som&quot;Starta&quot; ändras statusen automatiskt till&quot;Starta projekt&quot;. Om inställningen &quot;Automatiskt**** Ställ in utfärdandestatus för att matcha det matchningsbara objektet med hjälp av statusnycklarna&quot; inte var aktiverad, ändras problemstatusen till &quot;Pågår&quot; i stället (standardstatus).

Mer information om hur du skapar en anpassad status finns i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Synkronisera procentandelen färdigt för ett upplöst objekt med procentandelen för det upplösta objektet

Om ett problem har lösts av en aktivitet eller ett projekt uppdateras procentandelen slutfört av problemet när något av följande inträffar: 

* När någon sparar en ändring i uppgiften eller projektet.
* Projektets tidslinje räknas om.

Om och problemet löses av en annan utgåva uppdateras procentandelen slutfört när någon av utgåvorna uppdateras.

## Leta reda på det upplösta objektet för en aktivitet eller ett projekt

Att hitta det matchande objektet är identiskt för uppgifter och projekt.

1. Navigera till ett projekt eller en uppgift som du har skapat genom att konvertera ett ärende till projektet eller uppgiften.
1. Klicka på **Projektinformation** eller **Uppgiftsinformation** och klicka för att expandera den.
1. Klicka **Översikt**.
1. Längst ned på fliken går du till **Den här lösningen** fält: problemet som är det löstagbara objektet för projektet eller uppgiften listas i det här fältet.

   >[!NOTE]
   >
   >Problem kan inte konverteras till andra problem, men de kan manuellt kopplas till ett löst problem. Ett projekt, en uppgift eller ett problem kan ha flera problem som upplösbara objekt. När projektet, aktiviteten eller problemet är löst löses även problemet med det lösta objektet. Det lösta problemet är stängt även om projektet, aktiviteten eller problemet som löste det öppnas igen.

## Identifiera ett problem med ett löst objekt i en lista

I en lista över problem kan du identifiera problem som är märkta som lösta objekt via statusikoner genom att leta upp den här ikonen i dialogrutan **Statusikoner** eller **Flaggor** kolumner:

![](assets/ro1.png)

## Visa information om objekt som kan lösas och lösas i en rapport

Du kan visa information om Resolvable eller Resolving Objects i vyn eller rapporten för projekt, uppgifter eller problem.\
Tabellen nedan visar vilka fält du kan visa och i vilka vyer du kan visa dem:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Fält i vyn</strong> </th> 
   <th><strong>Ärendevy</strong> </th> 
   <th><strong>Uppgiftsvy</strong> </th> 
   <th><strong>Projektvy</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>Har upplösningar</strong>: Visar en <strong>True</strong> om projektet eller aktiviteten har kopplade till lösta problem, och ett <strong>Falskt</strong> om de inte gör det.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td><strong>Ursprungligt utfärdningsnamn, ursprungligt utgivningsdatum, upphovsmannens namn</strong>: Visar namnet och datumet för den ursprungliga utgåvan samt namnet på den användare som skapade utgåvan i en anpassad textvy.<br>Mer information om hur du skapar ett textläge för en anpassad vy för ett projekt, en aktivitetsrapport eller en lista med information om det ursprungliga problemet finns i <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md" class="MCXref xref">Visa: visa information om ursprungligt problem i uppgifts- och projektlistor</a>.<br></td> 
   <td> </td> 
   <td> ✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lösning:</strong> Visar en lista med alla upplösningsbara objekt i en anpassad textvy för ett projekt eller en uppgiftsrapport eller -lista.</p> <p>Mer information om hur du skapar den här vyn finns i <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-resolvable-objects-task-project-report.md" class="MCXref xref">Visa: Matchbara objekt i en uppgifts- eller projektrapport</a></p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td><strong>Originator för konverterat ärende</strong>: Visar information om den användare som ursprungligen loggade problemet och som senare konverterades till uppgiften. </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>Lös projekt</strong>: Visar information om lösningsprojektet, som antingen konverterades från det ursprungliga problemet eller manuellt har angetts som lösningsobjekt för ett problem.</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>Åtgärda aktivitet</strong>: Visar information om lösningsaktiviteten som antingen har konverterats från det ursprungliga problemet eller manuellt har angetts som lösningsobjekt för ett problem.</td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>Lös problem</strong>: Visar information om problemet som manuellt har angetts som objekt för problemlösning.</td> 
   <td> ✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

---
product-area: projects
navigation-topic: manage-projects
title: Beräkna om projekttidslinjer
description: Genom att beräkna om tidslinjer kan cheferna se hur olika faktorer som är kopplade till projektet påverkar projektets tidslinje. Ett projekts tidslinje refererar till planerade och planerade datum.
author: Alina
feature: Work Management
exl-id: ec5d9a07-e45a-4aa2-9f41-9421ca5d5920
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 0%

---

# Beräkna om projekttidslinjer

Genom att beräkna om tidslinjer kan cheferna se hur olika faktorer som är kopplade till projektet påverkar projektets tidslinje. Ett projekts tidslinje refererar till planerade och planerade datum.

Om du ändrar scheman, avaktiverar personalens tid och andra objekt utanför ett projekts omfång påverkas inte projektets tidslinje omedelbart. Projektets tidslinje påverkas när tidslinjen beräknas om. Extern påverkan får inte effekt på ditt projekt förrän omberäkningen görs.

I den här artikeln beskrivs hur omberäkning av tidslinje sker.

## Åtkomstkrav

<!--drafted for P&P: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>System administrator to recalculate timeline for all projects in the system</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
Automatisk omberäkning av tidslinjen sker utan särskild åtkomst för någon av de användare som arbetar med projektet.

Du måste dock ha följande åtkomst för att manuellt beräkna om tidslinjen för ett projekt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till projekt</p> <p>Systemadministratören beräknar om tidslinjen för alla projekt i systemet</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för ett projekt</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Automatisk omberäkning

Som standard räknas projekttidslinjer om automatiskt varje dag när projektomfånget ändras eller varje natt. Workfront-administratören avgör om tidslinjer ska beräknas automatiskt varje natt eller om omfångsändringar ska göras genom att hantera tidslinjeinställningarna under Projektinställningar i installationsprogrammet. Mer information finns i [Konfigurera tidslinjeomberäkningar för projekt](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

>[!NOTE]
>
>Om tidslinjen för ett projekt är längre än 15 år inaktiveras den automatiska omberäkningen för det projektet. Du kan bara välja en uppdateringstyp av handbok för ett projekt som är längre än 15 år. Om du ändrar datum för projektet till mindre än 15 år måste du beräkna om tidslinjen manuellt en gång innan den beräknas automatiskt.

* [Automatisk omberäkning av projekttidslinjer](#automatic-recalculation-of-project-timelines)
* [Åtgärder som utlöser en automatisk omberäkning av projekttidslinjer](#actions-that-trigger-an-automatic-recalculation-of-project-timelines)

### Automatisk omberäkning av projekttidslinjer {#automatic-recalculation-of-project-timelines}

Adobe Workfront beräknar om tidslinjer dagligen endast för projekt där alla följande villkor är uppfyllda:

* Har statusen Aktuell
* Uppdateringstypen för projektet är Automatisk eller Automatisk och Vid ändring

   Mer information om typen av projektuppdateringstyp finns i [Översikt över uppdateringstyp för projekt](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

* Har ett senaste uppdateringsdatum under de senaste tre månaderna\
   Workfront-administratören kan ändra den här standardfunktionen enligt beskrivningen i [Konfigurera tidslinjeomberäkningar för projekt](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

* Senaste beräkningsdatum för projekttidslinjen ligger inte inom den aktuella kalenderdagen. Det innebär att det sista beräkningsdatumet för projekttidslinjen är före 00:00 den aktuella dagen.

Du kan konfigurera hur ofta tidslinjen för ditt projekt uppdateras. När projekttidslinjen uppdateras beräknas den om baserat på ändringar som gjorts i projektet.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
or changes made to another project that the timeline is dependent on
</MadCap:conditionalText>
-->


<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: above, the last part is drafted because of this: I don't think this is right because we told people that in the case of cross-project predecessors, the timeline must be calculated manually for the successor to see the updates in the predecessor's project. Drafting for now.)</p>
-->

Mer information finns i [Välj typ av projektuppdatering](../../../manage-work/projects/manage-projects/select-project-update-type.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;content moved to the article linked above)</p>
<p>You can configure how the timeline for your project is updated:</p>
<ol>
<li value="1">Go to the project for which you want to configure how the timeline is updated.</li>
<li value="2"> <p>  Click the <strong>More</strong> icon <img src="assets/more-icon.png"> to the right of the project name, then click&nbsp; <strong>Edit</strong>. </p> <p>The <strong>Edit Project</strong> dialog box is displayed.</p> </li>
<li value="3"> <p>Click<strong>Settings.</strong><br><img src="assets/screen-shot-2013-09-18-at-10.36.16-am-350x347.png" alt="" style="width: 350;height: 347;"></p> </li>
<li value="4">In the <strong>Update Type</strong> drop-down list, select from the following options:<br><strong>- Automatic and On Change:</strong> (Default setting) The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on. The project timeline is also updated each night. <br>This is the recommended setting for this field because it ensures that the project timeline is always up to date.<br>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed.
<div>
<p><img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"></p>
</div><br>This indicates that the recalculation is not yet finished, and the dates are subject to change. <br><strong>- Change Only:</strong> The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur.<br>You might want to select this option if changes rarely occur in the project or in other projects that the timeline is dependent on.<br><strong>- Automatic Only:</strong> The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if many changes occur each day in the project or in other projects that the timeline is dependent on.<br><note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note><br><strong>- Manual Only:</strong> The project timeline is updated only when you select the option to Recalculate Timelines, as described in <a href="#manual-recalculation" class="MCXref xref">Manual recalculation</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).<br>For more information about the project Update Type, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a><note type="note">
If the timeline of a project is longer than 15 years, the automatic recalculation is disabled. If you change the dates on the project to less than 15 years, you must manually recalculate your timeline one time before it is calculated automatically.
</note></li>
<li value="5">Click <strong>Save Changes.</strong></li>
</ol>
</div>
-->

### Åtgärder som utlöser en automatisk omberäkning av projekttidslinjer {#actions-that-trigger-an-automatic-recalculation-of-project-timelines}

Olika omfångsförändringar i ett projekts livslängd beräknar automatiskt om projektets tidslinje, inklusive följande åtgärder:

* Uppdaterar aktivitetsstatus.
* Flytta en uppgift till ett annat projekt.
* Uppdaterar aktiviteternas planerade datum eller planerade slutförandedatum.
* Uppdaterar varaktighetstypen, aktivitetsbegränsningen eller antalet tilldelningar för aktiviteterna.
* Uppdaterar relationer till föregående aktiviteter.
* Lägga till ett godkännande för en aktivitet som också lägger till tid till aktivitetens planerade slutförandedatum.\
   Mer information om inställningar för godkännande finns i [Konfigurera globala inställningar för godkännande](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

## Manuell omberäkning {#manual-recalculation}

Som projektägare kan du manuellt beräkna om tidslinjerna för enskilda projekt. Workfront-administratören kan manuellt beräkna om alla tidslinjer i Workfront.

* [Beräkna om tidslinjer för enskilda projekt eller gruppvis](#recalculate-timelines-for-individual-projects-or-in-bulk)
* [Automatisk omberäkning av flera tidslinjer samtidigt i rutan Redigera projekt](#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box)
* [Beräkna om tidslinjer för alla projekt i systemet (endast Workfront-administratörer)](#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only)

### Beräkna om tidslinjer för enskilda projekt eller gruppvis {#recalculate-timelines-for-individual-projects-or-in-bulk}

Du kan beräkna om tidslinjen för ett projekt i Workfront från projektsidan eller från en projektlista eller rapport.

1. Gå till det projekt som du vill beräkna om tidslinjen för och klicka på **Mer** icon ![](assets/qs-more-menu.png) till vänster om projektnamnet

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   eller

   Gå till en projektlista eller rapport och välj ett eller flera projekt. Klicka sedan på **Mer** icon ![](assets/qs-more-menu.png) högst upp i listan.

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >Beroende på hur komplexa dina projekt är rekommenderar vi att du inte väljer ett stort antal projekt när du omberäknar deras tidslinjer i grupp för att få optimala prestanda. Vissa saker som kan göra ett projekt för komplext kan vara flera beroenden eller tilldelningar, eller ett stort antal anpassade fält.

1. Klicka **Beräkna om tidslinje**.

   När tidslinjen har beräknats om visas ett meddelande om att omberäkningen lyckades.

   >[!TIP]
   >
   >Innan tidslinjens omberäkning är klar kan vissa planerade eller projicerade datum visas som nedtonade. Detta innebär att omberäkningen inte är klar ännu och att datumen kan ändras.

### Automatisk omberäkning av flera tidslinjer samtidigt i rutan Redigera projekt {#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box}

Du kan manuellt beräkna om tidslinjerna i flera projekt genom att redigera dem flera gånger.

>[!TIP]
>
>Beroende på hur komplexa dina projekt är rekommenderar vi att du inte väljer ett stort antal projekt när du redigerar dem i grupp för att få optimala prestanda. Vissa saker som kan göra ett projekt för komplext kan vara flera beroenden, tilldelningar eller ett stort antal anpassade fält.

1. Gå till en lista med projekt.
1. Markera flera projekt i listan och klicka sedan på **Redigera**.
1. Klicka **Inställningar** väljer **Beräkna om tidslinjer**.

1. Klicka **Spara ändringar**.

### Beräkna om tidslinjer för alla projekt i systemet (endast Workfront-administratörer) {#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only}

Workfront-administratörer kan köra diagnostiken för att beräkna om tidslinjen för att omedelbart beräkna om alla tidslinjer i Workfront-systemet. Detta gör att alla projektledare kan se hur externa ändringar påverkar direkt både planerade och planerade datum.

Mer information om hur du beräknar om tidslinjer för hela Workfront-webbplatsen finns i avsnittet Beräkna om tidslinjer för hela Workfront-instansen i [Konfigurera tidslinjeomberäkningar för projekt](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Project Update Types</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and moved to thisa rticle: /Content/Manage work/Projects/Planning a Project/project-update-type-overview.htm)</p>
<p>For information about how to update the project's Update Type, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>. </p> <note type="important">
If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual.
</note>
<p>You can select how each project calculates its timeline by choosing between the following Update Types:</p> <note type="important">
If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual.
</note>
<ul>
<li> <p><strong>Automatic and On Change:</strong>&nbsp;This is the default setting. The project timeline is updated each time a change occurs&nbsp;in the project or in another project that the timeline is dependent on. The project timeline is also updated each night.&nbsp; <br>This is the recommended setting as it ensures that the project timeline is always up to date.</p> <p>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed. </p> <p> <img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"> </p> <p>This indicates that the recalculation is not yet finished, and the dates are subject to change. </p> </li>
<li><strong>Change Only:</strong>&nbsp;The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur. <br>You might want to select this option if you are concerned about system performance and if&nbsp;changes rarely occur in the project or in other projects that the timeline is dependent on.</li>
<li> <p><strong>Automatic Only:</strong>&nbsp;The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if you are concerned about system performance and if many changes occur each day in the project or in other projects that the timeline is dependent on.</p> <note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note> </li>
<li><strong>Manual Only:</strong>&nbsp;The project timeline is updated only&nbsp;when you select the option to <strong>Recalculate Timelines</strong>, as described in the section "Manual Recalculation" in&nbsp;the article <a href="#" class="MCXref xref selected">Recalculate project timelines</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).</li>
</ul>
</div>
-->

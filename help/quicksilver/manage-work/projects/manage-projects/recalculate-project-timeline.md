---
product-area: projects
navigation-topic: manage-projects
title: Beräkna om projekttidslinjer
description: Genom att beräkna om tidslinjer kan cheferna se hur olika faktorer som är kopplade till projektet påverkar projektets tidslinje. Ett projekts tidslinje refererar till planerade och planerade datum.
author: Alina
feature: Work Management
exl-id: ec5d9a07-e45a-4aa2-9f41-9421ca5d5920
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '1077'
ht-degree: 0%

---

# Beräkna om projekttidslinjer

<!--Audited: 06/2025-->

Genom att beräkna om tidslinjer kan cheferna se hur olika faktorer som är kopplade till projektet påverkar projektets tidslinje. Ett projekts tidslinje refererar till planerade och planerade datum.

Om du ändrar scheman, avaktiverar personalens tid och andra objekt utanför ett projekts omfång påverkas inte projektets tidslinje omedelbart. Projektets tidslinje påverkas när tidslinjen beräknas om. Extern påverkan får inte effekt på ditt projekt förrän omberäkningen görs.

I den här artikeln beskrivs hur omberäkning av tidslinje sker.

Automatisk omberäkning av tidslinjen sker utan särskild åtkomst för någon av de användare som arbetar med projektet. Dessutom kan du manuellt beräkna om tidslinjen.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Standard</p> 
    <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt</p> <p>Systemadministratören beräknar om tidslinjen för alla projekt i systemet</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för ett projekt</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Standard </p> 
    <p>Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> <p>System administrator to recalculate timeline for all projects in the system</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Automatisk omberäkning

Som standard räknas projekttidslinjer om automatiskt varje dag när projektomfånget ändras eller varje natt. Workfront-administratören avgör om tidslinjer ska beräknas automatiskt varje natt eller om omfångsändringar ska göras genom att hantera tidslinjeinställningarna under Projektinställningar i installationsprogrammet. Mer information finns i [Konfigurera tidslinjeomberäkningar för projekt](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

>[!IMPORTANT]
>
>* Om tidslinjen för ett projekt är längre än 15 år inaktiveras den automatiska omberäkningen för det projektet och du kan bara välja en manuell uppdateringstyp. Om du ändrar datum för projektet till mindre än 15 år måste du beräkna om tidslinjen manuellt en gång innan den beräknas automatiskt.
>* I sandlådemiljöerna Förhandsgranska och Anpassad uppdatering inaktiveras nattomberäkningen och projekttidslinjerna beräknas inte om automatiskt. Du måste beräkna om projekttidslinjen manuellt för miljöerna Preview och Custom Refresh Sandbox.
>* Om ett projekt är komplext kanske den automatiska tidslinjeberäkningen inte utförs.
> Ett exempel på ett komplext projekt kan vara ett projekt med flera beroenden, ett stort antal uppgifter, flera föregångare mellan projekt eller flera indrag för uppgifter.
> Workfront skickar en varning till höger om projektnamnet på projektsidan som talar om för användarna att projekttidslinjen måste beräknas om manuellt. Endast användare med behörigheten Hantera för projektet kan beräkna om tidslinjen manuellt.
>
>   ![Projektvarning för att beräkna om tidslinjen](assets/project-warning-to-manually-recalculate-timeline.png)
>

* [Automatisk omberäkning av projekttidslinjer](#automatic-recalculation-of-project-timelines)
* [Åtgärder som utlöser en automatisk omberäkning av projekttidslinjer](#actions-that-trigger-an-automatic-recalculation-of-project-timelines)



### Automatisk omberäkning av projekttidslinjer {#automatic-recalculation-of-project-timelines}

Workfront beräknar om tidslinjer dagligen endast för projekt där alla följande villkor är uppfyllda:

* Har statusen Aktuell.
* Projektuppdateringstypen är Automatisk eller Automatisk och Vid ändring.

  Mer information finns i [Översikt över projektuppdateringstyp](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

* Ha ett senaste uppdateringsdatum under de senaste tre månaderna. En Workfront-administratör kan ändra den här standardfunktionen. Mer information finns i [Konfigurera tidslinjeomberäkningar för projekt](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

* Senaste beräkningsdatum för projekttidslinjen ligger inte inom den aktuella kalenderdagen. Det innebär att det sista beräkningsdatumet för projekttidslinjen är före 0:00 på den aktuella dagen.

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
<p>(NOTE: content moved to the article linked above)</p>
<p>You can configure how the timeline for your project is updated:</p>
<ol>
<li value="1">Go to the project for which you want to configure how the timeline is updated.</li>
<li value="2"> <p>  Click the <strong>More</strong> icon <img src="assets/more-icon.png"> to the right of the project name, then click  <strong>Edit</strong>. </p> <p>The <strong>Edit Project</strong> dialog box is displayed.</p> </li>
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
  Mer information om godkännandeinställningar finns i [Konfigurera globala godkännandeinställningar](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

## Manuell omberäkning {#manual-recalculation}

Som projektägare kan du manuellt beräkna om tidslinjerna för enskilda projekt. Workfront-administratören kan manuellt beräkna om alla tidslinjer i Workfront.

* [Beräkna om tidslinjer för enskilda projekt eller gruppvis](#recalculate-timelines-for-individual-projects-or-in-bulk)
* [Beräkna flera tidslinjer manuellt i rutan Redigera projekt](#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box)
* [Beräkna om tidslinjer för alla projekt i systemet (endast Workfront-administratörer)](#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only)

### Beräkna om tidslinjer för enskilda projekt eller gruppvis {#recalculate-timelines-for-individual-projects-or-in-bulk}

Du kan beräkna om tidslinjen för ett projekt i Workfront från projektsidan eller från en projektlista eller rapport.

1. Gå till projektet som du vill beräkna om tidslinjen för och klicka på ikonen **Mer** ![Mer meny](assets/qs-more-menu.png) till vänster om projektnamnet.

   eller

   Gå till en projektlista eller rapport och välj ett eller flera projekt och klicka sedan på ikonen **Mer** ![Mer-menyn](assets/qs-more-menu.png) överst i listan.

   ![Omberäkna uttryckets tidslinje med listrutan Ekonomi](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >Beroende på hur komplexa dina projekt är rekommenderar vi att du inte väljer ett stort antal projekt när du omberäknar deras tidslinjer i grupp för att få optimala prestanda. Vissa saker som kan göra ett projekt för komplext kan vara flera beroenden eller tilldelningar, eller ett stort antal anpassade fält.

1. Klicka på **Beräkna om tidslinje**. Tidslinjen beräknas om och ett meddelande om att åtgärden lyckades visas på skärmen.

   >[!TIP]
   >
   >Innan tidslinjens omberäkning är klar kan vissa planerade eller projicerade datum visas som nedtonade. Detta innebär att omberäkningen inte är klar ännu och att datumen kan ändras.

### Automatisk omberäkning av flera tidslinjer samtidigt i rutan Redigera projekt {#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box}

Du kan manuellt beräkna om tidslinjerna i flera projekt genom att redigera dem flera gånger.

>[!TIP]
>
>Beroende på hur komplexa dina projekt är rekommenderar vi att du inte väljer ett stort antal projekt när du redigerar dem i grupp för att få optimala prestanda. Vissa saker som kan göra ett projekt för komplext kan vara flera beroenden eller tilldelningar, eller ett stort antal anpassade fält.

1. Gå till en lista med projekt.
1. Markera flera projekt i listan och klicka sedan på **Redigera**.
1. Klicka på **Inställningar** och välj sedan **Beräkna om tidslinjer**.

1. Klicka på **Spara ändringar**.

### Beräkna om tidslinjer för alla projekt i systemet (endast Workfront-administratörer) {#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only}

Workfront-administratörer kan köra diagnostiken för att beräkna om tidslinjen för att omedelbart beräkna om alla tidslinjer i Workfront. Detta gör att alla projektledare kan se hur externa ändringar påverkar direkt både planerade och planerade datum.

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
<li> <p><strong>Automatic and On Change:</strong> This is the default setting. The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on. The project timeline is also updated each night.  <br>This is the recommended setting as it ensures that the project timeline is always up to date.</p> <p>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed. </p> <p> <img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"> </p> <p>This indicates that the recalculation is not yet finished, and the dates are subject to change. </p> </li>
<li><strong>Change Only:</strong> The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur. <br>You might want to select this option if you are concerned about system performance and if changes rarely occur in the project or in other projects that the timeline is dependent on.</li>
<li> <p><strong>Automatic Only:</strong> The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if you are concerned about system performance and if many changes occur each day in the project or in other projects that the timeline is dependent on.</p> <note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note> </li>
<li><strong>Manual Only:</strong> The project timeline is updated only when you select the option to <strong>Recalculate Timelines</strong>, as described in the section "Manual Recalculation" in the article <a href="#" class="MCXref xref selected">Recalculate project timelines</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).</li>
</ul>
</div>
-->

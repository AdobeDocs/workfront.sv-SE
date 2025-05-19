---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Översikt över tilldelning av arbete i belastningsutjämnaren
description: Som resurshanterare kan du använda Adobe Workfront Workload Balancer för att visa arbetsobjekt som ännu inte har tilldelats användare samt tilldela dem dessa objekt.
author: Lisa
feature: Resource Management
exl-id: 98779b67-b975-4501-8426-63e255b1d7df
source-git-commit: 7f0aac7c8519b1e570e29fedf1492918e8120ad2
workflow-type: tm+mt
source-wordcount: '1032'
ht-degree: 0%

---

# Översikt över tilldelning av arbete i belastningsutjämnaren

<!-- Audited: 5/2025 -->

Som resurshanterare kan du använda Adobe Workfront Workload Balancer för att visa arbetsobjekt som ännu inte har tilldelats användare samt tilldela dem dessa objekt.

Allmän information om belastningsutjämnaren för arbetsbelastning finns i [Översikt över belastningsutjämnaren](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Du kan tilldela arbetsobjekt (uppgifter och ärenden) till användare i andra områden av Workfront. Genom att använda Utjämning av arbetsbelastning kan du enkelt förstå användarnas tillgänglighet och tydligt se alla andra objekt som de är tilldelade innan du tilldelar dem mer arbete.

Mer information om hur du tilldelar arbetsobjekt i andra delar av Workfront finns i följande artiklar:

* [Tilldela uppgifter](../../manage-work/tasks/assign-tasks/assign-tasks.md)
* [Tilldela ärenden](../../manage-work/issues/manage-issues/assign-issues.md)

## Tillgänglighet för användare i Utjämning av arbetsbelastning

Du kan tilldela arbete i belastningsutjämnaren så att det matchar användarens tillgängliga tid. För att vara säker på att du tilldelar rätt mängd arbete och inte överfördelar användaren måste summan för Planerade timmar för arbetsobjekten som tilldelats användaren matcha fördelningarna per dag eller vecka.

Det är viktigt att förstå hur Workfront beräknar den tillgängliga tiden för en användare.

Workfront använder följande information för att beräkna användarens kapacitet i belastningsutjämnaren:

* Inställningar för resurshantering. Workfront-administratören bestämmer hur den tillgängliga tiden beräknas för systemet genom att välja att använda något av följande i området Resurshantering under Konfigurera:

   * Standardschemat för Workfront-systemet och användarens FTE.
   * Användarens schema, enligt vad som anges i området Användarprofil.

     Detta beräknar användarens dagliga och veckovisa tillgänglighet. Eventuella schemaundantag för det valda schemat återspeglas i användarens kapacitet i Utjämning av arbetsbelastning.

  Mer information finns i [Konfigurera inställningar för resurshantering](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

  Mer information om scheman finns i [Skapa ett schema](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Användaren är ledig. Detta anger vilka dagar som användaren planerar att starta.

  Mer information finns i [Konfigurera personlig tid för ](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* Användarens arbetstid. Detta anger hur många procent av heltidstiden som användaren är tillgänglig för att utföra faktiskt projektrelaterat arbete, exklusive extrakostnader. Ange värdet 1 för Arbetstid för att ange att användaren är tillgänglig för projektrelaterat arbete och hela heltidsekvivalenten.


## Tilldela arbete i arbetsbelastningsutjämnaren

Du kan tilldela arbetsobjekt som ännu inte har tilldelats en användare eller tilldela om artiklar som har tilldelats användare i Utjämning för arbetsbelastning.

Du kan tilldela arbete i belastningsutjämnaren på följande sätt:

* Ett objekt i taget genom att tilldela varje objekt manuellt.

  Du kan göra avancerade uppdrag när du tilldelar objekt manuellt, en åt gången.

  Mer information finns i [Tilldela arbete manuellt med hjälp av arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

* Ett objekt i taget genom att dra och släppa arbetsobjekt till den användare som ska tilldelas.

  Mer information finns i [Tilldela arbete i Utjämning av arbetsbelastning genom att dra och släppa](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md).

* Flera objekt i taget med alternativet Gruppera tilldelningar. Du kan definiera regler som objekten tilldelas till flera användare samtidigt.

  Mer information finns i [Tilldela flera arbeten samtidigt med hjälp av arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

Mer information om hur du frigör arbete finns i [Ta bort tilldelning av arbete i arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

## Uppdragsområden i Utjämning av arbetsbelastning

Du kan tilldela användare arbete med hjälp av belastningsutjämnaren i resursområdet, i projektet eller på teamnivå. Mer information om var arbetsbelastningsutjämnaren finns i Workfront finns i [Hitta arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

Det finns två områden i belastningsutjämnaren där du kan visa arbetsobjekt:

* **Ej tilldelat arbete**: Visar objekt som inte har tilldelats användare.
* **Tilldelad arbetsuppgift**: Visar objekt som har tilldelats användare.

I följande tabell beskrivs vilka objekt som visas i varje område baserat på deras uppdrag:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Typ av tilldelning</strong> </td> 
   <td colspan="2"><strong>Områden där tilldelningarna är synliga</strong> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td>Ej tilldelat arbete </td> 
   <td>Tilldelat arbete </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span style="font-weight: normal;">Ej tilldelat objekt</span> </td> 
   <td><span> ✔</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Team</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span data-mc-edit-date="2020-04-08T15:57:40.7175506-04:00" data-mc-editor="alinawilson" data-mc-comment="Drafted because role only is not displayed; first it will be displayed in Unassigned - 20.2 beta" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2019-11-15T13:24:04.5189150-05:00">Roll</span> </td> 
   <td><span> ✔</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Roll och team</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Användare</td> 
   <td> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Användare och team</td> 
   <td> <p> </p> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Användare, roll och team</td> 
   <td>✔*</td> 
   <td>✔**</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Användare och roll</p> </td> 
   <td><span data-mc-edit-date="2019-11-15T13:37:42.5435254-05:00" data-mc-editor="alinawilson" data-mc-comment="drafted because it's not in the Unassigned" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2019-11-15T13:37:33.3097484-05:00"> ✔</span>*</td> 
   <td>✔**</td> 
  </tr> 
 </tbody> 
</table>

&#42;När en arbetsuppgift tilldelas till en användare och en roll visas den endast i arbetsytan Ej tilldelad när rollen är primär tilldelad.

&#42;&#42;När en arbetsuppgift tilldelas till en användare och en annan enhet visas den endast i den tilldelade arbetsytan när användaren är primär tilldelad.

Mer information om Ej tilldelade och tilldelade områden i Utjämning av arbetsbelastning finns i [Navigera i Utjämning av arbetsbelastning](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Överväganden för flera tilldelningar till jobbroller, team och användare

Tänk på följande när du tilldelar flera resurser till en arbetsuppgift:

* Användare kan ha mer än en jobbroll kopplad till sin profil. Mer information om hur du associerar användare med jobbroller finns i [Redigera en användares profil](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Uppgifter eller ärenden tilldelas vanligtvis först till en eller flera jobbroller eller till ett team. När projekten är klara att starta kan de behöva tilldelas användare.\
  Om en uppgift eller ett ärende tilldelas till en eller flera roller och du sedan även tilldelar en användare, bestämmer Adobe Workfront vilken jobbroll som ska associeras med den andra användaren (om någon) enligt följande regler:

   * Om det bara finns en tilldelad jobbroll och den matchar användarens primära roll, tilldelas uppgiften eller utgåvan endast den användare som fyller sin primära roll.
   * Om det finns flera roller tilldelade och minst en av rollerna matchar användarens sekundära roller, tilldelas uppgiften eller utgåvan till användaren som uppfyller en av deras övriga roller - som Workfront väljer slumpmässigt om det finns flera matchningar - samt eventuella ytterligare roller som tilldelas.
   * Om det finns en eller flera jobbroller tilldelade och det inte finns några matchningar mot användarens roller, tilldelas uppgiften eller utgåvan till både rollen eller rollerna och till användaren.

* Om en uppgift eller ett problem har tilldelats ett team och du även tilldelar en användare, förblir uppgiften eller utgåvan tilldelad till både teamet och användaren.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2 data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Manually assign one item at a time</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Moved manual assignment and drag-and-drop to their own articles) </p>
<ol>
<li value="1">Go to the Workload Balancer.</li>
<li value="2"> <p>Go to the <strong>Unassigned Work</strong> area and apply a filter to view work items</p> <p>Or</p> <p>Go to the <strong>Assigned Work</strong> area and expand the name of a user to view the work items assigned to them.</p> <note type="important">
<span>You cannot view and assign issues from the Unassigned Work area. You can only reassign issues already assigned to users in the Assigned Work area. Otherwise,</span> you can assign issues from a list or at the issue level. For information, see
<a href="../../manage-work/issues/manage-issues/assign-issues.md" class="MCXref xref">Assign issues</a>.
</note> </li>
<li value="3"> <p>Click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> on the bar of a work item, then click <strong>Assign this to</strong>. </p> <p> <img src="assets/workload-balancer-assign-this-to-link-from-task-350x117.png" style="width: 350;height: 117;"> </p> <note type="tip">
<p><span>You can also use the following shortcuts to assign tasks or issues:</span> </p>
<ul>
<li><span>In Windows: CTRL+click the task or issue bar.</span> </li>
<li><span>In&nbsp;Mac: CMD+click the task or issue bar.</span> </li>
</ul>
</note> </li>
<li value="4"> <p>Start typing the name of a user, job role, or team that you want to assign to the item in the <strong>Search people, role or teams</strong> field, select it when it displays in the list, then click&nbsp;<strong>Save</strong>. </p> <p> <img src="assets/assignments-box-wb.png"> </p> <p>This assigns or reassigns the work item to the specified assignees.</p> <p>If you assign an item to just a team or a job role, the item displays only in the Unassigned Work area. You must assign work items to users in order to display them in the Assigned Work area of the Workload Balancer.</p> <note type="tip">
<p>You can assign multiple users or job roles, and you can assign only one team. <span>You can assign only active users, <span>job roles</span>, and teams.</span></p>
<p><span>If a user, <span>job role</span>, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:</span> </p>
<ul>
<li> <p><span>Reassign the work item to active resources.</span> </p> </li>
<li> <p><span>Associate the users in a deactivated team with an active team and reassign the work item to the active team.</span> </p> </li>
</ul>
</note> </li>
<li value="5"> <p>(Optional) Click the <strong>Show allocations icon</strong> <img src="assets/show-allocations-icon-small.png">, then click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> > <strong>Edit allocations</strong>.</p> <p>Or</p> <p>Double-click a daily or weekly allocation to modify the amount of time the user is allocated to the work item.</p> <p>For information about modifying user allocations in the Workload Balancer, see the "Modify user allocations"&nbsp;section in the article <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> </li>
</ol>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<h2>Assign an item by dragging and dropping</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider retitling this to "Assign one item at a time by dragging and dropping" when bulk assignments will come???)&nbsp;</p>
<p>You can assign an item from the Unassigned Work area to a user, or you can reassign an already assigned item to another user in the Assigned Work area.</p>
<ol>
<li value="1">Go to the Workload Balancer.</li>
<li value="2"> <p>Go to the <strong>Unassigned Work</strong> area and apply a filter to view work items.</p> <note type="important">
<span>You cannot view and assign issues from the Unassigned Work area.</span>
</note> </li>
<li value="3"> <p>Click the bar of a work item that indicates either the planned or the projected timeline and drag it over the name of a user in the <strong>Assigned</strong> area.</p> <p>The user you hover over to drop the work item to is highlighted.</p> <note type="tip">
The Planned Hours for the user you're hovering over update in real time with the number of daily Planned Hours from the work item, to indicate what the impact of adding a new item might be to their overall allocation.
</note> <p> <img src="assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png" style="width: 350;height: 152;"> </p> </li>
<li value="4"> <p>When you are ready, drop the selected work item in the same line as the user's name in the Assigned Area. The item is assigned and the allocated Planned Hours are updated for the user with the new hours from the work item.</p> <note type="tip">
<p>If you enabled Group by Project in the Settings area, the assigned task displays under the corresponding project. If the setting is disabled, the assigned task displays in the user area. </p>
<p>The item displays according to the Workload Balancer criteria for sorting work items.&nbsp;For more information, see <a href="../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navigate the Workload Balancer</a>.</p>
</note> </li>
<li value="5"> <p>(Optional) Click the <strong>Show allocations icon</strong> <img src="assets/show-allocations-icon-small.png">, then click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> > <strong>Edit allocations</strong>. (NOTE: make sure these are still called this, and that the icon has not changed)</p> <p>Or</p> <p>Double-click a daily or weekly allocation to modify the amount of time the user is allocated to the work item.</p> <p>For information about modifying user allocations in the Workload Balancer, see the "Modify user allocations"&nbsp;section in the article <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> </li>
</ol> 
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Assign items in bulk</h2>
<p>(NOTE: This is also a separate article. Should we keep this section or the separate article?) </p>
</div>
<p>&nbsp;</p>
</div>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Unassign work items in the Workload Balancer</h2>
<p>(NOTE: moved this section to a new article. Draft here at release to preview) </p>
<p>You can either unassign items from users and move them to the Unassigned Work area, or reassign them to other users. </p>
<p>To unassign work items from users: </p>
<ol>
<li value="1">In the Workload Balancer, go to the <strong>Assigned Work</strong> area and expand a user.</li>
<li value="2">Do 
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
one of
</MadCap:conditionalText>
the following:
<ul>
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Find the item you want to unassign in a user's area, click it, drag and drop it in the Unassigned area or in another user's area. </p></li>
<li><p>Click the <strong>More</strong> icon <img src="assets/more-icon-task-list.png"> to the right of the name of a work item, click&nbsp;<strong>Assign this to</strong> , then remove the name of the entities assigned to the work item or enter another name and click&nbsp;<strong>Save</strong>.</p><p><img src="assets/workload-balancer-assign-this-to-link-from-task-350x117.png" style="width: 350;height: 117;"></p></li>
</ul><p>The item displays in the Unassigned Work area if it matches the filtering criteria for that area and it is not assigned to any users or it displays in the user area if it is assigned to that user. </p><note type="tip">
Unassigned issues do not display in the Unassigned area.
</note><p>For information about filtering information in the Workload Balancer, see <a href="../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md" class="MCXref xref">Manage filters in the Workload Balancer</a>. </p></li>
</ol>
</div>
-->

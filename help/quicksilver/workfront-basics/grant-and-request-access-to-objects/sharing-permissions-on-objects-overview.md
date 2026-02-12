---
content-type: overview
navigation-topic: grant-and-request-access-to-objects
title: Översikt över delningsbehörigheter för objekt
description: Du kan dela eller ta bort behörigheter till ett objekt som du har skapat eller ett objekt som delats med dig.
author: Courtney
feature: Get Started with Workfront
exl-id: 7c14702e-ac55-4266-88a7-f31618f84218
source-git-commit: 97f5adc8811a3be7be23137a82d10d45b76ec605
workflow-type: tm+mt
source-wordcount: '1332'
ht-degree: 0%

---

# Översikt över delningsbehörigheter för objekt

<!-- Audited: 12/2023 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Redundancy here with the article Permissions for shared objects?</p>
-->
När du delar ett objekt med någon i systemet kan du ge mottagaren någon av följande behörigheter: visa, bidra och hantera.

Du behöver inte vara Adobe Workfront-administratör för att dela behörigheter för objekt som du har åtkomst till, men dina behörigheter för objekt fungerar inom de åtkomstnivåer som anges av Workfront-administratören.

Du kan dela eller ta bort behörigheter till ett objekt som du har skapat eller ett objekt som delats med dig. När du inte är den som har skapat objektet måste du ha delningsåtkomst för objektet som du vill dela på åtkomstnivån, förutom att du måste ha delningsbehörighet för objektet. Mer information om åtkomstnivåer finns i [Översikt över nya åtkomstnivåer](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md) eller [Översikt över åtkomstnivåer](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

>[!NOTE]
>
>En Workfront-administratör kan lägga till eller ta bort behörigheter för alla objekt i systemet, för alla användare, utan att vara ägare av dessa objekt.

## Objekt som du kan dela i Workfront

Du kan dela följande objekt i Workfront med andra användare:

* **Projekt**: Mer information finns i [Dela ett projekt i Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* **Mallar**: Mer information finns i [Dela projektmallar](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

* **Portföljer**: Mer information finns i [Dela en portfölj](../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio.md).

* **Program**: Mer information finns i [Dela ett program](../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md) .

* **Uppgifter**: Mer information finns i [Dela en uppgift](../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

* **Problem**: Mer information finns i [Dela ett problem](../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

* **Dokument**: Mer information finns i [Dela ett dokument](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

* **Dokumentmappar**: Mer information finns i [Dela en dokumentmapp](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

* **Korrektur**: Mer information finns i [Dela ett korrektur i Workfront](/help/quicksilver/review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* **Rapporter, instrumentpaneler och kalendrar**: Mer information finns i [Dela rapporter, instrumentpaneler och kalendrar](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).  Se även följande artiklar:

   * [Dela en rapport i Adobe Workfront](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [Dela en kontrollpanel](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [Dela en kalenderrapport](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* **Filter, vyer och grupperingar**: Mer information finns i [Dela ett filter, en vy eller en gruppering](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

* **Planer**: Mer information finns i [Dela en plan i scenarioplanen](../../scenario-planner/share-a-plan.md).

  Detta kräver ytterligare en licens.

* **Mål**: Mer information finns i [Dela ett mål i Workfront-mål](../../workfront-goals/workfront-goals-settings/share-a-goal.md).

  Detta kräver ytterligare en licens.

## Att tänka på när du delar objekt

* Du kan bara dela samma nivå eller en lägre behörighetsnivå som du har på objektet.

  Om du till exempel har Contribute-behörighet för objektet kan du inte ge en annan användare behörigheten Hantera för det objektet.

* Du kan inte dela ett objekt med en behörighetsnivå som är högre än en användares åtkomstnivå.

  Om en användare till exempel har behörigheten Visa för projekt på åtkomstnivån kan du inte ge dem behörigheten Hantera för ett projekt.
* En användare med behörighet att åtminstone visa ett objekt kan dela objektet med någon annan.
* Du kan dela objekt med aktiva användare, jobbroller, team, grupper eller företag.

  >[!NOTE]
  >
  >Du kan bara dela en plan eller ett mål med andra aktiva användare. Detta kräver ytterligare licenser.
  >
  >
  >Mer information finns i:
  >
  >* [Dela en plan i scenarioplanen](../../scenario-planner/share-a-plan.md)
  >* [Dela ett mål i Workfront-mål](../../workfront-goals/workfront-goals-settings/share-a-goal.md)

* Workfront skickar meddelanden till användare när du delar ett objekt med dem. Meddelanden skickas när båda dessa inställningar är aktiverade:

   * E-postmeddelandena **Objektresurs för användare** och **Objektresurs för team** aktiveras i inställningsområdet av en system- eller gruppadministratör. Mer information finns i [Konfigurera händelsemeddelanden för alla i systemet](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
   * **Någon delar ett objekt med mig** och **Någon delar ett objekt med mitt team**-meddelanden aktiveras på användarens profilsida. Mer information finns i [Ändra dina egna e-postmeddelanden](/help/quicksilver/workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  Inställningarna på system- eller gruppnivå måste aktiveras först innan du kan aktivera meddelandeinställningarna för användaren.

## Delningsbegränsningar

* Du kan dela ett objekt med upp till 100 enheter (användare, team, grupper, jobbroller, företag). Vi rekommenderar att du delar objekt med grupper, team eller företag i stället för med enskilda användare för att undvika den här begränsningen.
* En användare vars åtkomstnivå inte tillåter åtkomst till ekonomiska data kan inte ge åtkomst som skulle göra det möjligt för andra att visa ekonomiska data. Detta innefattar att ge åtkomst till projekt som skulle visa ekonomiska data, eller ändra en åtkomstnivå för att tillåta visning av ekonomiska data.


## Dela behörigheter för objekt

Följande tabell visar behörighetsnivån som du kan välja när du delar ett objekt. Alla objekt har inte alla dessa inställningar tillgängliga. Du kan ge en annan entitet behörighet att visa eller hantera ett objekt. Om du delar ett projekt, en uppgift eller ett problem kan du även ge Contribute behörighet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Visa</strong></td> 
   <td> <p>Du kan utföra följande åtgärder på objektet:</p> 
    <ul> 
     <li><p>Visa objektet</p></li> 
     <li><p>Lägga till dokument i objektet</p></li> 
     <li><p>Lägg till problem i objektet (om det är en uppgift eller ett projekt)</p></li> 
     <li><p>Visa ekonomisk information om objektet</p></li> 
     <li> <p>Dela objektet<br></p> <p>När du delar objektet kan du ge andra användare samma behörighetsnivå som du bara har på objektet, inte en högre nivå.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Contribute</strong></td> 
   <td> <p>Du kan utföra följande åtgärder på objektet:</p> 
    <ul> 
     <li>Alla åtgärder som ingår i behörigheten Visa.</li> 
     <li>Lägg till utgifter i den</li> 
     <li>Lägg till uppgifter i den (om det är ett projekt)</li> 
     <li>Redigera anpassad Forms</li> 
     <li>Loggtimmar för objektet</li> 
     <li>Gör tilldelningar i den</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Hantera</strong></td> 
   <td> <p>Du kan utföra följande åtgärder på objektet:</p> 
    <ul> 
     <li>Alla åtgärder som ingår i behörigheterna Visa och Contribute</li> 
     <li>Ta bort den</li> 
     <li>Hantera finansiell information i den</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Gör detta offentligt för externa användare</strong></td> 
   <td> <p>Alla som saknar ett Workfront-konto kan visa objektet genom att klicka på en länk till det. Detta är inte tillgängligt för alla objekt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Gör detta synligt för hela systemet</strong></td> 
   <td> <p>Objektet kan hittas i sökningar och visas av användare med ett Workfront-konto.</p><p><b>Obs!</b>: Användare med Contributor- eller Requestor-licenser kan inte se projekt, även om den här inställningen är aktiverad. </td> 
  </tr> 
 </tbody> 
</table>

## Förstå ärvda behörigheter och objekthierarkin

### Behörigheter som ärvts från överordnade objekt {#permissions-inherited-from-parent-objects}

Behörigheter i Workfront ärvs hierarkiskt. Det innebär att om du tilldelar behörigheter till en användare för ett överordnat objekt får de samma behörigheter för de underordnade objekten som är kopplade till det som standard.

Om du till exempel ger en användare Contribute-behörighet till ett projekt, har användaren Contribute-behörighet för alla åtgärder och ärenden (underordnade objekt) som är kopplade till det projektet.

Om du fortsätter med exemplet ovan kan du inte begränsa behörigheter till underordnade objekt. Om du inte vill att användaren ska ha Contribute-behörigheter för underordnade objekt som är kopplade till projektet, måste du ta bort ärvda behörigheter från objekten manuellt och sedan justera behörigheterna för den enskilda användaren, inklusive eventuella avancerade inställningar.

Mer information om objekts hierarki och inbördes beroende i Workfront finns i avsnittet [Objektens inbördes beroende och hierarki](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#interdependency-and-hierarchy-of-objects) i artikeln [Översikt över Adobe Workfront-objekt](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>Din Workfront-administratör kan inaktivera ärvda behörigheter för dokument på din åtkomstnivå.  Mer information om hur du inaktiverar ärvda behörigheter för dokument på åtkomstnivå finns i [Skapa eller ändra anpassade åtkomstnivåer](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

### Tillstånd som förvärvats via organisationsmedlemskap   {#permissions-acquired-through-organizational-memberships}

Om du ger en grupp med användare behörigheten Hantera för ett objekt, och du ger en enskild användare i gruppen behörigheten Visa för samma objekt, har användaren den högsta behörighetsnivån (Hantera) som ges via gruppmedlemskapet för objektet.

Om du vill ge lägre behörigheter till en användare som redan är en del av en organisationsenhet (Grupp, Team, Jobbroll eller Företag) med en högre behörighetsnivå, måste du ta bort behörigheterna från organisationsenheten och lägga till användare individuellt med en lägre behörighetsnivå.


<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Remove permissions from objects</h2>
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">AL: draft/ hide this div when Becky makes Remove permissions from objects live and replace with the drafted content with the link at the top of this section</p>
<p>You can remove permissions from objects you have access to Share. Removing permissions from objects is identical for all objects that can be shared.  </p> <note type="note">
  You cannot remove permissions when you share items in bulk. You can remove permissions only when selecting individual items.  
</note>
<p>To remove permissions from objects consider the following:  </p>
<ul>
<li><a href="#remove-entities-from-the-sharing-list-of-an-object" class="MCXref xref">Remove entities from the sharing list of an object</a> </li>
<li><a href="#remove-inherited-permissions" class="MCXref xref">Remove inherited permissions</a> </li>
<li><a href="#make-an-object-private" class="MCXref xref">Make an object private</a> </li>
</ul>
<p><strong>Remove entities from the sharing list of an object</strong></p>
<p>You can remove entities from the sharing list of an object to remove their permissions from the object.</p>
<p>To remove permissions from objects:  </p>
<ol>
<li value="1">Navigate to an object on which you want to modify the permissions.</li>
<li value="2">Click the <strong>Actions</strong> menu, then click <strong>Sharing</strong>.<br>For example, on a project, click <strong>Project Actions</strong>, then <strong>Sharing</strong>.  </li>
<li value="3">Click the <strong>x</strong> next to the name of a user, team, group, company, job role to remove them.<br></li>
<li value="4">In the <strong><User Name>'s Workfront access will be removed from this</strong> drop-down menu, select whether you want their access to be removed just from the object you have selected, or from all children objects associated with it.<br>The following scenarios exist:
<ul>
<li>If you remove the entity only from the object, that entity loses their permissions on the object, and their inherited permissions to the children objects. If they are granted permissions to the children items individually, they retain the same permissions on all children objects associated with it when you select this option.  </li>
<li>If you remove the entity from the object and all the children objects, that entity loses their permissions to the object as well as all children objects, even when they have been given individual permission on each child object.  </li>
</ul></li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
<p> <p><strong>Remove inherited permissions</strong></p> </p>
<p>Inherited permissions can be removed from objects allowing for owners to specifically  identify who will get access to children objects regardless of the access of a user to a parent object. Only users with Manage permission are able to remove inherited permissions.</p>
<p>To remove inherited permissions:</p>
<ol>
<li value="1">Navigate to an object to which you have Manage permissions. <br>For example, navigate to a task.</li>
<li value="2">Go to the sharing list as described in the <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> section in this article. </li>
<li value="3">Select the <strong>X</strong>  mark next to <strong>Inherited Permission</strong>  on the sharing box to remove  anyone listed there.<br><br>This ensures that no one who is granted permissions to the parent object (for example, the project) has permissions to this task by default. You must list   individual entities in the sharing list of the task to grant permissions on the task.<br><note type="note">
You cannot remove individual entities from the Inherited Permissions list. You can only disable the Inherited Permissions for all entities listed.
</note></li>
<li value="4">Click <strong>Save</strong>.  </li>
</ol>
<p><strong>Make an object private</strong></p>
<p>If you have shared an object system-wide, or you have shared it with external uses by making it public, you can make it private again by removing the system-wide or public permissions.  </p>
<p>For more information about making an object available system-wide, or publicly, see the section <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> in this article.</p>
<p>To make an object private:</p>
<ol>
<li value="1">Go to the object you want to make private.<br>For example, navigate to a report.</li>
<li value="2">Click <strong>Report Actions</strong>, then <strong>Sharing</strong>.<br><br></li>
<li value="3">Click <strong>Remove public access</strong> to remove the access of external users to viewing the report.</li>
<li value="4">Click <strong>Remove system-wide access</strong> to stop sharing it with all Workfront users.  </li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Dela ett objekt

Mer information om hur du delar objekt finns i [Dela ett objekt](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

## Ta bort behörigheter från objekt

Mer information om hur du tar bort behörigheter från objekt finns i [Ta bort behörigheter från objekt](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Begär behörigheter för objekt

När någon skickar en länk till ett objekt som du inte har behörighet att visa, eller när du har lägre behörighet för ett objekt och vill begära en högre behörighetsnivå, kan du begära behörigheter för objektet.

Du kan begära åtkomst till ett objekt från alla som har delningsbehörighet till objektet.

Mer information om hur du begär behörigheter till objekt finns i [Begär åtkomst till objekt](../../workfront-basics/grant-and-request-access-to-objects/request-access.md).

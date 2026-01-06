---
title: Dela ett projekt
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Din Adobe Workfront-administratör kan ge dig åtkomst till att visa eller redigera projekt när du tilldelar din åtkomstnivå. Mer information finns i Bevilja åtkomst till projekt.
author: Courtney
feature: Get Started with Workfront
exl-id: eaeedff8-9114-40d9-8cd4-56996edc7dad
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1574'
ht-degree: 0%

---

# Dela ett projekt

<!-- Audited: 1/2024 -->

Din Adobe Workfront-administratör kan ge dig åtkomst till att visa eller redigera projekt när du tilldelar din åtkomstnivå. Mer information finns i [Bevilja åtkomst till projekt](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Förutom den åtkomstnivå som användarna har beviljats kan du även ge dem behörighet att visa, Contribute eller hantera specifika projekt som du har tillgång till för delning.

Behörigheterna är specifika för ett objekt i Workfront och definierar vilka åtgärder man kan vidta för det objektet.


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
   <p>Arbeta eller högre</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa åtkomst eller senare till de objekt som du vill dela</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter eller högre för de objekt som du vill dela</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på när du delar projekt

Förutom övervägandena nedan, se även [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* Som standard har den som skapat ett projekt behörighet att hantera projektet och anges även som projektägare. Om projektet har tilldelats en annan ägare har den användaren även behörighet att hantera projektet. När den som skapat projektet (eller ägaren) delar projektet med andra användare, ger de användarna vissa behörigheter för att styra vad de kan göra när de arbetar med projektet.

  Om en projektägare inte har någon plan- eller standardlicens har de dock inte fullständig åtkomst för att hantera projektet. Endast en användare med en plan- eller standardlicens kan ha behörighet att hantera ett projekt. Mer information finns i [Hur åtkomstnivåer och behörigheter fungerar tillsammans](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

* Du kan dela projekt individuellt eller dela flera i taget. Delningsprojekt är identiska med att dela andra objekt. Mer information om objektdelning i Workfront finns i [Dela ett objekt](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Du kan ge följande behörigheter till ett projekt:

   * Visa
   * Hantera
   * Contribute

* När du delar ett projekt ärver alla uppgifter, utgåvor och dokument samma behörigheter, om inget annat anges.

  Information om hur du hanterar åtkomst till aktiviteter och problem i projektet baserat på en användares behörigheter till projektet finns i avsnittet [](../../manage-work/projects/manage-projects/edit-projects.md#access) i artikeln [Redigera projekt](../../manage-work/projects/manage-projects/edit-projects.md).

  Workfront-administratören kan ange om dokument ska ärva behörigheter från högre objekt på användarens åtkomstnivå. Mer information om att begränsa ärvda behörigheter i dokument finns i [Skapa eller ändra anpassade åtkomstnivåer](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Du kan ta bort ärvda behörigheter från ett projekt så att de underordnade objekten inte ärver dem. Mer information om hur du tar bort ärvda behörigheter från objekt finns i [Ta bort behörigheter från objekt](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Begränsningar för olika licenstyper

* Användare med en Worker-licens har inte behörighet att hantera projekt. För arbetare är den högsta delningsbehörigheten Contribute.
* Användare med en Request-licens kan visa projektinformation, men har begränsad projektåtkomst.
* Ett undantag till att ändra status för ett projekt inträffar när en användare med behörigheterna Visa eller Contribute också inkluderas i en godkännandeprocess. De kan godkänna projektet, vilket ändrar projektets status, men statusen är fördefinierad för godkännande eller för avvisning.
* För att kunna kopiera ett projekt måste användaren också ha tillgång till dem för att kunna skapa projekt på åtkomstnivå.

## Olika sätt att dela ett projekt {#ways-to-share-a-project}

Du kan dela ett projekt på följande sätt:

* Manuellt genom att göra något av följande:

   * Lägga till användare i projektteamet. När du lägger till användare i projektteamet får de automatiskt behörigheten Visa i projektet.\
     Mer information om hur du lägger till användare i ett projektteam finns i avsnittet Lägga till användare i ett projektteam i [Översikt över projektteamet](../../manage-work/projects/planning-a-project/project-team-overview.md).
   * Dela projekten enskilt eller gruppvis när du använder alternativet **Delning**.

* Automatiskt genom att göra något av följande:

   * Placera ett projekt i ett **Portfolio** eller **Program** som redan delas med andra. Användarna får samma behörigheter till projektet som de har för portföljen eller programmet.\
     Mer information om hur du lägger till ett projekt i en **Portfolio** finns i [Lägga till projekt i en portfölj](../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md).\
     Mer information om hur du lägger till ett projekt i ett **program** finns i [Lägga till ett projekt i ett program](../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md).
Mer information om hur du visar ärvda behörigheter för ett objekt finns i [Visa ärvda behörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

   * Lägg till entiteter i projektdelning på en mall som används för att skapa projektet. Mer information om att dela projekt från mallar finns i [Dela en mall](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).
   * Definiera projektåtkomstmallen.

     >[!TIP]
     >
     >När du bifogar eller sparar en mall kan du rensa reglerna för Projektdelning av mallar.

   * Redigera ett projekt och definiera inställningen **När någon får åtkomst till det här projektet**.  Mer information finns i [Redigera projekt](../../manage-work/projects/manage-projects/edit-projects.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because I created new article and linked it above) </p>
<p>To view what users have inherited the access on the project from a portfolio or a program, do the following:</p>
<ol style="list-style-type: lower-alpha;">
<li value="1">Go to a project whose sharing permissions you want to view. </li>
<li value="2"> Click the <strong>More</strong> menu <img src="assets/more-icon.png">, then click <strong>Sharing</strong>. </li>
<li value="3"> <p>Expand the <strong>Inherited Permissions</strong> list. </p> <p>This list displays the names of users that have access to either the portfolio or the program that the project belongs to and also have permissions to the project. </p>  </li>
</ol>
</div>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a project whose sharing permissions you want for all projects you create from scratch. (NOTE: drafted because linked above)  </li>
<li value="2"> Click the More menu, then click <strong>Sharing</strong>. </li>
<li value="3"> <p>In the Project Access box that displays, near the upper-right corner, click the gear icon <img src="assets/gear-icon-settings.png">, then click <strong>Set as my project access template</strong>.</p> <p>The entities that are granted permissions on the selected project have the same permissions for all the projects you create from scratch in the future.</p> <p> The project access template overrides the sharing defaults granted to you by the Workfront administrator in your Access Level.<br>For more information about specifying sharing defaults for projects in the Access Level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>.</p> </li>
<li value="4">Click <strong>Save</strong>.</li>
</ol>
-->

## Dela ett projekt

{{step1-to-projects}}

1. På sidan **Projekt** väljer du det projekt du vill dela i listan. Projektsidan öppnas.

1. Klicka på **Dela** till höger om projektnamnet. Dialogrutan **Dela [Projektnamn]** öppnas.

   ![Knappen Dela projekt](assets/share-project.png)

1. I fältet **Bevilja projektåtkomst till** börjar du skriva namnet på den användare, det team, den roll, den grupp eller det företag som du vill dela projektet med och klickar sedan på namnet i listrutan.

   >[!TIP]
   >
   >Du kan bara dela ett projekt med aktiva användare, team, roller eller företag.


1. (Valfritt) Välj listrutan **Vem har åtkomst** och välj projektets åtkomstnivå:

   * **Endast inbjudna personer har åtkomst:** Endast användare som är inbjudna till projektet har åtkomst till det (Standard).
   * **Alla i systemet kan visa**: Alla användare i systemet kan visa projektet utan en inbjudan.

1. (Valfritt) Om du automatiskt vill använda de inställningar för projektåtkomst som du har valt för alla nya projekt klickar du på ikonen **Kugga** ![Markera kugghjulsikonen](assets/gear-icon.png) och markerar kryssrutan i linje med **Ange som mall för projektåtkomst**.

   >[!NOTE]
   >
   >Projektets åtkomstmall åsidosätter delningsstandardinställningarna som du har fått av Workfront-administratören på din åtkomstnivå.\
   >Mer information om hur du anger delningsstandardvärden för projekt på åtkomstnivå finns i [Bevilja åtkomst till projekt](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)

   <!--
   >this note also appears in Understanding Project Permissions-->


1. Klicka på listrutan till höger om användarens namn och välj behörighetsnivå för det här projektet:


   * **Visa**: Användaren kan granska och dela projektet.
   * **Contribute**: Användaren kan göra uppdateringar, logga information, göra mindre ändringar och dela projektet (inkluderar även alla visningsbehörigheter).
   * **Hantera**: Användaren har fullständig åtkomst till projektet utan administratörsbehörighet, som ges på åtkomstnivån (inkluderar även behörigheterna Visa och Contribute).

1. (Valfritt) Klicka på ikonen för avancerade alternativ bredvid behörighetsnivån som du har tilldelat för att konfigurera specifika behörigheter i projektet.

   ![Konfigurerade avancerade behörighetsalternativ](assets/advanced-permission-options.png)

1. (Valfritt) Om du snabbt vill dela projektet med hjälp av en länk klickar du på **Kopiera länk** och vidarebefordrar den till mottagaren.

1. Klicka på **Spara**.

## Dela projekt i grupp

{{step1-to-projects}}

1. På sidan **Projekt** markerar du rutan till vänster om varje projekt som du vill dela och klickar sedan på ikonen **Dela** ![Dela](assets/share-icon.png) längst upp på sidan. Delningen modal öppnas.

   ![Dela projekt gruppvis](assets/bulk-share-icon.png)

1. I fältet **Bevilja projektåtkomst till** börjar du skriva namnet på den användare, det team, den roll, den grupp eller det företag som du vill dela projekten med och klickar sedan på namnet när det visas i listrutan.

   >[!TIP]
   >
   >Du kan bara dela projekt med aktiva användare, team, roller eller företag.


1. (Valfritt) Välj listrutan **Vem har åtkomst** och välj åtkomstnivå för projekten:

   * **Endast inbjudna personer har åtkomst:** Endast användare som är inbjudna till projekten har åtkomst till dem (Standard).
   * **Alla i systemet kan visa**: Alla användare i systemet kan visa projekten utan en inbjudan.


1. Klicka på listrutan till höger om användarens namn och välj behörighetsnivå för projekten:

   * **Visa**: Användaren kan granska och dela projekten.
   * **Contribute**: Användaren kan göra uppdateringar, logga information, göra mindre ändringar och dela projekten (inklusive alla visningsbehörigheter).
   * **Hantera**: Användaren har fullständig åtkomst till projekten utan administratörsbehörighet, som ges på åtkomstnivån (inkluderar även behörigheterna Visa och Contribute).

1. (Valfritt) Klicka på ikonen för avancerade alternativ bredvid behörighetsnivån som du har tilldelat för att konfigurera specifika behörigheter för projekten.

   ![Konfigurerade avancerade behörighetsalternativ](assets/advanced-permission-options.png)

1. Klicka på **Spara**.


<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Configure default permissions for a project</h2>
<p>(NOTE: drafted because I added one more way to automatically share the project above in the bullet list and linked it to Edit Projects) </p>
<p>As a project owner, you can configure the default permissions for View, Manage, and Contribute access that are used when sharing  the project with others. When users share a project, the default permissions are used. Users can then adjust the default permissions when sharing the project, as described in <a title="Project Permissions" href="#ways-to-share-a-project" class="MCXref xref">Ways to share a project</a>. </p>
<p>To configure the default permissions that are included with each access level:</p>
<ol>
<li value="1">Go to the project where you want to set the default permissions.</li>
<li value="2"> <p>Click the More menu <img src="assets/more-icon.png">, then click <strong>Edit</strong>. <img src="assets/edit-icon.png"></p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">Click <strong>Access</strong> in the list on the left.</li>
<li value="4"> <p>In the <strong>When someone is given access to this PROJECT</strong> section, select permissions that you want to be available when users are given access to the project via sharing.</p> <p>Ensure that any permissions that you want to include in the selected access level are selected and deselect any permissions that you do not want to include in the selected permissions level.</p> <p>To view which permissions are available for each level, see  <a title="Project Permissions" href="#Understanding_Project_Permissions" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <note type="note">
The
<strong>Delete</strong> access in the
<strong>Manage</strong> permission level determines whether users can  delete the project itself. Users with
<strong>Manage</strong> access to the project can delete tasks and issues within the project regardless of whether this option is selected, if they have
<strong>Manage</strong> permissions to the tasks and issues.  
</note> </li>
<li value="5">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

## Behörighetsalternativ för projekt

I följande tabell visas de behörigheter som användare kan ge när de delar ett projekt. Mer information om vilka användare som får åtkomst baserat på deras licens finns i [Bevilja åtkomst till projekt](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Åtgärder</strong> </p> </th> 
   <th> <p><strong>Hantera</strong> </p> </th> 
   <th> <p><strong>Contribute</strong> </p> </th> 
   <th> <p><strong>Visa</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Lägg till anpassat formulär</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Uppdatera anpassade fält</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Lägg till en godkännandeprocess</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Godkänn ett projekt</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Godkänn timmar</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Skapa ett projekt</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Lägg till dokument</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Lägg till problem</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Lägg till uppgift(er)</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Kopiera projekt</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ta bort projekt</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ändra planerade datum</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dela projekt</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dela hela systemet</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Visa projekt</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Uppdateringar/kommentarer</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ändra status</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Loggtimmar</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Redigera uppdrag</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Hantera baslinje</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Hantera risker*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Hantera ekonomi*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Lägg till/redigera utgifter*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Visa ekonomi*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Bifoga mall</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Spara som mall</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Lägg till/redigera affärsärende</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Redigera projektinformation</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Redigera personal</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Exportera till MS-projekt</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Beräkna om ekonomi/tidslinje*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ange köegenskaper</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>    </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Redigera projekt gruppvis i en lista</p> </td> 
   <td> <p>✓</p> </td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;Användare som inte har tillgång till ekonomiska data kan inte hantera risker och ekonomi för projekt, även om de har Redigera-åtkomst till projekt. Mer information om åtkomst till ekonomiska data finns i [Bevilja åtkomst till ekonomiska data](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

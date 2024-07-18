---
title: Dela en mall
product-area: templates
navigation-topic: grant-and-request-access-to-objects
description: Som Adobe Workfront-administratör kan du ge användare åtkomst till att visa eller redigera mallar när du tilldelar deras åtkomstnivå. En användare måste ha en planlicens för att få tillgång till redigeringsmallar.
author: Alina
feature: Get Started with Workfront
exl-id: 19fb0de5-7db5-42a9-9f33-a4570acfeef8
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 0%

---

# Dela en mall

Som Adobe Workfront-administratör kan du ge användare åtkomst till att visa eller redigera mallar när du tilldelar deras åtkomstnivå. En användare måste ha en planlicens för att få tillgång till redigeringsmallar.

Mer information om att bevilja åtkomst till mallar finns i [Bevilja åtkomst till mallar](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

Förutom den åtkomstnivå som du ger kan en användare även få behörighet att visa eller hantera specifika mallar från andra användare som delar dem.

>[!NOTE]
>
>Behörighetsnivåer fungerar inom åtkomstnivåer. En användare kan t.ex. inte få behörighet att hantera en mall om åtkomstnivån endast tillåter dem att visa mallar.

Behörigheterna är specifika för ett objekt i Workfront och definierar vilka åtgärder man kan vidta för det objektet.

## Att tänka på när du delar en mall

* Förutom övervägandena nedan, se även [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).
* Skaparen av en mall, samt mallägaren, har som standard behörigheten Hantera för mallen. Mer information om hur du anger en användare som mallägare finns i [Redigera projektmallar](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* Du kan dela följande när du delar en mall:

   * Mallen

     Mer information om hur du delar en mall finns i [Dela projektmallar](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

     Du kan tilldela följande behörigheter till en mall:

      * Visa

        ![](assets/view-on-template-262x221.png)

      * Hantera

        ![](assets/manage-on-template-225x280.png)

   * Framtida projekt som skapas med mallen. Du kan ge samma behörighetsnivåer för projekt som skapats från en mall som för ett enskilt projekt. 

     Mer information om hur du delar ett projekt från en mall på mallnivå finns i [Dela projektmallar](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

* När du delar en mall eller ett projekt som skapas från mallen ärver användarna som standard samma behörigheter till alla underordnade objekt som är kopplade till mallen eller projektet.

  Mer information om objekthierarkin i Workfront finns i  [Förstå objekt i Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

* När du delar en mall ärver alla malluppgifter och -dokument, liksom problemen med det framtida projekt som skapas från mallen, samma behörigheter, om inget annat anges.

  Information om hur du hanterar åtkomsten till malluppgifter och problem i projektet baserat på en användares behörigheter till projektet finns i avsnittet [Åtkomst](../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) i artikeln [Redigera projektmallar](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* Workfront-administratören kan ange om dokument ska ärva behörigheter från högre objekt på användarens åtkomstnivå. Mer information om att begränsa ärvda behörigheter i dokument finns i [Skapa eller ändra anpassade åtkomstnivåer](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Share a template</h2>
<p>(NOTE: drafted because this is also linked above: Share project templates >> which is an article in the Manage Work section>> Templates)&nbsp;</p>
<ol>
<li value="1"> <p>Go to the template you want to share with other entities, click <strong>Template Actions</strong>, then <strong>Template Sharing</strong>.<br>Or</p> <p>Navigate to a list of templates, and select multiple templates from the list, then click <strong>Share Template</strong>.</p> <note type="note">
If you select multiple templates, you cannot view who already has permissions to the individual templates.
</note> </li>
<li value="2"> <p>Start typing the name of a user, group, team, job role, or company that you want to share the template with in the <strong>Give template access to</strong> or <strong>Edit template access for</strong> fields.</p> <p>Select them when they appear in the list.</p> <note type="tip">
You can share an object only with active users, teams,
<span>roles,</span> or companies.
</note> </li>
<li value="3">From the drop-down menu, select which level of permissions you want to grant:<br>
<ul>
<li><p><strong>View it</strong>: Users with these permissions are able to view the template and create a project using it, or attach it to an existing project.</p><p><img src="assets/template-permissions-350x197.png" alt="template_permissions.png" style="width: 350;height: 197;"></p></li>
<li><strong>Manage it</strong>: Users with these permissions are able to edit or delete the template.</li>
</ul></li>
<li value="4">(Optional) Click <strong>Advanced Settings</strong> to fine-tune your settings for each level of permissions.</li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
<h2>Share a project at the template level</h2>
<p>You can share the future projects that are created using a template with users at the template level.</p>
<ol>
<li value="1"> <p>Go to the template whose future projects you want to share with other entities, click <strong>Template Actions</strong>, then <strong>Project Sharing</strong>.</p> <p>Or</p> <p>Navigate to a list of templates, and select multiple templates from the list, then click <strong>Share Project</strong>.</p> <note type="note">
If you select multiple templates, you cannot view who already has project permissions to the individual templates.
</note> </li>
<li value="2"> <p>Start typing and then select the name of a user, group, team, job role, or company with whom you want to share future projects created from the template in the <strong>Give project access to</strong> or <strong>Edit template access for</strong> fields.</p> <note type="tip">
You can share an object only with active users, teams,
<span>roles,</span> or companies.
</note> </li>
<li value="3">From the drop-down menu, select which level of permissions you want to grant.<br>Select from the following:<br>
<ul>
<li><strong>No access</strong>: You can specify which users will not have any access to the template.<br>This option is available only when bulk sharing projects from templates.&nbsp;</li>
<li><strong>View</strong>: Users with these permissions can view projects created from the template.</li>
<li><strong>Contribute</strong>: Users with these permissions can contribute to projects created from the template&nbsp;</li>
<li><strong>Manage</strong>: Users with these permissions can manage or delete projects created from this template.<br><img src="assets/share-project-from-template-350x268.png" alt="share_project_from_template.png" style="width: 350;height: 268;"></li>
</ul></li>
<li value="4">(Optional) Click <strong>Advanced Settings</strong> to fine-tune your settings for each level of permissions. </li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Avancerade inställningar för malldelning

Tabellen nedan visar vilka behörigheter du kan ge användarna när de får visa eller hantera en mall. Instruktioner om hur du delar en mall finns i avsnittet [Dela en mall](../../manage-work/projects/create-and-manage-templates/share-project-template.md#share) i artikeln [Dela projektmallar](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Åtgärder</th> 
   <th>Hantera</th> 
   <th>Visa</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Kopiera</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ta bort</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Redigera mallinformation</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visa mall</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Dela</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Dela hela systemet</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Lägg till dokument</p> <p>Tips! Ibland lägger man till dokument i en projektmall som tror att de läggs till i ett projekt. Du kan förhindra detta för mottagarna genom att inaktivera den här inställningen.</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

Mer information om vilka behörigheter du ger användare till projekt som har skapats från en mall finns i [Dela ett projekt i Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

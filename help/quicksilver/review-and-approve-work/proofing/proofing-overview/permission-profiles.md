---
content-type: overview
product-area: documents
keywords: bevis,behörighet
navigation-topic: proofing-overview
title: Översikt över behörighetsprofiler för korrektur
description: Behörighetsprofiler för korrektur avgör vilka övergripande behörigheter användare har för alla korrektur i ditt konto. Behörighetsprofiler för korrektur tilldelas användare i deras användarprofil. Behörighetsprofiler för korrektur skiljer sig från korrekturroller. Mer information om korrekturroller finns i Översikt över korrekturroller.
author: Courtney
feature: Digital Content and Documents
exl-id: fb6faa48-d97b-4b7b-83ae-fe39d40b3963
source-git-commit: 9b60133c4cc20deb410f507854597f44d0607228
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 0%

---

# Översikt över behörighetsprofiler för korrektur

Behörighetsprofiler för korrektur avgör vilka övergripande behörigheter användare har för alla korrektur i ditt konto. Behörighetsprofiler för korrektur tilldelas användare i deras användarprofil. Behörighetsprofiler för korrektur skiljer sig från korrekturroller. Mer information om korrekturroller finns i [Översikt över profilroller](../../../review-and-approve-work/proofing/proofing-overview/proof-roles.md).

>[!NOTE]
>
>Om du är administratör kan du skapa anpassade profiler för användare i din organisation. Mer information finns i [Konfigurera anpassade profiler i Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Consider the following about roles and permissions:</p>
-->

<!--
<ul data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li> <p>Assigned profile permissions relate only to the users and items in your own account. The exception is in the case of Satellite accounts, where the Administrator and Billing Administrator for the main (hub) accounts can access and manage the&nbsp;account settings&nbsp;and billing of those accounts from the hub account level.</p> </li>
<li> <p>Billing Administrators and Administrators can delete users. This can only be done in&nbsp;Account settings.</p> </li>
<li>When Billing Administrators and Administrators view proofs that are owned by other users in their account, they view them with the role of a Reviewer.</li>
<li>Using the Read Only role, Billing Administrators and Administrators can access proofs in folders shared with them or in folders created by them.&nbsp;</li>
</ul>
-->

## Behörighetsprofiler

I följande tabell visas de behörigheter som är tillgängliga för respektive behörighetsprofil.

<table>
  <tr>
   <td colspan="5" ><strong>Egna objekt</strong>
   </td>
   <td colspan="3" ><strong>Andra användares objekt</strong>
   </td>
   <td><strong>Administratör</strong>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td><strong>Lägg till</strong>
   </td>
   <td><strong>Visa</strong>
   </td>
   <td><strong>Redigera</strong>
   </td>
   <td><strong>Ta bort</strong>
   </td>
   <td><strong>Visa</strong>
   </td>
   <td><strong>Redigera</strong>
   </td>
   <td><strong>Ta bort</strong>
   </td>
   <td><strong>Redigera och ta bort</strong>
   </td>
  </tr>
  <tr>
   <td>Administratör
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
  </tr>
  <tr>
   <td>Supervisor
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Manager
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Observer
   </td>
   <td>
   </td>
   <td>x
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
</table>

### Administratör

Administratörer har åtkomst till [Kontoinställningar](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings) och har följande behörigheter:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Administratörer kan:</td> 
   <td>Administratörer kan inte:</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Skapa korrektur, ladda upp filer och skapa mappar</p> </li> 
     <li> <p>Visa, redigera och ta bort korrektur och filer som de skapat</p> </li> 
     <li> <p>Visa, redigera och ta bort korrektur och filer som skapats av alla användare i organisationen</p> </li> 
     <li> <p>Ta bort de gemensamma mapparna för andra användare</p> </li> 
     <li> <p>Redigera alla korrektur som skapats i kontot</p> </li> 
     <li> <p>Ange som Dropzone-ägare*</p> </li> 
     <li> <p>Gå till sidan Kontoinställningar och redigera kontoinformationen</p> </li> 
     <li> <p>Töm papperskorgen</p> </li> 
     <li> <p>Lägga till, redigera och ta bort användare</p> </li> 
     <li> <p>Skapa grupper och lägg till nya kontakter</p> </li> 
     <li> <p>Ta bort kontakter</p> </li> 
     <li> <p>Redigera korrektur om det inte finns några svar på dem</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Redigera korrektursvar.</p> </li> 
     <li> <p>Ta bort andra användares privata mappar</p> </li> 
     <li> <p>Gå till faktureringssidan eller redigera faktureringsinformationen</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Finns endast i den fristående Workfront Proof-produkten.

### Supervisor

Tillsynsmannen har följande behörigheter:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Tillsynsmannen kan:</td> 
   <td>Supervisors kan inte:</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Skapa korrektur, ladda upp filer och skapa mappar</p> </li> 
     <li> <p>Visa, redigera och ta bort korrektur och filer som de skapat</p> </li> 
     <li> <p>Visa, redigera och ta bort korrektur och filer som skapats av alla användare i organisationen</p> </li> 
     <li> <p>Ta bort de gemensamma mapparna för andra användare</p> </li> 
     <li> <p>Redigera alla korrektur som skapats i kontot</p> </li> 
     <li> <p>Skapa grupper och lägg till nya kontakter</p> </li> 
     <li> <p>Ta bort kontakter</p> </li> 
     <li> <p>Redigera korrektur om det inte finns några svar på dem</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Redigera korrektursvar.</p> </li> 
     <li> <p>Ta bort andra användares privata mappar</p> </li> 
     <li> <p>Gå till faktureringssidan eller redigera faktureringsinformationen</p> </li> 
     <li> <p>Lägga till, redigera eller ta bort användare</p> </li> 
     <li> <p>Töm papperskorgen</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Manager

Chefer har följande behörigheter:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Chefer kan:</td> 
   <td>Chefer kan inte:</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Skapa korrektur, ladda upp filer och skapa mappar</p> </li> 
     <li> <p>Visa, redigera och ta bort korrektur och filer som de skapat</p> </li> 
     <li> <p>Se, granska och godkänn korrektur av andra användare som uttryckligen delas med dem (skrivskyddad behörighet till allt i en delad mapp)</p> </li> 
     <li> <p>Redigera alla korrektur som skapats i kontot</p> </li> 
     <li> <p>Skapa grupper och lägg till nya kontakter</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Visa, redigera eller ta bort korrektur och filer som skapats av andra användare i organisationen. </p> <p>Redigera korrektursvar.</p> </li> 
     <li> <p>Ta bort privata eller offentliga mappar för andra användare</p> </li> 
     <li> <p>Gå till faktureringssidan eller redigera faktureringsinformationen</p> </li> 
     <li> <p>Lägga till, redigera eller ta bort användare</p> </li> 
     <li> <p> Ta bort kontakter</p> </li> 
     <li> <p>Töm papperskorgen</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Observer</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers have the following permissions:</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can see, review, and approve proofs of other users that are explicitly shared with them (Read-only&nbsp;rights to everything in a shared folder). For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view files that are explicitly shared with them.&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot&nbsp;create proofs, upload files, and create folders. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md" class="MCXref xref">Upload Files and Web Content to Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot view, edit, or delete proofs and files created by other users in the organization.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot edit proofs&nbsp;or replies.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot delete any items created in the organization.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot access&nbsp;the Billing page or Account settings. For more information, see <a href="../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md" class="MCXref xref">The Workfront Proof Billing Page</a>&nbsp;and&nbsp;<a href="../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md" class="MCXref xref">Account settings in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot be set as the Dropzone owner. For more information, see <a href="../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md" class="MCXref xref">Configure the dropzone in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot empty the&nbsp;trash. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md" class="MCXref xref">Restore and Empty the Trash in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot add, edit, or delete users.&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot create groups or add new contacts.&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot delete contacts.&nbsp;</p>
-->


><!--
><p data-mc-conditions="QuicksilverOrClassic.Draft mode">Menus and functions available to Observers are limited.&nbsp;</p>>
>-->
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers do not see the Header menu or the green New menu in their Dashboard</li>>
>  -->
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers do not see the following links in their Settings:&nbsp;Account settings,&nbsp;Billing </li>>
>  -->


<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Guest</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Guest profile is used to give access to proofs for reviewers who do not have their own Workfront Proof account. Guests can access proofs shared with them directly via their personal email notifications.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view, review, and approve proofs that are explicitly shared with them.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view files that are explicitly shared with them.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot access the Dashboard.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot have folders shared with them. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md" class="MCXref xref">Manage Folders in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot be added as Authors or Moderators to the proofs. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p>
-->

<!--
<note type="note">
&nbsp;Guests are not Workfront Proof users, so they cannot see all the proofs shared with them in their own Dashboard.
</note>
-->

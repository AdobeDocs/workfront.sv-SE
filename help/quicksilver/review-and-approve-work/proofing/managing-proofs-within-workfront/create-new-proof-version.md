---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Skapa en ny version av ett korrektur
description: Det kan vara en stor utmaning att hantera feedback i flera versioner eller revisioner av ett verk. Workfront förenklar den här processen genom att du kan skapa och jämföra flera versioner av ett korrektur.
author: Courtney
feature: Digital Content and Documents
exl-id: ee0c859e-349b-4e7a-ac80-164740b950f0
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '1737'
ht-degree: 0%

---

# Skapa en ny version av ett korrektur

Det kan vara en stor utmaning att hantera feedback i flera versioner eller revisioner av ett verk. Workfront förenklar den här processen genom att du kan skapa och jämföra flera versioner av ett korrektur.

Tänk på följande när du skapar en ny version av ett korrektur:

* Du kan ge en användare behörighet att se en version men inte en annan. Om du däremot delar en senare version med en användare kan användaren inte se tidigare versioner om du inte går tillbaka och uttryckligen ger användaren åtkomst till de tidigare versionerna.
* Om du vill skapa en ny version av ett korrektur måste du ha redigeringsbehörighet för korrekturet.

  Mer information om vem som har redigeringsbehörighet för ett korrektur finns i [Hantera korrekturroller i Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) och [Behörighetsprofiler för korrektur i Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

  Mer information om att dela korrekturversioner finns i  [Dela ett bevis i Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

>[!IMPORTANT]
>
>Om ett korrektur skapas i Adobe Workfront måste alla nya versioner som skapas för det korrekturet också skapas i Workfront. Du kan inte skapa en ny version av ett korrektur i Workfront Proof om det beviset har skapats i Workfront.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Aktuell plan: Pro eller högre</p> <p>eller</p> <p>Äldre plan: Välj eller Premium</p> <p>Mer information om korrekturåtkomst för olika planer finns i <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Åtkomst till korrekturfunktioner i Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Aktuell plan: Arbete eller plan</p> <p>Äldre plan: Alla (du måste ha språkkontroll aktiverat för användaren)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Behörighetsprofil för bevis </td> 
   <td>Chef eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront- eller Workfront Proof-administratören om du vill ta reda på vilken plan, roll eller behörighetsprofil du har.

+++

## Skapa en ny version av ett korrektur i Workfront

Det finns flera sätt att överföra en ny korrekturversion i Workfront. Standardinställningarna för korrektur kan eventuellt överföras från den tidigare versionen beroende på vilken metod du väljer:

* **Generera korrektur automatiskt när dokument överförs**: Standardkorrekturinställningar överförs inte. Om den här inställningen är aktiverad i din användarprofil överförs inte standardkorrekturinställningarna när du drar och släpper en ny version.
* **Skapa korrektur > Enkel**: Standardkorrekturinställningar överförs inte. Om du väljer Enkel när du skapar en ny korrekturversion överförs inte standardinställningarna för korrektur från den tidigare versionen.
* **Lägg till ny > Version > Korrektur**: Standardkorrekturinställningar överförs från den tidigare versionen.
* **Skapa korrektur > Avancerat**: Standardkorrekturinställningar överförs från den tidigare versionen.

  <table>
  <tbody>
  <tr>
  <td>Generera korrektur automatiskt när dokument överförs</td>
  <td>Standardkorrekturinställningar överförs inte. Om den här inställningen är aktiverad i din användarprofil överförs inte standardkorrekturinställningarna när du drar och släpper en ny version.</td>
  </tr>
  <tr>
  <td>Skapa korrektur &gt; Enkelt</td>
  <td>Standardkorrekturinställningar överförs inte. Om du väljer Enkel när du skapar en ny korrekturversion överförs inte standardinställningarna för korrektur från den tidigare versionen.</td>
  </tr>
  <tr>
  <td>Lägg till nytt &gt; Version &gt; Korrektur</td>
  <td>Standardkorrekturinställningar överförs från den tidigare versionen.</td>
  </tr>
  <tr>
  <td>Skapa korrektur &gt; Avancerat</td>
  <td>Standardkorrekturinställningar överförs från den tidigare versionen.</td>
  </tr>
  </tbody>
  </table>




Så här skapar du en ny version av ett korrektur:

1. Öppna dokumentlistan som innehåller korrekturet.
1. Dra och släpp en ny fil från datorns filsystem över korrekturet.

   eller

   Markera den rad där korrekturet visas, klicka på **Lägg till ny** > **Version** och klicka sedan på det alternativ du vill använda för att lägga till den nya versionen av korrekturet.

   ![Lägg till ny version](assets/add-new-version-350x185.png)

## Skapa en ny version av ett korrektur från korrekturläsaren (endast Workfront Proof)

Om du använder den fristående Workfront Proof-versionen kan du skapa en ny version av ett korrektur som innehåller en enda fil eller webbfångst. 

>[!NOTE]
>
>Om ditt konto finns i en Enterprise-plan och du överför flera filer eller webbklipp kommer de automatiskt att kombineras till en enda ny version. Mer information finns i [Skapa ett flersidigt korrektur](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

Så här skapar du en ny version av ett korrektur i Workfront Proof:

1. Öppna beviset.
1. Klicka på listrutan **Version** i det övre vänstra hörnet och klicka sedan på **+ Ny version** i rutan som visas.

   På sidan **Ny korrekturversion av** som visas kan du se alla granskare från den tidigare versionen, inklusive deras roller och e-postmeddelandeinställningar. Du kan enkelt redigera roller och meddelanden för befintliga granskare eller ta bort befintliga granskare från den nya versionen på den här sidan.

1. Under **Lägg till filer** överför du en fil som en ny version av korrekturet genom att dra och släppa från datorn eller genom att klicka på **bläddra** och välja önskad fil. Du kan skriva ett **korrekturnamn** för versionen eller lämna rutan tom om du vill använda samma filnamn med ett versionsnummer som läggs till i slutet.

   eller

   Spara en webbsida som en ny version av korrekturet genom att skriva en URL.

   >[!NOTE]
   >
   >Dra och släpp är bara tillgängligt i webbläsare som har fullt stöd för HTML5. Detta utesluter Internet Explorer 7 till 9 och Safari.

1. Under **Arbetsflöde** gör du någon av följande ändringar för att ange granskarna för den här versionen av korrekturet.

   Granskare från den tidigare versionen ersätts av de granskare du lägger till.

   * Ändra **ägaren** för versionen till en annan användare i ditt konto.\
     Mer information om ägarbehörigheter finns i [Korrekturbehörighetsprofiler i Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * Använd **Skriv kontaktnamnet eller e-postadressen för att lägga till en mottagarruta** och lägg till granskare i versionen. Du kan ange en **korrekturroll** och en **e-postaviseringstyp** för varje mottagare.

     Mer information om hur du lägger till grupper i korrekturet finns i  [Lägg till grupper i ett korrektur](../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md). Mer information om roller finns i [Hantera korrekturroller i Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

     >[!NOTE]
     >
     >Om den som skapat eller äger  korrekturet har [e-postmeddelandet ](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) inaktiverat som standard (i sina personliga inställningar). De får inga e-postmeddelanden om korrektur eller nytt korrektur även om rutan Meddela personer via e-post är markerad på sidan Nytt korrektur. Mer information om e-postmeddelanden finns i [Konfigurera inställningar för e-postmeddelanden i Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md). Se även [Korrekturutskick via e-post](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) och [Nytt korrekturmeddelande](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

   * Ange en korrekturdeadline för versionen.
   * Håll muspekaren över en granskares namn för att se alla beslut han eller hon har fattat om en tidigare version.

1. Gör något av följande under **E-postmeddelande**:

   * Ange om du vill meddela granskarna om den nya versionen.\
     Ditt val loggas i aktivitetsavsnittet på sidan Korrekturinformation. Mer information finns i [Hantera korrekturinformation i Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

   * Lägg till ett eget ämne och meddelande.

1. Gör något av följande i avsnittet **Organisation**: 

   * Använd en eller flera taggar på korrekturet. Mer information finns i [Skapa och hantera taggar i Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-and-manage-tags.md).\
     Observera att taggar också ärvs från den tidigare versionen av korrekturet. Om du lägger till en ny tagg i den nya versionen taggas även tidigare versioner.

   * Lägg till versionen i en mapp. Mer information finns i [Hantera mappar i Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md). Mappen kopieras från den tidigare versionen av korrekturet. Om du väljer en annan mapp flyttas hela korrekturet (alla versioner).

   * Faktureringsadministratörer och administratörer kan göra mappfältet obligatoriskt för hela kontot på fliken Inställningar. Mer information finns i.

1. Gör någon av ändringarna nedan under Korrekturinställningar:

   * Kräv inloggning på korrekturet
   * Kräv elektroniska signaturer på beviset (endast Enterprise-planen)
   * Lås beviset när alla beslut fattas
   * Tillåt eller blockera hämtning av originalfil
   * Offentlig delning av beviset, inklusive inställningar för offentlig delning
   * Prenumeration på beviset\
     De val som görs i det här avsnittet visas på sidan Korrekturinformation (där vissa fält kan redigeras). Mer information finns i [Hantera korrekturinformation i Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Create a new version of a proof from the proofing viewer</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To create a new version from the proofing viewer</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Open the proof.</li>
<li value="2"> <p>Click the <strong>Version</strong> drop-down menu in the upper-left corner, then click <strong>+ New version</strong> in the box that appears.</p> <p>On the <strong>New proof version of</strong> page that appears, you can see all the reviewers from the previous version, including their roles and email notification settings. You can easily edit the roles and notifications of existing reviewers or remove existing reviewers from the new version on this page.</p> </li>
<li value="3"> <p>Under <strong>Add files</strong>, upload a file as a new version of the proof by dragging and dropping from your computer or by clicking <strong>browse</strong> and selecting the file you want. You can type a&nbsp;<strong>Proof name</strong>&nbsp;for the version or leave this box blank to&nbsp;use the same filename with a version number added on the end.</p> <p>Or<br></p> <p>Capture a web page as a new version of the proof by typing a URL</p> <note type="note">
Drag and drop is available only with browsers that fully support HTML5. This excludes Internet Explorer 7 through 9 and Safari.
<br>
</note> </li>
<li value="4"> <p>Under <strong>Workflow</strong>, make any of the following changes to specify the reviewers for this version of the proof.</p> <p>Reviewers from the previous version are replaced by the reviewers you add.</p>
<ul>
<li>Change the <strong>Owner</strong> of the version to another user in your account.<br>For information about owner permissions, see <a href="../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md" class="MCXref xref">Proof Permissions Profiles in Workfront Proof</a>.</li>
<li> <p>Using the <strong>Type contact name or email address to add a recipient box</strong>, add reviewers to the version. You can specify a <strong>Proof role</strong> and an <strong>Email alerts</strong> type for each recipient.</p> <p>For information about adding groups to the proof, see&nbsp;<a href="../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md" class="MCXref xref">Add Groups to a Proof</a>.&nbsp;For information about roles, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p> <note type="note">
If the creator or owner of&nbsp;&nbsp;the proof has
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a> disabled by default (in their personal settings), they won't receive any Proof made or New proof emails even if the Notify people by email box is checked on the New proof page. For information about email notifications, see
<a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Configure email notification settings in Workfront Proof</a>.&nbsp;See also
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a> and
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">New proof email</a>.
<br>
</note> </li>
<li>Set a proof deadline for the version.</li>
<li>Hover over a reviewer's name to see any decisions he or she made on a previous version.</li>
</ul> </li>
<li value="5">Under <strong>Email notification</strong>, do any of the following:
<ul>
<li>Specify whether you want to notify the reviewers of the new version.<br>Your selection will be logged in the Proof activity section on the Proof details page.</li>
<li>Add a custom subject and message.</li>
</ul></li>
<li value="6">Under Proof settings, make any of the changes below:
<ul>
<li>Require login on the proof</li>
<li>Require electronic signatures on the proof (Enterprise plan only)</li>
<li>Lock the proof when all decisions are made</li>
<li>Allow or block download of original file</li>
<li>Public sharing of the proof,&nbsp;including public sharing settings</li>
<li>Subscription to the proof<br>The selections made in this section will be shown in the Proof details page.</li>
</ul></li>
</ol>
-->

## Om meddelandet Ny version

Om det fanns ett eget ämne/meddelande i den tidigare versionen av korrekturet visas det som standard på sidan Ny version. Du kan:

* Redigera ämnet och meddelandet.
* Avmarkera rutan Meddela personer via e-post, vilket innebär att inga e-postmeddelanden skickas till granskarna för att meddela dem att de har en ny version att granska.

  >[!NOTE]
  >
  >Detta påverkas inte av något anpassat standardämne/standardmeddelande som sparats i dina personliga inställningar.

Om du har ett standardämne och ett standardmeddelande sparat i dina personliga inställningar påverkar detta vilket meddelande som visas som standard på sidan Ny version:

* Om du väljer att meddela granskarna via e-post om den tidigare versionen av korrekturet med hjälp av standardmeddelandet (t.ex. inget anpassat ämne/meddelande), visas ditt standardämne/standardmeddelande (dina personliga inställningar) på sidan Ny version. Du kan sedan redigera det anpassade ämnet och meddelandet eller avmarkera rutan Meddela personer via e-post (vilket innebär att inget e-postmeddelande skickas till granskarna för att meddela dem att de har en ny version att granska).
* Om du väljer att inte meddela granskarna via e-post om den tidigare versionen av korrekturet (t.ex. ingen standard eller anpassad e-postadress) kommer sidan Ny version inte att innehålla något meddelande som standard. Om du vill meddela granskarna om den nya versionen klickar du på länken Skicka ett meddelande, som visar ditt standardämne/standardmeddelande (enligt dina personliga inställningar). Du kan sedan redigera det anpassade ämnet och meddelandet om det behövs.

Om du inte har något standardämne och ett standardmeddelande sparat i dina personliga inställningar visas följande på sidan Ny version:

* Om du väljer att meddela granskarna via e-post om den tidigare versionen av korrekturet med hjälp av standardmeddelandet (t.ex. inget anpassat ämne/meddelande), väljs alternativet Meddela personer via e-post som standard på sidan Ny version. Klicka på länken om du vill lägga till ett anpassat meddelande.
* Om du väljer att inte meddela granskarna via e-post om den tidigare versionen av korrekturet (t.ex. ingen standard eller anpassad e-postadress) kommer sidan Ny version inte att innehålla något meddelande som standard. Om du vill meddela granskarna om den nya versionen klickar du på länken Skicka ett meddelande. Du kan sedan lägga till ett eget ämne och meddelande genom att klicka på länken Lägg till anpassat meddelande.

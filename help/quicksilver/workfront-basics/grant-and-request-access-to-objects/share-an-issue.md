---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Dela ett ärende
description: Din Adobe Workfront-administratör ger användarna åtkomst att visa eller redigera problem när de tilldelar åtkomstnivåer. Mer information om hur du beviljar åtkomst till problem finns i Bevilja åtkomst till problem.
author: Courtney
feature: Get Started with Workfront
exl-id: 91ee72e0-20a9-4b06-9f80-a343dd4fbe06
source-git-commit: fcf6165c9c641316c701d92af2e39294a9fe0123
workflow-type: tm+mt
source-wordcount: '1242'
ht-degree: 0%

---

# Dela ett ärende

Din Adobe Workfront-administratör ger användarna åtkomst att visa eller redigera problem när de tilldelar åtkomstnivåer. Mer information om att bevilja åtkomst till problem finns i [Bevilja åtkomst till problem](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md).

Förutom den åtkomstnivå som användarna har beviljats kan du även ge dem behörighet att visa, Contribute eller hantera specifika problem som du har åtkomst till att dela. Mer information om åtkomstnivåer och behörigheter finns i [Hur åtkomstnivåer och behörigheter fungerar tillsammans](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Behörigheterna är specifika för ett objekt i Workfront och definierar vilka åtgärder man kan vidta för det objektet.


## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande för att kunna dela objekt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Nytt: Standard</p> 
   eller
   <p>Aktuell: Arbete eller högre</p>
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

Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på när det gäller att dela problem

Förutom övervägandena nedan, se även [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>En Workfront-administratör kan lägga till eller ta bort behörigheter för alla objekt i systemet, för alla användare, utan att vara ägare av dessa objekt.

* Den som skapade ett problem har som standard behörigheten Hantera.
* Du kan dela problem individuellt eller dela flera i taget. Delningsproblem är identiska med att dela andra objekt i Workfront. Mer information om objektdelning i Workfront finns i [Dela ett objekt](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Du kan ge följande behörigheter till en utgåva: 

   * Visa
   * Contribute
   * Hantera

* När du delar ett problem ärver alla dokument som är bifogade problemet samma behörigheter.

  Workfront-administratören kan ange om dokument ska ärva behörigheter från högre objekt på användarens åtkomstnivå. Mer information om att begränsa ärvda behörigheter i dokument finns i [Skapa eller ändra anpassade åtkomstnivåer](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Du kan ta bort ärvda behörigheter från ett problem. Mer information finns i [Ta bort behörigheter från objekt](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Olika sätt att dela ett problem

* Manuellt, vilket liknar delning av andra objekt i Workfront.
* Gör något av följande automatiskt:

   * Ange behörigheter för något av de överordnade objekten i utgåvan: projekt, program eller portfölj. Problem ärver behörigheterna från sina överordnade objekt. Mer information om hur du visar ärvda behörigheter för objekt finns i [Visa ärvda behörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).
   * Lägg till entiteter i projektdelning på en mall som används för att skapa det projekt som utgåvan gäller. Mer information om att dela projekt från mallar finns i [Dela en mall](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * Ange behörigheter för alla problem i ett projekt när du redigerar projektet. Information om hur du hanterar åtkomst till problem eller begäranden i projektet baserat på en användares behörigheter till projektet finns i avsnittet [](../../manage-work/projects/manage-projects/edit-projects.md#access) i artikeln [Redigera projekt](../../manage-work/projects/manage-projects/edit-projects.md).

     >[!TIP]
     >
     >Om du inte anger vilka behörigheter du vill att användarna ska ha när de tilldelas till problemen i projektet får de som standard samma behörigheter som de har i projektet.

   * Ange de behörigheter som användare får för problem som de skickar i en begärandekö när de skapar en begärandekö. Mer information finns i [Skapa en frågekö](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

     >[!IMPORTANT]
     >
     >Behörigheter ges olika beroende på om projektet publiceras som en begärandekö eller inte:
     >
     >   
     >   
     >   * När en användare skickar en begäran till ett projekt som publicerats som en begärandekö, får den primära kontakten och användaren anger den angivna behörigheten.
     >   * När en användare skickar en begäran till ett projekt som inte har publicerats som en begärandekö, beviljas den primära kontakten (om annan än Anges av användaren) den angivna behörigheten och användaren Anges behörigheten Hantera för problemet.
     >   
     >

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Automatically share an issue at the project level</h2>
<p>(NOTE: this info duplicates in Edit projects - linked there instead (above).)&nbsp;</p>
<p>As the Project Owner, you can grant permissions automatically to users as the issues are added to a project.</p>
<ol>
<li value="1">Go to the project whose issues you want to share automatically.</li>
<li value="2"> Click the More menu <img src="assets/more-icon.png">, then click <strong>Edit</strong>. </li>
<li value="3">In the <strong>Edit Project</strong> box that displays, click <strong>Access</strong>.</li>
<li value="4">In the <strong>When someone is assigned to an ISSUE</strong> field, select from the following permissions levels:
<ul>
<li><strong>View</strong></li>
<li><strong>Contribute</strong></li>
<li><strong>Manage</strong><br>Now, when someone is assigned to an issue on the selected project, they are granted the specified permissions to the issue.&nbsp;</li>
</ul></li>
<li value="5">(Optional) Select the <strong>Also grant ... access to the project</strong> field to also grant View, Contribute, or Manage permissions to the projects to the user assigned to the issue</li>
<li value="6">In the <strong>When someone submits a REQUEST ...</strong> field, select from the following permissions levels:
<ul>
<li><strong>View</strong></li>
<li><strong>Contribute</strong></li>
<li><p><strong>Manage</strong></p><note type="important">
<p>Permissions are granted differently depending on whether or not the project is published as a request queue:</p>
<ul>
<li>When a user submits a request to a project published as a request queue, the Primary Contact and Entered By users are granted the permission specified.</li>
<li>When a user submits a request to a project not published as a request queue, the Primary Contact (if different from Entered By user) is granted the permission specified, and the Entered By user is granted Manage permissions to the issue.</li>
</ul>
</note></li>
</ul></li>
<li value="7"> <p>(Optional) Select the <strong>People from the same company will inherit the same permissions for all requests</strong> field.</p> <p>People from the same company as the user submitting the request are granted the same permissions on the requests as the user.&nbsp;</p> </li>
<li value="8">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Automatically share an issue in request queues</h2>
<p>(NOTE: drafted because it's duplicated from Create a Request Queue which is linked above)&nbsp;</p>
<p>As the Project Owner, you can grant permissions automatically to users as the issues are submitted to a request queue.</p>
<ol>
<li value="1">Go to the project whose issues you want to share automatically.</li>
<li value="2">Click <strong>Edit Project</strong>.</li>
<li value="3">Click <strong>More</strong> then click <strong>Queue Setup</strong>. </li>
<li value="4"> <p>On the <strong>Queue Details</strong> sub-tab, in the drop-down menu under <strong>When someone makes a request, automatically grant</strong>, select from the following permissions levels:</p>
<ul>
<li><strong>View Access</strong> </li>
<li><strong>Contribute Access</strong> </li>
<li> <p><strong>Manage Access</strong> </p> </li>
</ul> <p>Now, when someone submits a request to the selected project, they are granted the specified permissions to the request.</p> </li>
<li value="5"> <p>(Optional) Select the <strong>People from the same company will inherit the same permissions for all requests</strong>.</p> <p>People from the same company as the user submitting the request are granted the same permissions on the requests as the user.&nbsp;</p> </li>
<li value="6">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Dela ett ärende

1. Navigera till den utgåva som du vill dela.

1. Klicka på **Dela** till höger om problemnamnet. Dialogrutan **Dela [Ärendenamn]** öppnas.

   ![Knappen Dela problem](assets/share-issue-button.png)

1. I fältet **Bevilja utfärdandeåtkomst till** börjar du skriva namnet på den användare, det team, den roll, grupp eller det företag som du vill dela problemet med och klickar sedan på namnet i listrutan.

   >[!TIP]
   >
   >Du kan bara dela ett problem med aktiva användare, team, roller eller företag.


1. (Valfritt) Välj listrutan **Vem har åtkomst** och välj åtkomstnivå för problemet:

   * **Endast inbjudna personer har åtkomst:** Endast användare som är inbjudna till problemet har åtkomst till det (Standard).
   * **Alla i systemet kan visa**: Alla användare i systemet kan visa problemet utan en inbjudan.

1. Klicka på listrutan till höger om användarens namn och välj behörighetsnivå för det här problemet:

   * **Visa**: Användaren kan granska och dela problemet.
   * **Contribute**: Användaren kan göra uppdateringar, logga information, göra mindre ändringar och dela problemet (inklusive alla visningsbehörigheter).
   * **Hantera**: Användaren har fullständig åtkomst till problemet utan administratörsbehörighet, som ges på åtkomstnivån (inkluderar även behörigheterna Visa och Contribute).

1. (Valfritt) Klicka på ikonen för avancerade alternativ bredvid behörighetsnivån som du har tilldelat för att konfigurera specifika behörigheter för problemet.

   ![Konfigurerade avancerade behörighetsalternativ](assets/advanced-permission-options.png)

1. (Valfritt) Om du snabbt vill dela problemet med hjälp av en länk klickar du på **Kopiera länk** och vidarebefordrar den till mottagaren.

1. Klicka på **Spara**.

## Dela problem i grupp

1. Navigera till det projekt som innehåller de problem du vill dela.

1. På fliken **Problem** på projektsidan markerar du rutan till vänster om varje problem som du vill dela och klickar sedan på ikonen **Dela** ![Dela](assets/share-icon.png) högst upp på sidan. Delningen modal öppnas.

   ![Problem med massdelning](assets/bulk-share-issues.png)

1. I fältet **Bevilja utfärdandeåtkomst till** börjar du skriva namnet på den användare, det team, den roll, den grupp eller det företag som du vill dela problemen med och klickar sedan på namnet i listrutan.

   >[!TIP]
   >
   >Du kan bara dela problem med aktiva användare, team, roller eller företag.


1. (Valfritt) Välj listrutan **Vem har åtkomst** och välj åtkomstnivå för problemen:

   * **Endast inbjudna personer har åtkomst:** Endast användare som är inbjudna till problemen har åtkomst till dem (Standard).
   * **Alla i systemet kan visa**: Alla användare i systemet kan visa utgåvorna utan en inbjudan.


1. Klicka på listrutan till höger om användarens namn och välj behörighetsnivå för problemen:

   * **Visa**: Användaren kan granska och dela problemen.
   * **Contribute**: Användaren kan göra uppdateringar, logga information, göra mindre ändringar och dela problemen (inklusive alla visningsbehörigheter).
   * **Hantera**: Användaren har fullständig åtkomst till problemen utan administratörsbehörighet, som ges på åtkomstnivån (inkluderar även behörigheterna Visa och Contribute).

1. (Valfritt) Klicka på ikonen för avancerade alternativ bredvid behörighetsnivån som du har tilldelat för att konfigurera specifika behörigheter för problemen.

   ![Konfigurerade avancerade behörighetsalternativ](assets/advanced-permission-options.png)

1. Klicka på **Spara**.

## Utfärda behörigheter

Följande tabell visar vilka behörigheter du kan ge användare när de tillåts att visa, Contribute eller hantera ett problem:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Åtgärder</strong> </td> 
   <td><strong>Hantera</strong> </td> 
   <td><strong>Contribute</strong> </td> 
   <td><strong>Visa</strong> </td> 
  </tr> 
  <tr> 
   <td> <p>Lägg till problem</p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ta bort </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Bifoga eget formulär</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Redigera anpassade fält</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Godkänn problem</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Lägg till en godkännandeprocess</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Lägg till dokument</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Copy Issue*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Flytta problem</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Loggtimmar</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Konvertera till projekt*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Acceptera tilldelning</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Uppdateringar/kommentarer</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Ändra planerade datum</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Skapa uppdrag</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Dela</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Dela hela systemet</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontrolleras av åtkomstnivåerna och behörigheterna för projektet.

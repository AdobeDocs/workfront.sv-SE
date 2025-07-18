---
title: Dela arbetsytor
description: Du kan dela en arbetsyta med andra för att säkerställa samarbete när du arbetar i Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 58d2bf9f14b9a3adf4bacfad58f1b9862aeaf247
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# Dela arbetsytor

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Du kan dela en arbetsyta med andra för att säkerställa samarbete när du arbetar i Adobe Workfront Planning.

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

>[!NOTE]
>
>Om du ger behörighet till en arbetsyta ger det inte andra användare behörighet till vyerna på posttypssidorna. Du måste tilldela behörigheter till enskilda vyer på en posttypsida för att kunna dela dem med andra användare. Mer information finns i [Dela en vy](/help/quicksilver/planning/access/share-views.md).


## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produkter</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-plan*</p></td> 
   <td> 
<p>Något av följande Workfront-planer:</p> 
<ul><li>Välj</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning är inte tillgängligt för tidigare Workfront-planer</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning-paket*</p></td> 
   <td> 
<p>Alla </p> 
<p>Kontakta din kontoansvarige på Workfront om du vill ha mer information om vad som ingår i respektive Workfront Planning-plan. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront</p></td> 
   <td> 
<p>Din organisations instans av Workfront måste vara registrerad på Adobe Unified Experience för att få tillgång till Workfront Planning.</p>
<p>Din organisation måste vara registrerad på Adobe Unified Experience för att användare ska kunna begära och bevilja behörigheter till en arbetsyta från en behörighetsbegäran. </p> 
<p>Användare måste läggas till i Adobe Admin Console för att få behörighet till Workfront Planning Workspaces.</p>
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning är inte tillgängligt för tidigare Workfront-licenser</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>  <p>Hantera behörigheter till en arbetsyta</p>  </td> 
  </tr>

</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på när du delar arbetsytor

* Allmän information om delning av objekt i Workfront Planning finns även i [Översikt över delningsbehörigheter i Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
* Du kan dela arbetsytor med användare, team, roller, grupper eller företag i din organisation.
* Förutom team, grupper, företag och jobbroller kan du bara dela med användare som har lagts till i Adobe Admin Console.
* Du kan inte dela arbetsytor med användare utanför organisationen.
* När du delar en arbetsyta delas även alla posttyper, poster och fält som är kopplade till arbetsytorna.
* När du delar en arbetsyta delas inte vyerna. Du måste dela vyer separat.
* Workspace-behörigheter visas som ärvda behörigheter för posttyper.

## Dela behörigheter till en arbetsyta

Följande användare kan dela en arbetsyta med andra användare:

* Systemadministratörer kan dela alla arbetsytor, inklusive de som de inte skapade.
* Alla andra användare kan bara dela arbetsytor som de har behörighet att hantera.

Så här delar du en arbetsyta med andra:

{{step1-to-planning}}

1. Öppna arbetsytan som du vill dela och klicka sedan på **Dela** i skärmens övre högra hörn.

   ![Knappen Dela på arbetsytan längst upp till höger](assets/share-button-on-workspace-top-right.png)

1. I fältet **Bevilja åtkomst till den här arbetsytan** börjar du skriva namnet på en användare, grupp, team, företag eller jobbroll och klickar sedan på den när den visas i listan.

   ![Dela användargränssnitt med grupper](assets/sharing-ui-with-groups.png)

   >[!NOTE]
   >
   >   Förutom team, grupper, företag och jobbroller kan du bara dela med användare som har lagts till i Adobe Admin Console. Du kan inte lägga till användare med endast Workfront. Mer information finns i [Hantera användare i Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).


1. Välj någon av följande behörighetsnivåer i listrutan:
   * Visa
   * Contribute
   * Hantera

     Mer information om behörighetsnivåer och vilka åtgärder användare kan utföra för varje nivå finns i [Översikt över delningsbehörigheter i Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
1. Klicka på **Kopiera länk** om du vill kopiera en länk till arbetsytan till Urklipp.
1. Dela den kopierade länken med andra. Användare som tar emot länken måste vara aktiva användare och logga in på Workfront för att kunna komma åt arbetsytan.
1. Klicka på **Spara**.

   De användare som du delade arbetsytan med får både ett meddelande i programmet och ett e-postmeddelande om att de har behörighet till den.

## Bevilja behörigheter till en arbetsyta från en behörighetsbegäran

Användare som har åtkomst till en länk till en arbetsyta som de inte har behörighet till kan begära behörigheter till arbetsytan. Alla användare med behörigheten Hantera på arbetsytan får behörigheten och kan bevilja eller neka behörigheter.

1. (Villkorligt) Om du är chef för en arbetsyta kan du få en begäran från en annan användare om att få åtkomst till vyn i följande områden:

   * Ett meddelande i appen

     ![Meddelande i programmet om åtkomstbegäran](assets/in-app-notification-for-access-request.png)
   * Ett e-postmeddelande

     ![E-postmeddelande om åtkomstbegäran](assets/email-notification-for-access-request.png)
1. (Villkorligt) Klicka på meddelandet i appen i meddelandefältet i Workfront
eller
Klicka på **Visa alla meddelanden** i e-postmeddelandet och klicka sedan på meddelandet i listan.

   Rutan **Väntande åtkomstbegäranden** visas.

   ![Godkännanderuta för meddelandelista](assets/notifications-list-approval-box.png)

1. (Valfritt) För den användare vars behörigheter du vill godkänna väljer du något av följande alternativ på den nedrullningsbara menyn till höger om användarens namn:
   * **Visa**
   * **Contribute**
   * **Hantera**
1. Markera den användare som du vill godkänna eller neka behörighet för och klicka sedan på **Godkänn alla** eller **Neka alla**.
1. Klicka på vänsterpilen till vänster om **Väntande åtkomstbegäranden** och klicka sedan på **Spara**.

   Om du godkände begäran läggs användarna till i delningsrutan på arbetsytan. Användaren som begär behörighet får en e-postbekräftelse på att deras begäran har godkänts. <!--will they also get an in-app notification??-->


## Ta bort behörigheter till en arbetsyta


{{step1-to-planning}}

1. Öppna arbetsytan som du vill ta bort behörigheter till och klicka sedan på **Dela** i skärmens övre högra hörn.
1. Klicka på listrutan till höger om namnet på en enhet som du delar arbetsytan med och klicka sedan på **Ta bort**.
1. Klicka på **Spara**.

   De borttagna användarna har inte längre åtkomst till arbetsytan eller dess objekt.

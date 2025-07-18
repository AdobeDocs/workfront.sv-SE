---
title: Hantera e-postmeddelanden om planering av Adobe Workfront
description: När någon taggar dig eller dina team i en postkommentar i Adobe Workfront Planning får du ett e-postmeddelande om den taggen.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 3c505b3a-cda7-4e7b-b497-28b820e9bb8f
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---


# Hantera e-postmeddelanden om Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Du kan få e-postmeddelanden från Workfront Planning när följande scenarier finns:

* Någon taggar dig eller dina team i en postkommentar

  Mer information om hur du taggar andra i en postkommentar finns i [Hantera postkommentarer](/help/quicksilver/planning/records/manage-record-comments.md).
* Någon ber om din tillåtelse att komma åt en vy eller en arbetsyta
* Någon bekräftar att din åtkomst har beviljats för en vy eller en arbetsyta <!--Isk confirmed that there is nno email for denying access but did not test-->
* Du skickar en Workfront Planning-begäran. Mer information finns [i Skapa och hantera ett förfrågningsformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
* Någon godkänner eller avvisar en Workfront Planning-begäran som du har skickat. Mer information finns [i Godkänna en begäran i Adobe Workfront Planning](/help/quicksilver/planning/requests/approve-request.md)
* Statusen ändras till en Workfront Planning-begäran som du har skickat.

## Krav för åtkomst

+++ Expandera för att visa åtkomstkrav.

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
   <li><p> Planering av Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-plan*</p></td> 
   <td> 
<p>Någon av följande Workfront-planer:</p> 
<ul><li>Utvald</li> 
<li>Primtal</li> 
<li>Sist</li></ul> 
<p>Workfront Planning är inte tillgängligt för äldre Workfront-planer</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planeringspaket*</p></td> 
   <td> 
<p>Någon </p> 
<p>Om du vill ha mer information om vad som ingår i varje Workfront Planning-plan kontaktar du din Workfront-kontoansvarige. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-plattform</p></td> 
   <td> 
<p>Din organisations instans av Workfront måste registreras i Adobe Unified Experience.</p> 
<p>Användarna i din organisation får bara meddelanden från Workfront Planning när din organisation är registrerad i Adobe Unified Experience. </p>
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience för Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licens för Adobe Workfront*</p></td> 
   <td><p> Standard, Light eller Contributor</p>
   <p>Workfront Planning är inte tillgängligt för äldre Workfront-licenser</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration av åtkomstnivå</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Behörigheter för objekt</p></td> 
   <td>   <p>Visa eller högre behörigheter till en arbetsyta</a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, även de som de inte har skapat</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Mall för layout</p></td>
   <td> Användare med en Light- eller Contributor-licens måste tilldelas en layoutmall som innehåller Planering.
   <p>Standardanvändare och systemadministratörer har planeringsområdena aktiverade som standard.</p></div></li></ul>

</td>
  </tr>

</tbody> 
</table>

*Mer information om åtkomstkrav för Workfront finns [i Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>In order to receive notifications from Workfront Planning and manage notification preferences, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls in Workfront Planning. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>
-->


## Hantera e-postaviseringar när någon taggar dig i en kommentar

1. (Villkorligt och valfritt) När någon taggar dig eller ditt team i en kommentar i en post går du till e-postmeddelandet som informerar dig om taggen och kommentaren. Avsändaren av e-postmeddelandet är Adobe Experience Cloud.

   ![Exempel på e-postmeddelanden](assets/email-notification-example.png)

1. (Valfritt) Klicka på meddelandet i **rutan Workfront** i e-postmeddelandet.

   Sidan med postinformation öppnas i Workfront. Du kan göra uppdateringar i posten eller svara på kommentaren.

1. (Villkorligt) Om det är tillgängligt klickar du på **Visa alla aviseringar**. <!--check with Lilit - do non-IMS users have this button??-->Sidan **Meddelanden** öppnas i Adobe Experience Cloud. Alla meddelanden från alla Adobe Experience Cloud-program visas.

## Hantera e-postaviseringar när du begär och beviljar behörigheter

1. (Villkorligt och valfritt) När någon begär eller ger dig behörighet att komma åt en vy eller en arbetsyta går du till e-postmeddelandet som informerar dig om behörighetsbegäran. Avsändaren av e-postmeddelandet är Adobe Experience Cloud.

1. (Valfritt) Klicka på meddelandet i **rutan Workfront** i e-postmeddelandet.

   Sidan med postinformation öppnas i Workfront. Du kan göra uppdateringar i posten eller svara på kommentaren.

1. (Villkorligt) Om det är tillgängligt klickar du på **Visa alla aviseringar**.
Sidan **Meddelanden** öppnas i Adobe Experience Cloud. Alla meddelanden från alla Adobe Experience Cloud-program visas.


Information om hur du begär, beviljar eller nekar behörigheter till en vy eller en arbetsyta finns i [Begära behörigheter till en vy eller en arbetsyta](/help/quicksilver/planning/access/request-permissions.md).

Mer information om hur du hanterar dina Workfront Planning-meddelanden finns i [Hantera Adobe Workfront Planning-meddelandeinställningar](/help/quicksilver/planning/notifications/manage-notification-preferences.md).

## Hantera e-postmeddelanden om att skicka, godkänna eller avvisa Workfront Planning-förfrågningar

1. (Valfritt) Gå till e-postmeddelandet som Workfront skickar till dig
När du har skickat in en begäran, eller efter att en begäran som du har skickat har godkänts eller avvisats. Avsändaren av e-postmeddelandet är Adobe Workfornt.

1. (Valfritt) Klicka på **Öppna begäran**. Då öppnas begäran i Workfront Planning.

1. **Klicka på ikonen Meddelanden**![, ikonen för meddelandeområdet, Unified Shell](assets/notifications-area-icon-unified-shell.png) i det övre högra hörnet av skärmen för att komma åt **sidan Meddelanden**.

   Mer information om hur du hanterar dina Workfront Planning-meddelanden finns i [Hantera Adobe Workfront Planning-meddelandeinställningar](/help/quicksilver/planning/notifications/manage-notification-preferences.md).

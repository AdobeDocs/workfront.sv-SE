---
title: Hantera e-postmeddelanden om Adobe Workfront Planning
description: När någon taggar dig i en postkommentar i Adobe Workfront Planning får du ett e-postmeddelande om taggen.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 3c505b3a-cda7-4e7b-b497-28b820e9bb8f
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 0%

---


# Hantera e-postmeddelanden om Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Du kan få e-postmeddelanden från Workfront Planning när följande scenarier finns:

* Någon taggar dig i en postkommentar

  Mer information om hur du taggar andra i en postkommentar finns i [Hantera postkommentarer](/help/quicksilver/planning/records/manage-record-comments.md).
* Någon ber om din behörighet att komma åt en vy eller arbetsyta
* Någon bekräftar att din åtkomst har beviljats för en vy eller arbetsyta <!--Isk confirmed that there is nno email for denying access but did not test-->
* Du skickar en Workfront Planning-förfrågan. Mer information finns i [Skapa och hantera ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
* Någon godkänner eller avvisar en Workfront Planning-begäran som du har skickat in. Mer information finns i [Godkänn en begäran i Adobe Workfront Planning](/help/quicksilver/planning/requests/approve-request.md)
* Statusen ändras till en Workfront Planning-förfrågan som du har skickat in.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven.

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
<p>Din organisations instans av Workfront måste integreras med Adobe Unified Experience.</p> 
<p>Användarna i din organisation får meddelanden från Workfront Planning endast när din organisation är registrerad på Adobe Unified Experience. </p>
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td> 
   <td><p> Standard, Light eller Contributor</p>
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
   <td>   <p>Visa eller högre behörigheter på en arbetsyta </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutmall</p></td> 
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn. </p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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


## Hantera e-postmeddelanden när någon taggar dig i en kommentar

1. (Villkorligt och valfritt) När någon taggar dig i en kommentar för en post går du till e-postmeddelandet som informerar dig om taggen och kommentaren. E-postmeddelandets avsändare är Adobe Experience Cloud.

   ![Exempel på e-postmeddelanden](assets/email-notification-example.png)

1. (Valfritt) Klicka på meddelandet i rutan **Workfront** i e-postmeddelandet.

   Sidan med postinformation öppnas i Workfront. Du kan uppdatera posten eller svara på kommentaren.

1. (Villkorligt) Om det är tillgängligt klickar du på **Visa alla meddelanden**. <!--check with Lilit - do non-IMS users have this button??-->
Sidan **Meddelanden** öppnas i Adobe Experience Cloud. Alla meddelanden från alla Adobe Experience Cloud-program visas.

## Hantera e-postmeddelanden när du begär och beviljar behörigheter

1. (Villkorligt och valfritt) När någon har begärt eller gett dig behörighet att komma åt en vy eller en arbetsyta går du till det e-postmeddelande som informerar dig om behörighetsbegäran. E-postmeddelandets avsändare är Adobe Experience Cloud.

1. (Valfritt) Klicka på meddelandet i rutan **Workfront** i e-postmeddelandet.

   Sidan med postinformation öppnas i Workfront. Du kan uppdatera posten eller svara på kommentaren.

1. (Villkorligt) Om det är tillgängligt klickar du på **Visa alla meddelanden**.
Sidan **Meddelanden** öppnas i Adobe Experience Cloud. Alla meddelanden från alla Adobe Experience Cloud-program visas.


Mer information om att begära, bevilja eller neka behörigheter för en vy eller arbetsyta finns i [Begär behörigheter för en vy eller en arbetsyta](/help/quicksilver/planning/access/request-permissions.md).

Information om hur du hanterar dina Workfront Planning-meddelanden finns i [Hantera aviseringsinställningar för Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-notification-preferences.md).

## Hantera e-postmeddelanden om att skicka, godkänna eller avslå Workfront Planning-begäranden

1. (Valfritt) Gå till e-postmeddelandet som Workfront skickar till dig
när du har skickat en begäran eller efter att en begäran som du har skickat har godkänts eller avvisats. E-postmeddelandets avsändare är Adobe Workfornt.

1. (Valfritt) Klicka på **Öppna begäran**. Detta öppnar förfrågan i Workfront Planning.

1. Klicka på ikonen **Notifications** ![Notifications Area icon Unified Shell](assets/notifications-area-icon-unified-shell.png) i skärmens övre högra hörn för att komma åt sidan **Notifications** .

   Information om hur du hanterar dina Workfront Planning-meddelanden finns i [Hantera aviseringsinställningar för Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-notification-preferences.md).

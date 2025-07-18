---
title: Hantera Adobe Workfront Planning In-app-meddelanden
description: När någon taggar dig eller dina team i en postkommentar får du ett e-postmeddelande om den taggen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: a6eb8c7c-a34d-4c84-a45c-7e7f050a4302
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---


# Hantera aviseringar i appen för Adobe Workfront Planning

{{planning-important-intro}}

Du kan få meddelanden i appen från Workfront Planning när följande scenarier finns:

* Någon taggar dig eller dina team i en postkommentar

  Mer information om hur du taggar andra i en postkommentar finns i [Hantera postkommentarer](/help/quicksilver/planning/records/manage-record-comments.md).
* Någon ber om din tillåtelse att komma åt en vy eller en arbetsyta
* Någon bekräftar att din åtkomst har beviljats för en vy eller en arbetsyta <!--Isk confirmed there is no notification for denying permissions - did not test-->

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
   <p>Systemadministratörer har behörighet till alla arbetsytor, även de som de inte har skapat</p>  </td> 
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

+++ Expand to view access requirements. 

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
   <p>In order to receive notifications from Workfront Planning, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></td>
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

+++
-->

## Hantera aviseringar i appen när någon taggar dig i en kommentar

1. (Villkorligt) När någon har taggat dig eller dina team i en kommentar på en post går du till ikonen för meddelanden **&#x200B;**&#x200B;i appen ![Experience Cloud notifications](assets/experience-cloud-notifications-icon.png) i Adobe Experience Cloud.

   ![Exempel på aviseringar i appen](assets/in-app-notification-example.png)

1. Klicka på aviseringen.

   Sidan med postinformation öppnas i Workfront Planning. Du kan göra uppdateringar i posten eller svara på kommentaren.

1. (Valfritt) Klicka på **Markera alla som lästa** för att ange att du har läst alla aviseringar.
1. (Valfritt) Klicka på **Visa alla** för att gå till **sidan Meddelanden** i Adobe Experience Cloud.

## Hantera aviseringar i appen när du begär och beviljar behörigheter

Du får meddelanden i appen när någon begär eller ger dig behörighet till en vy eller en arbetsyta.

Information om hur du begär, beviljar eller nekar behörigheter till en vy eller en arbetsyta finns i [Begära behörigheter till en vy eller en arbetsyta](/help/quicksilver/planning/access/request-permissions.md).

Mer information om hur du hanterar dina Workfront Planning-meddelanden finns i [Hantera Adobe Workfront Planning-meddelandeinställningar](/help/quicksilver/planning/notifications/manage-notification-preferences.md).

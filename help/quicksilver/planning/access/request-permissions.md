---
title: Begär behörighet till en vy eller en Workspace
description: När någon delar en länk till en vy eller arbetsyta som du inte har åtkomst till, kan du begära behörighet för att kunna öppna den. I den här artikeln förklaras stegen för att begära åtkomst till en vy eller arbetsyta när du stöter på en delad länk som du inte kan öppna.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 94dfa36a-801a-4eef-bcf5-4a3fecc5a3d0
source-git-commit: c879d06cfe7ba76df3e974c160a7349f1503f17f
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# Begära behörigheter till en vy eller arbetsyta

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

>[!IMPORTANT]
>
>De funktioner som beskrivs i den här artikeln är bara tillgängliga när din organisation har anslutit sig till Adobe Unified Experience.
>
>Mer information finns i [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).


Du kan begära behörigheter för en vy eller arbetsyta när någon delar en länk med dig till vyn eller arbetsytan som du inte har åtkomst till.

Att begära behörigheter till en vy liknar att begära behörigheter till en arbetsyta.

I den här artikeln beskrivs hur du begär åtkomst till en vy eller arbetsyta när någon delar en länk med dig och du inte har åtkomst till den delade sidan.

Mer information om hur du tilldelar behörigheter till vyer och arbetsytor finns i följande artiklar:

* [Visa](/help/quicksilver/planning/access/share-views.md)
* [Dela arbetsytor](/help/quicksilver/planning/access/share-workspaces.md)


## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Alla Workfront- och Planning-paket</p> 
eller
<p>Alla arbetsflödes- och planeringspaket</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p>Alla</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>  <p>När din behörighetsbegäran har beviljats kan du få följande behörigheter:</p>
   <ul><li><p>Visa eller hantera för en vy</p></li>
   <li><p>Visa, Contribute eller Hantera för en arbetsyta</p></li></ul>  
   <p>Endast användare med behörigheten Hantera på en arbetsyta och en vy kan dela en vy offentligt.</p></td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> Användare med en Light- eller Contributor-licens måste tilldelas en layoutmall som innehåller Planning.
   <p>Standardanvändare och systemadministratörer har planeringsområdena aktiverade som standard.</p></div></li></ul>

</td>
  </tr>

</tbody> 
</table>

Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
 
 <table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p><b>IMPORTANT</b></p>
<p>The users in your organization can request permissions for views and workspaces only when your organization is onboarded to the Adobe Unified Experience. </p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard, Light, or Contributor</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  <p>After your request for permission is granted, you could gain the following permissions:</p>
   <ul><li><p>View or Manage for a view</p></li>
   <li><p>View, Contribute, or Manage to a workspace</p></li></ul>  
   <p>Only users with Manage permissions to a workspace and a view can share a view publicly.</p></td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
  
</td>
  </tr>
 
</tbody> 
</table> -->


## Begär behörigheter till en vy eller arbetsyta

Att begära behörigheter till en vy liknar att begära behörighet till en arbetsyta.

När någon delar en länk till en arbetsyta eller en vy där du inte har tillgång till den med dig:

1. Klicka på länken som delas med dig för vyn eller arbetsytan.

   En **Du har inte åtkomst**-sida visas som informerar dig om att du inte har åtkomst till vyn eller arbetsytan.

   ![Begär åtkomst för visning](assets/request-access-to-view.png)

1. (Villkorligt) Om den delade länken är för en vy för en arbetsyta där du har åtkomst klickar du på **Öppna med befintlig vy**. Om du har behörighet att komma åt arbetsytan öppnas posttypssidan i standardvyn.

1. (Valfritt och villkorligt) Om du inte har behörighet att visa arbetsytan lägger du till ett anpassat meddelande i rutan som är tillgänglig och klickar sedan på **Begär åtkomst**.

   Alla användare med behörigheten Hantera för vyn eller arbetsytan får följande meddelanden om åtkomstbegäran:
   * Ett meddelande i appen
     ![Meddelande i programmet om åtkomstbegäran](assets/in-app-notification-for-access-request.png)
   * Ett e-postmeddelande
     ![E-postmeddelande om åtkomstbegäran](assets/email-notification-for-access-request.png)

1. (Villkorligt) När arbetsytehanteraren ger dig behörighet till vyn eller arbetsytan får du ett e-postmeddelande och ett meddelande i appen med en bekräftelse på att behörighet har beviljats. <!--check this - I was not able to test this, but Isk confirmed.-->

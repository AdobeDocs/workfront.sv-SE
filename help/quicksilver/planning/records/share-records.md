---
title: Dela poster
description: Du kan dela poster med andra för att öka samarbetet.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: a3c82d8be6945a91a249d64923c6377a5edfa268
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---


<!--should this move to the Access folder when we have sharing for ALL the objects???-->

# Dela poster

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

<!--take out preview and production references at release-->

{{planning-important-intro}}

Om du vill samarbeta med andra användare kan du dela poster med andra.

Du kan dela en Adobe Workfront Planning-post på följande sätt:

* Kopiera länken till postsidan från webbläsaren när sidan är öppen.

* Kopiera en länk till postens sida när du visar poster i posttypens tabellvy.

* Du kan dela alla poster på en arbetsyta med andra användare genom att dela arbetsytan <!--<span class="preview">and record type</span>-->. Mer information finns i [Dela en arbetsyta](/help/quicksilver/planning/access/share-workspaces.md).

<!-- replace the last sentence above with this: 

For more information see the following articles:

* [Share a workspace](/help/quicksilver/planning/access/share-workspaces.md)


<div class="preview">

* [Share a record type](/help/quicksilver/planning/access/share-record-types.md)

</div>

-->

I den här artikeln beskrivs hur du kan kopiera en länk till en posts sida från en posttyps tabellvy.

## Åtkomstkrav

+++ Expandera för att visa åtkomstkrav..

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
<p>Din organisations instans av Workfront måste integreras med Adobe Unified Experience för att få tillgång till alla funktioner i Workfront Planning.</p> 
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td> 
   <td><p> Medarbetare, ljus eller standard </p>
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
   <td>  <p>Visa eller högre behörigheter på en arbetsyta för att dela <!--<span class="preview">and record type</span>--> en post med hjälp av en länk </p>
   <p>Hantera behörigheter till en arbetsyta <!--<span class="preview">and record type</span>--> för att dela posterna på arbetsytan </p>
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutmall</p></td> 
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn. </p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--OLD:

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
   <p> Adobe Workfront</p> </td>
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
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace to share a record using a link </p>
   <p>Manage permissions to a workspace to share the workspace the record belongs to </p>
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

## Dela postlänkar från posttypstabellvyn

{{step1-to-planning}}

Arbetsytan som du senast öppnade öppnas.
1. Klicka på ett posttypskort.

   Posttypssidan öppnas.
1. (Villkorligt) Välj en tabellvy i listrutan **Visa** i tabellens övre högra hörn. Detta bör vara standardvyn, såvida du inte har visat posttypen i tidslinjevyn när du senast öppnade den.

   Posterna som är associerade med den valda posttypen visas i tabellvyn.
1. Högerklicka på en postrad

   eller

   Håll markören över en posts namn, klicka på menyn **Mer** ![](assets/more-menu.png) och klicka sedan på **Kopiera länk**.

   ![](assets/contextual-menu-for-record-row.png)

   Länken kopieras till Urklipp.

1. Klistra in länken i ett e-postmeddelande eller i ett chattfönster om du vill dela den med andra användare. När användarna får länken öppnas postsidan.

   >[!TIP]
   >
   >Fälten på postsidan är samma fält som är tillgängliga i postens tabellvy.


   <!--add there when it will be available: if they have access to this record-->

## Dela alla poster på en arbetsyta genom att dela arbetsytan

Du kan dela alla poster på en arbetsyta när du delar arbetsytan med andra.

Endast användare med behörigheten Hantera för en arbetsyta kan dela den med andra.

Mer information finns i [Dela en arbetsyta](/help/quicksilver/planning/access/share-workspaces.md).


<!--
<div class="preview">

## Share all records in a record type by sharing the record type

In the Production environment, records inherit permissions from the workspace. 

In the Preview environment, records inherit permissions from the record type. 

By default, record types inherit permissions from the workspace. 

However, you can do any of the following:

* Turn off inherited permissions from the workspace on a record type. This removes permissions from the records. 
* Manually grant permissions to users to a record type, even when they have no permissions to the workspace. This automatically gives them View permissions to the workspace. This grants permissions to users to the records. 

Only users with Manage permissions to a workspace can share its record types and records with others. 

For more information, see [Share record types](/help/quicksilver/planning/access/share-record-types.md). 

</div>

-->
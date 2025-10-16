---
title: Dela poster
description: Du kan dela poster med andra för att öka samarbetet.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 0%

---


<!--should this move to the Access folder when we have sharing for ALL the objects???-->

<!--take out preview and production references at release-->

# Dela poster

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>  -->

{{planning-important-intro}}

Om du vill samarbeta med andra användare kan du dela poster med andra.

Du kan dela en Adobe Workfront Planning-post på följande sätt:

* Kopiera länken till postsidan från webbläsaren när sidan är öppen.

* Kopiera en länk till postens sida när du visar poster i posttypens tabellvy.

* Du kan dela alla poster på en arbetsyta med andra användare genom att dela arbetsytan och posttypen.

  Mer information finns i följande artiklar:

   * [Dela en arbetsyta](/help/quicksilver/planning/access/share-workspaces.md)

   * [Dela en posttyp](/help/quicksilver/planning/access/share-record-types.md)

I den här artikeln beskrivs hur du kan kopiera en länk till en posts sida från en posttyps tabellvy.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Alla Workfront- och Planning-paket</p> <p>Alla arbetsflöden och alla planeringsdokument</p>
<p>Mer information om vad som ingår i respektive Workfront Planning-paket får du av Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p>Medarbetare eller högre</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>  <p>Visa eller högre behörigheter på en arbetsyta och posttyp för att dela en post med en länk</p>
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>  </td> 
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
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Contributor or higher license </p>
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
   <td>  <p>View or higher permissions to a workspace and record typeto share   a record using a link </p>
   <p>Manage permissions to a workspace and record type to share the records in the workspace </p>
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table> -->


## Dela postlänkar från posttypstabellvyn

{{step1-to-planning}}

Arbetsytan som du senast öppnade öppnas.
1. Klicka på ett posttypskort.

   Posttypssidan öppnas.
1. (Villkorligt) Välj en tabellvy i listrutan **Visa** i tabellens övre högra hörn. Detta bör vara standardvyn, såvida du inte har visat posttypen i tidslinjevyn när du senast öppnade den.

   Posterna som är associerade med den valda posttypen visas i tabellvyn.
1. Högerklicka på en postrad

   eller

   Håll markören över en posts namn, klicka på menyn **Mer** ![Mer](assets/more-menu.png) och klicka sedan på **Kopiera länk**.

   ![Sammanhangsbaserad meny för postrad](assets/contextual-menu-for-record-row.png)

   Länken kopieras till Urklipp.

1. Klistra in länken i ett e-postmeddelande eller i ett chattfönster om du vill dela den med andra användare. När användarna får länken öppnas postsidan.

   >[!TIP]
   >
   >Fälten på postsidan är samma fält som är tillgängliga i postens tabellvy.


   <!--add there when it will be available: if they have access to this record-->

## Dela alla poster på en arbetsyta genom att dela arbetsytan

Du kan dela alla poster på en arbetsyta när du delar arbetsytan med andra.

Posttyper och poster ärver samma behörigheter från arbetsytan.

Endast användare med behörigheten Hantera för en arbetsyta kan dela den med andra.

Mer information finns i [Dela en arbetsyta](/help/quicksilver/planning/access/share-workspaces.md).

## Dela alla poster i en posttyp genom att dela posttypen

Poster ärver behörigheter från posttypen.

Som standard ärver posttyper behörigheter från arbetsytan.

Du kan dock göra något av följande:

* Inaktivera ärvda behörigheter från arbetsytan för en posttyp. Detta tar bort högre behörigheter till posterna, men behåller behörigheterna Visa till arbetsytan, posttypen och posterna.
* Bevilja manuellt behörigheter till användare för en posttyp, även om de inte har några behörigheter till arbetsytan. Detta ger dem automatiskt behörigheten Visa på arbetsytan. Detta ger användarna behörighet till posterna.

Endast användare med behörigheten Hantera på en arbetsyta kan dela sina posttyper och poster med andra.

Mer information finns i [Dela posttyper](/help/quicksilver/planning/access/share-record-types.md).


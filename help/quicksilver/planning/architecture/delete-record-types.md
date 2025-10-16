---
title: Ta bort posttyper
description: Du kan ta bort posttyper när de inte längre är relevanta. När du tar bort posttyper tas även all information som är kopplad till posttyperna bort, som poster, fält och vyer.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---


<!--keep the global record type reference in yellow till January 2026-->

# Ta bort posttyper

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Du kan ta bort posttyper när de inte längre är relevanta.

Om du tar bort posttyper tas även all information som är kopplad till posttyperna bort. Mer information finns i avsnittet [Att tänka på när du tar bort posttyper](#considerations-when-deleting-record-types) i den här artikeln.

Mer information om posttyper finns i [Översikt över posttyper](/help/quicksilver/planning/architecture/overview-of-record-types.md).

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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
<ul> 
<li><p>Alla Workfront- och Planning-paket</p></li>
<p>eller</p>
<li><p>Alla arbetsflöden och alla planeringsdokument</p></li></ul>
<!--<p>To delete global record types:</p>
<ul><li><p>Any Workfront package and a Planning Plus package</p></li>
<p>Or</p>
<li><p>Workflow and Planning Prime and Ultimate packages</p></li></ul>-->
<p>Mer information om vad som ingår i respektive Workfront Planning-paket får du av Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>   <p>Hantera behörigheter till en arbetsyta</p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>  </td> 
  </tr>  
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <td><p> Standard</p>
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
   <td>   <p>Manage permissions to a workspace and record type</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> 
-->


## Att tänka på när du tar bort posttyper

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* Du kan bara ta bort posttyper från arbetsytor som du har behörigheten Hantera.
* När du tar bort posttyper tas följande information bort som är kopplad till dem:

   * Alla poster av den typen.
   * Alla fält som är associerade med posttypen.
   * Alla vyer (inklusive filter, grupperingar och sorteringsvillkor) av posttypen.
* Posttypen tas bort från alla användare som använder arbetsytan.
* Du kan inte återställa borttagna posttyper eller deras information.
* Vi rekommenderar att du återskapar de fält och poster som är kopplade till den posttyp som du vill ta bort på en annan posttyp innan du tar bort dem.

<!--
<div class="preview">

* You cannot delete a global record type that has been added to other workspaces. 

   For more information, see the section [Delete global record types](#delete-global-record-types) in this article. 

</div>-->

## Ta bort posttyper

{{step1-to-planning}}

1. Klicka på arbetsytan vars posttyper du vill ta bort,

   eller

   Utöka den nedåtriktade pilen till höger om namnet på en befintlig arbetsyta i en arbetsyta, sök efter en arbetsyta och markera den när den visas i listan.

   Arbetsytan öppnas och posttyperna visas.
1. Gör något av följande:

   * Håll markören över posttypkortet, klicka på menyn **Mer** och sedan på **Ta bort**.
   * Klicka på kortet för den posttyp som du vill ta bort och klicka på menyn **Mer** ![Mer](assets/more-menu.png) till höger om posttypens namn på posttypssidan och klicka sedan på **Ta bort**.

   ![Ta bort posttypsbekräftelse permanent](assets/permanently-delete-record-type-confirmation.png)


1. Skriv **delete** i bekräftelserutan och klicka sedan på **Ta bort permanent**. Detta är inte skiftlägeskänsligt.

   Den valda posttypen, tillsammans med deras fält, associerade poster och vyer, tas bort och kan inte återställas.

<!--

<div class="preview">

## Delete global record types

The following scenarios exist when deleting global record types:

* If a record type configured as global has not yet been added to another workspace, you can delete it from its original workspace. 

* If a record type configured as a global record type has been added to at least one other workspace, you cannot delete it from its original workspace. You must first remove (by deleting) global record types from the secondary workspaces where they were added and then you can permanently delete the global record type from its original workspace. 

### Delete a global record type from the original workspace

You can delete a record type from its original workspace if it's no longer relevant. 

1. Go to the global record type in its original workspace. 

1. (Conditional) Do one of the following, depending on whether the global record type has been added to secondary workspaces: 

   * If the record type was not added to a secondary workspace, click on the **More** menu ![More menu](assets/more-menu.png) on the record type's card, or to the right of the record type's name on its page, then click **Delete**. 
   * If the record type was added to at least one other secondary workspace, first, go to the secondary workspace and delete the global record from that space. 

      For information, see the section [Delete a global record type from a secondary workspace](#delete-a-global-record-type-from-a-secondary-workspace) in this article. 
   
1. (Conditional) Continue deleting the record type, as described in the section [Delete record types](#delete-record-types-1) in this article.

   The following things occur: 

   * The global record type is removed from the original workspace and the record type, its records and fields cannot be recovered.
   * All global record types from the secondary workspaces and their records are also removed.

### Delete a global record type from a secondary workspace

You can delete a record type you added from another workspace if no longer needed. 

Consider the following:

* Deleting a global record type from a secondary workspace will only remove it from the secondary workspace. The record type remains in the original workspace. 

* When you delete a global record type from a secondary workspace, the following are also deleted:

   * The records added from the secondary workspace.

   ***************Not yet there, coming soon:* The fields added from the secondary workspace.*********

* Global record types deleted from their secondary workspaces cannot be recovered. 

* The original record type remains in its original workspace as well as in other workspaces where it's been added. 

To delete a global record type from a secondary workspace: 

1. Go to the global record type in its secondary workspace. 

1. (Optional) Click on the **More** menu ![More menu](assets/more-menu.png) on the record type's card, or to the right of the record type's name on its page, then click **Delete**.
1. (Conditional) Type **delete** in the field provided, then click **Permanently delete**.

   ![Delete secondary global record type confirmation box](assets/delete-secondary-global-record-type.png)

   The following things occur: 

   * The record type created from a global record type is removed from the selected workspace. 
   * The original record type with its fields remain in their original workspace. 
   * The record type remains in all other workspaces where it's been added.
   * The records *******and fields****** added to the record type from the current workspace are deleted. All other records added from additional workspaces where the global record type was added are preserved in their respective workspaces and in the original workspace. <!--Fields are preserved in the workspaces where they were added.
   
</div>   
   -->
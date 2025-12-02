---
title: Ta bort fält
description: I Adobe Workfront Planning kan du ta bort anpassade fält som inte längre är relevanta.
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
author: Alina
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 476e10f2962f19fd17705cb5f20619d3b636aaa4
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---



# Ta bort fält

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

I Adobe Workfront Planning kan du skapa anpassade fält för att lagra information om poster.

Mer information om hur du skapar anpassade fält i Workfront Planning finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

Du kan ta bort Workfront Planning-fält som inte längre är relevanta.

## Att tänka på när du tar bort Workfront Planning-fält:

* Du kan bara ta bort ett fält i posttyptabellvyn.
* Du kan inte ta bort det primära fältet för en post.
* All information som lagras i fältet tas bort och kan inte återställas.
* När du tar bort ett anslutet postfält tas även alla anslutna sökfält bort från den posttyp som du ansluter från. De anslutna postfälten för de posttyper du ansluter till tas också bort från den post du ansluter till.

  Om du till exempel ansluter kampanjer till en annan posttyp som kallas product, och du tar bort fältet Product connected och fältet Product&#39;s Status lookup från kampanjen, tas följande bort:

   * Det produktanslutna fältet från kampanjen
   * Uppslagsfältet Produktstatus från kampanjen
   * Det kampanjanslutna fältet från produkten.

  Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

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
eller
<li><p>Alla arbetsflöden och alla planeringsdokument</p></li></ul>

<!--
<p><span class="preview">To delete global record types:</span</p>
<ul><li><p><span class="preview">Any Workfront package and a Planning Plus package</span></p></li>
Or
<li><p><span class="preview">Workflow and Planning Prime and Ultimate packages</span></p></li></ul>
-->

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
   <td><p> Standard </p>
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
   <td>   <p>Manage permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> -->

## Ta bort fält

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. Klicka på arbetsytan vars postfält du vill ta bort.

   Arbetsytan öppnas och posttyperna visas.

1. Klicka på kortet för en posttyp.

1. (Villkorligt) Om det inte redan är markerat klickar du på fliken för en **tabellvy** på posttypssidan.

   Alla befintliga poster som är associerade med posttypen visas i tabellvyns rader.

1. Leta reda på fältet som du vill ta bort i kolumnrubrikerna, håll markören över kolumnrubriken och klicka sedan på nedåtpilen efter fältnamnet.

   ![Pilmeny efter fältets namn i tabellhuvudet markerat](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Klicka på **Ta bort**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Bekräfta genom att klicka på **Ta bort**.

   Fältet tas bort, kan inte återställas och kan inte längre kopplas till några poster.

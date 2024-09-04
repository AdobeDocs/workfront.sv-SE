---
title: Ta bort fält
description: I Adobe Workfront Planning kan du ta bort anpassade fält som inte längre är relevanta.
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
author: Alina
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: bd202821687453288c96147933331c8a7a6b3acb
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---



# Ta bort fält

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

+++ Expandera om du vill visa åtkomstkraven för Workfront Planning.

Du måste ha följande för att kunna komma åt Workfront Planning:

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
   <td role="rowheader"><p>Adobe Workfront Planning*</p></td> 
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
   <td>   <p>Hantera behörigheter till en arbetsyta </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p></td> 
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
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

## Ta bort fält

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. Klicka på arbetsytan vars postfält du vill ta bort.

   Arbetsytan öppnas och posttyperna visas.

1. Klicka på kortet för en posttyp.

1. (Villkorligt) Om det inte redan är markerat klickar du på fliken för en **tabellvy** på posttypssidan.

   Alla befintliga poster som är associerade med posttypen visas i tabellvyns rader.

1. Leta reda på fältet som du vill ta bort i kolumnrubrikerna, håll markören över kolumnrubriken och klicka sedan på nedåtpilen efter fältnamnet.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Klicka på **Ta bort**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Bekräfta genom att klicka på **Ta bort**.

   Fältet tas bort, kan inte återställas och kan inte längre kopplas till några poster.

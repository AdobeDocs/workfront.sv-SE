---
title: Ta bort fält
description: I Adobe Workfront Planning kan du ta bort anpassade fält som inte längre är relevanta.
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
author: Alina
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 1dc2791bed0dfada109ee102e09c25ae9a52e6b0
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---



# Ta bort fält

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

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
   <td>   <p>Hantera behörigheter till en arbetsyta <span class="preview">och posttyp</span> </a> </p>  
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

<!--replace the layout template info in the table with this at release: 


<p>In the Production environment, all users including the System Administrators must be assigned to a layout template that includes the Planning areas.</p>
<p><span class="preview">In the Preview environment, Standard users and System Administrators have the Planning area enabled by default.</span></p>

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

   ![Pilmeny efter fältets namn i tabellhuvudet markerat](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Klicka på **Ta bort**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Bekräfta genom att klicka på **Ta bort**.

   Fältet tas bort, kan inte återställas och kan inte längre kopplas till några poster.

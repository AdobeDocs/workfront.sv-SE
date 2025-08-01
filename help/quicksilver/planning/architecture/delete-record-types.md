---
title: Ta bort posttyper
description: Du kan ta bort posttyper när de inte längre är relevanta. När du tar bort posttyper tas även all information som är kopplad till posttyperna bort, som poster, fält och vyer.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---


# Ta bort posttyper

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Du kan ta bort posttyper när de inte längre är relevanta.

Om du tar bort posttyper tas även all information som är kopplad till posttyperna bort. Mer information finns i avsnittet [Att tänka på när du tar bort posttyper](#considerations-when-deleting-record-types) i den här artikeln.

Mer information om posttyper finns i [Översikt över posttyper](/help/quicksilver/planning/architecture/overview-of-record-types.md).

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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
<p>Din organisations instans av Workfront måste vara registrerad på Adobe Unified Experience för att få tillgång till Workfront Planning.</p> 
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td> 
   <td><p> Standard</p>
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
   <td>   <p>Hantera behörigheter till en arbetsyta och en posttyp</p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p></td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


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

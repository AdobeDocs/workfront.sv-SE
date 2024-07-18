---
title: Ta bort fält
description: I Adobe Workfront Planning kan du ta bort anpassade fält som inte längre är relevanta.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Delete fields
description: In Adobe Planning, you can delete custom fields that are no longer relevant.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# Ta bort fält

{{planning-important-intro}}

I Adobe Workfront Planning kan du skapa anpassade fält för att lagra information om poster.

Mer information om hur du skapar anpassade fält i Workfront Planning finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

Du kan ta bort Workfront Planning-fält som inte längre är relevanta.

## Att tänka på när du tar bort Workfront Planning-fält:

* Du kan bara ta bort ett fält i posttyptabellvyn.
* Du kan inte ta bort det primära fältet för en post.
* All information som lagras i fältet tas bort och kan inte återställas.
* När du tar bort ett länkat postfält tas även alla länkade sökfält bort från den posttyp du länkar från. De länkade postfälten för de posttyper som du länkar till tas inte bort.

  Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

## Åtkomstkrav

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
   <p> Produkt</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-avtal</p></td>
   <td>
<p>Din organisation måste vara registrerad på Workfront Planning i ett tidigt skede </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront</p></td>
   <td>
<p>Alla</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licens</p></td>
   <td>
   <p>Alla</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td>
   <td> <p>Det finns inga åtkomstnivåkontroller för Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Workfront- eller gruppadministratören måste lägga till planeringsområdet i layoutmallen. Mer information finns i <a href="/help/quicksilver/planning/access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Hantera behörigheter till en arbetsyta </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>
</td>
  </tr>
 </tbody>
</table>



<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

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

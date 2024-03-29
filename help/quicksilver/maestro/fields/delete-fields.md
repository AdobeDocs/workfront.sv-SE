---
title: Ta bort fält
description: I Adobe Workfront-planeringen kan du ta bort anpassade fält som inte längre är relevanta.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: a0f12a016ae8ac73136f05bf3255f9882e2ce6d4
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Delete fields
description: In Adobe Maestro, you can delete custom fields that are no longer relevant.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# Ta bort fält

{{maestro-important-intro}}

I Adobe Workfront kan du skapa anpassade fält för att lagra information om poster.

Mer information om hur du skapar anpassade fält i Workfront-planeringen finns i [Skapa fält](../fields/create-fields.md).

Du kan ta bort planeringsfält i Workfront som inte längre är relevanta.

## Att tänka på när du tar bort planeringsfält i Workfront:

* Du kan bara ta bort ett fält i posttyptabellvyn.
* Du kan inte ta bort det primära fältet för en post.
* All information som lagras i fältet tas bort och kan inte återställas.
* När du tar bort ett länkat postfält tas även alla länkade sökfält bort från den posttyp du länkar från. De länkade postfälten för de posttyper som du länkar till tas inte bort.

  Mer information finns i [Koppla posttyper](../architecture/connect-record-types.md).

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
<p>Din organisation måste vara registrerad i betaprogrammet för Adobe Workfront-planering. Kontakta din kontorepresentant om du vill veta mer om det nya erbjudandet. </p>
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
   <td> <p>Det finns inga åtkomstnivåkontroller för Workfront-planering</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Workfront- eller gruppadministratören måste lägga till planeringsområdet i layoutmallen. Mer information finns i <a href="../access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Hantera behörigheter till en arbetsyta</a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>
</td>
  </tr>
 </tbody>
</table>



<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Ta bort fält

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-maestro}}

Då öppnas den senast använda arbetsytan i Workfront planering.
1. Klicka på kortet för en posttyp vars fält du vill ta bort.
1. (Villkorligt) Välj en **Tabellvy** från **Visa** nedrullningsbar meny i det övre högra hörnet på posttypssidan.
1. Leta reda på fältet som du vill ta bort i kolumnrubrikerna, håll markören över kolumnrubriken och klicka sedan på nedåtpilen efter fältnamnet.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Klicka **Ta bort**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Klicka **Ta bort** för att bekräfta.

   Fältet tas bort, kan inte återställas och kan inte längre kopplas till några poster.

---
title: Ta bort fält
description: I Adobe Maestro kan du ta bort anpassade fält som inte längre är relevanta.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 4cdebe4890b775a097469e7d7035a38397b71094
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Ta bort fält

>[!IMPORTANT]
>
>Informationen i den här artikeln handlar om Adobe Maestro, ett nytt erbjudande från Adobe.
>
>För närvarande ingår Adobe Maestro i ett betaprogram som är öppet för ett begränsat antal kunder.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.
>
>Mer information finns i [Adobe Maestro - översikt](../maestro-overview.md).

I Adobe Maestro kan du skapa anpassade fält för att lagra information om poster.

Mer information om hur du skapar anpassade fält i Maestro finns i [Skapa fält](../architecture-and-fields/create-fields.md).

Du kan ta bort fält i Maestro som inte längre är relevanta.

## Att tänka på när du tar bort Maestro-fält:

* Du kan ta bort fält som du har skapat eller fält som har skapats av andra användare eller av systemet. <!--this will change with access levels/ permissions-->
* Du kan inte ta bort namnfältet för en post. <!--change this to say you can't delete the field selected to be the primary-->
* Du kan bara ta bort ett fält i posttyptabellen.
* All information som lagras i fältet tas bort och kan inte återställas.
* När du tar bort ett länkat postfält tas även alla länkade sökfält bort från den posttyp du länkar från. De länkade postfälten för de posttyper som du länkar till tas inte bort.

  Mer information finns i [Koppla posttyper](../architecture-and-fields/connect-record-types.md).
  <!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-avtal</p></td>
   <td>
<p>Din organisation måste vara registrerad i det betaprogram som Adobe Maestro stängt. Kontakta din kontorepresentant om du vill veta mer om det nya erbjudandet. </p>
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
   <td role="rowheader">Åtkomstnivå</td>
   <td> <p>Alla</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Layoutmall</td>
   <td> <p>Systemadministratören måste lägga till Maestro-området i layoutmallen. Mer information finns i <a href="../access/grant-access.md">Ge åtkomst till Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Ta bort fält

<!--When they release the sharing of fields between other records, revise this section.  -->

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-workfront.png) i det övre högra hörnet av Workfront eller **Huvudmeny** icon ![](assets/main-menu-shell.png)  i det övre vänstra hörnet, om det är tillgängligt, klickar du på **Maestro** ![](assets/maestro-icon.png).

   Då öppnas den senast använda arbetsytan i Maestro.
1. Klicka på kortet för en posttyp vars fält du vill ta bort.
1. (Villkorligt) Välj en **Tabellvy** från **Visa** nedrullningsbar meny i det övre högra hörnet på posttypssidan.
1. Leta reda på fältet som du vill ta bort i kolumnrubrikerna, håll markören över kolumnrubriken och klicka sedan på nedåtpilen efter fältnamnet.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Klicka **Ta bort**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Klicka **Ta bort** för att bekräfta.

   Fältet tas bort, kan inte återställas och kan inte längre kopplas till några poster.

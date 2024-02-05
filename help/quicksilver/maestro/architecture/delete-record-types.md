---
title: Ta bort posttyper
description: Du kan ta bort driftsposttyper eller taxonomiposttyper när de inte längre är relevanta.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 5681b540bceddaae85116b632e968d94761eec0d
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav:
---
title: Delete record types
description: You can delete operational record types or taxonomy record types when they are no longer relevant. 
author: Alina
feature: Work Management
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->

# Ta bort posttyper

{{maestro-important-intro}}

Du kan ta bort driftsposttyper eller taxonomiposttyper när de inte längre är relevanta.

Mer information om posttyper och taxonomier finns i [Översikt över posttyper och taxonomier](../architecture/overview-of-record-types-and-taxonomies.md).

Vi rekommenderar att du återskapar de fält och de poster som är kopplade till den posttyp eller taxonomi som du vill ta bort på en annan posttyp innan du tar bort dem.

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td>
   <td> <p>Det finns inga åtkomstnivåkontroller för Maestro</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Hantera behörigheter till en arbetsyta</a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Din Workfront- eller gruppadministratör måste lägga till Maestro-området i layoutmallen. Mer information finns i <a href="../access/access-overview.md">Åtkomstöversikt</a>. </p>  
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

## Att tänka på när du tar bort posttyper

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* Du kan bara ta bort posttyper eller taxonomier från arbetsytor där du har behörigheten Hantera.
* När du tar bort posttyper tas all information som är kopplad till dem bort, inklusive fält och poster av den typen. Posttypen tas bort från alla användare som använder arbetsytan.
* Du kan inte återställa borttagna posttyper eller deras information.

## Ta bort posttyper

Att ta bort taxonomiposttyper är identiskt med att ta bort driftsposttyper.

{{step1-to-maestro}}

Den senast använda arbetsytan bör öppnas som standard.

1. (Valfritt) Expandera den nedåtriktade pilen till höger om namnet på en befintlig arbetsyta och markera den arbetsyta som du vill ta bort posttyper för.

   Arbetsytan öppnas och posttyperna och taxonomierna som är kopplade till den visas.
1. Klicka på kortet för den posttyp eller taxonomi som du vill ta bort.

   Då öppnas posttypens sida.
1. Klicka på **Mer** meny ![](assets/more-menu.png) till höger om posttypens namn och klicka sedan på **Ta bort**.
1. Klicka **Ta bort** för att bekräfta.

   Den valda posttypen eller taxonomin, tillsammans med fälten och tillhörande poster, tas bort.

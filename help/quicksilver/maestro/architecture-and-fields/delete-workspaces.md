---
title: Ta bort arbetsytor
description: Du kan ta bort arbetsytor när de inte längre är relevanta.
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Ta bort arbetsytor

>[!IMPORTANT]
>
>För närvarande ingår Adobe Maestro i ett slutet betaprogram som är öppet för ett begränsat antal kunder.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.
>
>Mer information finns i [Adobe Maestro - översikt](../maestro-overview.md).

I Adobe Maestro är arbetsytorna centraliserade platser där team kan planera sitt arbete. Mer information finns i [Skapa arbetsytor](../architecture-and-fields/create-workspaces.md).

Du kan ta bort arbetsytor som inte längre är relevanta.

Vi rekommenderar att du återskapar vissa eller alla posttyper och taxonomier som är kopplade till arbetsytan som du vill ta bort på en annan arbetsyta innan du tar bort den.

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
<p>Din organisation måste vara registrerad i betaprogrammet Adobe Maestro. Kontakta din kontorepresentant om du vill veta mer om det nya erbjudandet. </p>
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

## Att tänka på när du tar bort arbetsytor

* Du kan ta bort alla arbetsytor som du eller någon i organisationen har skapat. <!--this will change with access levels and permissions-->
* När du tar bort arbetsytor tas även alla posttyper, taxonomier och deras fält bort. <!--asked Lilit because the confirmation says the records don't delete, but not sure how they can exist outside of a workspace?!-->
* Borttagna arbetsytor och den information de innehåller kan inte återställas.

## Ta bort en arbetsyta

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-workfront.png) i Workfront övre högra hörn, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> klicka sedan på **Maestro** ![](assets/maestro-icon.png).

   Då öppnas den senaste arbetsytan som du använde.

1. (Valfritt) Expandera den nedåtriktade pilen till höger om namnet på en befintlig arbetsyta och markera den arbetsyta som du vill ta bort.
1. Klicka på **Mer** meny ![](assets/more-menu.png) bredvid arbetsytans namn och klicka sedan på **Ta bort**.
1. Klicka **Ta bort** för att bekräfta.

   Arbetsytan tas bort och kan inte återskapas. Alla posttyper, taxonomier, deras poster och fälten som är kopplade till dem tas också bort. <!--ensure this is right after closed beta-->
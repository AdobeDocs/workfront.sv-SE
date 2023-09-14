---
title: Redigera posttyper
description: Du kan redigera posttyper när de har sparats. Posttyperna är objekttyperna för Adobe Maestro.
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---


<!--update the metadata with real information when making this available in TOC and in the left nav
---
title: Edit record types
description: You can edit record types after they have been saved. Record types are the objec types of Adobe Maestro.
author: Alina
role: User
feature: Work Management 
topic: Architecture
hidefromtoc: yes
hide: yes
---

-->

# Redigera posttyper

>[!IMPORTANT]
>
>För närvarande ingår Adobe Maestro i ett betaprogram som är öppet för ett begränsat antal kunder.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.
>
>Mer information finns i [Adobe Maestro - översikt](../maestro-overview.md).

Posttyperna är objekttyperna för Adobe Maestro. Du kan redigera utseendet på posttyper som du eller någon annan har skapat. Mer information om hur du skapar posttyper i Maestro finns i [Skapa posttyper](../architecture-and-fields/create-record-types.md).

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

## Redigera posttyper

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-workfront.png) i Workfront övre högra hörn, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> klicka sedan på **Maestro** ![](assets/maestro-icon.png).

   Den senast använda arbetsytan bör öppnas som standard.

1. (Valfritt) Expandera den nedåtriktade pilen till höger om namnet på en befintlig arbetsyta och markera den arbetsyta som du vill skapa posttyper för.
1. Håll muspekaren över ett kort av en posttyp och klicka på knappen **Mer** meny ![](assets/more-menu.png) i det övre högra hörnet av posttypskortet och klicka sedan på **Uppdatera utseende**.

   ![](assets/update-appearance-link-from-more-menu-on-record-type-card.png)

1. Uppdatera följande information i rutan Uppdatera posttyp:

   * **Postnamn**: Redigera posttypens namn om det behövs. <!--correct this - I asked Garik to change this field to "Record type name"-->
   * **Utseende**: Redigera färg och form för ikonen som är associerad med posttypen. Gör följande:
      * Välj en färg som identifierar posttypen. Det här är färgen på ikonen för posttyp. Grått är markerat som standard.
      * Välj en ikon i listan eller börja skriva namnet på en ikon för att beskriva vad den representerar och markera den sedan när den visas. Det här är ikonen för posttypen. Som standard är en filikon markerad.

     ![](assets/update-record-type-box.png)

1. Klicka utanför rutan Uppdatera posttyp för att spara ändringarna.
1. (Valfritt) Klicka på posttypskortet i arbetsytan för att öppna posttypens sida.
1. Klicka på **Mer** till höger om posttypens namn och klicka sedan på **Byt namn** för att byta namn på posttypen

   eller

   Byt namn på posttypen i rubriken.  <!--check to see if they renamed this to "Rename" - it kept going back and forth between Rename and Edit-->

   ![](assets/more-menu-options-from-record-details-page.png) <!--check this screen shot - not sure this is valid ???-->

   Du kan också byta namn på en posttyp i huvudet på posttypens sida.


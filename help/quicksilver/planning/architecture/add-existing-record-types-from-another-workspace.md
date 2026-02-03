---
title: Lägg till befintliga posttyper från en annan Workspace
description: Posttyperna är objekttyperna för Adobe Workfront Planning. I Workfront Planning kan du lägga till en befintlig posttyp som har skapats på en annan arbetsyta.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: 187505de92f9a912547018865f2742bfecec77ad
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 0%

---


# Lägga till befintliga posttyper från en annan arbetsyta

{{planning-important-intro}}

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Som arbetsytehanterare kan du lägga till en posttyp som finns i en annan arbetsyta i en arbetsyta som du hanterar i Adobe Workfront Planning.

En arbetsytehanterare måste först ange en posttyp som global posttyp innan du kan lägga till den i arbetsytor som du hanterar som en befintlig posttyp. Workspace-hanterare kan ange en posttyp som global när de skapar eller redigerar den genom att definiera posttypens inställningar för arbetsytan mellan arbetsytorna.

Mer information finns i [Konfigurera funktioner för arbetsytan över arbetsytor för posttyper](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

I den här artikeln beskrivs hur du kan lägga till en posttyp från en befintlig.

Innan du lägger till poster på en arbetsyta från en global posttyp, ska du även läsa artikeln [Översikt över posttyper på arbetsytan](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).


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
<ul><li><p>Alla Workfront-paket och ett Planning Plus-paket</p></li>
eller
<li><p>Alla arbetsflöden och ett Planning Prime- eller Ultimate-paket</p></p></li></ul>
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

  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<ul><li><p>Any Workfront package</p></li>
<p>And</p>
<li><p>Any Planning package to create connectable record types</p></li>
<li><p>A Planning Plus package to create global record types</p></li>
</ul>
Or:
<ul><li><p>A Prime or Ultimate Workflow package</p> </li>
And
<li><p>A Planning Prime or Ultimate package</p></li></ul>
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
   </td> 

  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and to the record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table>-->

## Skapa en posttyp genom att lägga till en befintlig från en annan arbetsyta

>[!NOTE]
>
>Se till att det finns minst en posttyp som är global på minst en annan primär arbetsyta.
>
>Mer information finns i [Konfigurera funktioner för arbetsytan över arbetsytor för posttyper](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

1. Gå till en arbetsyta där du vill skapa en posttyp (sekundär arbetsyta).
1. Börja skapa en posttyp enligt beskrivningen i artikeln [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md) och klicka sedan på **Lägg till befintlig**. <!--check this - the option might have been renamed in the UI-->

   ![Modal för att lägga till posttyp med möjlighet att lägga till från en annan arbetsyta](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

   >[!TIP]
   >
   >Om det inte finns några konfigurerade posttyper som kan läggas till i andra arbetsytor i systemet visas inte alternativet **Lägg till befintlig**.

1. Klicka på **Fortsätt**.
1. I rutan **Välj posttyp** klickar du på kortet för den posttyp som du vill lägga till från en befintlig arbetsyta och sedan på **Lägg till**.

   Posttypen läggs till på den sekundära arbetsytan som du har valt och den **globala posttypen** ikonen ![den primära arbetsytan för den globala posten](assets/global-icon.png) visas på posttypens kort.

   Följande saker händer:

   * Följande information läggs också till från den befintliga globala posttypen:

      * Alla originalfält
      * Alla postanslutningar
   * Du kan inte visa poster som lagts till från den ursprungliga arbetsytan för posttypen från den sekundära arbetsytan.
   * Du kan bara visa poster som lagts till från den ursprungliga arbetsytan för den posttypen på den arbetsytan, om du har minst behörigheten Visa på den arbetsytan.
   * Det skrivskyddade fältet **Workspace** läggs till i den nya posttypstabellvyn. I fältet visas arbetsytan där varje post skapades.

     >[!NOTE]
     >
     >Du kan inte redigera den nya posttypens utseende, ytterligare inställningar eller originalfält. Du kan bara redigera posttypen och alla dess ursprungliga fält och inställningar från den ursprungliga arbetsytan.
     >

1. (Valfritt) Klicka och dra och släpp den nya posttypen till valfritt avsnitt på arbetsytan.
1. (Valfritt) Klicka på menyn **Mer** på den nya posttypens kort eller till höger om posttypens namn på sidan och klicka sedan på något av följande:

   * **Dela** om du vill dela posttypen från den sekundära arbetsytan.
   * **Ta bort** om du vill ta bort posttypen från den sekundära arbetsytan. När du tar bort posttyper från den sekundära arbetsytan tas även poster som lagts till från den sekundära arbetsytan bort.

     Vyer som lagts till från den sekundära arbetsytan tas inte bort. <!--checking with Lilit - not sure if this is by design??-->

   Mer information finns i avsnittet Ta bort globala posttyper i artikeln [Ta bort posttyper](/help/quicksilver/planning/architecture/delete-record-types.md).

<!--This will be released later with another epic: 
1. In the table view, click the **+** icon in the upper-right corner to add new fields. For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).
1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.
-->

&lt;!—check with Lilit if we can add automations or request forms to secondary global RTs??—add step with links to those articles if/ when yes—>








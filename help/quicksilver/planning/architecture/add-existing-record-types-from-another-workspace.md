---
title: Lägg till befintliga posttyper från en annan Workspace
description: Posttyperna är objekttyperna för Adobe Workfront Planning. I Workfront Planning kan du lägga till en befintlig posttyp som har skapats på en annan arbetsyta.
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: 393f858ba3711b367cf06ad846ea60be0d6d9034
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Lägga till befintliga posttyper från en annan arbetsyta

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Som arbetsytehanterare kan du lägga till en posttyp som finns i en annan arbetsyta i en arbetsyta som du hanterar i Adobe Workfront Planning.

I den här artikeln beskrivs hur du kan lägga till en posttyp från en befintlig och hur du kan ta bort den, om den inte längre behövs.

En arbetsytehanterare måste ange en posttyp som global innan du kan lägga till den i arbetsytor som du hanterar som en befintlig posttyp.

Du kan ange en posttyp som global när du skapar eller redigerar den, medan du definierar inställningarna för den gemensamma arbetsytan.

Mer information finns i [Konfigurera funktioner för arbetsytan över arbetsytor för posttyper](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

Innan du lägger till poster på en arbetsyta från en global posttyp läser du [Översikt över posttyper på arbetsytan](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).


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
<ul><li><p>Alla Workfront-paket</p></li>
<p>Och</p>
<li><p>Planeringspaket för att skapa kopplingsbara posttyper</p></li>
<li><p>Planning Plus-paket för att skapa globala posttyper</p></li>
</ul>
<!--Or:
<ul><li><p>Any Workflow package</p> </li>
And
<li><p>Planning Prime or Ultimate package</p></li></ul>-->
<p>Mer information om vad som ingår i respektive Workfront Planning-paket får du av din kontoansvarige på Workfront. </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>   <p>Hantera behörigheter till en arbetsyta </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>  </td> 
  </tr>  
</tbody> 
</table>

Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Skapa en posttyp från en befintlig posttyp

1. Börja skapa en posttyp enligt beskrivningen i artikeln [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md) och klicka sedan på **Lägg till befintlig**. <!--check this - the option might have been renamed in the UI-->

   ![Modal för att lägga till posttyp med möjlighet att lägga till från en annan arbetsyta](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

1. Klicka på **Fortsätt**.
1. I rutan **Välj posttyp** klickar du på kortet för den posttyp som du vill lägga till från en befintlig arbetsyta och sedan på **Lägg till**.

   Posttypen läggs till på den arbetsyta som du har valt.

   >[!TIP]
   >
   >Om det inte finns några konfigurerade posttyper som ska läggas till på en annan arbetsyta visas inte alternativet att lägga till dem från en annan arbetsyta.

   Följande saker händer:

   * Följande information läggs också till från den befintliga globala posttypen:

      * Alla originalfält
      * Alla postanslutningar
   * Du kan bara visa poster som lagts till från andra arbetsytor som använder samma globala posttyp om du har minst behörigheten Visa på dessa arbetsytor.
   * Ikonen **Global posttyp** ![Global posttyp ](assets/global-icon.png) läggs till på kortet med den nya posttypen.
   * Det skrivskyddade fältet **Workspace** läggs till i den nya posttypstabellvyn. Fältet visar vilken arbetsyta varje post skapades i.

     >[!NOTE]
     >
     >Du kan inte redigera den nya posttypens utseende, ytterligare inställningar eller originalfält. Du kan bara redigera posttypen och alla dess ursprungliga fält och inställningar från den ursprungliga arbetsytan.

1. (Valfritt) Klicka och dra och släpp den nya posttypen till valfritt avsnitt på arbetsytan.

<!--This will be released later with another epic: 1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.-->

## Ta bort en global posttyp från en sekundär arbetsyta

Du kan ta bort en posttyp som du har lagt till från en annan arbetsyta om den inte längre behövs. Om du tar bort den tas den bara bort från den sekundära arbetsytan och de poster som läggs till på den arbetsytan tas bort. Den ursprungliga posttypen finns kvar på den ursprungliga arbetsytan och i andra arbetsytor där den har lagts till.

Ta bort en global posttyp från en sekundär arbetsyta:

1. Gå till den globala posttypen på den sekundära arbetsytan.

1. (Valfritt) Klicka på menyn **Mer** ![Mer ](assets/more-menu.png) på posttypens kort, eller till höger om posttypens namn på sidan, och klicka sedan på **Ta bort**.
1. (Villkorligt) Skriv **delete** i det angivna fältet och klicka sedan på **Ta bort permanent**.

   Följande saker händer:

   * Posttypen som skapas från en global posttyp tas bort från den valda arbetsytan.
   * Den ursprungliga posttypen och dess fält finns kvar på den ursprungliga arbetsytan.
   * Posttypen finns kvar på alla andra arbetsytor där den har lagts till.
   * Posterna som lagts till posttypen från den aktuella arbetsytan tas bort. Alla andra poster som lagts till från ytterligare arbetsytor där den globala posttypen lades till bevaras.






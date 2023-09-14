---
title: Hantera tidslinjevyn
description: Du kan visa poster i en tidslinjevy när du öppnar posttypssidan i Adobe Maestro.
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '1077'
ht-degree: 0%

---


# Hantera tidslinjevyn

<!--
title: Manage the timeline view in Adobe Maestro
description: You can display records in a timeline view, when accessing the record type page in Adobe Maestro. 
hidefromtoc: yes
hide: yes
author: Alina
feature: Work Management
role: User
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>För närvarande ingår Adobe Maestro i ett betaprogram som är öppet för ett begränsat antal kunder.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.
>
>Mer information finns i [Adobe Maestro - översikt](../maestro-overview.md).

Du kan visa poster i en tidslinjevy när du öppnar posttypssidan i Adobe Maestro.

Mer information om vyerna i maestro finns i [Hantera postvyer i Adobe Maestro](../views/manage-record-views.md).

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

## Hantera en tidslinjevy {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

När du skapar en tidslinjevy visas alla poster av den valda posttypen på en kronologisk tidslinje.

Tänk på följande:

* Du kan bara skapa en tidslinjevy om du har minst två datumfält associerade med en posttyp. När du har ett eller inga datumfält som är associerade med en posttyp är alternativet för tidslinjevy nedtonat.
* Beroende på vilka datum som är associerade med posterna kanske vissa poster inte visas i tidslinjevyn i följande scenarier:

   * När start- och slutdatum inte har några värden
   * När start- eller slutdatumet inte har något värde
   * När startdatumet infaller efter slutdatumet

<!--these are NOT available now because there won't be a table for the timeline view for the near future, per Andy: 
* The records displayed in the timeline view also display in a view-only table to the left of the timeline. 
* Each row in the table and each bar on the timeline represent the same record. 
* Each column in the table is a record field. The columns of this table are preconfigured and cannot be customized. 
* Only a limited number of fields (or columns) display in the timeline view table. 
* You cannot do the following in a timeline view:
     * Add rows or records
     * Add columns or fields
     * Edit record information
-->

När du skapar en tidslinjevy visas alla poster av den valda posttypen som fält på en tidslinje som standard.

Så här hanterar du en tidslinjevy:

1. Gå till den posttypssida som du vill visa tidslinjen för.
1. Skapa en tidslinjevy enligt beskrivningen i artikeln [Hantera postvyer](../views/manage-record-views.md).

   ![](assets/timeline-view-example.png)

   Posterna som är associerade med den posttyp du valde visas som staplar på en kronologisk tidslinje.

1. Navigera genom tidslinjen på något av följande sätt:

   * Klicka på vänster- och högerikonerna eller använd den vågräta rullningen för att flytta bakåt och framåt i tidslinjen.
   * Klicka **Idag** för att centrera tidslinjen till dagens datum.
   * Välj något av följande alternativ på den nedrullningsbara menyn för tidsram för att uppdatera tidsstegen:

      * År
      * Kvartal
      * Månad
1. Klicka **Växla till Standard** visa poster på separata rader <!--check to see if they updated the name of the setting here-->

   eller

   Klicka **Växla till komprimerad vy** för att visa de poster vars datum inte överlappar på samma rad. <!--check to see if they updated the name of the setting here-->

   Poster visas som standard i den komprimerade vyn.

1. Uppdatera följande vyelement enligt beskrivningen i underavsnitten nedan:
   * [Filter](#add-filters)
   * [Gruppering](#add-grouping)
     <!--* [Sort](#add-sort) not sure if this is present in timeline views?!; also check the anchor and make sure it's correct-->
   * [Inställningar](#edit-the-timeline-view-settings)

### Lägg till filter

Med filter kan du minska mängden information som visas på skärmen.

Tänk på följande när du arbetar med filter i tidslinjevyn:

<!-- this list is almost identical to the one for the table view - update both-->

* De filter som du skapar för tidslinjevyn fungerar oberoende av filtren i tabellvyn när de används för samma posttyp.

* Filtren är unika för den vy du väljer. Två tidslinjevyer av samma posttyp kan ha olika filter. Två användare som tittar på samma tidslinjevy ser samma filter som används för närvarande.

* Du kan inte namnge de filter som du skapar och använder i en tidslinjevy.

* När du tar bort filter tas de bort från alla som använder samma posttyp som du och använder samma vy som du använder.

Att lägga till filter i tidslinjevyn är detsamma som att lägga till filter i tabellvyn.

Mer information finns i avsnittet&quot;Lägg till filter&quot; i artikeln [Hantera tabellvyn](../views/manage-the-table-view.md).

### Lägg till gruppering

<!-- if groupings are identical between the table and the timeline, consider replacing this section with this: 

Adding groupings in the timeline view is identical to adding filters in the table view. 

For more information, see the "Add filters" section in the article [Manage the table view](../views/manage-the-table-view.md). -->


Du kan gruppera poster efter liknande information när du tillämpar en gruppering på en vy.

Tänk på följande när du arbetar med grupperingar i tidslinjevyn:

* Du kan använda grupperingar både i tabell- och tidslinjevyerna. Grupperingarna i tabellvyn är oberoende av grupperingarna i tidslinjevyn av samma posttyp.
* Du kan använda tre nivåer av gruppering i en maestro-vy. Posterna grupperas i den ordning som du väljer grupperingar.
* Du kan använda upp till fyra nivåer av gruppering när du använder API:t.

Så här lägger du till en gruppering:

1. Skapa en tidslinjevy enligt beskrivningen i artikeln [Hantera postvyer](../views/manage-record-views.md).
1. Klicka **Gruppering**.

   ![](assets/grouping-ui-timeline-view.png)

1. Klicka på ett av de föreslagna fälten eller klicka på **Välj ett annat fält** och söker efter ett annat fält och klickar sedan på det när det visas i listan.

   >[!TIP]
   >
   >Du kan inte markera länkade fält.

   Grupperingen används automatiskt på tidslinjen och posterna visas inuti grupperingsrutan. Antalet objekt i en gruppering visas på grupperingsraden.

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. (Valfritt) Upprepa stegen ovan om du vill lägga till upp till tre grupperingar.

   Antalet grupperingar som används visas till vänster om grupperingsikonen i det övre högra hörnet av verktygsfältet.

   ![](assets/grouping-applied-in-timeline-view.png)

1. (Valfritt) Klicka på **x** till höger om en gruppering för att ta bort grupperingen

   eller

   Klicka **Rensa alla** om du vill ta bort alla grupperingar.

1. Klicka utanför **Gruppera poster efter** för att stänga den.

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### Redigera inställningarna för tidslinjevyn {#edit-the-timeline-view-settings}

Uppdatera inställningarna för tidslinjevyn för att ange vilken information som ska visas i tidslinjeavsnittet i vyn.

1. Skapa en tidslinjevy enligt beskrivningen i artikeln [Hantera postvyer](../views/manage-record-views.md).
1. Klicka **Inställningar**.
1. Klicka **Datum och tid** i den vänstra panelen väljer du en **Startdatum** och **Slutdatum** som ska visas på tidslinjen. Du kan välja standarddatum för start och slut eller välja ett tillgängligt datumfält. De staplar som representerar posterna börjar på det datum som du anger som startdatum och slutar på det datum som motsvarar slutdatumet.

   >[!NOTE]
   >
   >    Poster som inte har några värden för start- eller slutdatum eller som har ett startdatum efter slutdatumet visas inte i tidslinjevyn.


1. Klicka **Postinformation** för att ange vilka fält du vill visa på poststrecken.

   Fältet Namn är markerat som standard.

1. Klicka **Lägg till fält** om du vill lägga till upp till fyra fält i postfälten.
1. Klicka inuti **Sökfält** och klicka på det fält som du vill lägga till.

   >[!TIP]
   >
   >   * Du måste skapa fälten innan du kan lägga till dem i postfälten.
   > 
   >   * Du måste ha minst ett fält markerat. **Namn** är markerat som standard.

   En förhandsvisning av hur staplarna kommer att se ut på tidslinjen visas till höger.

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. Klicka **Spara**.

   Posterna visas i tidslinjevyn med de specifikationer som du har valt.



---
title: Hantera tabellvyn
description: Du kan visa poster och deras fält i en tabellvy när du öppnar posttypssidan i Adobe Maestro.
hidefromtoc: true
hide: true
source-git-commit: 4a3cf7211eef2b161a29b74e8e9b2b12c21eaf4d
workflow-type: tm+mt
source-wordcount: '1494'
ht-degree: 0%

---


# Hantera tabellvyn

<!--
title: Manage the table view
description: You can display records in a table view when using Adobe Maestro. 
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>För närvarande ingår Adobe Maestro i ett slutet betaprogram som är öppet för ett begränsat antal kunder.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.
>
>Mer information finns i [Adobe Maestro - översikt](../maestro-overview.md).

Du kan visa poster och deras fält i en tabellvy när du öppnar posttypssidan i Adobe Maestro.

Mer information om Maestro-vyer och hur du hanterar dem finns i [Hantera postvyer](../views/manage-record-views.md).

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

## Hantera en tabellvy {#manage-a-table-view}

<!--insert screen shot of table view-->

När du skapar en tabellvy visas alla poster av den valda typen i en tabell. Varje rad är en unik post och varje kolumn är ett postfält. Alla fält och alla poster visas som standard.

Så här hanterar du en tabellvy:

1. Skapa en tabellvy enligt beskrivningen i artikeln [Hantera postvyer](../views/manage-record-views.md).

   ![](assets/table-view-example.png)

1. Uppdatera följande vyelement enligt beskrivningen i underavsnitten nedan:
   * [Kolumner (eller fält)](#add-columns-or-fields)
   * [Rader (eller poster)](#add-rows-or-records)
   * [Filter](#add-filters)
   * [Gruppering](#add-groupings)
   * [Sortera](#sort-information)


### Lägg till kolumner (eller fält) {#add-columns}

Kolumnrubrikerna i en Maestro-tabellvy visar fält som är kopplade till posterna i vyn. Samma fält som visas i tabellvyn visas även i detaljavsnittet för en Maestro-post. Mer information finns i [Redigera poster](../records/edit-records.md).

<!-- this is not available yet:You can display record fields (or columns) in both a table and a timeline view. However, the number of columns displayed in the table of the timeline view is limited and you cannot add columns in addition to those selected by default. -->

Att lägga till kolumner i en vy är detsamma som att lägga till fält i en posttyp.

Du kan lägga till upp till 500 fält (eller kolumner) i en tabellvy.

1. Gå till en posttypssida och välj en **Tabell** i listrutan.
1. Börja lägga till fält (eller kolumner) enligt beskrivningen i artikeln [Skapa fält](../architecture-and-fields/create-fields.md).

   Kolumnerna som du lägger till är synliga för alla användare som kommer åt posttypen och läggs till som nya fält på sidan Detaljer för posterna av den valda posttypen.

1. Gör något av följande om du vill ändra ordning på kolumnerna i tabellen:

   * Ta kolumnrubriken och dra den till önskad plats. Kolumnen som du flyttade snabbt visas med en blå bakgrund tills du gör andra justeringar i tabellen.

   * Klicka **Fält** i tabellens verktygsfält, dra och släpp fälten i önskad ordning och klicka sedan utanför **Fältens synlighet och ordningsruta** för att stänga den.

     ![](assets/fields-setting-table-view-toolbar-expanded.png)

   >[!TIP]
   >
   >* Fältet Namn är alltid det första fältet i tabellvyn.
   >
   >* Du kan inte flytta fältet Namn till en annan position.
   >
   >* Du kan inte dölja fältet Namn.
   >
   >* Fältet Namn är fryst och ingår inte i den vågräta rullningen.

1. Om du vill öka bredden på kolumnerna klickar du på och drar kolumnseparationslinjerna och släpper dem på önskad plats.

   >[!TIP]
   >
   >De ändringar du gör i kolumnbredden och kolumnordningen är permanenta och synliga för alla användare som har åtkomst till posttypen.

1. Om du vill dölja en kolumn håller du pekaren över kolumnrubriken, klickar på nedåtpilen och klickar sedan på **Dölj fält**

   eller

   Klicka **Fält** i tabellens verktygsfält och avaktiverar det växlingsknapp som är kopplat till de fält som du vill dölja.

   >[!TIP]
   >
   >Antalet dolda fält visas till vänster om ikonen Fält i verktygsfältet.


1. Från **Fält** aktiverar du den växlingsknapp som är kopplad till de fält som du vill visa i tabellens kolumner. Alla fält visas som standard.

### Lägga till rader (eller poster) {#add-rows}

Raderna i en Maestro-tabellvy visar enskilda poster av den valda posttypen.

Du kan ha upp till 10 000 poster (eller rader) för en posttyp i Maestro.

Att lägga till rader i en Maestro-tabellvy är detsamma som att skapa poster i en tabell.

Mer information finns i [Skapa poster](../records/create-records.md).

<!-- this is not possible right now:

1. To reorder the rows, click the row header, drag and drop it in the desired location. 

    The changes you make to the row order are permanent and visible to all users who access the record type
-->

### Lägg till filter {#add-filters}

<!-- this section links from the timeline view; consider splitting them if they become different-->

Med filter kan du minska mängden information som visas på skärmen.

Tänk på följande när du arbetar med filter i tabellvyn:
<!-- this list is almost identical to the one for the table view - update both-->

* De filter som du skapar för tabellvyn fungerar oberoende av filtren i tidslinjevyn när de används för samma posttyp.

* Filtren är unika för den vy du väljer. Två tabellvyer av samma posttyp kan ha olika filter. Två användare som tittar på samma tabellvy ser samma filter som används för närvarande.

* Du kan inte namnge de filter som du skapar och använder i en tabellvy.

* När du tar bort filter tas de bort från alla som använder samma posttyp som du och använder samma vy som du använder.

* Att lägga till filter i tabellvyn är detsamma som att lägga till filter i tidslinjevyn.

Så här lägger du till ett filter i en tabellvy:

1. Skapa en tabellvy för en posttypsida, enligt beskrivningen i artikeln [Hantera postvyer](../views/manage-record-views.md).
1. Markera en tabellvy och klicka sedan på **Filter** i tabellens övre högra hörn.
1. Klicka **Lägg till villkor** och lägga till följande information:

   * Markera ett fält som du vill filtrera efter <!-- the tip below might change-->

   * Välj ett alternativ (eller en filtermodifierare) för att definiera vilken typ av villkor fältet måste uppfylla

     Tabellen nedan visar tillgängliga modifierare för varje typ av fält.

     >[!TIP]
     >
     > Du kan inte markera länkade fält. Mer information finns i [Skapa fält](../architecture-and-fields/create-fields.md).

     <table>
        <thead>
        <tr>
            <th><b>Fälttyp</b></th>
            <th><b>Modifierare</b></th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>Enkelrad, stycke </td>
            <td><p>Innehåller</p>
            <p>Innehåller inte</p>
            <p>Är</p>
            <p>Är inte</p>
            <p>Är tom</p>
            <p>Är inte tom</p></td>
        </tr>
        <tr><td>Enkelval</td>
            <td><p>Är</p>
            <p>Är inte</p>
            <p>Är något av</p>
            <p>Är inget av</p>
            <p>Är tom</p>
            <p>Är inte tom</p></td>
        </tr>
        <tr>
            <td>Flera val</td>
            <td><p>Har någon av</p>
            <p>Har alla</p>
            <p>Är exakt</p>
            <p>Har ingen av</p>
            <p>Är tom</p>
            <p>Är inte tom</p></td>
        </tr>
        <tr>
            <td>Numeriskt, procenttal, valuta</td>
            <td><p>=</p>
            <p>≠</p>
            <p> &lt; </p>
            <p>&gt;</p>
            <p>≤</p>
            <p>≥</p>
            <p>Är tom</p>
            <p>Är inte tom</p></td>
        </tr>
        <tr>
            <td>Datum</td>
            <td><p>Är</p>
            <p>Är inte</p>
            <p>Är efter</p>
            <p>Är före</p>
            <p>Är mellan</p><p>Är inte mellan</p>
            <p>Är tom</p><p>Är inte tom</p></td>
        </tr>

     <tr>
            <td>Kryssruta</td>
            <td><p>Är</p>
        </tr>
        </tbody>
        </table>

   * Välj ett värde för det markerade fältet.

   ![](assets/filter-ui-table-view.png)

   Det finns ingen gräns för hur många filtreringsvillkor du kan lägga till.

1. (Valfritt) Klicka på **Lägg till villkor** om du vill lägga till ytterligare ett filteralternativ och upprepa stegen ovan. Antalet filter som används visas till vänster om filterikonen.
1. Klicka på följande operatorer för att ange hur filtervillkoren ska kopplas och användas:

   * **Och**: Alla angivna villkor måste vara uppfyllda.
   * **eller**: Alla angivna villkor måste vara uppfyllda. Det här är standardalternativet.

   Postlistan filtreras automatiskt.  <!--at this time, you can't name and save the filter - but will this change?!-->
   <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->

1. (Valfritt) Klicka på **Filter** och klickar sedan på **x** för att ta bort ett filter. <!--right now you cannot "clear all" for filters, but this might come later-->

<!-- this is not available yet

### Add groupings {#add-groupings}

*******************this section might link in the future from the timeline view; right now it's only documented there; also, check the steps below because this was not released to the table when they were written*****************

You can group records by similar information when applying  a grouping to a view.

You can apply groupings both in the table and timeline views. The groupings of the table view are independent from those in the timeline view of the same record type. 

Consider the following:

* You can apply 3 levels of grouping in a Maestro view. The records are grouped in the order of groupings that you select. (***************check on this; this might be true for timeline, but not for table??? One dev said in a demo that there are unlimited groupings in a table - check *********************)
* You can apply up to 4 levels of grouping when using the API. 

To add a grouping:

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. (Conditional) To apply a grouping in the table view, do the following:
    
    1. ***************start adding steps for building a grouping - see if there it a global setting or just per column; also, see if the steps are different for a table vs a timeline view?!**********************
1. (Conditional) To apply a grouping in the timeline view, do the following:

    1. Go to a timeline view, then click **Group**. ************************did they rename this to "Grouping"?!****************************
        ******************insert screen shot***********
    1. Click one of the 5 suggested fields, or click **Choose a different field** to display all fields, then click one when it displays in the list. 
    
        >[!TIP]
        >
        > You cannot select linked fields. For information, see [Create fields](../architecture-and-fields/create-fields.md).  
    The grouping is applied automatically to the timeline and records display inside the grouping box.    <********************ensure this is correct functionality here*************
    
    1. (Optional) Click **Add grouping** to add up to 3 groupings. 

        The number of groupings applied displays to the left of the Grouping icon in the upper-right corner of the toolbar. **********ensure this says "grouping" and not "group"*****************
    
    1. (Optional) Click **Clear all** to remove all groupings.  

-->

### Lägg till en sortering {#sort-information}

Genom att använda en sortering kan du ordna information i en viss ordning.

Du kan sortera följande information:

* Alla poster i en tabellvy. <!--or timeline view. ***********verify this is the case for the timeline view*********************-->
  <!--* All groupings. - this is not available yet-->

Tänk på följande när du sorterar poster i tabellvyn:

<!-- if this is available for the timeline view, update both when you update one-->

* Sorteringen är unik för den vy du väljer. Två tabellvyer av samma posttyp kan ha olika sorteringsvillkor. Två användare som tittar på samma tabellvy ser samma sortering som för närvarande används.

* Du kan inte namnge sorteringarna som du skapar och använder i en tabellvy.

* Den sortering du skapar bevaras när du navigerar bort.

* Du kan sortera efter så många fält som du ser i tabellvyn för en posttyp.

* När du tar bort sorteringsvillkor tas de bort från alla som använder samma posttyp som du och samma vy som du använder.

Sortera <!--ungrouped (add this when sorting for groupings will be available--> poster, gör följande:

1. Skapa en tabellvy enligt beskrivningen i artikeln [Hantera postvyer](../views/manage-record-views.md).
1. Klicka på **Sortera** icon ![](assets/sort-icon.png) i tabellens övre högra hörn

   eller

   Håll markören över namnet på en kolumn i tabellvyn, klicka på nedåtpilen till höger om kolumnrubriknamnet och klicka sedan på **Sortera efter det här fältet**. Fältet läggs till som en sorteringsmarkering i sorteringsikonen i tabellvyns övre högra hörn.
1. I **Sortera poster efter** klickar du på ett av de föreslagna fälten eller klickar på **Välj ett annat fält** och söker efter ett annat fält och klickar sedan på det när det visas i listan.

   Sorteringen tillämpas automatiskt på tabellvyn och posterna visas sorterade efter de valda villkoren.

   <!-- add a step that you can rearrange the sorting fields here, when this will be possible-->

1. (Valfritt) Upprepa stegen ovan om du vill sortera efter ytterligare fält.

   Antalet fält som du sorterar efter visas till vänster om sorteringsikonen i det övre högra hörnet av verktygsfältet. Du kan bara välja fält som visas i kolumnerna i tabellvyn.

   >[!TIP]
   >
   > Du kan inte markera länkade fält. Mer information finns i [Skapa fält](../architecture-and-fields/create-fields.md).

1. (Valfritt) I dialogrutan **Sortera poster efter** klickar du på **x** till höger om ett sorteringsfält för att ta bort sorteringen

   eller

   Klicka **Rensa alla** om du vill ta bort alla fält från sorteringen.

1. Klicka utanför **Sortera poster efter** för att stänga den.

   Den information som visas i tabellen sorteras efter de valda villkoren.

   I de fält som är markerade för sorteringen visas en sorteringsikon följt av ett tal som anger i vilken ordning sorteringen används.

   ![](assets/sorting-in-table-view.png)


<!-- this is not available yet: 

To sort grouped records: 

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. ************************* add steps here for sorting grouped records****************

-->
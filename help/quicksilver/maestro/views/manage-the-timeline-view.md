---
title: Hantera tidslinjevyn
description: Du kan visa poster i en tidslinjevy när du öppnar posttypssidan i Adobe Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: f348af7f-5bb9-4d88-9bcb-3bef7e8892dd
source-git-commit: ef313bf912c65b9b316bd7403235ccf6f05a0ac6
workflow-type: tm+mt
source-wordcount: '1658'
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

{{maestro-important-intro}}

Du kan visa poster i en tidslinjevy när du öppnar posttypssidan i Adobe Maestro.

Mer information om vyerna i maestro finns i [Hantera postvyer i Adobe Maestro](../views/manage-record-views.md).

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
   <td role="rowheader">Åtkomstnivåkonfiguration</td>
   <td> <p>Det finns inga åtkomstnivåkontroller för Maestro </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Hantera behörigheter till vyn</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Layoutmall</td>
   <td> <p>Systemadministratören måste lägga till Maestro-området i layoutmallen. Mer information finns i <a href="../access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>
 </tbody>
</table>


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

Så här hanterar du en tidslinjevy:

1. Gå till den posttypssida som du vill visa tidslinjen för.
1. Skapa en tidslinjevy enligt beskrivningen i artikeln [Hantera postvyer](../views/manage-record-views.md).

   ![](assets/timeline-view-example.png)

   Posterna som är associerade med den posttyp du valde visas som staplar på en tidslinje och sorteras som standard i kronologisk ordning efter startdatum.

   >[!TIP]
   >
   >    Sorteringen av posterna på tidslinjen är inte synlig i den komprimerade vyn.


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

1. Gör följande för att snabbt hitta poster som matchar ett nyckelord:

   1. Klicka på **Sök** icon ![](assets/search-icon.png) och börja skriva ett nyckelord som är associerat med valfritt fält i en post som visas på skärmen. Antalet korrekta matchningar visas bredvid sökobjektet och posten med rätt matchning markeras.

      ![](assets/search-box-and-results-timeline-view.png)

      Du kan använda vilket ord eller specialtecken som helst som visas på skärmen.

      Du kan inte använda nyckelord som är associerade med fält som inte visas i tidslinjevyn.

   1. Tryck på Retur på tangentbordet för att gå till nästa sökbara fält.
   1. (Valfritt) Om det finns mer än en matchning klickar du på upp- och nedpilarna till höger om söknyckelordet för att hitta alla matchningar i tabellen.
   1. Klicka på **x** -ikonen i sökrutan för att rensa sökordet.

1. Uppdatera följande vyelement enligt beskrivningen i underavsnitten nedan:
   * [Filter](#add-filters)
   * [Gruppering](#add-grouping)
   * [Inställningar](#edit-the-timeline-view-settings)
     <!--* [Sort](#add-sort) not sure if this is present in timeline views?!; also check the anchor and make sure it's correct-->

### Lägg till filter

Du kan minska mängden information som visas på skärmen genom att använda filter.

Tänk på följande när du arbetar med filter i tidslinjevyn:

<!-- this list is almost identical to the one for the table view - update both-->

* De filter som du skapar för tidslinjevyn fungerar oberoende av filtren i tabellvyn när de används för samma posttyp.

* Filtren är unika för den vy du väljer. Två tidslinjevyer av samma posttyp kan ha olika filter. Två användare som tittar på samma tidslinjevy ser samma filter som används för närvarande.

* Du kan inte namnge de filter som du skapar för en tidslinjevy.

* När du tar bort filter tas de bort från alla som använder samma posttyp som du och som visar samma vy som du.

* Att lägga till filter i tidslinjevyn är detsamma som att lägga till filter i tabellvyn.

  Mer information finns i avsnittet&quot;Lägg till filter&quot; i artikeln [Hantera tabellvyn](../views/manage-the-table-view.md).

### Lägg till gruppering

<!-- groupings are almost identical between this view and table  but they display a little differently, so I kept the steps for both; update in both places if they make changes to groupings-->

Du kan gruppera poster efter liknande information när du tillämpar en gruppering på en vy.

Att lägga till grupperingar i tidslinjevyn påminner om att lägga till grupperingar i tabellvyn.

Tänk på följande när du arbetar med grupperingar i tidslinjevyn:

* Du kan använda grupperingar både i tabell- och tidslinjevyerna. Grupperingarna i tabellvyn är oberoende av grupperingarna i tidslinjevyn av samma posttyp.
* Du kan använda tre nivåer av gruppering i en maestro-vy. Posterna grupperas i den ordning som du väljer grupperingar.
* Du kan använda upp till fyra nivåer av gruppering när du använder API:t.
* Grupperingarna är unika för den vy du väljer. Två tidslinjevyer av samma posttyp kan ha olika grupperingar. Två användare som tittar på samma tidslinjevy ser samma gruppering som används för närvarande.
* Du kan inte namnge grupperingarna som du skapar för en tidslinjevy.
* Om du tar bort grupperingar tas de bort från alla som har åtkomst till samma posttyp som du och som visar samma vy som du.

Så här lägger du till en gruppering i tidslinjevyn:

1. Skapa en tidslinjevy för en posttyp, enligt beskrivningen i artikeln [Hantera postvyer](../views/manage-record-views.md).
1. Klicka **Gruppering** i det övre högra hörnet av tidslinjevyn.

   ![](assets/grouping-ui-timeline-view-with-linked-fields.png)

1. Klicka på ett av de föreslagna fälten eller klicka på **Välj ett annat fält** söker du efter ett annat fält och klickar sedan på det när det visas i listan.

   Grupperingen används automatiskt på tidslinjen och posterna visas inuti grupperingsrutan.

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. (Valfritt) Upprepa stegen ovan om du vill lägga till upp till tre grupperingar.

   Antalet fält som har valts för grupperingen visas bredvid grupperingsikonen.

   ![](assets/grouping-applied-in-timeline-view.png)

1. (Valfritt) I **Gruppera poster efter** klickar du på **x** till höger om ett fält som är markerat för grupperingen för att ta bort grupperingen

   eller

   Klicka **Rensa alla** om du vill ta bort alla fält.

1. Klicka utanför **Gruppera poster efter** för att stänga den.
1. (Valfritt) Klicka på **Inställningar** sedan **Färg** till färgkodsgrupperingar. Mer information finns i [Redigera inställningarna för tidslinjevyn](#edit-the-timeline-view-settings) i den här artikeln.

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### Redigera inställningarna för tidslinjevyn {#edit-the-timeline-view-settings}

Uppdatera inställningarna för tidslinjevyn för att ange vad och hur informationen ska visas i tidslinjeavsnittet i vyn.

1. Skapa en tidslinjevy för en posttyp, enligt beskrivningen i artikeln [Hantera postvyer](../views/manage-record-views.md).
1. Klicka **Inställningar**.
1. Klicka **Datum och tid** i den vänstra panelen väljer du en **Startdatum** och **Slutdatum** som ska visas på tidslinjen. Du kan välja standarddatum för start och slut eller välja ett tillgängligt datumfält. De staplar som representerar posterna börjar på det datum som du anger som startdatum och slutar på det datum som motsvarar slutdatumet.

   >[!NOTE]
   >
   >Poster som inte har några värden för start- eller slutdatum eller som har ett startdatum efter slutdatumet visas inte i tidslinjevyn.

1. Klicka **Stapelformat** i den vänstra panelen för att ange vilka fält som ska visas i postfälten.

   Fältet Namn är markerat som standard. <!--adjust this when the primary field is released??-->

1. (Valfritt och villkorligt) Om du har lagt till miniatyrbilder i poster, markerar du alternativet Miniatyrbild för att visa den bild som är associerad med posterna i deras postfält.

   >[!NOTE]
   >
   >    Du måste först lägga till miniatyrbilder i tabellvyn innan du kan visa dem i tidslinjevyn. Mer information finns i [Lägga till miniatyrbilder i poster](/help/quicksilver/maestro/records/add-thumbnails-to-records.md).

1. Klicka **Lägg till fält** om du vill lägga till upp till fyra fält i postfälten.
1. Klicka inuti **Sökfält** och klicka på det fält som du vill lägga till.

   >[!TIP]
   >
   >   * Du måste skapa fälten innan du kan lägga till dem i postfälten.
   > 
   >   * Du måste ha minst ett fält markerat. **Namn** är markerat som standard.

   En förhandsvisning av hur staplarna kommer att se ut på tidslinjen visas till höger.

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. Klicka **Färg** i den vänstra panelen, om du vill anpassa färgerna för posterna och grupperingarna på tidslinjen.

   ![](assets/color-tab-timeline-view.png)

1. (Villkorligt och valfritt) Om du har lagt till en gruppering i tidslinjevyn väljer du bland följande alternativ för att ange en färg för grupperingen i **Ange grupperingsfärg** avsnitt:

   * **Standard (grått)**: Färgen på grupperingarna är inställd på grått. Det här är standardinställningen.
   * **Fältvärden**: Färgen på grupperingarna matchar färgen på fältet som du grupperar efter.
Du kan bara matcha färgen på grupperingarna mot fält med färgkodade alternativ.

   Flervalsfält eller envalsfält kan t.ex. ha färgkodade alternativ.

   Om du grupperar efter fält utan färgkodade alternativ förblir grupperingsfärgen grå.

   >[!TIP]
   >
   >Om du inte har lagt till grupperingar i tidslinjevyn visas inte det här avsnittet.

1. I **Ange postfärg** väljer du bland följande alternativ för att ange en färg för posterna:

   * **Posttyp**: Färgen på posterna matchar färgen på den posttyp du valde. Det här är standardalternativet.
   * **Fältvärden**: Färgen på posterna matchar färgen i ett fält som du anger. Fortsätt med steg 10. <!--ensure this stays accurate-->
   * **Gruppering**: Färgen på posterna matchar färgen som du angav för grupperingarna. Det här alternativet är nedtonat när du inte har använt några grupperingar på tidslinjevyn.
   * **Ingen**: Poster visas i ett vitt fält.

1. (Villkorligt) Om du har valt **Fältvärden** för postfärgerna väljer du ett fält på menyn **Matcha postfärgen till** listruta.

   ![](assets/field-selector-drop-down-menu-timeline-view.png)

   Endast fält med färgkodade alternativ visas i listrutan.

   Flervalsfält eller envalsfält kan t.ex. ha färgkodade alternativ.

   Om du inte har något fält med färgkodade alternativ för den valda posttypen är det här alternativet nedtonat.

1. Klicka **Spara**.

   Posterna visas i tidslinjevyn med de specifikationer som du har valt.

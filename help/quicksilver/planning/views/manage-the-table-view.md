---
title: Hantera tabellvyn
description: Du kan visa poster och deras fält i en tabellvy när du öppnar posttypssidan i Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 0dd723b5-d674-4626-8fc2-7da41f3b7f35
source-git-commit: 7882b67578cd5b8792ce582ebab118c8993c9214
workflow-type: tm+mt
source-wordcount: '2543'
ht-degree: 0%

---

# Hantera tabellvyn

<!--
title: Manage the table view
description: You can display records in a table view when using Adobe Workfront Planning. 
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

Du kan visa poster och deras fält i en tabellvy när du öppnar posttypssidan i Adobe Workfront Planning.

Mer information om postvyer och hur du hanterar dem finns i [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).

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
<p>Din organisation måste vara registrerad på Workfront Planning i ett tidigt skede </p>
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
   <p>Systemadministratörer har bara åtkomst till de vyer de har skapat eller som delas med dem. </p>
  </td>
  </tr>

<tr>
   <td role="rowheader">Åtkomstnivåkonfiguration</td>
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workforme-planering</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Hantera behörigheter till vyn</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Layoutmall</td>
   <td> <p>Systemadministratören måste lägga till planeringsområdet i layoutmallen. Mer information finns i <a href="/help/quicksilver/planning/access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## Hantera en tabellvy {#manage-a-table-view}

<!--insert screen shot of table view-->

När du skapar en tabellvy visas alla poster av den valda typen i en tabell. Varje rad är en unik post och varje kolumn är ett postfält. Alla fält och alla poster visas som standard.

Så här hanterar du en tabellvy:

1. Skapa en tabellvy enligt beskrivningen i artikeln [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).

   ![](assets/table-view-example.png)

1. (Valfritt) Klicka på **Radhöjd** väljer du sedan bland följande alternativ för att ändra höjden på tabellraderna:
   * Kort
   * Medel
   * Hög

1. Uppdatera följande vyelement enligt beskrivningen i underavsnitten nedan:
   * [Kolumner (eller fält)](#add-columns-or-fields)
   * [Rader (eller poster)](#add-rows-or-records)
   * [Filter](#add-filters)
   * [Gruppering](#add-groupings)
   * [Sortera](#add-a-sort)


### Lägg till kolumner (eller fält) {#add-columns}

Kolumnrubrikerna i en tabellvy visar fält som är kopplade till posterna i vyn. Samma fält som visas i tabellvyn visas även i avsnittet Detaljer för en post. Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

<!--this is not available yet:You can display record fields (or columns) in both a table and a timeline view. However, the number of columns displayed in the table of the timeline view is limited and you cannot add columns in addition to those selected by default.-->

Att lägga till kolumner i en vy är detsamma som att lägga till fält i en posttyp.

Du kan lägga till upp till 500 fält (eller kolumner) i en tabellvy.

1. Gå till en posttypssida och välj en **Tabell** i listrutan.

   <!-- replace above with this when view redesign: Go to a record type page and click a table view tab, or click **+ View **to add a new view, then choose **Table**. -->
1. Börja lägga till fält (eller kolumner) enligt beskrivningen i artikeln [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

   Kolumnerna som du lägger till är synliga för alla användare som kommer åt posttypen och läggs till som nya fält på postens sida.

1. Gör något av följande om du vill ändra ordning på kolumnerna i tabellen:

   * Ta kolumnrubriken och dra den till önskad plats. Kolumnen som du flyttade snabbt visas med en blå bakgrund tills du gör andra justeringar i tabellen.

   * Klicka **Fält** i tabellens verktygsfält, dra och släpp fälten i önskad ordning och klicka sedan utanför **Fältens synlighet och ordning** för att stänga den.

     ![](assets/fields-setting-table-view-toolbar-expanded.png)


     >[!TIP]
     >
     >* Fältet Namn är som standard alltid det första fältet i tabellvyn. Detta betraktas som ett primärt fält.
     >
     >* Du kan inte flytta fältet Namn till en annan plats om du inte anger ett annat fält som primärt fält. Mer information finns i steg 4. <!--accurate?-->
     >
     >

   * Ersätt fältet i den första kolumnen med ett annat fält genom att ändra det primära fältet. Mer information finns i steg 4. <!--accurate?-->

1. (Valfritt) Håll markören över ett fältnamn i kolumnrubriken för ett fält som inte visas i den första kolumnen i tabellen, klicka på nedåtpilen till höger om fältnamnet och klicka sedan på **Ange som primärt fält**.

   ![](assets/set-as-primary-field-option-table-view.png)

1. Klicka **Ange fält** för att bekräfta.

   Fältet blir ett primärt fält, vilket betyder att det visas som den första kolumnen i tabellvyn. Det föregående primära fältet flyttas till den andra kolumnen.

   Primära fält blir postens titel och visas i rubrikområdet på postens sida, och överallt där posterna visas. Postens titel visas till exempel i anslutna fält och i alla vyer. Mer information om primära fält finns i [Översikt över primärt fält](/help/quicksilver/planning/fields/primary-field-overview.md).

1. Klicka och dra kolumnseparationslinjerna och släpp dem på önskad plats för att öka kolumnbredden.

   >[!TIP]
   >
   >De ändringar du gör i kolumnbredden och kolumnordningen är permanenta och synliga för alla användare som har åtkomst till posttypen.

1. Håll pekaren över kolumnrubriken, klicka på nedåtpilen och klicka sedan på **Dölj fält**

   eller

   Klicka **Fält** i tabellens verktygsfält och avaktiverar alternativet som är kopplat till de fält (eller kolumner) som du vill dölja. The **Fältens synlighet och ordning** visas.

   >[!TIP]
   >
   >Antalet dolda fält visas till vänster om ikonen Fält i verktygsfältet.


1. Klicka på **Fält** och aktivera den växlingsknapp som är kopplad till de fält som du vill visa i tabellens kolumner. Alla fält visas som standard.

1. Gör följande för att snabbt hitta poster som matchar ett nyckelord:

   1. Klicka på **Sök** icon ![](assets/search-icon.png) och börja skriva ett nyckelord som är associerat med valfritt fält i en post som visas på skärmen. Antalet korrekta matchningar visas bredvid sökobjektet och fältet med rätt matchning markeras.

      ![](assets/search-box-with-results-blue-outline-table-view.png)

      Du kan använda vilket ord eller specialtecken som helst som visas på skärmen.

      Du kan inte använda nyckelord som är kopplade till fält som är dolda i tabellvyn.

   1. Tryck **Retur** på tangentbordet för att gå till nästa sökbara fält.

   1. (Valfritt) Om det finns mer än en matchning klickar du på upp- och nedpilarna till höger om söknyckelordet för att hitta alla matchningar i tabellen.

   1. Klicka på **x** -ikonen i sökrutan för att rensa sökordet.


### Lägga till rader (eller poster) {#add-rows}

Raderna i en tabellvy visar enskilda poster av den valda posttypen.

Du kan ha upp till 50 000 poster (eller rader) för posttypen S.

1. Gå till en posttypssida och välj en **Tabell** i listrutan.

<!-- replace above with this when view redesign: Go to a record type page and click a table view tab, or click **+ View **to add a new view, then choose **Table**. -->
1. Börja lägga till poster (eller rader) enligt beskrivningen i artikeln [Skapa poster](/help/quicksilver/planning/records/create-records.md).

   Posterna som du lägger till i tabellvyn sparas omedelbart och visas för alla användare som har behörigheten Visa eller högre på arbetsytan.

1. (Valfritt) Lägg till en miniatyrbild för varje post och klicka på **Fält** i tabellens övre högra hörn och välj sedan alternativet för **Miniatyrbild** för att visa det till vänster om det primära fältet. Det är som standard avmarkerat.

   Mer information finns i [Lägga till en miniatyrbild i en post](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

1. (Valfritt) Markera en eller flera poster i en rad och dra och släpp sedan **handtag** icon ![](assets/handle-icon.png) till vänster om posten för att ändra ordning på raderna.

   >[!NOTE]
   >
   >Du kan inte ändra ordning på rader om du använder minst en sortering i tabellvyn.

   <!-- this is not possible right now:

    1. To reorder the rows, click the row header, drag and drop it in the desired location. 

        The changes you make to the row order are permanent and visible to all users who access the record type
    -->

<!-- this section below links from the timeline view; consider splitting them if they become different-->

### Lägg till filter {#add-filters}

Med filter kan du minska mängden information som visas på skärmen.

Tänk på följande när du arbetar med filter i tabellvyn:
<!-- this list is almost identical to the one for the table view - update both-->

* De filter som du skapar för tabellvyn fungerar oberoende av filtren i tidslinjevyn när de används för samma posttyp.

* Filtren är unika för den vy du väljer. Två tabellvyer av samma posttyp kan ha olika filter. Två användare som tittar på samma tabellvy ser samma filter som används för närvarande.

* Du kan inte namnge de filter som du skapar och använder i en tabellvy.

* När du tar bort filter tas de bort från alla som använder samma posttyp som du och använder samma vy som du använder.

* Att lägga till filter i tabellvyn är detsamma som att lägga till filter i tidslinjevyn.

* Du kan filtrera efter anslutna postfält eller sökfält, men inte efter de fält som tillåter länkning till flera poster.

* Du kan referera till ett fält som ligger upp till fyra nivåer från den aktuella posttypen. Om du till exempel skapar ett filter för en aktivitetsposttyp, och aktiviteten är ansluten till produktposttypen som är kopplad till Campaign-posttypen som är kopplad till ett Workfront-projekt, kan du referera till projektets budget i filtret som du skapar för aktivitetsposttypen.

Så här lägger du till ett filter i en tabellvy:

1. Skapa en tabellvy för en posttypsida, enligt beskrivningen i artikeln [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).
1. Markera en tabellvy och klicka sedan på **Filter** i tabellens övre högra hörn.
1. Klicka **Lägg till villkor** och lägga till följande information:

   * **Markera ett fält** som du vill filtrera efter <!-- the tip below might change-->

   * **Välj ett alternativ** (eller en filtermodifierare) för att definiera vilket villkor fältet måste uppfylla

     Tabellen nedan visar tillgängliga modifierare för varje typ av fält.

     <table>
        <thead>
        <tr>
            <th><b>Fälttyp</b></th>
            <th><b>Modifierare</b></th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>Enkelrad, Stycke, Formel </td>
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
            <td>Flera val, personer</td>
            <td><p>Har någon av</p>
            <p>Har alla</p>
            <p>Är exakt</p>
            <p>Har ingen av</p>
            <p>Är tom</p>
            <p>Är inte tom</p></td>
        </tr>
        <tr>
            <td>Antal, Procentandel, Valuta</td>
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

### Lägg till grupperingar {#add-groupings}

<!--this section exists in the timeline view too, but the display is slightly different, so I kept both steps; consider updating both sections if any updates to groupings are introduced-->

Du kan gruppera poster efter liknande information när du tillämpar en gruppering på en vy.

Att lägga till grupperingar i tabellvyn påminner om att lägga till grupperingar i tidslinjevyn.

Tänk på följande:

* Du kan använda grupperingar både i tabell- och tidslinjevyerna. Grupperingarna i tabellvyn är oberoende av grupperingarna i tidslinjevyn av samma posttyp.
* Du kan använda tre nivåer av gruppering i en vy. Posterna grupperas i den ordning som du väljer grupperingar.
&lt;!—* Du kan använda upp till fyra nivåer av gruppering när du använder API:t. —check on this for now—>
* Grupperingarna är unika för den vy du väljer. Två tabellvyer av samma posttyp kan ha olika grupperingar. Två användare som tittar på samma tabellvy ser samma gruppering som används för närvarande.
* Du kan inte namnge grupperingarna som du skapar för en tabellvy.
* Om du tar bort grupperingar tas de bort från alla som har åtkomst till samma posttyp som du och som visar samma vy som du.
* Du kan redigera poster som listas under en gruppering.
* Du kan gruppera efter kopplade postfält eller sökfält, men inte för de fält som tillåter länkning till flera poster.
* Du kan referera till ett fält som ligger upp till fyra nivåer från den aktuella posttypen. Om du till exempel skapar en gruppering för en aktivitetsposttyp, och aktiviteten är ansluten till produktposttypen som är kopplad till Campaign-posttypen som är kopplad till ett Workfront-projekt, kan du referera till projektets status i den gruppering du skapar för aktivitetsposttypen.
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

Så här lägger du till en gruppering:

1. Skapa en tidslinjevy för en posttyp, enligt beskrivningen i artikeln [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).
1. Klicka **Gruppering** i tabellvyns övre högra hörn.

   ![](assets/grouping-ui-table-view-with-linked-fields.png)

1. Klicka på ett av de föreslagna fälten eller klicka på **Välj ett annat fält** söker du efter ett annat fält och klickar sedan på det när det visas i listan.

   Grupperingen tillämpas automatiskt på tabellen och posterna visas under grupperingsseparationslinjen.

1. (Valfritt) Klicka på **Lägg till villkor** och upprepa stegen ovan för att lägga till upp till tre grupperingar.

   Antalet fält som har valts för grupperingen visas bredvid grupperingsikonen.

   ![](assets/grouping-applied-in-table-view.png)

1. (Valfritt) I **Gruppera poster efter** klickar du på **x** till höger om ett fält som är markerat för grupperingen för att ta bort grupperingen

   eller

   Klicka **Rensa alla** om du vill ta bort alla fält.

1. Klicka utanför **Gruppera poster efter** för att stänga den.
1. (Valfritt) Klicka på **+ Ny post** i slutet av en gruppering för att lägga till nya poster, och sedan uppdatera sidan för att lägga till den nya posten i rätt gruppering. <!--this might need to be changed when they add the Refresh button on the toolbar of the table view-->

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

* Länkade fält kan bara sorteras om de tillåter enskilda värden, eller om de tillåter flervalsvärden när sammanfattningsalternativet är markerat (summa, medel, max, min).

* När du tar bort sorteringsvillkor tas de bort från alla som använder samma posttyp som du och samma vy som du använder.

* Du kan sortera efter kopplade postfält eller sökfält, men inte efter de fält som tillåter länkning till flera poster.

* Du kan referera till ett fält som ligger upp till fyra nivåer från den aktuella posttypen. Om du till exempel skapar en sortering för en aktivitetsposttyp, och aktiviteten är ansluten till produktposttypen som är kopplad till Campaign-posttypen som är kopplad till ett Workfront-projekt, kan du referera till projektets status i den sortering du skapar för aktivitetsposttypen.

Sortera <!--ungrouped (add this when sorting for groupings will be available--> poster, gör följande:

1. Skapa en tabellvy enligt beskrivningen i artikeln [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).
1. Klicka på **Sortera** icon ![](assets/sort-icon.png) i tabellens övre högra hörn

   eller

   Håll markören över namnet på en kolumn i tabellvyn, klicka på nedåtpilen till höger om kolumnrubriknamnet och klicka sedan på **Sortera efter det här fältet**. Fältet läggs till som en sorteringsmarkering i sorteringsikonen i tabellvyns övre högra hörn.

1. (Villkorligt) I dialogrutan **Sortera poster efter** klickar du på ett av de föreslagna fälten eller klickar på **Välj ett annat fält** och söker efter ett annat fält och klickar sedan på det när det visas i listan.

   Sorteringen tillämpas automatiskt på tabellvyn och posterna visas sorterade efter de valda villkoren.

   <!-- add a step that you can rearrange the sorting fields here, when this will be possible-->

1. (Valfritt) Klicka på **Lägg till villkor** och upprepa stegen ovan för att sortera efter ytterligare fält.

   Antalet fält som du sorterar efter visas till vänster om sorteringsikonen i det övre högra hörnet av verktygsfältet. Du kan bara välja fält som visas i kolumnerna i tabellvyn.

1. (Valfritt) I dialogrutan **Sortera poster efter** klickar du på **x** till höger om ett sorteringsfält för att ta bort sorteringen

   eller

   Klicka **Rensa alla** om du vill ta bort alla fält från sorteringen.

1. Klicka utanför **Sortera poster efter** för att stänga den.

   ![](assets/sorting-in-table-view.png)

   Den information som visas i tabellen sorteras efter de valda villkoren.

   I de fält som är markerade för sorteringen visas en sorteringsikon följt av ett tal som anger i vilken ordning sorteringen används.

<!-- this is not available yet: 

To sort grouped records: 

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. ************************* add steps here for sorting grouped records****************

-->

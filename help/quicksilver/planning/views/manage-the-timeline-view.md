---
title: Hantera tidslinjevyn
description: Få åtkomst till och redigera poster i en tidslinjevy på posttypssidan för Adobe Workfront Planning. I den här artikeln beskrivs hur du skapar en tidslinjevy och redigerar eller tar bort en befintlig. Anpassa tidslinjen med filter, grupperingar och inställningar. Använd funktionen Uppdelning för att visa kopplade poster.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: f348af7f-5bb9-4d88-9bcb-3bef7e8892dd
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '2874'
ht-degree: 0%

---

# Hantera tidslinjevyn

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Du kan visa poster i en tidslinjevy när du öppnar posttypssidan i Adobe Workfront Planning.

Mer information om postvyer finns i [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven.

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
   <p> Produkter</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-plan*</p></td> 
   <td> 
<p>Något av följande Workfront-planer:</p> 
<ul><li>Välj</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning är inte tillgängligt för tidigare Workfront-planer</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning-paket*</p></td> 
   <td> 
<p>Alla </p> 
<p>Kontakta din kontoansvarige på Workfront om du vill ha mer information om vad som ingår i respektive Workfront Planning-plan. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront</p></td> 
   <td> 
<p>Din organisations instans av Workfront måste integreras med Adobe Unified Experience för att få tillgång till alla funktioner i Workfront Planning.</p> 
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning är inte tillgängligt för tidigare Workfront-licenser</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>   <p>Hantera behörigheter till en vy</p>  
   <p>Visa behörigheter till en vy för att tillfälligt ändra visningsinställningarna</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutmall</p></td> 
   <td> <p>I produktionsmiljön måste alla användare, inklusive systemadministratörer, tilldelas en layoutmall som innehåller Planning.</p>
<p><span class="preview">I förhandsvisningsmiljön har standardanvändare och systemadministratörer Planering aktiverat som standard.</span></p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Hantera en tidslinjevy {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

När du skapar en tidslinjevy visas alla poster av den valda posttypen på en kronologisk tidslinje.

Tänk på följande:

* Du kan bara skapa en tidslinjevy om du har minst två datumfält associerade med en posttyp. När du har ett eller inga datumfält som är associerade med en posttyp är alternativet för tidslinjevy nedtonat.

  Du kan välja mellan följande datumfält när du skapar en tidslinjevy:

   * Registreringsdatum
   * Registrera systemgenererade fält: Skapat den, Senast ändrat den
   * Sök efter datum från anslutna poster eller objekttyper.
* Beroende på vilka datum som är associerade med posterna kanske vissa poster inte visas i tidslinjevyn i följande scenarier:

   * När start- och slutdatum inte har några värden
   * När start- eller slutdatumet inte har något värde
   * När startdatumet infaller efter slutdatumet

Så här hanterar du en tidslinjevy:

1. Gå till den posttypssida som du vill visa tidslinjen för.
1. Skapa en tidslinjevy enligt beskrivningen i artikeln [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).

   ![Exempel på tidslinjevy](assets/timeline-view-example.png)

   Posterna som är associerade med den posttyp du valde visas som staplar på en tidslinje och sorteras som standard i kronologisk ordning efter startdatum.

   >[!TIP]
   >
   >    Sorteringen av posterna på tidslinjen är inte synlig i den komprimerade vyn.

1. (Valfritt och villkorligt) När postnamnet trunkeras håller du pekaren över ett postfält för att visa postens fullständiga namn och ytterligare information.

1. Navigera genom tidslinjen på något av följande sätt:

   * Klicka på vänster- och högerikonerna eller använd den vågräta rullningen för att flytta bakåt och framåt i tidslinjen. När du uppdaterar sidan bevaras den markerade tidsramen.
   * Klicka på **Idag** för att centrera tidslinjen till dagens datum.
   * Välj något av följande alternativ i listrutan Tidsram för att uppdatera tidsstegen:

      * År
      * Kvartal
      * Månad
1. Klicka på **Växla till standardvyn** om du vill visa poster på separata rader <!--check to see if they updated the name of the setting here-->

   eller

   Klicka på **Växla till komprimerad vy** för att visa de poster vars datum inte överlappar på samma rad. <!--check to see if they updated the name of the setting here-->

   Poster visas som standard i den komprimerade vyn.

1. Gör följande för att snabbt hitta poster som matchar ett nyckelord:

   1. Klicka på ikonen **Sök** ![Sök ](assets/search-icon.png) och börja skriva ett nyckelord som är associerat med ett fält i en post som visas på skärmen. Antalet korrekta matchningar visas bredvid sökobjektet och posten med rätt matchning markeras.

      ![Sökruta och tidslinjevy för resultat](assets/search-box-and-results-timeline-view.png)

      Du kan använda vilket ord eller specialtecken som helst som visas på skärmen.

      Du kan inte använda nyckelord som är associerade med fält som inte visas i tidslinjevyn.

   1. Tryck på Retur på tangentbordet för att gå till nästa sökbara fält.
   1. (Valfritt) Om det finns mer än en matchning klickar du på upp- och nedpilarna till höger om söknyckelordet för att hitta alla matchningar i tabellen.
   1. Klicka på ikonen **x** i sökrutan för att ta bort söknyckelordet.

1. Uppdatera följande vyelement enligt beskrivningen i underavsnitten nedan:
   * [Filter](#add-filters)
   * [Gruppering](#add-grouping)
   * [Inställningar](#edit-the-timeline-view-settings)
     <!--* [Sort](#add-sort) not yet in timeline; also check the anchor and make sure it's correct-->

1. (Valfritt) Klicka på **Uppdelning** om du vill visa anslutna poster på tidslinjen.

   Mer information finns i avsnittet [Använd fördelningsfunktionen för att visa anslutna poster i tidslinjevyn](#break-down-connected-records-in-the-timeline-view)

### Lägg till filter

Du kan minska mängden information som visas på skärmen genom att använda filter.

Tänk på följande när du arbetar med filter i tidslinjevyn:

<!-- this list is almost identical to the one for the table view - update both-->

* De filter som du skapar för en tidslinjevy fungerar oberoende av filtren i andra vyer som används för samma posttyp.

* Filtren är unika för den vy du väljer. Två tidslinjevyer av samma posttyp kan ha olika filter.

* Två användare som tittar på samma tidslinjevy ser samma filter som används för närvarande.

* Du kan inte namnge de filter som du skapar för en tidslinjevy.

* När du tar bort filter tas de bort från alla som använder samma posttyp som du och som visar samma vy som du.

* Att lägga till filter i tidslinjevyn är detsamma som att lägga till filter i tabellvyn.

  Mer information finns i avsnittet&quot;Lägg till filter&quot; i artikeln [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md).

* Du kan filtrera efter anslutna postfält eller uppslagsfält.
* Du kan filtrera efter uppslagsfält som visar flera värden.


### Lägg till gruppering

<!-- groupings are almost identical between this view and table  but they display a little differently, so I kept the steps for both; update in both places if they make changes to groupings-->

Du kan gruppera poster efter liknande information när du tillämpar en gruppering på en vy.

Att lägga till grupperingar i tidslinjevyn påminner om att lägga till grupperingar i tabellvyn.

Tänk på följande när du arbetar med grupperingar i tidslinjevyn:

* Du kan använda grupperingar både i tabell- och tidslinjevyerna. Grupperingarna i tabellvyn är oberoende av grupperingarna i tidslinjevyn av samma posttyp.
* Du kan använda tre nivåer av gruppering i en vy. Posterna grupperas i den ordning som du väljer grupperingar.
&lt;!—* Du kan använda upp till fyra nivåer av gruppering när du använder API:t. —check on this for now—>
* Grupperingarna är unika för den vy du väljer. Två tabellvyer av samma posttyp kan ha olika grupperingar. Två användare som tittar på samma tabellvy ser samma gruppering som används för närvarande.
* Du kan inte namnge grupperingarna som du skapar för en tabellvy.
* Om du tar bort grupperingar tas de bort från alla som har åtkomst till samma posttyp som du och som visar samma vy som du.
* Du kan redigera poster som listas under en gruppering.
* Du kan gruppera efter anslutna postfält eller sökfält.
* När du grupperar efter uppslagsfält med flera värden (som inte har summerats av en aggregator) grupperas posterna efter varje unik kombination av fältvärden.
* Du kan referera till ett fält som ligger upp till fyra nivåer från den aktuella posttypen. Om du till exempel skapar en gruppering för en aktivitetsposttyp, och aktiviteten är ansluten till produktposttypen som är kopplad till Campaign-posttypen som är kopplad till ett Workfront-projekt, kan du referera till projektets status i den gruppering du skapar för aktivitetsposttypen.
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

Så här lägger du till en gruppering i tidslinjevyn:

1. Skapa en tidslinjevy för en posttyp enligt beskrivningen i artikeln [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).
1. Klicka på **Gruppering** i det övre högra hörnet av tidslinjevyn.

   ![Gruppera vyn för användargränssnittets tidslinje med länkade fält](assets/grouping-ui-timeline-view-with-linked-fields.png)

1. Klicka på ett av de föreslagna fälten eller klicka på **Välj ett annat fält**, sök efter ett annat fält och klicka sedan på det när det visas i listan.

   Grupperingen används automatiskt på tidslinjen och posterna visas inuti grupperingsrutan.

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. (Valfritt) Upprepa stegen ovan om du vill lägga till upp till tre grupperingar.

   Antalet fält som har valts för grupperingen visas bredvid grupperingsikonen.

   <!-- update screen shot with view redesign-->

   ![Grupperingen tillämpas i tidslinjevyn](assets/grouping-applied-in-timeline-view.png)

1. (Valfritt) I rutan **Gruppera poster efter** klickar du på ikonen **x** till höger om ett fält som är markerat för grupperingen för att ta bort grupperingen

   eller

   Klicka på **Rensa alla** om du vill ta bort alla fält.

1. Klicka utanför rutan **Gruppera poster efter** för att stänga den.
1. (Valfritt) Klicka på **Inställningar** och sedan på **Färg** för att färgkoda grupperingar. Mer information finns i avsnittet [Redigera tidslinjevisningsinställningar](#edit-the-timeline-view-settings) i den här artikeln.

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### Redigera inställningarna för tidslinjevyn {#edit-the-timeline-view-settings}

Uppdatera inställningarna för tidslinjevyn för att ange vad och hur informationen ska visas i tidslinjeavsnittet i vyn.

1. Skapa en tidslinjevy för en posttyp enligt beskrivningen i artikeln [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).
1. Klicka på **Inställningar**.
1. Klicka på **Datum och tid** på den vänstra panelen och välj sedan ett **Startdatum** och ett **slutdatum** som ska visas på tidslinjen. Du kan välja standarddatum för start och slut eller välja ett tillgängligt datumfält. De staplar som representerar posterna börjar på det datum som du anger som startdatum och slutar på det datum som motsvarar slutdatumet.

   >[!NOTE]
   >
   >Poster som inte har några värden för start- eller slutdatum eller som har ett startdatum efter slutdatumet visas inte i tidslinjevyn.

1. Klicka på **Stapelformat** i den vänstra panelen för att ange vilken information du vill visa i postfälten.

   Postens primära fält (eller rubrik), enligt postens tabellvy, är markerat som standard. <!--adjust this when the primary field is released??-->

1. (Valfritt och villkorligt) Om du har lagt till miniatyrbilder i poster, markerar du alternativet Miniatyrbild för att visa den bild som är associerad med posterna i deras postfält.

   >[!NOTE]
   >
   >    Du måste först lägga till miniatyrbilder i tabellvyn innan du kan visa dem i tidslinjevyn. Mer information finns i [Lägga till en miniatyrbild i en post](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

1. Klicka på **Lägg till fält**, klicka i rutan **Sök fält** och klicka på det fält som du vill lägga till.

   >[!TIP]
   >
   >   * Du måste skapa fälten innan du kan lägga till dem i postfälten.
   > 
   >   * Du måste ha minst ett fält markerat. **Namn** är markerat som standard.
   >
   >   * Du kan lägga till upp till fem fält.

   En förhandsvisning av hur staplarna kommer att se ut på tidslinjen visas till höger.

   ![Spela in tidslinjeinställningar för informationspanelen med förhandsgranskning](assets/record-details-panel-timeline-settings-with-preview.png)

1. <span class="preview"> (Valfritt och villkorligt) Om du visar tidslinjen i standardläge aktiverar du inställningen **Trunkera fältinformation** . När det här alternativet är aktiverat trunkeras informationen på postfälten och visas bara helt när du håller muspekaren över fälten. Den här inställningen är inaktiverad som standard och informationen visas helt i fälten. </span>

   ![Trunkera inställning aktiverad i rutan för tidslinjeinställningar markerad](assets/truncate-setting-enabled-on-timeline-settings-highlighted.png)

   >[!TIP]
   >
   >* <span class="preview">Inställningen för detaljer i fältet för trunkering är inte tillgänglig när vyn Tidslinje visas i läget Kompakt och är inte tillgänglig i kalendervyn.</span>
   >
   >* <span class="preview">Om du bryter ned tidslinjevyn för att visa anslutna objekt, gäller inställningen för detaljer i fältet Trunkera bara för huvudposttypen. Det gäller inte för de anslutna postfälten.</span>


1. Klicka på **Färg** i den vänstra panelen om du vill anpassa färgerna för posterna och grupperingarna i tidslinjen.

   ![Tidslinjevy på fliken Färg](assets/color-tab-timeline-view.png)

1. (Villkorlig och valfri) Om du har lagt till en gruppering i tidslinjevyn väljer du bland följande alternativ för att ange en färg för grupperingen i avsnittet **Ange grupperingsfärg**:

   * **Standard (grått)**: Färgen på grupperingarna är inställd på grått. Det här är standardinställningen.
   * **Fältvärden**: Färgen på grupperingarna matchar färgen på fältet som du grupperar efter.

     >[!NOTE]
     >
     >    * Du kan bara matcha färgen mot fält med färgkodade alternativ. Du kan till exempel matcha färgen mot statusfälten eller fält med alternativ som är kopplade till färger.
     >    
     >    * Du kan inte matcha färgen mot uppslagsfält från länkade poster eller objekttyper.


   Flervalsfält eller envalsfält kan t.ex. ha färgkodade alternativ.

   Om du grupperar efter fält utan färgkodade alternativ förblir grupperingsfärgen grå.

   >[!TIP]
   >
   >Om du inte har lagt till grupperingar i tidslinjevyn visas inte det här avsnittet.

1. I avsnittet **Ange postfärg** väljer du bland följande alternativ för att ange en färg för posterna:

   * **Posttyp**: Färgen på posterna matchar färgen på den posttyp du valde. Det här är standardalternativet.
   * **Fältvärden**: Färgen på posterna matchar färgen i ett fält som du anger. Fortsätt med steg 10. <!--ensure this stays accurate-->
   * **Gruppering**: Färgen på posterna matchar färgen som du angav för grupperingarna. Det här alternativet är nedtonat när du inte har använt några grupperingar på tidslinjevyn.
   * **Ingen**: Posterna visas i ett vitt fält.

1. (Villkorligt) Om du valde **Fältvärden** för postfärgerna väljer du ett fält i listrutan **Matcha postfärgen till**.

   ![Listruta för fältväljare i tidslinjevyn](assets/field-selector-drop-down-menu-timeline-view.png)

   Endast fält med färgkodade alternativ visas i listrutan.

   Flervalsfält eller envalsfält kan t.ex. ha färgkodade alternativ.

   Om du inte har något fält med färgkodade alternativ för den valda posttypen är det här alternativet nedtonat.

1. Klicka på **Spara**.

   Posterna visas i tidslinjevyn med de specifikationer som du har valt.

### Dela upp kopplade poster i tidslinjevyn

Du kan visa anslutna poster i en posts tidslinjevy genom att använda funktionen Uppdelning. Genom att dela upp poster efter deras anslutningar kan du visa tidslinjerna för andra anslutna poster och förstå hur de kan påverka posternas prestanda och deadlines.

#### Att tänka på när du använder fördelningsfunktionen

* Du kan visa anslutna poster eller objekt under posterna för den valda posttypen i tidslinjevyn.
* Du kan visa följande i tidslinjevyn med hjälp av funktionen Uppdelning:
   * Workfront Planning-poster kopplade till den valda posttypen.
   * Workfront-objekttyper eller Experience Manager-resurser som är kopplade till den valda posttypen.
   * Workfront Planning-poster eller objekt från andra program som är anslutna till poster som är kopplade till den valda posttypen.

     Du kan till exempel koppla kampanjer till portföljer. Dessutom kan ni koppla samman en annan posttyp, produkter, projekt och kampanjer. När ni bygger kampanjens tidslinjevy kan ni dela upp kampanjerna efter portföljer, produkter och projekt.

* Du kan inte visa objekttyper som bara är anslutna till Workfront-objekt i Workfront, men som inte är kopplade till någon Workfront Planning-posttyp. Du kan bara visa objekt eller posttyper som är anslutna i Workfront Planning.

  Till exempel är uppgifter kopplade till projekt i Workfront. Med hjälp av fördelningsfunktionen kan du visa projekt som är kopplade till kampanjer i Planning, men inte aktiviteter som är kopplade till projekt i Workfront.

  Om du vill visa både portföljer och projekt i tidslinjevyn för en Workfront Planning-posttyp måste både portföljerna och projekten vara kopplade till Planning-posten eller till en post kopplad till Planning-posten vars tidslinjevy du hanterar.
* Du kan bara visa posttyper som är associerade med minst två datumfält.
* Datumfälten för de posttyper som du vill visa i tidslinjevyn måste vara synliga i tabellvyn för den valda posttypen, som uppslagsfält.
* Start- och slutdatumen för de posttyper som du vill visa i tidslinjevyn måste anges i kronologisk ordning. Om en post till exempel har startdatumet 31 januari och slutdatumet 1 januari visas den inte i tidslinjevyn. Mer information finns i avsnittet [Hantera en tidslinjevy](#manage-a-timeline-view) i den här artikeln.
* Det finns en gräns på 5 posttyper som du kan inkludera i en posts uppdelning.

#### Dela upp anslutna poster

1. Skapa en tidslinjevy för en posttyp enligt beskrivningen i artikeln [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).
1. (Villkorligt) Om du visar tidslinjevyn i standardläge klickar du på **Brytning**.
1. Expandera rutan **Markera en länkad posttyp** och välj en ansluten posttyp. <!--add a new screen shot - submitted a bug to remove the "the"-->

   ![Brytningsväljaren och knappen i tidslinjevyn](assets/breakdown-picker-and-button-on-timeline.png)

   >[!TIP]
   >
   >    Om du inte har några anslutna poster, eller om de anslutna posterna inte har minst två datumfält, är rutan **Välj en länkad posttyp** inte tillgänglig.

1. Välj ett **startdatum** och ett **slutdatumfält**.

   >[!TIP]
   >
   >    Start- och slutdatum måste vara sekventiella. Om slutdatumet är före startdatumet visas inga poster på tidslinjen.

   En högerpil visas på den markerade postens fält på tidslinjen, om de är kopplade till andra poster.
1. Klicka på högerpilen om du vill expandera en posttyp och visa anslutningarna.

   ![Kampanjer uppdelade efter program i tidslinjevyn](assets/campaigns-broken-down-by-programs-in-timeline-highlighted.png)

1. (Valfritt) Upprepa stegen ovan om du vill lägga till fler anslutna poster.




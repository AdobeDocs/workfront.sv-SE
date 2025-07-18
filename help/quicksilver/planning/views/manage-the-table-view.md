---
title: Hantera tabellvyn
description: Du kan visa poster och deras fält i en tabellvy när du öppnar sidan för posttyper i Adobe Workfront Planning. I den här artikeln beskrivs hur du kan skapa eller redigera en tabellvy och hur du aktiverar närvaroindikatorer i realtid för vyn.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 0dd723b5-d674-4626-8fc2-7da41f3b7f35
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '3387'
ht-degree: 0%

---

# Hantera tabellvyn

<!--<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Du kan visa poster och deras fält i en tabellvy när du öppnar sidan för posttyper i Adobe Workfront Planning.

Mer information om postvyer och hur du hanterar dem finns i [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).

I den här artikeln beskrivs följande information:

* [Skapa eller redigera kolumner och rader i en tabellvy](#manage-a-table-view)
* [Aktivera närvaroindikatorer i realtid för tabellvyn](#enable-the-real-time-presence-indicator)

Information om hur du exporterar tabellvyn till en Excel- eller CSV-fil finns i [Exportera poster från tabellvyn](/help/quicksilver/planning/records/export-records-from-the-table-view.md).

## Krav för åtkomst

+++ Expandera för att visa åtkomstkrav.

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
   <li><p> Planering av Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-plan*</p></td> 
   <td> 
<p>Någon av följande Workfront-planer:</p> 
<ul><li>Utvald</li> 
<li>Primtal</li> 
<li>Sist</li></ul> 
<p>Workfront Planning är inte tillgängligt för äldre Workfront-planer</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planeringspaket*</p></td> 
   <td> 
<p>Någon </p> 
<p>Om du vill ha mer information om vad som ingår i varje Workfront Planning-plan kontaktar du din Workfront-kontoansvarige. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-plattform</p></td> 
   <td> 
<p>Din organisations instans av Workfront måste vara registrerad i Adobe Unified Experience för att kunna komma åt Workfront Planning.</p> 
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience för Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
    <td role="rowheader"><p>Licens för Adobe Workfront*</p></td> 
   <td><p> Standard för att skapa och ta bort vyer</p>
   <p>Deltagare eller högre för att uppdatera vyelement</p>
   <p>Workfront Planning är inte tillgängligt för äldre Workfront-licenser</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration av åtkomstnivå</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Behörigheter för objekt</p></td> 
   <td>   <p>Hantera behörigheter till en vy</p>  
   <p>Visa behörigheter till en vy för att tillfälligt ändra vyinställningarna eller duplicera den</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Mall för layout</p></td>
   <td> Användare med en Light- eller Contributor-licens måste tilldelas en layoutmall som innehåller Planering.
   <p>Standardanvändare och systemadministratörer har planeringsområdena aktiverade som standard.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table>

*Mer information om åtkomstkrav för Workfront finns [i Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Redigera poster med hjälp av tabellvyn

Du kan bara redigera postinformation i tabellvyn.

Mer information om hur du redigerar poster i tabellvyn finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

## Hantera en tabellvy {#manage-a-table-view}

När du skapar en tabellvy visas alla poster av den valda typen i en tabell. Varje rad är en unik post och varje kolumn är ett postfält. Alla fält och alla poster visas som standard.

Så här hanterar du en tabellvy:

1. Skapa en tabellvy på det sätt som beskrivs i artikeln [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).

   ![Exempel på tabellvy](assets/table-view-example.png)

1. (Valfritt) Klicka på **Radhöjd** och välj sedan bland följande alternativ för att ändra höjden på tabellraderna:
   * Kort
   * Medium
   * Lång

1. Uppdatera följande vyelement enligt beskrivningen i underavsnitten nedan:
   * [Kolumner (eller fält)](#add-columns-or-fields)
   * [Rader (eller poster)](#add-rows-or-records)
   * [Filter](#add-filters)
   * [Sort](#add-a-sort)
   * [Gruppering](#add-groupings)
   * [Radens färger](#add-row-colors)
   * [Indikator för närvaro i realtid](#enable-the-real-time-presence-indicator)


### Lägga till kolumner (eller fält) {#add-columns}

Kolumnrubrikerna i en tabellvy visar fält som är associerade med posterna i vyn. Fält som visas i tabellvyn visas också i avsnittet Detaljer i en post.

Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

<!--this is not available yet:You can display record fields (or columns) in both a table and a timeline view. However, the number of columns displayed in the table of the timeline view is limited and you cannot add columns in addition to those selected by default.-->

Att lägga till kolumner i en vy är identiskt med att lägga till fält i en posttyp.

Du kan lägga till upp till 500 fält (eller kolumner) i en tabellvy.

1. Gå till en posttypssida och klicka på en flik för tabellvy, eller klicka på **+ Visa** för att lägga till en ny vy och välj **sedan Tabell**.

1. Börja lägga till fält (eller kolumner) enligt beskrivningen i artikeln [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

   Kolumnerna som du lägger till är synliga för alla användare som har åtkomst till posttypen och läggs till som nya fält på postens sida.

1. Gör något av följande för att ändra ordningen på kolumnerna i tabellen:

   * Ta tag i kolumnrubriken och dra och släpp den i önskad position. Kolumnen som du flyttade visas en kort stund med en blå bakgrund tills du gör andra justeringar i tabellen.

   * Klicka på **Fält** i tabellens verktygsfält, dra och släpp sedan fälten i önskad ordning och klicka sedan utanför **rutan Fältsynlighet och ordning** för att stänga den.

     ![Fält som ställer in tabellvyns verktygsfält expanderat](assets/fields-setting-table-view-toolbar-expanded.png)


     >[!TIP]
     >
     >* Fältet Namn är som standard alltid det första fältet i tabellvyn. Detta anses vara ett primärt fält.
     >
     >* Du kan inte flytta fältet Namn till en annan plats, såvida du inte anger ett annat fält som primärt fält. Om du vill ha mer information fortsätter du med steg 4. <!--accurate?-->
     >
     >

   * Ersätt fältet i den första kolumnen med ett annat fält genom att ändra det primära fältet. Om du vill ha mer information fortsätter du till steg 4. <!--accurate?-->

1. (Valfritt) Håll muspekaren över ett fältnamn i kolumnrubriken för ett fält som inte visas i den första kolumnen i tabellen, klicka på den nedåtpekande pilen till höger om fältnamnet och klicka sedan på **Ange som primärt fält**.

   ![Ange som primärt fältalternativ i tabellvyn](assets/set-as-primary-field-option-table-view.png)

1. Klicka på **Ange fält** för att bekräfta.

   Fältet blir ett primärt fält, vilket innebär att det visas som den första kolumnen i tabellvyn. Föregående primära fält flyttas till den andra kolumnen.

   Primära fält blir postens titel och visas i rubrikområdet på postens sida och överallt där posterna visas. Postens titel visas till exempel i anslutna fält och i alla vyer. Mer information om primära fält finns i [Översikt över](/help/quicksilver/planning/fields/primary-field-overview.md) primära fält.

1. Klicka och dra kolumnseparationslinjerna och släpp dem på önskad plats för att öka bredden på kolumnerna.

   >[!TIP]
   >
   >De ändringar du gör i kolumnbredden och ordningen är permanenta och synliga för alla användare som har åtkomst till posttypen.

1. Håll muspekaren över kolumnrubriken, klicka sedan på den nedåtriktade pilen och klicka sedan på **Dölj fält**

   Eller

   Klicka på **Fält** i tabellverktygsfältet och inaktivera växlingsknappen som är kopplad till de fält (eller kolumner) som du vill dölja. Rutan **Fältsynlighet och ordning** visas.

   >[!TIP]
   >
   >Antalet dolda fält visas till vänster om ikonen Fält i verktygsfältet.


1. **Klicka på ikonen Fält** och aktivera växlingsknappen som är kopplad till de fält som du vill visa i kolumnerna i tabellen. Alla fält visas som standard.

1. Gör så här för att snabbt hitta poster som matchar ett nyckelord:

   1. **Klicka på sökikonen**![ Sökikon](assets/search-icon.png) och börja skriva ett nyckelord som är associerat med ett fält i en post som visas på skärmen. Antalet korrekta matchningar visas bredvid sökobjektet och fältet med rätt matchning markeras.

      ![Sökruta med resultatblå kontur i tabellvy](assets/search-box-with-results-blue-outline-table-view.png)

      Du kan använda vilket ord eller specialtecken som helst som är synligt på skärmen.

      Du kan inte använda nyckelord som är associerade med fält som är dolda i tabellvyn.

   1. Tryck **på Retur** på tangentbordet för att gå till nästa hittade fält.

   1. (Valfritt) Om det finns fler än en matchning klickar du på upp- och nedpilarna till höger om sökordet för att hitta alla matchningar i tabellen.

   1. **Klicka på x-ikonen** i sökrutan för att rensa sökordet.


### Lägga till rader (eller poster) {#add-rows}

Raderna i en tabellvy visar enskilda poster av den valda posttypen.

Du kan ha upp till 50 000 poster (eller rader) för en posttyp.

1. Gå till en posttypssida och klicka på en flik för tabellvy, eller klicka på **+ Visa** för att lägga till en ny vy och välj **sedan Tabell**.

1. Börja lägga till poster (eller rader) enligt beskrivningen i artikeln [Skapa poster](/help/quicksilver/planning/records/create-records.md).

   De poster som du lägger till i tabellvyn sparas direkt och är synliga för alla användare som har behörigheten Visa eller högre till arbetsytan.

1. (Valfritt) Lägg till en miniatyrbild för varje post och klicka på **Fält** i det övre högra hörnet av tabellen och välj sedan växlingsknappen för **fältet Miniatyrbild** för att visa det till vänster om det primära fältet. Den är avmarkerad som standard.

   Mer information finns i [Lägga till en miniatyrbild i en post](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

1. (Valfritt) Markera en eller flera poster i en rad och dra och släpp **sedan handtagsikonen**![ Handtagsikonen](assets/handle-icon.png) till vänster om posten för att ändra ordningen på raderna.

   >[!NOTE]
   >
   >Du kan inte ändra ordningen på raderna om du använder minst en sortering i tabellvyn.
   >
   >De ändringar du gör i radordningen är synliga för alla användare som har åtkomst till posttypen

<!-- this section below links from the timeline view; consider splitting them if they become different-->

### Lägga till filter {#add-filters}

Filter hjälper dig att minska mängden information som visas på skärmen.

Tänk på följande när du arbetar med filter i tabellvyn:

<!-- this list is almost identical to the one for the table view - update both-->

* De filter som du skapar för tabellvyn fungerar oberoende av filtren i tidslinjevyn när de tillämpas på samma posttyp.

* Filtren är unika för den vy som du väljer. Två tabellvyer av samma posttyp kan ha olika filter tillämpade på dem. Två användare som tittar på samma tabellvy ser samma filter som för närvarande används.

* Du kan inte namnge de filter som du skapar och använder i en tabellvy.

* Om du tar bort filter tas de bort från alla som har åtkomst till samma posttyp som du och använder samma vy som du använder.

* Du kan filtrera efter anslutna postfält eller uppslagsfält.

* Du kan filtrera efter uppslagsfält som visar flera värden.

* Du kan referera till ett fält som är upp till 4 nivåer bort från den aktuella posttypen. Om du till exempel skapar ett filter för en aktivitetsposttyp och aktiviteten är kopplad till posttypen Produkt som är kopplad till posttypen Kampanj som är kopplad till ett Workfront-projekt, kan du referera till projektets budget i filtret som du skapar för posttypen Aktivitet.

Så här lägger du till ett filter i en tabellvy:

1. Skapa en tabellvy för en posttypssida enligt beskrivningen i artikeln [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).
1. Välj en tabellvy och klicka sedan på **Filter** i det övre högra hörnet av tabellen.
1. Klicka på **Lägg till villkor** och lägg till följande information:

   * **Välj ett fält** som du vill filtrera efter <!-- the tip below might change-->

   * **Välj ett alternativ** (eller en filtermodifierare) för att definiera vilken typ av villkor fältet måste uppfylla

     I tabellen nedan visas tillgängliga modifierare för varje typ av fält.

     <table>
        <thead>
        <tr>
            <th><b>Typ av fält</b></th>
            <th><b>Modifierare</b></th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>Enradig, Stycke, Formel </td>
            <td><p>Innehåller</p>
            <p>Innehåller inte</p>
            <p>Vara</p>
            <p>Är inte</p>
            <p>Är tom</p>
            <p>Är inte tom</p></td>
        </tr>
        <tr><td>Välj en gång</td>
            <td><p>Vara</p>
            <p>Är inte</p>
            <p>Är någon av följande</p>
            <p>Är ingen av</p>
            <p>Är tom</p>
            <p>Är inte tom</p></td>
        </tr>
        <tr>
            <td>Välj flera, personer</td>
            <td><p>Har någon av följande</p>
            <p>Har alla</p>
            <p>Är exakt</p>
            <p>Har ingen av</p>
            <p>Är tom</p>
            <p>Är inte tom</p></td>
        </tr>
        <tr>
            <td>Tal, procent, valuta</td>
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
            <td><p>Vara</p>
            <p>Är inte</p>
            <p>Är efter</p>
            <p>Är före</p>
            <p>Är mellan</p><p>Är inte mellan</p>
            <p>Är tom</p><p>Är inte tom</p></td>
        </tr>

     <tr>
            <td>Kryssrutan</td>
            <td><p>Vara</p>
        </tr>
        </tbody>
        </table>

   * Välj ett värde för det valda fältet.

   ![Filtrera tabellvy för användargränssnitt](assets/filter-ui-table-view.png)

   Det finns ingen gräns för hur många filtreringsvillkor du kan lägga till.

1. (Valfritt) Klicka på **Lägg till villkor** för att lägga till ytterligare ett filtreringsalternativ och upprepa stegen ovan. Antalet filter som används visas till vänster om filterikonen.
1. Klicka på följande operatorer för att ange hur filtervillkoren är kopplade och ska tillämpas:

   * **OCH:** Alla angivna villkor måste uppfyllas.
   * **ELLER:** Något av de angivna villkoren måste uppfyllas. Det här är standardalternativet.

   1. (Valfritt) Lägg till ytterligare **AND-** eller **OR-operatorer** mellan flera villkorsgrupperingar.

      ![Filter med flera nivåer i vyer](assets/multi-tiered-filters-in-views.png)

   Listan med poster filtreras automatiskt.  <!--at this time, you can't name and save the filter - but will this change?!-->
   <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->

1. (Valfritt) Klicka på **x-ikonen** för att ta bort ett filtervillkor.
1. (Valfritt) Klicka på **Filter** för att stänga filterrutan. <!--right now you cannot "clear all" for filters, but this might come later-->

### Lägga till en sortering {#sort-information}

Genom att använda en sortering kan du ordna information i en viss ordning.

Du kan sortera följande information:

* Alla poster i en tabellvy. <!--or timeline view. ***********verify this is the case for the timeline view*********************-->
  <!--* All groupings. - this is not available yet-->

Tänk på följande när du sorterar poster i tabellvyn:

<!-- if this is available for the timeline view, update both when you update one-->

* Sorteringen är unik för den vy som du väljer. Två tabellvyer av samma posttyp kan ha olika sorteringskriterier. Två användare som tittar på samma tabellvy ser samma sortering som för närvarande används.

* Du kan inte namnge de sorteringar som du skapar och använder i en tabellvy.

* Sorteringen du skapar bevaras när du navigerar bort.

* Du kan sortera efter så många fält som visas i tabellvyn för en posttyp.

* Du kan inte sortera efter anslutna postfält, men du kan sortera efter uppslagsfält från anslutna posttyper.

* När du sorterar efter uppslagsfält med flera värden (som inte har summerats av en aggregator) används det första värdet för sortering.

* Om du tar bort sorteringskriterier tas de bort från alla som har åtkomst till samma posttyp som du och använder samma vy som du.

* Du kan referera till ett fält som är upp till 4 nivåer bort från den aktuella posttypen. Om du till exempel skapar en sortering för en aktivitetsposttyp och aktiviteten är kopplad till produktposttypen som är kopplad till posttypen Kampanj som är kopplad till ett Workfront-projekt, kan du referera till projektets status i den sortering som du skapar för posttypen Aktivitet.

Så här sorterar <!--ungrouped (add this when sorting for groupings will be available--> du posterna:

1. Skapa en tabellvy på det sätt som beskrivs i artikeln [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).
1. **Klicka på sorteringsikonen**![](assets/sort-icon.png) Sortera längst upp till höger i tabellen

   Eller

   Håll muspekaren över namnet på en kolumn i tabellvyn, klicka på den nedåtriktade pilen till höger om kolumnrubrikens namn och klicka sedan på **Sortera efter det här fältet**. Fältet läggs till som ett sorteringsval i ikonen Sortera i det övre högra hörnet av tabellvyn.

1. (Villkorligt) **Klicka på ett av de föreslagna fälten i rutan Sortera poster efter** eller klicka på **Välj ett annat fält** och sök efter ett annat fält och klicka sedan på det när det visas i listan.

   Sorteringen tillämpas automatiskt i tabellvyn och posterna visas sorterade efter de valda kriterierna.

   <!-- add a step that you can rearrange the sorting fields here, when this will be possible-->

1. (Valfritt) Klicka på **Lägg till villkor** och upprepa stegen ovan för att sortera efter ytterligare fält.

   Antalet fält som du sorterar efter visas till vänster om sorteringsikonen i det övre högra hörnet av verktygsfältet. Du kan bara välja vilka fält som ska visas i kolumnerna i tabellvyn.

1. (Valfritt) **I rutan Sortera poster efter** klickar du på **x-ikonen** till höger om ett sorteringsfält för att ta bort sorteringen

   Eller

   Klicka på **Rensa alla** om du vill ta bort alla fält från sorteringen.

1. Klicka utanför **rutan Sortera poster efter** för att stänga den.

   ![Sortering i tabellvy](assets/sorting-in-table-view.png)

   Informationen som visas i tabellen sorteras enligt dina valda kriterier.

   De fält som väljs för sorteringen visar en sorteringsikon följt av en siffra som anger i vilken ordning sorteringen tillämpas.

### Lägga till grupperingar {#add-groupings}

<!--this section exists in the timeline view too, but the display is slightly different, so I kept both steps; consider updating both sections if any updates to groupings are introduced-->

Du kan gruppera poster efter liknande information när du använder en gruppering i en vy.

Tänk på följande:

* Du kan använda grupperingar både i tabell- och tidslinjevyn. Grupperingarna i tabellvyn är oberoende av dem i tidslinjevyn av samma posttyp.
* Du kan använda 3 nivåer av gruppering i en vy. Posterna grupperas i den ordning du väljer.
&lt;!--* Du kan använda upp till 4 grupperingsnivåer när du använder API:et. --kollar på den här för nu-->
* Grupperingarna är unika för den vy som du väljer. Två tabellvyer av samma posttyp kan ha olika grupperingar tillämpade på dem. Två användare som tittar på samma tabellvy ser samma gruppering som för närvarande används.
* Du kan inte namnge de grupperingar som du skapar för en tabellvy.
* Om du tar bort grupperingar tas de bort från alla som har åtkomst till samma posttyp som du och som visar samma vy som du.
* Du kan redigera poster som listas under en gruppering.
* Du kan gruppera efter anslutna postfält eller uppslagsfält.
* När du grupperar efter uppslagsfält med flera värden (som inte har summerats av en aggregator) grupperas posterna efter varje unik kombination av fältvärden.
* Du kan referera till ett fält som är upp till 4 nivåer bort från den aktuella posttypen. Om du till exempel skapar en gruppering för en aktivitetsposttyp och aktiviteten är kopplad till produktposttypen som är kopplad till posttypen Kampanj som är kopplad till ett Workfront-projekt, kan du referera till projektets status i den gruppering som du skapar för posttypen Aktivitet.
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

Så här lägger du till en gruppering:

1. Skapa en tidslinjevy för en posttyp enligt beskrivningen i artikeln [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).
1. Klicka på **Gruppering** i det övre högra hörnet av tabellvyn.

   ![Gruppera användargränssnittstabellvy med länkade fält](assets/grouping-ui-table-view-with-linked-fields.png)

1. Klicka på ett av de föreslagna fälten eller klicka på **Välj ett annat fält**, sök efter ett annat fält och klicka sedan på det när det visas i listan.

   Grupperingen tillämpas automatiskt på tabellen och posterna visas under grupperingsseparationslinjen.

1. (Valfritt) Klicka på **Lägg till villkor** och upprepa stegen ovan för att lägga till upp till 3 grupperingar.

   Antalet fält som valts för grupperingen visas bredvid ikonen Gruppering.

   ![Gruppering som används i tabellvyn](assets/grouping-applied-in-table-view.png)

1. (Valfritt) I **rutan Gruppera poster efter** klickar du på **x-ikonen** till höger om ett fält som är markerat för grupperingen för att ta bort grupperingen

   Eller

   Klicka på **Rensa alla** om du vill ta bort alla fält.

1. Klicka utanför **rutan Gruppera poster efter** för att stänga den.
1. (Valfritt) Klicka på **+ Ny post** i slutet av en gruppering för att lägga till nya poster och uppdatera sedan sidan för att lägga till den nya posten i lämplig gruppering. <!--this might need to be changed when they add the Refresh button on the toolbar of the table view-->

1. Om du vill expandera eller komprimera grupperingar gör du något av följande:

   1. Klicka på ikonen Gruppering och **sedan** på Expandera alla **eller** Komprimera alla **.** Då expanderas alla grupperingar och undergrupperingar i tabellvyn.

      ![Expandera och komprimera alla knappar i tabellvyn för grupperingsruta](assets/expand-collapse-all-buttons-on-grouping-box-table-view.png)

   1. Högerklicka på någon av grupperingsrubrikerna i tabellvyn och klicka sedan på något av följande alternativ:
      * **Expandera grupp**
      * **Komprimera grupp**
      * **Expandera alla**
      * **Komprimera alla**
      * **Expandera undergrupper**
      * **Komprimera undergrupper**

      Beroende på hur många grupperingar du använder i vyn kanske vissa alternativ inte är tillgängliga.

<!-- this is not available yet: 

To sort grouped records: 

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. ************************* add steps here for sorting grouped records****************

-->

### Lägga till radfärger

1. (Valfritt) Klicka på **Radfärger** för att definiera villkor och välja konfigurera olika färger för tabellrader.

1. Klicka på **Lägg till färg** och välj sedan **ett fält** vars värde du vill ska bestämma färgen på en rad.

   Om du till exempel vill visa kampanjer med statusen Aktiv i grönt väljer du **Status** och väljer sedan en modifierare och ett värde för fältet.

   ![Ruta för radfärger med Aktiv status vald och standardfärgval](assets/row-colors-box-with-active-status-selected-default-color-choice.png)

1. Klicka på rullgardinsmenyn för färgväljaren i det övre vänstra hörnet av det villkor du valde för att välja färg för villkoret och klicka sedan utanför färgväljarrutan för att stänga det.

   ![Rullgardinsmenyn för färgväljaren i rutan Radfärger är markerad](assets/drop-down-color-picker-menu-in-row-colors-box-highlighted.png)

1. (Valfritt) Klicka på **Lägg till villkor** om du vill lägga till fler fält och värden i den första uppsättningen villkor

   Eller

   Klicka på **Lägg till färg** om du vill lägga till en ny uppsättning villkor och identifiera en ny färg.

   Du kan till exempel visa kampanjer med en planeringsstatus i gult genom att definiera en ny uppsättning villkor.

   ![Ruta för radfärger med Aktiv och Planeringsstatus](assets/row-colors-box-with-active-and-planning-status-custom-colors.png)

1. (Valfritt) **Aktivera inställningen Använd på hela raden** i det övre högra hörnet av rutan Radfärger. Hela raden där villkoret uppfylls visas automatiskt i den valda färgen.

   >[!NOTE]
   >
   >* Om inställningen Använd på hela raden är inaktiverad visas endast den vänstra sidan av fältet Primär en smal färgindikator med den valda färgen. Inställningen är avstängd som standard.
   >
   >* Du kan inte använda radfärger på en hel rad när du har minst en gruppering markerad i tabellvyn.

1. Klicka utanför **rutan Radfärger** för att stänga den. Färgerna används automatiskt.

### Aktivera närvaroindikatorn i realtid

Avatarer för andra användare som redigerar postinformation samtidigt som du visas som standard i det övre högra hörnet i alla postvyer.

När du visar tabellvyn kan du också se vilket fält en annan användare redigerar när du visar posten.

1. Gå till en sida för posttyp och öppna valfri vy.
1. (Villkorligt) Om det finns andra användare som redigerar posterna av den valda typen samtidigt visas deras avatarer i det övre högra hörnet av vyn.
1. Klicka på rullgardinsmenyn bredvid avatarerna och välj sedan växlingsknappen **Visa medarbetare** . Växlingsknappen är markerad som standard.

   ![Visa medarbetare växla valda](assets/show-collaborators-toggle-selected.png)

1. (Villkorligt) Öppna en tabellvy och fältet som en annan person aktivt redigerar markeras i den färg som motsvarar konturen av deras avatar i tabellvyn.

   Om markeringsfärgen för avataren är grå slutade användaren att aktivt redigera posten för mer än 30 sekunder sedan.

   ![Realtidsindikator, tabellfält och avataranslutning](assets/real-time-indicator-table-field-and-avatar-connection.png)

   >[!TIP]
   >
   >Du kan välja **växlingsknappen Visa medarbetare** från vilken vy som helst. Det fält som för närvarande redigeras av andra visas endast i tabellvyn.






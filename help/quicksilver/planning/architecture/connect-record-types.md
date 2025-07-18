---
title: Anslut posttyper
description: Ett sätt att ange hur enskilda posttyper relaterar till varandra är att koppla ihop dem. Du kan också koppla ihop Adobe Workfront Planning-posttyper med objekttyper från andra program för att förbättra användarnas upplevelse och behålla deras fokus i ett program.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '2499'
ht-degree: 0%

---


# Koppla posttyper

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

<!--
You can use Adobe Workfront Planning to design fully-customizable workspaces that contain record types needed in your organization. A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application. -->

Du kan koppla posttyper till varandra eller så kan du koppla posttyper med objekttyper från andra program.

Det är praktiskt att koppla posttyper när du har flera typer av arbetsobjekt som påverkar varandra. Du kan till exempel arbeta med kampanjer och varje kampanj kan rikta sig till flera varumärken. För att indikera detta förhållande kan du koppla kampanjer till varumärken. Dessutom kan arbetet för varje kampanj planeras i flera projekt i Workfront. För att indikera detta kan du koppla kampanjerna till relevanta projekt. Genom att koppla posttyper och sedan koppla enskilda poster uppnås den här relationen i Workfront Planning.

I den här artikeln beskrivs hur du kan ansluta två Workfront Planning-posttyper eller en Workfront Planning-posttyp med ett objekt från ett annat program.

När du har upprättat anslutningen mellan poster eller objekttyper kan du koppla enskilda poster till varandra och visa fält från den länkade posten eller objekttyperna i en Workfront Planning-post.

Allmän information om anslutningstyper finns i [Översikt över](/help/quicksilver/planning/architecture/connect-record-types-overview.md) anslutna posttyper.

Mer information om hur du kopplar ihop poster eller poster med objekt från andra program finns i [Koppla poster](/help/quicksilver/planning/records/connect-records.md).

Ett exempel på hur du kopplar posttyper och poster finns i [Exempel på hur du kopplar ihop posttyper och poster](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md).

<!--ensure this last linked article is right; the title and the link should have changed-->

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
   <li><p> Planering av Adobe Workfront<p></li>
   <li><p> Adobe Experience Manager Assets, om du vill koppla AEM resurser med posttyper för planering<p>
   <p>Du måste ha en Adobe Experience Manager Assets-licens och en integrering mellan AEM Assets och Workfront.    Mer information finns i <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront för Experience Manager Assets och Assets Essentials: artikelindex</a>. </p>
   </li>
   </ul></td> 
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
  <tr> 
   <td role="rowheader"><p>Licens för Adobe Workfront*</p></td> 
   <td> <p>Standard</p> 
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
   <td>   <p>Hantera behörigheter till en arbetsyta</a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, även de som de inte har skapat.</p></td> 
  </tr>

</tbody> 
</table>

*Mer information om åtkomstkrav för Workfront finns [i Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Koppla posttyper

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-planning}}

1. Klicka på den arbetsyta vars posttyper du vill ansluta,

   Eller

   Från en arbetsyta expanderar du den nedåtpekande pilen till höger om ett befintligt arbetsytenamn, söker efter en arbetsyta och väljer den sedan när den visas i listan.
1. Klicka på kortet för en posttyp för att öppna sidan för posttypen.
1. Klicka på **ikonen +** i det övre högra hörnet av tabellvyn och klicka sedan på fliken Ny **anslutning** .

   ![Ny anslutningsflik med AEM alternativ för Workfront](assets/new-connection-tab-with-workfront-aem-options.png)

1. **I fältet Posttyp** söker du efter en posttyp eller väljer något av följande:

   * En annan posttyp från den aktuella arbetsytan

     ![Många till många anslutningsväljare](assets/many-to-many-connection-picker.png)

     >[!TIP]
     >
     > 
     >Om du inte har några andra posttyper i den valda arbetsytan visas inte avsnittet Arbetsyta.


   * En posttyp från en annan arbetsyta som har konfigurerats för att ansluta från andra arbetsytor.

     >[!TIP]
     >
     >Inställningen **Tillåt anslutning till den här posttypen på andra arbetsytor** måste vara aktiverad för en posttyp på fliken Avancerade **inställningar** i **rutan Redigera posttyp** för att en posttyp ska vara tillgänglig från andra arbetsytor. Om det inte finns några posttyper som är konfigurerade för att ansluta från andra arbetsytor visas inte avsnittet för arbetsyta.
     > ![Rutan Redigera posttyp fliken Fliken Avancerade inställningar](assets/edit-record-type-box-advanced-settings-tab.png)

     Mer information finns i [Redigera posttyper](/help/quicksilver/planning/architecture/edit-record-types.md).

     ![Ny anslutning för att tillåta flera postrutor](assets/new-connection-allow-multiple-records-box.png)

   * Ett projekt, en portfölj, ett program, ett företag **eller** en **grupp** från **avsnittet Workfront Object Types**.

     ![Val av projektanslutning för Workfront](assets/workfront-project-connection-selection.png)

   * **Experience Manager Assets** från **avsnittet Adobe Applications** .

     ![Val av AEM Assets-anslutning](assets/aem-assets-connection-selection.png)

1. Uppdatera följande information:

   * **Namn**: Namnet på det anslutna fältet, så som det kommer att visas i tabellvyn eller på postsidan för den ursprungliga posttypen. Då skapas kolumnen för den länkade posten i tabellvyn för den ursprungliga posttypen eller det länkade postfältet för de ursprungliga posterna. Som standard är namnet på fältet namnet på den post eller det objekt som du ansluter till.

   >[!TIP]
   >
   >Du kan ha flera kopplingar till samma post eller objekttyp. Om du inte redigerar namnet på det anslutna fältet lägger Workfront till en siffra efter namnet på den anslutna posten för att ange antalet anslutna posttyper med samma namn.

   * **Beskrivning**: Ytterligare information om det anslutna postfältet. Beskrivningen av ett fält visas när du håller muspekaren över fältets kolumn i en tabell.
   * **Tillåt flera poster**: Välj det här alternativet om du vill ange att du tillåter användare att lägga till flera poster när det länkade posttypsfältet visas på de ursprungliga posterna. Detta är markerat som standard.

     Det här alternativet är bara tillgängligt när du kopplar poster från två olika arbetsytor eller en post och ett Adobe Experience Manager-resursobjekt.

     ![Ny anslutning för att tillåta flera postrutor](assets/new-connection-allow-multiple-records-box.png)

   * **Anslutningstyp**: Välj ett av följande alternativ för att ange hur många poster de kan ansluta till och från:

      * Många till många
      * En till många
      * Många till en
      * En till en

     Det här alternativet är endast tillgängligt när du ansluter poster från samma arbetsyta eller en post och en Workfront-objekttyp.

     ![Många till många anslutningsväljare](assets/many-to-many-connection-picker.png)

     Mer information om anslutningstyper finns i [Översikt över](/help/quicksilver/planning/architecture/connect-record-types-overview.md) anslutna posttyper.

     >[!NOTE]
     >
     > Om du väljer En till många eller En till en som Anslutningstyp och senare vill ansluta en post eller ett objekt som redan är anslutet någon annanstans, får du en varning om att om du ansluter det igen kommer det att tas bort från den ursprungliga anslutningen. Du kan tillåta borttagning eller välja en annan post.

   * **Välj uppslagsfält**: Välj det här alternativet om du vill lägga till fält från den valda posttypen. Uppslagsfälten är fält som är associerade med den post- eller objekttyp som du länkar till. När du länkar dem visas information från den post eller det objekt som du länkar till på den post som du länkar från. Detta är markerat som standard.

   >[!TIP]
   >
   >* Du kan inte lägga till Workfront typeahead-fält (inklusive fält som Projektägare eller Projektsponsor) som uppslagsfält.
   >
   >* Workfront-objektens datumfältsinformation visas i 24-timmarsformat i Workfront Planning, oavsett hur den visas i Workfront.
   >
   >   Om ett projekts planerade startdatum till exempel visas som 15:00 :00 i Workfront visas det som 15:00 i Workfront Planning i ett importerat uppslagsfält.

1. (Villkorligt och valfritt) Om du har valt att ansluta ett Workfront-objekt väljer du ett **anpassat formulär** i **avsnittet Länka endast objekt som matchar dessa kriterier** . Endast objekt som har de valda anpassade formulären kopplade kan länkas till den valda posttypen. Du kan välja mer än ett formulär.

   >[!NOTE]
   >
   > Du måste skapa anpassade formulär i Workfront för de markerade objekten innan de visas i den här listan.

1. (Villkorligt) Om du har valt att ansluta till Experience Manager Assets väljer du en databas i **listrutan Experience Manager-databas** i **avsnittet Link assets from the following repository** . Det här fältet är obligatoriskt. Endast databaser som du har tillgång till i Experience Manager Assets visas i det här fältet.

   >[!NOTE]
   >
   >Workfront-administratören kan mappa Workfront Planning-fält till Experience Manager Assets-fält via metadatamappningen i Workfront. Mer information finns i [Konfigurera mappning av resursmetadata mellan Adobe Workfront och Experience Manager Assets](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).

1. (Villkorligt) Om du har valt att ansluta till Experience Manager Assets eller till en Workfront Planning-posttyp väljer du ett av följande alternativ i **området Record appearance** :

   * **Namn och bild**: Både namnet och miniatyrbilden eller ikonen för de anslutna posterna visas i fältet för den anslutna posten. Det här är standardalternativet.
   * **Namn**: Endast namnet på de anslutna posterna visas i fältet för den anslutna posten.
   * **Bild**: Endast miniatyrbilden eller ikonen för de anslutna posterna visas i fältet för den anslutna posten.

   Poster utan en miniatyrbild visas i stället för ikonen för posttyp. Ett exempel på hur de anslutna posterna kommer att visas visas i **området Arkiveringsutseende** .

   >[!NOTE]
   >
   >* När du tillåter att flera poster länkas kan det spara utrymme i mindre områden, till exempel postvyer, om du bara visar miniatyrbilden.
   >
   >* Namnet på en post är det primära fältet i posten. Mer information finns i [Översikt över](/help/quicksilver/planning/fields/primary-field-overview.md) primärt fält.
   >
   >* Det går inte att välja ett utseende för en post när du väljer Workfront-objekttyper.
   >
   >* Det du väljer i området Arkivskivans utseende avgör hur posterna visas i anslutningar överallt i systemet, inklusive alla vyer och detaljsidor.

1. Klicka på **Skapa**.

1. (Villkorligt) Om du har valt **inställningen** Välj uppslagsfält **öppnas rutan Lägg till uppslagsfält**.

   Klicka på **ikonen +** för att lägga till fält från **området Omarkerade fält** .

   Eller

   Klicka på **ikonen -** för att ta bort fält från **området Valda fält**

   ![Lägga till uppslagsfält för en annan posttypsruta](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   Värdena för de kopplade fälten fylls i automatiskt när du har länkat poster eller objekt.

   >[!IMPORTANT]
   >
   >    Alla med visningsbehörighet eller högre behörighet till arbetsytan kan visa informationen i de länkade fälten, oavsett deras behörigheter eller åtkomstnivå i tillämpningen av de länkade objekttyperna.

1. (Valfritt) Klicka på **Hoppa** över om du vill hoppa över att lägga till fält från den länkade posten eller objekttypen. Namnet eller Primärt fält för den länkade posten är det enda synliga fältet i tabellvyn för den posttyp som du ansluter från.

1. Välj en aggregator för de uppslagsfält som du lägger till.

   >[!NOTE]
   >
   >Du kan inte lägga till aggregatorer för följande fälttyper:
   >
   >    * Paragraf
   >    * Kryssrutan

   Värdena för de länkade fälten visas antingen avgränsade med kommatecken eller som ett summerat värde enligt den aggregator du väljer, när användare väljer mer än en länkad post i det länkade postfältet.

   Om uppslagsfältet innehåller flera värden som inte summeras bör du tänka på följande när du använder fältet för att sortera eller gruppera i en vy:

   * Sorteringen görs efter det första värdet

   * Posterna grupperas efter varje unik kombination av fältvärden

   * Tidslinjevyn skapas baserat på det första datumvärdet för den anslutna posttypen, när den visas i vyn

   >[!IMPORTANT]
   >
   > Du måste välja ett aggregatorvärde när du lägger till uppslagsdatumfält om du vill att fälten ska vara tillgängliga att lägga till som start- och slutdatum för tidslinjen och kalendervyerna. Du kan till exempel välja aggregatorn MAX eller MIN för ett fält för uppslagsdatum.

   ![Listruta för aggregator för länkat nummerfält](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > Aggregatorer är inte tillgängliga när du ansluter posttyper till Experience Manager Assets.

   Välj bland följande:

   * **Ingen**: Visar de värden som kommer från flera poster avgränsade med kommatecken. Det här är standardvalet.
   * **MAX**: Visar det högsta värdet från alla värden som kommer från flera poster som är markerade i det länkade postfältet.
   * **MIN:** Visar det lägsta värdet av alla värden som kommer från flera poster som är markerade i det länkade postfältet.
   * **SUMMA:** Visar summan av alla värden som kommer från flera poster som är markerade i det länkade postfältet.
   * **AVG**: Visar medelvärdet av alla värden som kommer från flera poster som valts i det länkade postfältet.
   * **UNIK**: Tar bort dubbletter från uppslagsfältets värden och visar endast de unika värdena. Detta är inte tillgängligt för följande fälttyper:
      * Paragraf
      * Kryssrutan
      * Folk

   >[!NOTE]
   >
   >Du kan till exempel länka produktposten (länkad post) från kampanjposten (ursprunglig post) och ge den namnet &quot;Produktfält&quot;. Du kan också välja att länka fältet Budget i produktposten från kampanjposten och kalla det &quot;Produktbudget&quot;. Om du tillåter att välja flera poster i fältet &quot;Produkt&quot; kan du välja Produkt 1 med en budget på 100 000 USD och Produkt 2 med en budget på 110 000 USD och Produkt 3 med en budget på 100 000 USD. Du kan visa följande budgetinformation i det länkade fältet från den ursprungliga posten, beroende på vilken aggregator du väljer:
   >
   >* **Ingen**: $100 000, $110 000, $100 000
   >* **MAX**: $110,000
   >* **MIN:** $100,000
   >* **SUMMA:** $310,000
   >* **Genomsnitt**: $103,000.33
   >* **UNIKT: $** 100,000
   >

1. (Valfritt) **Använd sökikonen** ![Sök för](assets/search-icon.png) att söka efter ett fält.

1. Klicka på **Lägg till fält** för att spara ändringarna.

   Följande objekt ska läggas till:

   * Ett länkat postfält på den posttyp som du länkar från. Det länkade postfältet visar enskilda poster från den länkade posttypen när du har lagt till dem manuellt. Mer information om hur du lägger till poster finns i [Koppla poster](/help/quicksilver/planning/records/connect-records.md). Namnet på det länkade postfältet är det namn som du valde i steg 6. <!--accurate-->

   * Ett länkat fält (eller länkdatafält) som visar information om de länkade post- eller objekttyperna när du manuellt har lagt till posterna eller objekten i det länkade postfältet. Uppslagsfält skapas bara när **inställningen Välj uppslagsfält** är markerad när anslutningen skapas. Uppslagsfält namnges automatiskt enligt det här mönstret:

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

     Om du till exempel har länkat en kampanjposttyp med en programposttyp och gett fältet för den programlänkade posten namnet &quot;Programinformation&quot; och sedan valt att även visa programmets budgetfält i kampanjens tabellvy, namnges `Budget (from Program information)` det länkade fältet automatiskt i kampanjens tabellvy.

   * När du länkar posttyper till varandra läggs även ett länkat postfält till på den posttyp som du länkar till. Namnet på det länkade postfältet i den länkade posttypen är namnet på den posttyp som du länkar från.

     Om du till exempel länkar posttypen &quot;Produkt&quot; från posttypen &quot;Kampanj&quot; och du har gett det kopplade fältet i kampanjen namnet &quot;Länkad produkt&quot; skapas ett länkat postfält &quot;Kampanj&quot; för posttypen Produkt.

     >[!TIP]
     >
     > Ett länkat postfält skapas inte för objekt från ett annat program till den posttyp som du länkar från i Workfront Planning.

1. (Valfritt och villkorligt) Från antingen den ursprungliga posttypen eller den länkade posttypens tabellvy klickar du på den nedåtpekande pilen i rubriken för de länkade postfälten och klickar sedan på något av följande:

   * **Redigera fält**: Uppdatera fältets **namn** och **beskrivningsinformation** .
   * **Redigera uppslagsfält**: Lägg till eller ta bort något av den länkade postens fält.

   ![Rullgardinsmenyn Redigera fält och uppslagsfält i tabellkolumnen](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   Om du vill lägga till eller ta bort uppslagsfält följer du anvisningarna i steg 16–17 ovan. <!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > Du kan inte lägga till uppslagsfält som tillhör posttyper som du länkar från till objekttyper från ett annat program.
   >
   > Du kan till exempel inte lägga till uppslagsfältet &quot;Campaign Status&quot; i ett Workfront-projekt som du länkar till från kampanjerna.

1. (Valfritt) Klicka på den nedåtriktade pilen i sidhuvudet för ett länkat postfält eller i sidhuvudet för ett uppslagsfält från den posttyp som du länkar från och klicka sedan på **Ta bort**.

   Postfältet eller uppslagsfältet tas bort. Om du tar bort ett postfält tas även alla uppslagsfält som är kopplade till den länkade posten bort.

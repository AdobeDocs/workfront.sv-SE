---
title: Koppla posttyper
description: Ett sätt att ange hur enskilda posttyper relaterar till varandra är att koppla dem. Du kan även koppla posttyperna Adobe Workfront Planning till objekttyper från andra program för att förbättra användarupplevelsen och behålla fokus i ett program.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 1eb1e919bede7e366956d8c0bd969329a641123f
workflow-type: tm+mt
source-wordcount: '2196'
ht-degree: 0%

---


# Koppla posttyper

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i sandlådemiljön för förhandsgranskning.</span>

{{planning-important-intro}}

<!--
You can use Adobe Workfront Planning to design fully-customizable workspaces that contain record types needed in your organization. A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application. -->

Du kan ansluta posttyper till varandra eller koppla posttyper med objekttyper från andra program.

I den här artikeln beskrivs hur du kan koppla två typer av Workfront Planning-poster, eller en Workfront Planning-posttyp, till ett objekt från ett annat program.

När du har upprättat anslutningen mellan poster eller objekttyper kan du koppla enskilda poster till varandra och visa fält från den länkade posten eller objekttypen på en Workfront Planning-post.

Allmän information om anslutningstyper finns i [Översikt över anslutna posttyper](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

Mer information om hur du ansluter poster eller poster med objekt från andra program finns i [Koppla poster](/help/quicksilver/planning/records/connect-records.md).

Ett exempel på hur du ansluter posttyper och poster finns i [Exempel på att ansluta posttyper och poster](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md).

<!--ensure this last linked article is right; the title and the link should have changed-->

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven för Workfront Planning.

Du måste ha följande för att kunna komma åt Workfront Planning:

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
   <td role="rowheader"><p>Adobe Workfront Planning*</p></td> 
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
   <td> <p>Standard</p> 
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
   <td>   <p>Hantera behörigheter till en arbetsyta </a> </p>  
   <p>Systemadministratörer har behörighet för alla arbetsytor, inklusive de som de inte skapade.</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutmall</p></td> 
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn </p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!-- OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p> Adobe Workfront Planning</p>
   <p>To connect Adobe Workfront Planning record types with Experience Manager Assets, you must have an Adobe Experience Manager Assets license and your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p> 
   <p>Current: Plan</p>
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.</p>
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

+++


## Koppla posttyper

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-planning}}

1. Klicka på arbetsytan vars posttyper du vill ansluta,

   eller

   Utöka den nedåtriktade pilen till höger om namnet på en befintlig arbetsyta i en arbetsyta, sök efter en arbetsyta och markera den när den visas i listan.
1. Klicka på kortet för en posttyp för att öppna posttypssidan.
1. Klicka på ikonen **+** i tabellvyns övre högra hörn och klicka sedan på fliken **Ny anslutning** .

   ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. I fältet **Posttyp** söker du efter en posttyp eller väljer något av följande:

   * En annan posttyp från den aktuella arbetsytan

     <span class="preview">![](assets/many-to-many-connection-picker.png)</span>
     >[!TIP]
     >
     > 
     >Om du inte har andra posttyper i den valda arbetsytan visas inte arbetsyteavsnittet.


   * En posttyp från en annan arbetsyta som konfigurerats för anslutning från andra arbetsytor. Mer information finns i [Redigera posttyper](/help/quicksilver/planning/architecture/edit-record-types.md).

     <span class="preview">![](assets/new-connection-allow-multiple-records-box.png)</span>

     >[!TIP]
     >
     >Om det inte finns några posttyper som har konfigurerats för att ansluta från andra arbetsytor visas inte arbetsyteavsnittet.


   * Ett **projekt, Portfolio, program, företag** eller **grupp** från avsnittet **Workfront-objekttyper**.

     ![](assets/workfront-project-connection-selection.png)

   * **Experience Manager Assets** från avsnittet **Adobe-program**.

     <span class="preview">![](assets/aem-assets-connection-selection.png)</span>

1. Uppdatera följande information:

   * **Namn**: Namnet på det anslutna fältet, så som det kommer att visas i tabellvyn eller på postsidan för den ursprungliga posttypen. Då skapas den länkade postkolumnen i tabellvyn för den ursprungliga posttypen eller det länkade postfältet för de ursprungliga posterna. Som standard är namnet på fältet namnet på den post eller det objekt som du ansluter till.

   >[!TIP]
   >
   >Du kan ha flera anslutningar till samma post eller objekttyp. Om du inte redigerar namnet på det anslutna fältet lägger Workfront till en siffra efter namnet på den anslutna posten för att ange antalet anslutna posttyper med samma namn.

   * **Beskrivning**: Ytterligare information om det anslutna postfältet. Beskrivningen av ett fält visas när du hovrar över fältets kolumn i en tabell.
   * **Tillåt flera poster**: Välj det här alternativet om du vill ange att du tillåter användare att lägga till flera poster när fältet för den länkade posttypen visas på de ursprungliga posterna. Detta är markerat som standard.

     Det här alternativet är endast tillgängligt när du ansluter poster från två olika arbetsytor eller en post och ett Adobe Experience Manager-resursobjekt.

     <span class="preview">![](assets/new-connection-allow-multiple-records-box.png)</span>

   * **Anslutningstyp**: Välj ett av följande alternativ för att ange hur många poster de kan ansluta till och från:

      * Många till många
      * En till många
      * Många till ett
      * En till en

     Det här alternativet är endast tillgängligt när du ansluter poster från samma arbetsyta eller en post och en Workfront-objekttyp.

     <span class="preview">![](assets/many-to-many-connection-picker.png)</span>

     Mer information om anslutningstyper finns i [Översikt över anslutna posttyper](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

   * **Välj uppslagsfält**: Välj det här alternativet om du vill lägga till fält från den valda posttypen. Uppslagsfälten är fält som är kopplade till den post eller objekttyp som du länkar till. När du länkar dem visas information från posten eller objektet som du länkar till på posten som du länkar från. Detta är markerat som standard.

     >[!TIP]
     >
     > Du kan inte lägga till följande fälttyper som sökfält:
     >
     >    * Folk
     >    * Skapad av
     >    * Senast ändrad av
     >    * Workfront typsnittsfält (inklusive fält som Projektägare eller Projektsponsor)

1. (Villkorligt och valfritt) Om du har valt att ansluta ett Workfront-objekt väljer du ett **anpassat formulär** bland **Länka endast objekt som matchar villkoren**. Endast objekt som har de markerade anpassade formulären kopplade kan länkas till den valda posttypen. Du kan markera flera formulär.

   >[!NOTE]
   >
   > Du måste skapa anpassade formulär i Workfront för de markerade objekten innan de visas i den här listan.

1. (Villkorligt) Om du valde att ansluta till Experience Manager Assets väljer du en databas i listrutan **Experience Manager-databas** i avsnittet **Länka resurser i följande databas**. Detta är ett obligatoriskt fält. Endast databaser som du har åtkomst till i Experience Manager Assets visas i det här fältet.

   >[!NOTE]
   >
   >Workfront-administratören kan mappa Workfront Planning-fält till Experience Manager Assets-fält via metadatamappningen i Workfront. Mer information finns i [Konfigurera mappning av metadata för resurser mellan Adobe Workfront och Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).

1. (Villkorligt) Om du har valt att ansluta till Experience Manager Assets eller till posttypen Workfront Planning väljer du något av följande alternativ i området **Postutseende**:

   * <span class="preview">**Namn och bild**: Både namnet och miniatyrbilden eller ikonen för de anslutna posterna visas i det anslutna postfältet. Det här är standardalternativet. </span>
   * <span class="preview">**Namn**: Endast namnet på de anslutna posterna visas i det anslutna postfältet.</span>
   * <span class="preview">**Bild**: Endast miniatyrbilden eller ikonen för de anslutna posterna visas i det anslutna postfältet.</span>

   Poster utan miniatyrbild visar istället posttypsikonen. Ett exempel på hur de anslutna posterna visas visas i området **Postutseende**.

   >[!TIP]
   >
   >    När du tillåter att flera poster länkas kan det hända att endast miniatyrbilden sparar utrymme i mindre områden, som i postvyer.
   >
   >Namnet på en post är det primära fältet i posten. Mer information finns i [Översikt över primärt fält](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >Det går inte att välja ett postutseende när du väljer Workfront-objekttyper.

1. Klicka på **Skapa**.

1. (Villkorligt) Om du valde inställningen **Välj uppslagsfält** öppnas rutan **Lägg till uppslagsfält** .

   Klicka på ikonen **+** för att lägga till fält från området **Omarkerade fält**.

   eller

   Klicka på ikonen **-** för att ta bort fält från området **Markerade fält**

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   Värdena för de anslutna fälten fylls i automatiskt när du länkar poster eller objekt.

   >[!IMPORTANT]
   >
   >    Alla som har behörighet att visa eller högre på arbetsytan kan visa informationen i de länkade fälten, oavsett behörighet eller åtkomstnivå i programmet för de länkade objekttyperna.


1. (Valfritt) Klicka på **Hoppa över** om du inte vill lägga till fält från den länkade posten eller objekttypen. Namnet eller det primära fältet för den länkade posten är det enda synliga fältet i tabellvyn för den posttyp som du ansluter från.

1. (Valfritt och villkorligt) Om du väljer att länka ett tal, en valuta, en procentandel eller ett datumtypsfält, ska du också välja ett aggregeringsvärde som ska sammanfatta flera värden. Värdena för de länkade fälten visas antingen avgränsade med kommatecken eller som ett summerat värde enligt den aggregator du väljer, när användare markerar mer än en länkad post i det länkade postfältet.

   Om sökfältet innehåller flera värden som inte är summerade bör du tänka på följande när du använder fältet för att sortera eller gruppera i en vy:

   * Sorteringen görs med det första värdet

   * Posterna grupperas efter varje unik kombination av fältvärden

   * Tidslinjevyn byggs utifrån det första datumvärdet

   >[!IMPORTANT]
   >
   >    Du måste välja ett aggregeringsvärde när du lägger till sökdatumfält om du vill att fälten ska vara tillgängliga för att lägga till som start- och slutdatum för tidslinjen och kalendervyer. Du kan till exempel välja MAX eller MIN-aggregering för ett datumsökningsfält.

   ![](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > Aggregatorer är inte tillgängliga när du ansluter posttyper till Experience Manager Assets.

   Välj bland följande:

   * **Ingen**: Visar värden som kommer från flera poster avgränsade med kommatecken. Det här är standardvalet.
   * **MAX**: Visar det högsta värdet från alla värden som kommer från flera markerade poster i det länkade postfältet.
   * **MIN**: Visar det lägsta värdet från alla värden som kommer från flera markerade poster i det länkade postfältet.
   * **SUM**: Visar summan av alla värden som kommer från flera markerade poster i det länkade postfältet.
   * **AVG**: Visar medelvärdet av alla värden som kommer från flera markerade poster i det länkade postfältet.
   * **UNIQUE**: Tar bort dubbletter från sökfältsvärden och bara visar unika värden. Detta är inte tillgängligt för följande fälttyper:
      * Stycke
      * Kryssruta
      * Folk

   >[!NOTE]
   >
   >Du kan till exempel länka produktposten (länkad post) från Campaign-posten (ursprungsposten) och ge den namnet&quot;Produktfält&quot;. Du kan också välja att länka produktpostens budgetfält från kampanjposten och kalla det&quot;Produktbudget&quot;. Om du tillät att välja flera poster i fältet&quot;Produkt&quot; kan du välja Produkt 1 med en budget på 100 000 och Produkt 2 med en budget på 110 000 och Produkt 3 med en budget på 100 000 dollar. Du kan visa följande budgetinformation i det länkade fältet från den ursprungliga posten, beroende på vilken aggregator du väljer:
   >
   >* **Ingen**: $100 000, $110 000, $100 000
   >* **MAX**: 110 000 USD
   >* **MIN**: $100 000
   >* **SUM**: 310 000 USD
   >* **AVG**: $103,000.33
   >* **UNIQUE**: $100 000
   >

1. (Valfritt) Använd ikonen **sök** ![](assets/search-icon.png) för att söka efter ett fält.

1. Klicka på **Lägg till fält** för att spara ändringarna.

   Följande objekt läggs till:

   * Ett länkat postfält på posttypen som du länkar från. Det länkade postfältet visar enskilda poster av den länkade posttypen efter att du har lagt till dem manuellt. Mer information om hur du lägger till poster finns i [Koppla poster](/help/quicksilver/planning/records/connect-records.md). Namnet på det länkade postfältet är det namn du valde i steg 6. <!--accurate-->

   * Ett länkat (eller sökbart) fält (eller fält) som visar information om den länkade posten eller objekttypen efter att du manuellt har lagt till posterna eller objekten i det länkade postfältet. Uppslagsfält skapas bara när inställningen **Välj uppslagsfält** väljs när anslutningen skapas. Uppslagsfält får automatiskt namn enligt det här mönstret:

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

     Om du t.ex. har länkat en kampanjposttyp med en programposttyp och namngett det programlänkade postfältet&quot;Programinformation&quot;, markerat för att även visa programmets budgetfält i kampanjens tabellvy, får det länkade fältet automatiskt namnet `Budget (from Program information)` i kampanjens tabellvy.

   * När du länkar posttyper till varandra läggs ett länkat postfält också till i den posttyp som du länkar till. Namnet på det länkade postfältet på den länkade posttypen är namnet på den posttyp som du länkar från.

     Om du t.ex. länkar posttypen &quot;Produkt&quot; från posttypen &quot;Kampanj&quot; och namnger det anslutna fältet i Campaign &quot;Länkad produkt&quot;, skapas ett &quot;Kampanjlänkat&quot; postfält för posttypen Produkt.

     >[!TIP]
     >
     > Ett länkat postfält skapas inte för objekt från ett annat program till den posttyp som du länkar från i Workfront Planning.

1. (Valfritt och villkorligt) Klicka på nedåtpilen i rubriken för de länkade postfälten i den ursprungliga posttypen eller i tabellvyn för den länkade posttypen och klicka sedan på något av följande:

   * **Redigera fält**: Uppdatera informationen för fältet **Namn** och **Beskrivning**.
   * **Redigera sökfält**: Lägg till eller ta bort fält för den länkade posten.

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   Följ instruktionerna i steg 16-17 ovan för att lägga till eller ta bort uppslagsfält. <!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > Du kan inte lägga till uppslagsfält som tillhör posttyper som du länkar från till objekttyper från ett annat program.
   >
   > Du kan till exempel inte lägga till sökfältet för Campaign Status till ett Workfront-projekt som du länkar till från kampanjerna.

1. (Valfritt) Klicka på nedåtpilen i huvudet för ett länkat postfält eller i huvudet för ett uppslagsfält från den posttyp som du länkar från och klicka sedan på **Ta bort**.

   Postfältet eller sökfältet tas bort. Om du tar bort ett postfält tas även uppslagsfält som är kopplade till den länkade posten bort.

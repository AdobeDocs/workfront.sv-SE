---
title: Hantera postvyer
description: Du kan visa poster i en tabell-, tidslinje- eller kalendervy när du använder Adobe Workfront Planning. I den här artikeln beskrivs hur du skapar en vy och redigerar en befintlig.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: b2f1bbfbbec23a5400552eb0f989e0a0dc58413c
workflow-type: tm+mt
source-wordcount: '1343'
ht-degree: 0%

---


# Hantera postvyer

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

{{planning-important-intro}}

När du har valt en posttyp i Adobe Workfront Planning kan du visa alla poster av den typen på olika sätt.

Du kan visa poster i vyer med flera format som ger dig flexibilitet att utforska och förstå information på det sätt som passar dig bäst. Vare sig du vill ha en strukturerad översikt, en kronologisk artikel, en datumbaserad layout eller en enkel rullningsbar lista ger varje vy ett unikt perspektiv.

Du kan visa poster i följande vyer:

* Tabell

  Mer information finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md).

* Tidslinje

  Mer information finns i [Hantera tidslinjevyn](/help/quicksilver/planning/views/manage-the-timeline-view.md).

* Kalender

  Mer information finns i [Hantera kalendervyn](/help/quicksilver/planning/views/manage-the-calendar-view.md).

* Lista

  Du kan visa poster på en postsida med en anslutning i en listvy.

  >[!IMPORTANT]
  >
  >Du kan inte använda en listvy för en lista med poster på en posttypssida. Du kan bara använda en listvy på en postsida med en kopplad post i en lista med anslutna projekt. <!--this will change-->

  Mer information finns i följande artiklar:

   * [Lägga till en sida med kopplade poster i en post](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md)
   * [Hantera listvyn](/help/quicksilver/planning/views/manage-the-list-view.md)

I den här artikeln beskrivs följande information om postvyer:

* [Skapa och redigera en vy](#create-or-edit-record-views)
* [Aktivera visningsindikatorer i realtid i en vy](#enable-the-real-time-presence-indicator-in-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->

Mer information om hur du hanterar postvyer i Workfront Planning finns i följande artiklar:

* [Ta bort postvyer](/help/quicksilver/planning/views/delete-record-views.md)
* [Duplicera postvyer](/help/quicksilver/planning/views/duplicate-record-views.md)
* [Visa](/help/quicksilver/planning/access/share-views.md)


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
<p>Alla Workfront- och Planning-paket</p>
<p>Alla arbetsflöden och alla planeringsdokument</p>
<p>Mer information om vad som ingår i respektive Workfront Planning-paket får du av Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p> Standard för att skapa och ta bort vyer</p>
   <p>Medarbetare eller högre för att uppdatera vyelement</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>   <p>Hantera behörigheter till en vy</p>  
   <p>Visa behörigheter till en vy om du tillfälligt vill ändra visningsinställningarna eller duplicera den</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> Användare med en Light- eller Contributor-licens måste tilldelas en layoutmall som innehåller Planning.
   <p>Standardanvändare och systemadministratörer har planeringsområdena aktiverade som standard.</p></div></li></ul>
</td>
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
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard to create and delete views</p>
   <p>Contributor or higher to update view elements</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings or to duplicate it</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table>-->

## Att tänka på när du arbetar med postvyer

* Vyer i Workfront Planning är posttypsspecifika. Du kan inte använda samma vy för två olika posttyper.
* Vyer som du skapar visas bara för dig och de användare som du delar vyerna med.
* När du ändrar eller tar bort en vy ändras den och tas bort för alla användare som har behörighet till vyn.
* Varje användare kan skapa högst 100 vyer. Du kan visa mer än 100 vyer för en posttyp, men en användare kan bara skapa 100 vyer.
* Vissa vyelement kan användas på flera vyer för samma post, men de är unika för varje postvy:

   * Filter
   * Sortera (för tabellvyn)
   * Radfärger (för tabellvyn)
   * Fält (för tabellvyn)
   * Uppdelning (för tidslinjevyn)
   * Gruppering (för tabellen och tidslinjevyerna)
   * Stolputseende (för tidslinjen och kalendervyer)
   * Radhöjd (för tabellen och den månatliga kalendervyn)

  När du till exempel skapar ett filter i en tabellvy visas filterresultaten bara i den markerade vyn (tabellvyn) och inte i alla vyer som är kopplade till posttypen.

  >[!TIP]
  >
  >Vissa vyelement är inte tillgängliga för alla vyer.


## Likheter och skillnader mellan postvyer

I följande tabell visas likheter och skillnader mellan tabell-, tidslinje- och kalendervyer:

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Funktion | Tabellvy | Tidslinjevy | Kalendervy | Listvy |
|-----------------------------------------------------------------------|------------|---------------|--------------|---------|
| Visa poster i ett tabellformat | ✓ |              | | ✓ |
| Visa alla fält som kolumner i en tabell eller lista | ✓ |              |    | ✓ |
| Dölj eller visa fält (eller kolumner) | ✓ |               |    | ✓ |
| Redigera fältvärden för varje post | ✓ |               |             | ✓ |
| Lägga till poster som nya rader i vyn | ✓ |               |        | ✓ |
| Lägga till fält som nya kolumner i vyn | ✓ |               |         | ✓ |
| Kopiera rader från en extern lista och klistra in dem i en tabell | ✓ |               |          | ✓ |
| Visa poster på en tidslinje |            | ✓ |             |  |
| Filtrera poster | ✓ | ✓ | ✓ | ✓ |
| Visa poster i en kalender |           |              | ✓ |  |
| Gruppposter | ✓ | ✓ |  |  |
| Sortera poster | ✓ |              |  | ✓ |
| Färgkodsposter | ✓ | ✓ | ✓ |  |
| Färgkodsgrupperingar |           | ✓ |  |  |
| Sök efter specifika poster | ✓ | ✓ |  | ✓ |
| Dela vyn med andra | ✓ | ✓ | ✓ | ✓ |
| Öppna postens sida från vyn | ✓ | ✓ |    | ✓ |
| Visa poster per år och kvartal |           | ✓ |    |  |
| Visa poster per månad |           | ✓ | ✓ |  |
| Visa poster per vecka |           |               | ✓ |  |
| Exportera information från en vy | ✓ |               |    |  |
| Visa i helskärmsläge | ✓ | ✓ | ✓ |  |
| Skapa poster i vyn | ✓ | ✓ | ✓ | ✓ |
| Dela upp poster efter deras anslutningar |          | ✓ |    |  |

## Skapa eller redigera vyer {#create-or-edit-views}

Informationen i det här avsnittet gäller följande vytyper:

* Tabell
* Tidslinje
* Kalender

Mer information om listvyer finns i [Hantera listvyn](/help/quicksilver/planning/views/manage-the-list-view.md).

{{step1-to-planning}}


1. Klicka på kortet för en arbetsyta.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett posttypskort.

   Posttypssidan öppnas.

   Som standard visas alla poster av den valda typen i tabellvyn.

1. Klicka på listruteikonen ![listruteikonen](assets/drop-down-icon.png) bredvid den aktuella vyns namn och klicka sedan på **+Ny vy**.

1. Välj bland följande typer av vyer:

   * Tabell
   * Tidslinje
   * Kalender

1. Välj en visningstyp och klicka sedan på **Skapa**. En ny vy läggs till i listrutan.

   >[!TIP]
   >
   >När du skapar en posttyp skapas även tabellvyn som standard.
   >
   >Om du vill skapa en tidslinje eller en kalendervy måste posttypen som du skapar vyn för ha minst två datumfält.
   >
   >I annat fall är tidslinjen och kalenderalternativen nedtonade.
   >  

   ![Skapa visningsruta](assets/create-view-box.png)

1. (Valfritt) Om du vill redigera en befintlig vy klickar du på den nedrullningsbara menyn till höger om den aktuella vyns namn, skriver namnet på en vy i fältet **Sök** och trycker på Retur på tangentbordet.
1. (Valfritt) Dra och släpp vyer i den ordning du vill ha dem från den nedrullningsbara menyn.

   ![Listrutan Visa typer från posttypslistan](assets/view-types-drop-down-from-record-type-list.png)

1. (Villkorligt) Klicka på **Nästa** när du skapar en tidslinje eller kalendervy.

   Som standard ger Workfront vyn ett av följande namn:

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   Talet är ett automatiskt genererat steg.

1. (Villkorligt) Markera **Start** och **Slutdatum** för posterna som ska visas i tidslinjen eller kalendervyn.

   >[!NOTE]
   >
   >    Du kan välja från postdatumfält eller uppslagsdatumfält från anslutna post- eller objekttyper.
   >
   >Du måste använda aggregerare för datumfält (MAX eller MIN) när du väljer sökfält när du ansluter posttyper. Om du bara lägger till aggregatorerna kan du använda anslutningsdatumen som start- och slutdatum för tidslinjen och kalendervyer.
   >
   >Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Klicka på **Skapa**.

   Vyn visas som en ny flik. Vyer visas i den kronologiska ordning som de skapades eller delades med dig.
1. (Valfritt) Klicka på **Mer**-menyn ![Fler vyer med nedåtriktade ikoner](assets/more-caret-down-icon-views.png) bredvid den senaste vyn om du vill visa alla vyer för den valda posttypen.

   Ytterligare vyer visas på menyn **Mer** efter fliken för den senaste vyn. Siffran bredvid menyn **Mer** visar antalet ytterligare vyer.
1. (Valfritt) Om du vill byta namn på en vy efter att den har skapats klickar du på listrutan Visa och sedan på menyn **Mer** ![Mer ](assets/more-menu.png) > **Byt namn** för att uppdatera visningsnamnet

   eller

   Dubbelklicka på vynamnet och börja skriva det nya namnet.  <!--ensure there is not another saving step here?!-->

1. (Valfritt) Klicka på ikonen **Helskärm** ![Öppna helskärmsikonen](assets/open-full-screen-icon.png) om du vill öppna en vy i helskärmsläge och sedan **Avsluta helskärmsikonen** ![Avsluta helskärmsikonen](assets/exit-full-screen-icon.png) eller Esc på tangentbordet om du vill avsluta helskärmsläget.

1. (Valfritt) Mer information om hur du hanterar en viss typ av vy finns i följande artiklar:

   * [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md)
   * [Hantera tidslinjevyn](/help/quicksilver/planning/views/manage-the-timeline-view.md)
   * [Hantera kalendervyn](/help/quicksilver/planning/views/manage-the-calendar-view.md)

## Aktivera närvaroindikatorn i realtid i en vy

Du kan se om andra användare redigerar poster samtidigt som du genom att följa visningsindikatorerna i realtid i vyn.

>[!NOTE]
>
>Du kan inte visa visningsindikatorer i realtid i en listvy.

Avatarerna för andra användare som redigerar postinformation samtidigt som du visar i det övre högra hörnet av alla postvyer, som standard.

När du visar tabellvyn kan du även visa vilket fält en annan användare redigerar när du visar posten.

Mer information finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md).



<!--## Add a view as a favorite - this is not possible yet-->

---
title: Hantera postvyer
description: Du kan visa poster i en tabell-, tidslinje- eller kalendervy när du använder Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: 6ec985d10a5fd7a4a9307b705f48734d76aec181
workflow-type: tm+mt
source-wordcount: '1091'
ht-degree: 0%

---

# Hantera postvyer

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

När du har valt en posttyp i Adobe Workfront Planning kan du visa alla poster av den typen i följande vyer:

* Tabell

  Mer information finns i [Hantera tabellvyn](../views/manage-the-table-view.md).

* Tidslinje

  Mer information finns i [Hantera tidslinjevyn](../views/manage-the-timeline-view.md).

* Kalender

  Mer information finns i [Hantera kalendervyn](/help/quicksilver/maestro/views/manage-the-calendar-view.md).

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
<p>Din organisation måste vara registrerad i betaprogrammet Adobe Workfront Planning closed. Kontakta din kontorepresentant om du vill veta mer om det nya erbjudandet. </p>
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
   <td> <p>Det finns inga åtkomstnivåkontroller för Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Hantera behörigheter till vyn</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Layoutmall</td>
   <td> <p>Systemadministratören måste lägga till planeringsområdet i layoutmallen. Mer information finns i <a href="../access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## Att tänka på när du arbetar med postvyer

* Vyer i Workfront Planning är posttypsspecifika. Du kan inte använda samma vy för två olika posttyper.
* Vyer som du skapar visas bara för dig och de användare som du delar vyerna med.
* När du ändrar eller tar bort en vy ändras den och tas bort för alla användare som har behörighet till vyn.
<!--* Each user can create a maximum of 100 views. -->
* Följande element är unika för varje postvy:

   * Filter
   * Gruppering
   * Sortera
   * Stolputseende (för tidslinjevyn)

  <!-- some of these are not available in all of the views - edit above-->

  När du till exempel skapar ett filter i en tabellvy visas filterresultaten bara i den markerade vyn och inte i alla vyer som är kopplade till posttypen.

  >[!NOTE]
  >
  > Eftersom Adobe Workfront Planning för närvarande är en betaversion, kanske vissa vyelement inte är tillgängliga för alla vyer.

I den här artikeln beskrivs följande information om postvyer:

* [Skapa och redigera en vy](#create-or-edit-record-views)
* [Ta bort en vy](#delete-views)
* [Duplicera en vy](#duplicate-views)
* [Dela en vy](#share-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->

## Likheter och skillnader mellan postvyer

I följande tabell visas likheter och skillnader mellan tabell-, tidslinje- och kalendervyer:

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Funktion | Tabellvy | Tidslinjevy | Kalendervy |
|-----------------------------------------------------------------------|------------|---------------|--------------|
| Visa poster i en lista eller tabell | ✓ |              | |
| Visa alla fält som kolumner i tabellen som standard | ✓ |              |    |
| Dölj eller visa fält (eller kolumner) | ✓ |               |    |
| Redigera fältvärden för varje post | ✓ |               |             |
| Lägga till poster som nya rader i vyn | ✓ |               |        |
| Lägga till fält som nya kolumner i vyn | ✓ |               |         |
| Kopiera rader från en extern lista och klistra in dem i en tabell | ✓ |               |          |
| Visa poster på en tidslinje |            | ✓ |             |
| Filtrera poster | ✓ | ✓ | ✓ |
| Visa poster i en kalender |           |              | ✓ |
| Gruppposter | ✓ | ✓ |
| Sortera poster | ✓ |              |
| Färgkodsposter |           | ✓ | ✓ |
| Färgkodsgrupperingar |           | ✓ |
| Sök efter specifika poster | ✓ | ✓ |
| Dela vy | ✓ | ✓ | ✓ |
| Öppna postens sida från vyn | ✓ | ✓ |    |


## Skapa eller redigera vyer {#create-or-edit-views}

{{step1-to-maestro}}


Arbetsytan som du senast öppnade öppnas som standard. Mer information om hur du skapar arbetsytor finns i [Skapa arbetsytor](../architecture/create-workspaces.md).

1. Klicka på ett posttypskort. Mer information om hur du skapar en posttyp finns i [Skapa posttyper](../architecture/create-record-types.md).

   Som standard visas alla poster av den valda typen i tabellvyn.

1. Klicka **+ Visa** för att lägga till en ny vy.
1. Välj bland följande typer av vyer:

   * Tabell
   * Tidslinje
   * Kalender

   En ny flik skapas med den valda vyn.

   Beroende på skärmens bredd kan ytterligare vyer visas i **Mer** meny ![](assets/more-menu.png).


>[!TIP]
>
>När du skapar en posttyp skapas även tabellvyn som standard.
>
>Om du vill skapa en tidslinje eller en kalendervy måste posttypen som du skapar vyn för ha minst två datumfält. I annat fall är tidslinjen och kalenderalternativen nedtonade.
>

![](assets/view-types-drop-down-from-record-type-list.png)

>[!NOTE]
>
>    Om du vill skapa en tidslinje eller en kalendervy måste posttypen som du skapar vyn för ha minst två datumfält. I annat fall är tidslinjen eller kalenderalternativen nedtonade.

1. (Villkorligt) Klicka **Nästa** när du skapar en tidslinje eller kalendervy.

   Som standard ger Workfront vyn ett av följande namn:

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   Talet är ett automatiskt genererat steg.

1. (Villkorligt) Välj **Starta** och **Slutdatum** för de poster som ska visas i tidslinjen eller kalendervyn.
1. Klicka **Skapa**.

   Vyn visas som en ny flik. Vyer visas i den kronologiska ordning som de skapades eller delades med dig.
1. (Valfritt) Klicka på **Mer** meny ![](assets/more-caret-down-icon-views.png) bredvid den sista vyn om du vill visa alla vyer för den valda posttypen.

   Fler vyer visas under **Mer** efter den sista vyfliken. Talet bredvid **Mer** visas antalet ytterligare vyer.
1. (Valfritt) Om du vill byta namn på en vy efter att den har skapats klickar du på listrutan Visa och sedan på **Mer** meny ![](assets/more-menu.png) > **Byt namn** för att uppdatera vynamnet

   eller

   Dubbelklicka på vynamnet och börja skriva det nya namnet.  <!--ensure there is not another saving step here?!-->

1. (Valfritt) Mer information om hur du hanterar en viss typ av vy finns i följande artiklar:

   * [Hantera tabellvyn](../views/manage-the-table-view.md)
   * [Hantera tidslinjevyn](../views/manage-the-timeline-view.md)
   * [Hantera kalendervyn](/help/quicksilver/maestro/views/manage-the-calendar-view.md)


## Ta bort vyer

{{step1-to-maestro}}

Arbetsytan som du senast öppnade öppnas som standard. Mer information om hur du skapar arbetsytor finns i [Skapa arbetsytor](../architecture/create-workspaces.md).

1. Klicka på ett posttypskort.

   Mer information om hur du skapar en posttyp finns i [Skapa posttyper](../architecture/create-record-types.md).

   Som standard visas alla poster av den valda typen i tabellvyn.

1. Håll muspekaren över ett av vyns namn på fliken Visa och klicka sedan på **Mer** ![](assets/more-menu.png) till vänster om vynamnet och klicka sedan på **Ta bort**.
Först kan du behöva klicka **Mer** till vänster om den sista fliken för att hitta vyn som du vill ta bort.

1. Klicka **Ta bort** för att bekräfta. <!--ensure there is not another saving step here?!-->

   Vyn tas bort för alla användare som har åtkomst till postområdet och kan inte återställas.

## Dela en vy

Mer information om att dela vyer finns i [Visa](/help/quicksilver/maestro/access/share-views.md).

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: -->

## Duplicera en vy

Om du vill behålla flera versioner av en vy och göra mindre ändringar mellan versionerna, kan du duplicera en vy.

När du duplicerar en vy skapas identiska kopior av en befintlig vy.

Delningsbehörigheterna för den ursprungliga vyn överförs inte till den duplicerade vyn.

{{step1-to-maestro}}

Arbetsytan som du senast öppnade öppnas som standard.

Mer information om hur du skapar arbetsytor finns i [Skapa arbetsytor](../architecture/create-workspaces.md).

1. Klicka på ett posttypskort. Mer information om hur du skapar en posttyp finns i [Skapa posttyper](../architecture/create-record-types.md).

   Som standard visas alla poster av den valda typen i tabellvyn.

1. Håll pekaren över fliken för den vy du vill duplicera och klicka på knappen **Mer** meny ![](assets/more-menu.png) till höger om vynamnet och klicka sedan på **Duplicera**.

   ![](assets/view-more-menu-with-duplicate-option.png)


   Vyn dupliceras och den nya vyns namn följer följande mönster: `Original view's name (Copy)`. Fliken Ny vy visas i slutet av alla visningsflikar.


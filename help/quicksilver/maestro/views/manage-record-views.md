---
title: Hantera postvyer
description: Du kan visa poster i en tabell eller i en tidslinjevy när du använder Adobe Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: ff52e43fc5ed5a7939b9e28b2bda195e94e81724
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 0%

---

# Hantera postvyer

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

När du har valt en posttyp i Adobe Maestro kan du visa alla poster av den typen i följande vyer:

* Tabell

  Mer information finns i [Hantera tabellvyn](../views/manage-the-table-view.md).
* Tidslinje

  Mer information finns i [Hantera tidslinjevyn](../views/manage-the-timeline-view.md).

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
   <td> <p>Det finns inga åtkomstnivåkontroller för Maestro</p>  
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

## Att tänka på när du arbetar med maestro-vyer

* Vyer i maestro är posttypsspecifika. Du kan inte använda samma vy för två olika posttyper.
* Vyer som du skapar visas bara för dig och de användare som du delar vyerna med.
* Att skapa vyer för driftsposttyper är identiskt med att bygga vyer för taxonomiposttyper.
* När du ändrar eller tar bort en vy ändras den och tas bort för alla användare som har behörighet till vyn.
* Följande element är unika för varje vy i Maestro:

   * Filter
   * Gruppering
   * Sortera

  <!-- some of these are not available in all of the views - edit above-->

  När du till exempel skapar ett filter i en tabellvy visas filterresultaten bara i den markerade vyn och inte i alla vyer som listas i listrutan Visa.

  >[!NOTE]
  >
  > Eftersom Maestro för närvarande är i betaversion är vissa vyelement kanske inte tillgängliga för båda vyerna.

I den här artikeln beskrivs följande information om maestro-vyer:

* [Skapa och redigera en vy](#create-or-edit-record-views)
* [Ta bort en vy](#delete-views)
  <!--* [Duplicate a view](#duplicate-views)-->
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->
* [Dela en vy](#share-a-view)

## Likheter och skillnader mellan tabell- och tidslinjevyerna

I följande tabell visas likheter och skillnader mellan tabell- och tidslinjevyerna i Maestro:

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Funktion | Tabellvy | Tidslinjevy |
|-----------------------------------------------------------------------|------------|---------------|
| Visa poster i en lista eller tabell | ✓ |              |
| Visa alla fält som kolumner i tabellen som standard | ✓ |              |
| Dölj eller visa fält (eller kolumner) | ✓ |               |
| Redigera fältvärden för varje post | ✓ |               |
| Lägga till poster som nya rader i vyn | ✓ |               |
| Lägga till fält som nya kolumner i vyn | ✓ |               |
| Kopiera rader från en extern lista och klistra in dem i en tabell | ✓ |               |
| Visa poster på en tidslinje |            | ✓ |
| Filtrera poster | ✓ | ✓ |
| Gruppposter | ✓ | ✓ |
| Sortera poster | ✓ |              |
| Färgkodsposter |           | ✓ |
| Färgkodsgrupperingar |           | ✓ |
| Sök efter specifika poster | ✓ | ✓ |
| Dela vy | ✓ | ✓ |
| Öppna postens informationssida från vyn | ✓ | ✓ |

## Skapa eller redigera vyer {#create-or-edit-views}

{{step1-to-maestro}}


Arbetsytan som du senast öppnade öppnas som standard. Mer information om hur du skapar arbetsytor finns i [Skapa arbetsytor](../architecture/create-workspaces.md).

1. Klicka på ett posttypskort. Mer information om hur du skapar en posttyp finns i [Skapa posttyper](../architecture/create-record-types.md).

   Som standard visas alla poster av den valda typen i tabellvyn.

<!--
    1. Click **+ View** to add a new view. 

    1. Select from the following types of views: 

        * Table
        * Timeline
        * Calendar

        >[!TIP]
        >
        >When you create a record type, the table view is also created by default. 
        >
        >To create a timeline or a calendar view, the record type you build the view for must have at least two date fields. Otherwise, the Timeline and the Calendar options are dimmed.
        >
        >(*********remove all of the below steps and replace the screen shot when calendar view releases*********)
    -->

1. Klicka på **Visa** och välj en befintlig **Tabellvy** ![](assets/table-view-icon.png) eller klicka **Skapa vy > Tabell** skapa en tabellvy

   eller

   Välj en befintlig **Tidslinjevy** ![](assets/timeline-view-icon.png) visa eller klicka **Skapa vy > Tidslinje** för att skapa en tidslinjevy.

   ![](assets/view-types-drop-down-from-record-type-list.png)

   >[!NOTE]
   >
   >    Om du vill skapa en tidslinjevy måste posttypen som du skapar vyn för ha minst två datumfält. I annat fall är alternativet Tidslinje nedtonat.

1. (Valfritt) Uppdatera namnet på vyn och klicka sedan på **Skapa** spara en tabellvy

   Eller klicka **Nästa** när du skapar en tidslinje <!--or calendar--> vy.

   Som standard får vyn namnet &quot;Tabell &lt; nummer >&quot; eller &quot;Tidslinje &lt; nummer >&quot;. Talet är ett automatiskt genererat steg.

1. (Villkorligt) Välj start- och slutdatum för posterna som ska visas på tidslinjen <!--or calendar--> visa och sedan klicka **Skapa**.
1. (Valfritt) Om du vill byta namn på en vy efter att den har skapats klickar du på listrutan Visa och sedan på **Mer** meny ![](assets/more-menu.png) > **Byt namn** för att uppdatera vynamnet. <!--ensure there is not another saving step here?!-->
   <!--1. (Optional) To rename a view after it is created, double-click the view name and start typing the new name, or click the **More** menu ![](assets/more-menu.png) to the right of the view name, then click **Rename**.-->
1. (Valfritt) Mer information om hur du hanterar en viss typ av vy finns i följande artiklar:

   * [Hantera tabellvyn](../views/manage-the-table-view.md)
   * [Hantera tidslinjevyn](../views/manage-the-timeline-view.md)
     <!--* [Manage the calendar view](/help/quicksilver/maestro/views/manage-the-calendar-view.md)-->


## Ta bort vyer

{{step1-to-maestro}}

Arbetsytan som du senast öppnade öppnas som standard. Mer information om hur du skapar arbetsytor finns i [Skapa arbetsytor](../architecture/create-workspaces.md).

1. Klicka på ett posttypskort.

   Mer information om hur du skapar en posttyp finns i [Skapa posttyper](../architecture/create-record-types.md).

   Som standard visas alla poster av den valda typen i tabellvyn.

<!--1. Hover over on the of the view's names in the view tab, then click **More** ![](assets/more-menu.png) > **Delete**. (********delete the instructions below but keep the last step***********)-->
1. Klicka på den nedrullningsbara menyn för vyn, håll markören över en av vyerna i listan och klicka sedan på **Mer** meny ![](assets/more-menu.png) > **Ta bort**.
1. Klicka **Ta bort** för att bekräfta. <!--ensure there is not another saving step here?!-->

   Vyn tas bort för alla användare som har åtkomst till Maestro-området och kan inte återställas.

## Dela en vy

Mer information om att dela vyer finns i [Visa](/help/quicksilver/maestro/access/share-views.md).

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: 

## Duplicate views

If you want to keep multiple versions of a view and make slight changes between the version, you can duplicate a view. Duplicating a view creates identical copies of an existing view. 

1. From the **Main Menu**, click **Maestro**. 
    The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture/create-workspaces.md).
1. Click a record type. For information about creating a record type, see [Create record types](../architecture/create-record-types.md). 

    By default, all the records of the type selected display in the table view. 

1. Click the view drop-down menu, then click the **More** menu ![](assets/more-menu.png) to the right of the view name > **Duplicate**. (**********ensure there is not another saving step here?! also, add how this view is named; the button to duplicate was there but not the functionality yet************)
    
    The view is duplicated and visible to all users who can access the Maestro area. 

-->

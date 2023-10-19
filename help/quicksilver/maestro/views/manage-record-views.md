---
title: Hantera postvyer
description: Du kan visa poster i en tabell eller i en tidslinjevy när du använder Adobe Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: 89d590551ffbd23b357f5697163fa56651f294fb
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 0%

---

# Hantera postvyer

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>Informationen i den här artikeln handlar om Adobe Maestro, ett nytt erbjudande från Adobe.
>
>För närvarande ingår Adobe Maestro i ett betaprogram som är öppet för ett begränsat antal kunder.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.
>
>Mer information finns i [Adobe Maestro - översikt](../maestro-overview.md).

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

## Att tänka på när du arbetar med maestro-vyer

* Vyer i maestro är posttypsspecifika. Du kan inte använda samma vy för två olika posttyper.
* Vyer som du skapar är synliga för alla som kommer åt Maestro-området. <!-- edit this when we have permissions and the views will be shared only to be visible by others-->
  <!-- this is not yet possible: * You can share views with others if you want them to also apply them to the same record types.-->
* Att skapa vyer för driftsposttyper är identiskt med att bygga vyer för taxonomiposttyper.
* När du ändrar eller tar bort en vy ändras den och tas bort för alla användare som har åtkomst till Maestro-området.
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
  <!--* [Share a view](#share-views) - not possible yet-->

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
| Gruppposter |           | ✓ |
| Sortera poster | ✓ |              |
| Färgkodsposter |           | ✓ |
| Färgkodsgrupperingar |           | ✓ |

<!--| Sort groupings                                                        | ✓          | ✓             |-->
<!--| Display a limited number of fields as columns, by default                      | ✓          |               |-->

## Skapa eller redigera vyer {#create-or-edit-views}

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-workfront.png) längst upp till höger <!--or the **Main Menu** icon ![](assets/main-menu-shell.png) in the upper-left corner, if available-->och sedan klicka **Maestro** ![](assets/maestro-icon.png).
Arbetsytan som du senast öppnade öppnas som standard. Mer information om hur du skapar arbetsytor finns i [Skapa arbetsytor](../architecture-and-fields/create-workspaces.md).
1. Klicka på ett posttypskort. Mer information om hur du skapar en posttyp finns i [Skapa posttyper](../architecture-and-fields/create-record-types.md).

   Som standard visas alla poster av den valda typen i tabellvyn.

1. Klicka på **Visa** och välj en befintlig **Tabellvy** ![](assets/table-view-icon.png) eller klicka **Skapa vy > Tabell** skapa en tabellvy

   eller

   Välj en befintlig **Tidslinjevy** ![](assets/timeline-view-icon.png) visa eller klicka **Skapa vy > Tidslinje** för att skapa en tidslinjevy.

   ![](assets/view-types-drop-down-from-record-type-list.png)

   >[!NOTE]
   >
   >    Om du vill skapa en tidslinjevy måste posttypen som du skapar vyn för ha minst två datumfält. I annat fall är alternativet Tidslinje nedtonat.

1. (Valfritt) Uppdatera namnet på vyn och klicka sedan på **Skapa** för att spara den.

   Som standard får vyn namnet &quot;Tabell &lt; nummer >&quot; eller &quot;Tidslinje &lt; nummer >&quot;. Talet är ett automatiskt genererat steg.

1. (Valfritt) Om du vill byta namn på en vy efter att den har skapats klickar du på listrutan Visa och sedan på **Mer** meny ![](assets/more-menu.png) > **Byt namn** för att uppdatera vynamnet. <!--ensure there is not another saving step here?!-->
1. (Valfritt) Mer information finns i följande artiklar om du vill hantera en vy:

   * [Hantera tabellvyn](../views/manage-the-table-view.md)
   * [Hantera tidslinjevyn](../views/manage-the-timeline-view.md)


<!--# Add a view as a favorite - this is not possible yet-->

<!-- ## Share views - not possible yet-->

## Ta bort vyer

1. Från **Huvudmeny** ![](assets/main-menu-workfront.png) i skärmens övre högra hörn <!--or the **Main Menu** ![](assets/main-menu-shell.png) in the upper-left corner of the screen, if available,--> klicka **Maestro** ![](assets/maestro-icon.png).

   Arbetsytan som du senast öppnade öppnas som standard. Mer information om hur du skapar arbetsytor finns i [Skapa arbetsytor](../architecture-and-fields/create-workspaces.md).
1. Klicka på ett posttypskort.

   Mer information om hur du skapar en posttyp finns i [Skapa posttyper](../architecture-and-fields/create-record-types.md).

   Som standard visas alla poster av den valda typen i tabellvyn.

1. Klicka på den nedrullningsbara menyn för vyn, håll markören över en av vyerna i listan och klicka sedan på **Mer** meny ![](assets/more-menu.png) > **Ta bort**.
1. Klicka **Ta bort** för att bekräfta. <!--ensure there is not another saving step here?!-->

   Vyn tas bort för alla användare som har åtkomst till Maestro-området och kan inte återställas.

<!--not possible yet - August 30, 2023: 

## Duplicate views

If you want to keep multiple versions of a view and make slight changes between the version, you can duplicate a view. Duplicating a view creates identical copies of an existing view. 

1. From the **Main Menu**, click **Maestro**. 
    The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture-and-fields/create-workspaces.md).
1. Click a record type. For information about creating a record type, see [Create record types](../architecture-and-fields/create-record-types.md). 

    By default, all the records of the type selected display in the table view. 

1. Click the view drop-down menu, then click the **More** menu ![](assets/more-menu.png) to the right of the view name > **Duplicate**. (**********ensure there is not another saving step here?! also, add how this view is named; the button to duplicate was there but not the functionality yet************)
    
    The view is duplicated and visible to all users who can access the Maestro area. 

-->

---
title: Hantera postvyer
description: Du kan visa poster i en tabell-, tidslinje- eller kalendervy när du använder Adobe Workfront Planning. I den här artikeln beskrivs hur du skapar en vy och redigerar en befintlig.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '1177'
ht-degree: 0%

---


# Hantera postvyer

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

När du har valt en posttyp i Adobe Workfront Planning kan du visa alla poster av den typen i följande vyer:

* Tabell

  Mer information finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md).

* Tidslinje

  Mer information finns i [Hantera tidslinjevyn](/help/quicksilver/planning/views/manage-the-timeline-view.md).

* Kalender

  Mer information finns i [Hantera kalendervyn](/help/quicksilver/planning/views/manage-the-calendar-view.md).

I den här artikeln beskrivs följande information om postvyer:

* [Skapa och redigera en vy](#create-or-edit-record-views)
* [Aktivera visningsindikatorer i realtid i en vy](#enable-the-real-time-presence-indicator-in-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->

Mer information om hur du hanterar postvyer i Workfront Planning finns i följande artiklar:

* [Ta bort postvyer](/help/quicksilver/planning/views/delete-record-views.md)
* [Duplicera postvyer](/help/quicksilver/planning/views/duplicate-record-views.md)
* [Visa](/help/quicksilver/planning/access/share-views.md)


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
<p>Din organisations instans av Workfront måste vara registrerad på Adobe Unified Experience för att få tillgång till Workfront Planning.</p> 
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
   <p>Visa behörigheter till en vy om du tillfälligt vill ändra visningsinställningarna eller duplicera den</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutmall</p></td> 
   <td> <p>I produktionsmiljön måste alla användare, inklusive systemadministratörer, tilldelas en layoutmall som innehåller Planning.</p>
<p><span class="preview">I förhandsvisningsmiljön har standardanvändare och systemadministratörer Planering aktiverat som standard.</span></p></td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på när du arbetar med postvyer

* Vyer i Workfront Planning är posttypsspecifika. Du kan inte använda samma vy för två olika posttyper.
* Vyer som du skapar visas bara för dig och de användare som du delar vyerna med.
* När du ändrar eller tar bort en vy ändras den och tas bort för alla användare som har behörighet till vyn.
* Varje användare kan skapa högst 100 vyer. Du kan visa mer än 100 vyer för en posttyp, men en användare kan bara skapa 100 vyer.
* Vissa vyelement kan användas på flera vyer för samma post, men de är unika för varje postvy:

   * Filter
   * Gruppering (för tabellen och tidslinjevyerna)
   * Stolputseende (för tidslinjen och kalendervyer)

  När du till exempel skapar ett filter i en tabellvy visas filterresultaten bara i den markerade vyn (tabellvyn) och inte i alla vyer som är kopplade till posttypen.

  >[!TIP]
  >
  >Vissa vyelement är inte tillgängliga för alla vyer.


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
| <span class="preview">Färgkodsposter</span> | <span class="preview">✓</span> | ✓ | ✓ |
| Färgkodsgrupperingar |           | ✓ |
| Sök efter specifika poster | ✓ | ✓ |
| Dela vyn med andra | ✓ | ✓ | ✓ |
| Öppna postens sida från vyn | ✓ | ✓ |    |
| Visa poster per år och kvartal |           | ✓ |    |
| Visa poster per månad |           | ✓ | ✓ |
| Visa poster per vecka |           |               | ✓ |
| <span class="preview">Exportera information från en vy</span> | <span class="preview">✓</span> |               |    |


## Skapa eller redigera vyer {#create-or-edit-views}

{{step1-to-planning}}


1. Klicka på kortet för en arbetsyta.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett posttypskort.

   Posttypssidan öppnas.

   Som standard visas alla poster av den valda typen i tabellvyn.

1. Klicka på **+ Visa** för att lägga till en ny vy.
1. Välj bland följande typer av vyer:

   * Tabell
   * Tidslinje
   * Kalender

   En ny flik skapas med den valda vyn.

   Beroende på skärmens bredd kan ytterligare vyer visas på menyn **Mer** ![Mer](assets/more-menu.png).


>[!TIP]
>
>När du skapar en posttyp skapas även tabellvyn som standard.
>
>Om du vill skapa en tidslinje eller en kalendervy måste posttypen som du skapar vyn för ha minst två datumfält.
>
>I annat fall är tidslinjen och kalenderalternativen nedtonade.
>

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

1. (Valfritt) Mer information om hur du hanterar en viss typ av vy finns i följande artiklar:

   * [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md)
   * [Hantera tidslinjevyn](/help/quicksilver/planning/views/manage-the-timeline-view.md)
   * [Hantera kalendervyn](/help/quicksilver/planning/views/manage-the-calendar-view.md)

## Aktivera närvaroindikatorn i realtid i en vy

Du kan se om andra användare redigerar poster samtidigt som du genom att följa visningsindikatorerna i realtid i vyn.

Avatarerna för andra användare som redigerar postinformation samtidigt som du visar i det övre högra hörnet av alla postvyer, som standard.

När du visar tabellvyn kan du även visa vilket fält en annan användare redigerar när du visar posten.

Mer information finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md).



<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: -->

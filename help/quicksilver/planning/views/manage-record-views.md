---
title: Hantera postvyer
description: Du kan visa poster i en tabell-, tidslinje- eller kalendervy när du använder Adobe Workfront Planning. I den här artikeln beskrivs hur du skapar en vy och redigerar eller tar bort en befintlig vy.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '1533'
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
* [Ta bort en vy](#delete-views)
* [Duplicera en vy](#duplicate-views)
* [Aktivera visningsindikatorer i realtid i en vy](#enable-the-real-time-presence-indicator-in-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->


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
* Du kan dela vyer som du skapar med andra. Mer information finns i [Dela vyer](/help/quicksilver/planning/access/share-views.md).
* Följande element är unika för varje postvy:

   * Filter
   * Gruppering
   * Sortera
   * Stolputseende (för tidslinjevyn)

  <!-- some of these are not available in all of the views - edit above-->

  När du till exempel skapar ett filter i en tabellvy visas filterresultaten bara i den markerade vyn och inte i alla vyer som är kopplade till posttypen.

  >[!NOTE]
  >
  > Vissa vyelement kanske inte är tillgängliga för alla vyer.


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
| Dela vyn med andra | ✓ | ✓ | ✓ |
| Öppna postens sida från vyn | ✓ | ✓ |    |
| Visa poster per år och kvartal |           | ✓ |    |
| Visa poster per månad |           | ✓ | ✓ |
| Visa poster per vecka |           |               | ✓ |


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

   >[!TIP]
   >
   >    Du kan välja från postdatumfält eller uppslagsdatumfält från anslutna post- eller objekttyper. Du måste använda aggregerare för datumfält (MAX eller MIN) när du väljer uppslagsfält som start- och slutdatum för tidslinjen och kalendervyer. Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).

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


## Ta bort vyer

{{step1-to-planning}}

1. Klicka på kortet för en arbetsyta.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett posttypskort.

   Posttypssidan öppnas.

   Som standard visas alla poster av den valda typen i tabellvyn.

1. Håll markören över ett av vynamnen på fliken Visa, klicka sedan på **Mer** ![Mer-menyn](assets/more-menu.png) till vänster om vynamnet och klicka sedan på **Ta bort**.
Först kan du behöva klicka på **Mer** till vänster om den sista fliken för att hitta vyn som du vill ta bort.

1. Bekräfta genom att klicka på **Ta bort**. <!--ensure there is not another saving step here?!-->

   Vyn tas bort för alla användare som har åtkomst till postområdet och kan inte återställas.

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: -->

## Duplicera en vy

Om du vill behålla flera versioner av en vy och göra mindre ändringar mellan versionerna, kan du duplicera en vy.

När du duplicerar en vy skapas identiska kopior av en befintlig vy.

Delningsbehörigheterna för den ursprungliga vyn överförs inte till den duplicerade vyn.

{{step1-to-planning}}

1. Klicka på kortet för en arbetsyta.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett posttypskort.

   Posttypssidan öppnas.
Som standard visas alla poster av den valda typen i tabellvyn.

1. Håll pekaren över fliken för den vy du vill duplicera och klicka på menyn **Mer** ![Mer](assets/more-menu.png) till höger om vynamnet. Klicka sedan på **Duplicera**.

   ![Visa mer meny med duplicerat alternativ](assets/view-more-menu-with-duplicate-option.png)


   Vyn är duplicerad och den nya vyns namn följer följande mönster: `Original view's name (Copy)`. Fliken Ny vy visas i slutet av alla visningsflikar.

## Aktivera närvaroindikatorn i realtid i en vy

Avatarerna för andra användare som redigerar postinformation samtidigt som du visar i det övre högra hörnet av alla postvyer, som standard.

När du visar tabellvyn kan du även visa vilket fält en annan användare redigerar när du visar posten.

1. Gå till en posttypssida och öppna en vy.
1. (Villkorligt) Om andra användare redigerar poster av den markerade typen samtidigt visas deras avatarer i vyns övre högra hörn.
1. Klicka på listrutan intill avatarerna och välj **Visa medarbetare**. Växlingsknappen är markerad som standard.

   ![Visa medarbetare växla mellan markerade](assets/show-collaborators-toggle-selected.png)

1. (Villkorligt) Öppna en tabellvy och det fält som någon annan redigerar markeras i den färg som motsvarar konturen för avataren i tabellvyn.

   Om avatarens högdagerfärg är grå redigerade användaren inte posten för mer än 30 sekunder sedan.

   ![Tabellfält för realtidsindikator och avataranslutning](assets/real-time-indicator-table-field-and-avatar-connection.png)

   >[!TIP]
   >
   >Du kan välja alternativet **Visa medarbetare** från vilken vy som helst. Det fält som redigeras av andra kontureras bara i tabellvyn.

---
product-area: projects
navigation-topic: create-projects
title: Skapa och visa projektbilder
description: Med ögonblicksbilder i Adobe Workfront kan du se skillnader mellan ögonblicksbilder (tagna på ett visst datum och en viss tid) och projektets aktuella data.
author: Lisa
feature: Work Management
exl-id: 9ff84f9a-46bd-46e8-a58d-7dafbc333507
source-git-commit: dc71072107ce80f6cb9033fcb17fe4ac74d5af18
workflow-type: tm+mt
source-wordcount: '1278'
ht-degree: 0%

---

# Skapa och visa ögonblicksbilder av projekt

Projektledare behöver ofta jämföra tidigare data i ett projekt med aktuell status för att fatta välgrundade beslut och se hur deras projekt har ändrats över tid.

Med ögonblicksbilder i Adobe Workfront kan du se skillnaderna mellan ögonblicksbilder (tagna på ett visst datum och en viss tid) och projektets aktuella data snabbt och korrekt, vilket gör att du kan hantera projekt mer effektivt och fatta bättre beslut. Jämförelser av ögonblicksbilder visar hur projektet har utvecklats sida vid sida.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td> <p>Arbetsflöde Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
    <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Åtkomstnivåkonfiguration</td> 
   <td>Redigera åtkomst till projekt</td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td> 
   <td>När du visar en ögonblicksbild kan du visa alla fält som du har behörighet att visa i det ursprungliga projektet </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa en fixering

1. Gå till ett projekt.
1. Klicka på **Ögonblicksbilder** i den vänstra panelen.

   ![Fixeringar för ett projekt](assets/snapshot-list.png)

1. Klicka på **Ny fixering**.
1. Skriv ett namn för ögonblicksbilden i dialogrutan **Ny fixering** och klicka på **Spara**.

   Namnet på ögonblicksbilden visas i listan.

   >[!NOTE]
   >
   >När du skapar en ögonblicksbild är den inte tillgänglig för visning direkt. Baserat på data som körs i bakgrunden kan det ta upp till 4 timmar att vara redo. Skapandestatusen är **Väntande** när ögonblicksbilden inte är tillgänglig än och **Klar** när du kan visa den.

## Visa en ögonblicksbild

1. Gå till ett projekt och klicka på **Ögonblicksbilder** i den vänstra panelen.
1. Klicka på ett fixeringsnamn i listan för att öppna den. Statusen måste vara **Klar** innan du kan öppna den.

   >[!TIP]
   >
   >Bröderna högst upp på skärmen länkar tillbaka till projektet och hjälper dig att identifiera att du visar en ögonblicksbild.

   Följande objekt visas som de var när ögonblicksbilden skapades:

   * Hierarkin för aktiviteter och underaktiviteter i projektet
   * Projektinformation och eventuella anpassade formulär som är kopplade till informationen
   * Associerade projekt och deras hierarki
   * Problem
   * Kurser
   * Faktureringsposter
   * Utgifter <!--* Bookings (on its own line of course when they get released)-->
   * Projektgrupp (fliken Personer)

   Du kan anpassa alla listor i ögonblicksbilden genom att filtrera, sortera, lägga till och ta bort kolumner eller använda en vy. KPI:er med tidsfaser är tillgängliga för att läggas till i ögonblicksbildvyn. Mer information finns i [Anpassa listor med ögonblicksbilder](#customize-snapshot-lists) i den här artikeln.

## Jämför ögonblicksbilder

1. Gå till ett projekt och klicka på **Ögonblicksbilder** i den vänstra panelen.
1. Välj ett alternativ för att jämföra ögonblicksbilder:

   * Om du vill jämföra två eller flera ögonblicksbilder med varandra markerar du kryssrutorna bredvid ögonblicksbilderna i listan och klickar på **Jämför** i åtgärdsfältet längst ned på skärmen.
   * Om du vill jämföra ögonblicksbilder med det aktuella projektet markerar du kryssrutorna bredvid ögonblicksbilderna i listan och klickar på **Jämför med aktuell** i åtgärdsfältet längst ned på skärmen.

     >[!NOTE]
     >
     >Status för varje ögonblicksbild som du vill jämföra måste vara **Ready**.

1. Expandera varje ögonblicksbild och det aktuella projektet på jämförelseskärmen för att se hierarkin under.

   ![Skärm för jämförelse av ögonblicksbilder](assets/snapshot-comparison.png)

1. Du kan anpassa jämförelsen genom att sortera, lägga till och ta bort kolumner eller använda en vy. Mer information finns i [Anpassa listor med ögonblicksbilder](#customize-snapshot-lists) i den här artikeln.

## Exportera ögonblicksbilder

Du kan exportera listan över alla ögonblicksbilder eller en ögonblicksbildsjämförelse i formatet .xlsx eller .csv. Alla kolumner som visas inkluderas i den exporterade filen.

1. Klicka på ikonen **Exportera** ![Exportera ](assets/export-icon.png) i ögonblicksbildslistan eller i ögonblicksbildsjämförelsen.
1. Välj exportfilens format.

   Filen sparas på datorn. Du kan uppmanas att välja plats.

1. (Valfritt) Öppna den exporterade listan med lämpligt program.

## Anpassa ögonblicksbildslistor

Du kan anpassa listan över alla ögonblicksbilder samt alla listor i en ögonblicksbild eller jämförelse genom att filtrera, sortera, lägga till och ta bort kolumner eller använda en vy.

Mer information om anpassningar av listor finns i [Använda förbättrade listor](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

### Filtrera objekt i en lista

Med filter kan du minska mängden information som visas i listan.

1. Klicka på **Filter** ovanför listan.
1. Klicka på **Lägg till villkor** i rutan Filter.
1. Välj ett fält att filtrera efter.
1. Välj en filtermodifierare, till exempel &quot;Har någon av,&quot; &quot;Har ingen av,&quot; &quot;Är före&quot; eller &quot;Är efter&quot;. Modifieringsalternativen varierar beroende på vilken typ av fält du filtrerar efter.
1. Markera fältvärdet eller -värdena. Beroende på vilken fälttyp du filtrerar efter kan du uppmanas att välja objektet från en lista, söka efter det eller använda en kalender för att välja ett datumintervall.

   ![Filtrera listan över ögonblicksbilder](assets/filter-snapshot-list.png)

   Filtret tillämpas automatiskt på listan.

1. Klicka på **Lägg till villkor** om du vill lägga till ytterligare ett villkor i filtret.

   Du kan förena flera filter med en AND- eller en OR-koppling.

1. När filtret används kan du öppna alternativen för **Filter** igen och ändra filteralternativen eller ta bort alla filter.

   En indikator visas på knappen **Filter** när ett filter används i listan.

   ![Filtrera tillämpad indikator](assets/glist-filter-applied-indicator.png)

### Sortera i en lista

Så här sorterar du enskilda kolumner:

1. Håll markören över kolumnen, klicka sedan på nedpilen och välj **Sortera**.

   En ikon bredvid ett kolumnnamn anger att listan sorteras efter värdena i den kolumnen och sorteringsriktningen.

   ![Sortera listan över ögonblicksbilder](assets/sort-snapshot-list.png)

### Anpassa kolumner i en lista

Du kan dölja, visa och ordna om kolumner i en lista.

1. Klicka på **Kolumner** ovanför listan.

   ![Kolumner för ögonblicksbildslista](assets/hide-display-columns-on-snapshot.png)

1. Använd reglagen för att visa eller dölja kolumner i listan.
1. Om du vill ändra ordning på kolumnerna klickar du på ikonen **Dra** ![Dra ikonen](assets/drag-icon.png) och flyttar en kolumn till önskad plats. När du flyttar kolumner ändras listan automatiskt.

   >[!NOTE]
   >
   >Det primära fältet är den första kolumnen i listan. Den är fast på den första positionen och du kan inte ändra dess kolumn. Om antalet kolumner är stort, fryses det primära fältet till vänster och när du rullar vågrätt visas det alltid.
   >
   >Ikonen bredvid ett fältnamn visar fälttypen, till exempel text eller datumfält.

   En indikator visas på knappen **Kolumner** när kolumnerna är dolda. Indikatorn visas inte när du ändrar ordning på kolumnerna.

   ![Indikator för dolda kolumner](assets/glist-columns-hidden-indicator.png)

### Lägga till och ta bort kolumner med kolumnhanteraren

Du kan använda kolumnhanteraren i vissa förbättrade listor för att enkelt lägga till och ta bort kolumner i listan. Du kan lägga till eller ta bort både systemfält och anpassade fält som redan finns i Workfront som kolumner.

1. Klicka på ikonen **+** i tabellens övre högra hörn för att öppna rutan **Kolumnhanteraren** .

   ![Kolumnhanterare för ögonblicksbilder](assets/column-manager-on-snapshot-no-kpi-tab.png)

1. Sök efter ett befintligt objektfält i kolumnen **Tillgängligt** och klicka sedan på **+** till höger om fältnamnet för att lägga till det i kolumnen **Markerat**.
1. Klicka på **-** till höger om ett fält i kolumnen **Markerad** för att ta bort det från listan.
1. Klicka på **Spara**.

   Listan uppdaterar kolumnerna enligt de val du har gjort.

### Använda en vy i en lista

Så här använder eller skapar du en vy:

1. Klicka på listrutan **Vyer** och välj en befintlig vy för att använda den i listan

   ELLER

   Klicka på **Ny vy** för att skapa en.

   ![Vymenyn på en ögonblicksbild](assets/views-on-snapshot-list.png)

1. (Villkorligt) Om du vill lägga till en ny vy anger du ett namn för vyn och klickar sedan på **Skapa**.
1. (Valfritt) Dölj, visa eller ordna om kolumnerna. Mer information finns i [Anpassa kolumner i en lista](#customize-columns-in-a-list).
1. (Valfritt) Filtrera listan. Mer information finns i [Filtrera objekt i en lista](#filter-items-in-a-list).

Ändringar av vyer sparas automatiskt. Nästa gång du använder den här vyn behåller du inställningarna för kolumner och filter. Mer information om vyer finns i [Använd förbättrade listor](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

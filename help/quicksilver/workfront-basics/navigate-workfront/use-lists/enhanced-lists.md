---
navigation-topic: get-started-with-workfront
title: Använd utökade listor
description: De förbättrade listorna har ett tabellformat för att visa listobjekten, och de har ett annat utseende och en annan känsla än standardlistorna
author: Lisa
feature: Get Started with Workfront
exl-id: 4c25ed54-b147-4fd3-8d00-6f1ba61bbd38
source-git-commit: 2b01a9b4c697ae814ff894120fcc61df1a461e4e
workflow-type: tm+mt
source-wordcount: '2342'
ht-degree: 0%

---

# Använd förbättrade listor

{{preview-fast-release-general}}

Förbättrade listor finns i vissa delar av Adobe Workfront. De här listorna har ett tabellformat för att visa listobjekten, och de har ett annat utseende och en annan känsla än standardlistorna. Hanteringen av vyer har också förbättrats, bland annat filtrering, gruppering, hantering av kolumner och sökning.

Mer information om standardlistorna finns i [Kom igång med listor i Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

>[!NOTE]
>
>Varje förbättrad lista kan konfigureras på olika sätt så att du kan visa de data du behöver. Alla listor använder inte alla funktioner som beskrivs i den här artikeln och vissa listor kan ha specialfunktioner som bara gäller för den listan.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td>
   <p>Medarbetare eller högre</p>
   <p>Begäran eller senare</p></td>
  </tr>
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Objekt som använder utökade listor

Nedan visas några typer av Workfront-objektlistor som använder det förbättrade listformatet och några av de områden där de visas som standard när du har behörighet att visa objektet.

>[!NOTE]
>
>Den här listan är inte heltäckande. Var och en av de här objektlistorna kan också visas i en rapport eller på en kontrollpanel. En Request-rapport eller en kontrollpanel som innehåller en Request-rapport visar till exempel även en lista med begäranden.

| Workfront-lista | Objektlistans plats |
| --- | --- |
| Prioriteringar | <ul><li>Hem > välj ikonen Prioriteter i den vänstra menyn</li><li>Huvudmeny > Prioriteter</li></ul> |
| Lista över begäranden | <ul><li>Begäranden (endast ny upplevelse)</li><li>Widgeten Mina förfrågningar på startsidan</li></ul> |
| Statuslistor, prioriteter, allvarlighetsgrader och valutakurser i installationsprogrammet | <ul><li>Inställningar > Projektinställningar > Status</li><li>Inställningar > Projektinställningar > Prioriteter</li><li>Inställningar > Projektinställningar > Allvarlighetsgrader</li><li>Inställningar > Projektinställningar > Exchange-priser</li></ul> |
| <span class="preview">Lista över rapporter</span> | <span class="preview">Huvudmeny > Rapporter</span> <p><span class="preview">Det utökade listformatet används bara när **Använd delningsbara mappar** är aktiverat. Mer information finns i [Använd delningsbara rapportmappar](/help/quicksilver/reports-and-dashboards/reports/report-usage/use-sharable-report-folders.md).</span> |

## Lägga till objekt i en förbättrad lista

Beroende på vilken förbättrad lista du visar gör du något av följande:

1. Klicka på den blå knappen uppe till höger i listan. Med det här alternativet öppnas en dialogruta där du kan ange information. Data sparas som en ny rad i tabellen.

   ELLER

1. Klicka på **Ny rad** längst ned i listan. Med det här alternativet läggs en ny rad till i tabellen. Dubbelklicka i en cell för att ange information. Varje cell representerar ett fält för listobjektet. Fälten måste finnas innan du kan se dem i listan.

   Förbättrade listor har stöd för följande fälttyper:

   * Text
   * Nummer
   * Valuta
   * Datum
   * Datum och tid
   * Enstaka/flera urvalslistrutor
   * Typeahead
   * Stycke
   * Uppdragare (en eller flera)
   * Färgväljaren

   >[!NOTE]
   >
   >Varje fälttyp har sina egna redigeringsalternativ. Vissa fält kan vara skrivskyddade.

![Exempel på utökad lista](assets/glist-exchange-rates.png)

## Redigera objekt med åtgärdsfältet

Du kan använda åtgärdsfältet i en förbättrad lista för att redigera objekt i listan. Alla åtgärdsfält innehåller inte samma alternativ. Vissa listor kanske inte tillåter dig att markera objekt och åtgärdsfältet är inte tillgängligt.

1. Markera kryssrutan bredvid ett objekt i en förbättrad lista.

   Åtgärdsfältet visas längst ned på skärmen.

   >[!NOTE]
   >
   >Beroende på vilken lista du redigerar kan du markera ett eller flera objekt som ska användas i åtgärdsfältet.

1. Klicka på en åtgärd i fältet för att redigera objekt. Exempel på åtgärder du kan välja är:

   * Visa
   * Redigera
   * Ta bort

   Om det inte finns några tillgängliga åtgärder för det valda objektet visas&quot;Inga tillgängliga åtgärder&quot; i åtgärdsfältet.

   ![Exempel på åtgärdsfält](assets/glist-action-bar-statuses.png)

1. Håll markören över det primära fältet för ett listobjekt och klicka sedan på **Mer** meny ![Mer menyikon](assets/more-icon.png) för att se ytterligare åtgärder. Vissa åtgärder kan vara specifika för den listan.

   >[!TIP]
   >
   >Det primära fältet visas i den första kolumnen i listan.

   ![Exempel på fler menyer](assets/glist-more-menu-priorities.png)

## Anpassa kolumner

Beroende på vilka objekt du visar i en förbättrad lista kan du dölja, visa och ändra ordning på kolumner i listan.

1. Klicka på **Kolumner** ovanför listan.

   ![Exempel på visning av kolumner](assets/glist-display-move-columns.png)

1. Använd reglagen för att visa eller dölja kolumner i listan.
1. Om du vill ändra ordning på kolumnerna klickar du på ikonen **Dra** ![Dra ikonen](assets/drag-icon.png) och flyttar en kolumn till önskad plats. När du flyttar kolumner ändras listan automatiskt.

   >[!NOTE]
   >
   >Det primära fältet är den första kolumnen i listan. Den är fast på den första positionen och du kan inte ändra dess kolumn. Om antalet kolumner är stort, fryses det primära fältet till vänster och när du rullar vågrätt visas det alltid.
   >
   >Ikonen bredvid ett fältnamn visar fälttypen, till exempel text eller datumfält.

   En indikator visas på knappen **Kolumner** när kolumnerna är dolda. Indikatorn visas inte när du ändrar ordning på kolumnerna.

   ![Indikator för dolda kolumner](assets/glist-columns-hidden-indicator.png)

### Byt namn på kolumner

I vissa kolumner kan du spara ett anpassat namn för kolumnrubriken.

1. Håll markören över kolumnen, klicka sedan på nedpilen och välj **Byt namn**.

   ![Välj Byt namn på kolumn](assets/glist-rename-or-sort-column.png)

1. I dialogrutan **Byt namn** skriver du namnet på kolumnen i fältet **Egen etikett** och klickar på **Spara**.

   Det nya kolumnnamnet visas i listan.

## Lägga till och ta bort kolumner med kolumnhanteraren

Du kan använda **kolumnhanteraren** i vissa förbättrade listor för att enkelt lägga till och ta bort kolumner i listan. Du kan lägga till eller ta bort både systemfält och anpassade fält som redan finns i Workfront som kolumner i en förbättrad lista.

Så här lägger du till och tar bort kolumner:

1. Klicka på ikonen + i tabellens övre högra hörn för att öppna rutan **Kolumnhanteraren**.
1. Sök efter ett befintligt objektfält i kolumnen **Tillgängligt** och klicka sedan på + till höger om fältnamnet för att lägga till det i kolumnen **Markerat**.
1. Klicka på - till höger om ett fält i kolumnen **Markerad** för att ta bort det från listan.

   >[!NOTE]
   >
   >Vissa fält kan vara åtgärdade och kan inte tas bort.

   <!-- Add info about Properties and KPIs when something gets released with those options -->

1. Klicka på **Spara**.

   ![Kolumnhanteraren](assets/glist-column-manager.png)

   Listan uppdaterar kolumnerna enligt de val du har gjort.

## Uppdatera utökade listelement

Följande element är komponenter i en förbättrad lista:

* Visa: Definierar kolumner, filter och grupperingar i listan med förinställningar
* Filter: Begränsar mängden information som visas i listan
* Grupperingar: Ordna listobjekten enligt vanliga fält
* Sortera: Ordnar objekten i en lista i den ordning som du anger för ett visst fält
* Sök: Hitta snabbt ett objekt med ett söknyckelord

### Använda och skapa vyer

>[!NOTE]
>
>Alla förbättrade listor har inte alla element som beskrivs i det här avsnittet.

Så här använder eller skapar du en vy:

1. Klicka på listrutan **Vyer** och välj en befintlig vy för att använda den i listan

   ELLER

   Klicka på **Ny vy** för att skapa en.

1. (Villkorligt) Om du vill lägga till en ny vy anger du ett namn för vyn och klickar sedan på **Skapa**.
1. (Valfritt) Dölj, visa eller ordna om kolumnerna. Mer information finns i [Anpassa kolumner i en förbättrad lista](#customize-columns-in-an-enhanced-list).
1. (Valfritt) Filtrera listan. Mer information finns i [Filtrera objekt i en förbättrad lista](#filter-items-in-an-enhanced-list).
1. (Valfritt) Gruppera objekten i listan. Mer information finns i [Gruppera objekt i en förbättrad lista](#group-items-in-an-enhanced-list).

   Ändringar av vyer sparas automatiskt. Nästa gång du använder den här vyn behåller du inställningarna för kolumner och filter.

### Filtrera objekt i en förbättrad lista

>[!NOTE]
>
>Alla förbättrade listor har inte alla element som beskrivs i det här avsnittet.

Med filter kan du minska mängden information som visas i listan.

1. Klicka på **Filter** ovanför listan.
1. Klicka på **Lägg till villkor** i rutan Filter.
1. Välj ett fält att filtrera efter.
1. Välj en filtermodifierare, till exempel &quot;Har någon av,&quot; &quot;Har ingen av,&quot; &quot;Är före&quot; eller &quot;Är efter&quot;. Modifieringsalternativen varierar beroende på vilken typ av fält du filtrerar efter.
1. Markera fältvärdet eller -värdena. Beroende på vilken fälttyp du filtrerar efter kan du uppmanas att välja objektet från en lista, söka efter det eller använda en kalender för att välja ett datumintervall.

   ![Filtrera i förbättrade listor](assets/glist-filter-with-options.png)

   Filtret tillämpas automatiskt på listan.

   >[!TIP]
   >
   >Om du vill använda ett aktuellt användarens jokertecken väljer du **Jag (inloggad användare)** som fältvärde. Filtret gäller sedan den användare som visar listan. Jokertecknet är tillgängligt i fält där värdet är en användare.

1. Klicka på **Lägg till villkor** om du vill lägga till ytterligare ett villkor i filtret.

   Du kan förena flera filter med en AND- eller en OR-koppling.

1. När filtret används kan du öppna alternativen för **Filter** igen och ändra filteralternativen eller ta bort alla filter.

   En indikator visas på knappen **Filter** när ett filter används i listan.

   ![Filtrera tillämpad indikator](assets/glist-filter-applied-indicator.png)

### Gruppera objekt i en förbättrad lista

>[!NOTE]
>
>Alla förbättrade listor har inte alla element som beskrivs i det här avsnittet.

Grupperingar delar upp objekten i listan i områden baserat på specifika kriterier.

Workfront har ett begränsat antal fördefinierade grupperingar och du kan inte ändra dem.

1. Klicka på **Grupp** ovanför listan.
1. Välj en gruppering för att ordna listan.

   ![Välj en gruppering](assets/glist-grouping-choose-a-group-by.png)

1. Klicka på **Komprimera alla** om du vill visa listan med alla grupperingar komprimerade. Standardalternativet är att visa listan med alla grupperingar utökade.
1. När grupperingen används kan du öppna grupperingsalternativen igen om du vill komprimera eller utöka alla grupperingar samtidigt, ändra grupperingen till gruppering i ett annat fält eller ta bort alla grupperingar.

   ![Gruppering i utökade listor](assets/glist-group-by-due-date-priorities.png)

   En indikator visas på knappen **Grupp** när en gruppering används i listan.

   ![Gruppering av tillämpad indikator](assets/glist-grouping-applied-indicator.png)

### Sortera i en förbättrad lista

>[!NOTE]
>
>Alla förbättrade listor har inte alla element som beskrivs i det här avsnittet.

Så här sorterar du enskilda kolumner:

1. Håll markören över kolumnen, klicka sedan på nedpilen och välj **Sortera**.

   En ikon bredvid ett kolumnnamn anger att listan sorteras efter värdena i den kolumnen och sorteringsriktningen.

   >[!NOTE]
   >
   >Vissa kolumner kanske inte kan sorteras, beroende på listan.

   ![Sortera efter kolumn](assets/glist-sort-by-column.png)

Så här sorterar du arbetet i en grupp:

1. Klicka på **Grupp**, gå till raden för den använda grupperingen, klicka på sorteringslistrutan och välj en stigande eller fallande ordning.

   ![Sortera i en gruppering](assets/sort-in-groups.png)

### Söka i en förbättrad lista

>[!NOTE]
>
>Alla förbättrade listor har inte alla element som beskrivs i det här avsnittet.

1. Skriv ett nyckelord som du vill söka efter i sökrutan i det övre högra hörnet av listan. Resultatet markeras i listan när du skriver.

   ![Söktermen är markerad](assets/glist-search-highlighted.png)

   >[!NOTE]
   >
   >Sökningen söker i alla kolumner i alla listobjekt. Om listan är lång innehåller sökningen objekt som du kan behöva rulla för att se. När listan filtreras, söker sökningen endast efter det som för närvarande visas.

### Dela en vy

>[!NOTE]
>
>Alla förbättrade listor har inte alla element som beskrivs i det här avsnittet.

I listrutan **Vyer** kan du se tre vykategorier:

* **Systemvyer**: Vyer som systemadministratören har tilldelat dig. Du kan inte dela systemvyer.
* **Delade vyer**: Vyer som har delats med dig av andra användare.
* **Mina vyer**: Vyer som du har skapat och kan dela med andra. Du kan dela vyer med andra användare, team eller grupper.

När du delar en vy inkluderas alla vyelement (kolumner, filter och grupperingar).

Så här delar du en vy:

1. I listrutan **Vyer** håller du muspekaren över vyn i **Mina vyer** som du vill dela, klickar på menyn **Mer** ![Mer](assets/more-icon.png) och klickar på **Dela**.
1. I dialogrutan Dela anger du namnen på de användare, team, grupper, företag eller jobbroller som du vill dela vyn med och markerar dem sedan i listan när de visas.

   Du kan ge följande behörigheter till mottagarna:

   * **Visa**: Användare kan tillämpa vyn på listan men inte dela den.

     <span class="preview">När Visa-användare uppdaterar vyn sparas de ändringarna i användarens personliga inställningar. En blå punkt på vynamnet (i användarens **delade vyer**) visar att personliga uppdateringar tillämpas på vyn.</span>

   * **Hantera**: Användare kan byta namn på, dela eller ta bort vyn och redigera vyns element.

     <span class="preview">När du hanterar åtkomstanvändare gör ändringar i vyn kommer alla användare som har den delade vyn att se uppdateringarna när vyn används i listan.</span>

1. Klicka på **Spara**.

   <span class="preview">Om du delar en vy med en användare och sedan tar bort åtkomsten tas vyn bort från användarens **delade vyer**. Om användaren använde den delade vyn i listan när åtkomsten togs bort används systemets standardvy.</span>

<div class="preview">

### Kopiera en vy

>[!NOTE]
>
>Alla förbättrade listor har inte alla element som beskrivs i det här avsnittet.

När en vy delas med dig som du inte har behörighet att redigera, kan du kopiera vyn och spara den med ett nytt namn. Du måste ändra vyn innan du kan kopiera den.

1. I listrutan Vyer håller du pekaren över vyn i **Delade vyer** som du vill kopiera, klickar på menyn **Mer** ![Mer](assets/more-icon.png) och klickar på **Kopiera med inställningar**.

   En ny vy skapas automatiskt. Det använder det ursprungliga vynamnet med (kopia) i slutet, och det visas i avsnittet **Mina vyer** för vyer.

   Du är ägare av den här vyn och du kan byta namn på, redigera, dela eller ta bort den. Om ägaren av den ursprungliga vyn tar bort din delade åtkomst till den vyn har du fortfarande åtkomst till den här vyn som du har skapat.

   >[!NOTE]
   >
   >Alternativet **Kopiera med inställningar** är bara tillgängligt när du har gjort ändringar i en vy som delats med dig.

</div>

<div class="preview">

### Återställ en vy

>[!NOTE]
>
>Alla förbättrade listor har inte alla element som beskrivs i det här avsnittet.

När en vy delas med dig som du inte har behörighet att redigera, och du uppdaterar den vyn, kan du återställa den till den ursprungliga vyn.

1. I listrutan **Vyer** håller du muspekaren över den vy i **Delade vyer** som du vill återställa, klickar på menyn **Mer** ![Mer](assets/more-icon.png) och klickar på **Återställ till standard**.

   Vyelementen (kolumner, filter och grupperingar) återställs till sina ursprungliga inställningar som delades med dig.

   >[!NOTE]
   >
   >Alternativet **Återställ till standard** är bara tillgängligt när du har gjort ändringar i en vy som delats med dig.

   ![Kopiera och återställa visningsalternativ](assets/glist-copy-view-shared-with-you.png)

</div>

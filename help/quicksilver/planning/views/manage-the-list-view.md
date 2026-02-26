---
title: Hantera listvyn i Adobe Workfront Planning
description: Du kan visa objekt och deras fält i en listvy när du öppnar dem på postens sida Anslutna poster i Adobe Workfront Planning. I den här artikeln beskrivs hur du kan skapa eller redigera en listvy på sidan Anslutna poster i en post.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1c7e6973-6e9e-4c93-9d3b-89ed90df9d14
source-git-commit: 973a095e8ff08e382010247d9ed38e48d4b2c564
workflow-type: tm+mt
source-wordcount: '1342'
ht-degree: 0%

---


# Hantera listvyn i Adobe Workfront Planning

<span class="preview">Informationen som är markerad på den här sidan avser funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Du kan visa objekt och deras fält i en listvy när du öppnar dem på postens sida Anslutna poster i Adobe Workfront Planning.

I den här artikeln beskrivs hur du kan skapa eller redigera en listvy på sidan Anslutna poster i en post och hur du kan redigera objekten i vyn.

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

## Överväganden om listvyer

* Du kan inte visa poster på posttypsidorna i en listvy. Du kan bara visa följande objekt i en listvy när du visar dem på postens sida Anslutna poster:

   * Workfront-projekt

  Mer information om hur du skapar en ansluten postsida finns i [Lägga till en kopplad postsida till en post](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).
* Innan du kan visa en listvy på en postsida med anslutna poster måste du koppla Workfront-projekt till posttyperna Planering. Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).
* Listvyer liknar Förbättrade listor. Mer information finns i [Använd förbättrade listor](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


## Hantera en listvy {#manage-a-list-view}

Mer information om hur du hanterar listvyer i Workfront finns i [Använda förbättrade listor](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

{{step1-to-planning}}

1. Klicka på ett arbetsytekort och klicka sedan på ett posttypskort.
1. Klicka i valfri vy på namnet på en post för att öppna postens förhandsgransknings- eller informationssida.
1. Lägg till en **sida för anslutna poster** för anslutna projekt enligt beskrivningen i artikeln [Lägg till en sida för kopplade poster i en post](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

   På sidan Anslutna poster visas projekt som är kopplade till posten i listvyn.

   <!--add new screen shot when they release Conditional formatting MVP -->

   ![Projekt på sidan med anslutna poster i listvyn](assets/projects-on-connected-records-page-list-view.png)

1. (Valfritt) Gör något av följande om du vill ändra listvyn:

   1. Expandera menyn för listvyer i det övre högra hörnet av listan om du vill välja en annan vy, eller klicka på **Ny vy** och skapa en annan.

      Vyer delas i hela systemet. Om du skapar en projektvy för en posttyp kan du visa den på andra posttyper som visar anslutna projekt.

   1. Håll muspekaren över namnet på en befintlig vy och klicka på menyn **Mer** ![Mer](assets/more-menu.png) och klicka sedan på något av följande:
      * **Byt namn** om du vill ge vyn ett nytt namn
      * **Dela** om du vill dela vyn med andra
      * **Ta bort** om du vill ta bort vyn.

      >[!NOTE]
      >
      >* Du måste ha behörigheten Hantera för en vy för att kunna redigera, dela eller ta bort den.
      >
      >* Du kan inte ändra systemvyer.
      >
      >* <span class="preview">Du kan återställa en vy som delades med dig efter att du har ändrat den för att återställa de ursprungliga inställningarna, eller så kan du kopiera den med dina ändringar och dela kopian. Mer information finns i [Använd förbättrade listor](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>

   1. Klicka på ikonen **Filter** ![Filter ](assets/filter-icon.png) för att lägga till ett filter i vyn. Resultaten filtreras omedelbart i listan. Du kan inte spara och namnge filter. Filter sparas när du öppnar sidan i framtiden och de är en del av delade vyer.
   1. Klicka på ikonen **Kolumner** ![Kolumner](assets/columns-icon.png) för att välja vilka kolumner som ska visas eller döljas i vyn.
   1. Håll pekaren över namnet på en kolumn, klicka sedan på nedåtpilen till vänster om kolumnnamnet och klicka sedan på något av följande:
      * **Byt namn** om du vill lägga till en **anpassad etikett** för kolumnen. Namnet på det ursprungliga fältet i Workfront ändras inte.
      * **Sortera** om du vill sortera listan efter det markerade fältet. En sorteringsikon som anger sorteringsriktningen läggs till i kolumnrubriken.
   1. Klicka på ikonen **+** i det övre högra hörnet av listan för att lägga till eller ta bort kolumner i listan och klicka sedan på **Spara**.

      **Kolumnhanteraren** öppnas.

      Du kan bara lägga till befintliga fält i listvyn.
Du kan inte ta bort det primära fältet i listvyn som visas i den första kolumnen.


   1. <span class="preview">Klicka på ikonen **Formatera celler** ![Formatera celler](assets/format-cells-icon.png) . Rutan **Format** öppnas.</span> <!--change the name of the box when they update it-->
      <span class="preview">Gör följande: </span>

      <div class="preview">

      1. Klicka på **Lägg till villkor** på raden **Om**, markera sedan ett fält som du vill formatera med och välj ett fältvärde.

         >[!TIP]
         >
         >Endast fält som är synliga i listvyn är tillgängliga för villkorsstyrd formatering.

      1. (Valfritt) Klicka på **Lägg till villkor** på raden **Om** om du vill lägga till fler villkor i samma regel.

         >[!TIP]
         >
         >Du kan lägga till upp till 10 villkor i en villkorsregel och du kan ha upp till 20 regler för ett fält.

      1. Klicka på **Eller**-kopplingen mellan villkor om du vill ändra till **och** och ange att flera villkor måste uppfyllas samtidigt. **Eller** är standardkoppling.
      1. På raden **Format** markerar du ett fält som anger vilken kolumn som ska formateras. <!--edit this area, if it changes names??-->
      1. (Valfritt) Klicka på ikonen **färgcirkel** ![Färgcirkel](assets/color-circle.png) bredvid det markerade fältet för att expandera det och välja en annan färg.
      1. Aktivera inställningen **Använd på rad** om du vill använda formateringen på hela raden i fältet som uppfyller villkoren.
      1. (Valfritt) Klicka på **Lägg till villkor** i rutan **Format** om du vill lägga till en annan regel för ett annat fält och upprepa stegen ovan.
      1. (Valfritt) Klicka på **Rensa alla** om du vill ta bort all formatering.
      1. Klicka utanför rutan **Format** för att stänga den.

         Du kommer nu tillbaka till listvyn.
Formateringen används omedelbart i listvyn.
Det finns en blå punkt bredvid ikonen **Formatera celler** som anger att specialformatering används i vyn.

      </div>

1. (Valfritt) Lägg till ett nyckelord i sökrutan i det övre högra hörnet av listan för att söka efter ett objekt.

   Objekt som matchar söktermen markeras i listan.

1. (Valfritt) Gör något av följande om du vill lägga till fler objekt i listan och automatiskt koppla dem till den valda posten:

   * Klicka på **Anslut poster** i det övre högra hörnet av listan om du vill lägga till befintliga objekt.
   * Klicka på **Ny rad** längst ned i listan om du vill lägga till nya objekt.
1. Klicka på namnet på ett anslutet objekt i listan för att öppna det på en annan webbläsarflik.
1. Dubbelklicka inuti en cell i listan för att redigera informationen i ett fält och tryck sedan på Retur för att spara ändringarna.

   Vissa fält är skrivskyddade. Procent färdigt i ett projekt är till exempel ett fält som beräknas av systemet och du kan inte redigera det manuellt.

1. Håll muspekaren över ett objektnamn i listan och klicka på menyn **Mer** [Mer](assets/more-menu.png) och klicka på **Visa** för att öppna projektet på en annan flik

   eller

   Markera ett eller flera objekt och lägg märke till åtgärdsfältet längst ned i listan och klicka sedan på något av följande:

   * **Ta bort** om du vill ta bort projektet. Om du tar bort ett projekt kopplas det från posten och flyttas till Workfront papperskorg. Workfront-administratörer kan återställa borttagna projekt upp till 30 dagar efter att de tagits bort.
   * **Koppla från** om du vill koppla från projektet från posten. När du kopplar från ett projekt tas det bort och alla värden i sökfälten tas bort från den aktuella posten.

   ![Åtgärdsfältet i sidvyn Anslutna poster](assets/actions-bar-connected-records-page-list-view.png)


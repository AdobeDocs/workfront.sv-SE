---
title: Hantera poster i planeringsavsnittet i Adobe Workfront Objects
description: Du kan visa Workfront Planning-poster som är anslutna till Adobe Workfront-objekt i avsnittet Planering av ett Workfront-objekt i den vänstra panelen.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '1734'
ht-degree: 0%

---


<!--add also Group and Company when they are available-->

# Hantera postanslutningar från Workfront-objekt

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->

{{planning-important-intro}}

Du kan visa Workfront Planning-poster i Workfront i följande områden av de objekt som är anslutna till dem:

* Avsnittet Planering av ett Workfront-objekt: Visar alla posttyper som är kopplade till ett objekt och deras respektive anslutna poster.
* Ett anpassat fält för planeringsanslutning: Visar en posttyp, dess respektive anslutna poster och upp till 7 uppslagsfält för de anslutna posterna.

## Krav för åtkomst

+++ Expandera för att visa åtkomstkrav.

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
   <li><p> Planering av Adobe Workfront<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront-plan*</p></td>
   <td>
<p>Någon av följande Workfront-planer:</p>
<ul><li>Utvald</li>
<li>Primtal</li>
<li>Sist</li></ul>
<p>Workfront Planning är inte tillgängligt för äldre Workfront-planer</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront Planeringspaket*</p></td>
   <td>
<p>Någon</p>
<p>Om du vill ha mer information om vad som ingår i varje Workfront Planning-plan kontaktar du din Workfront-kontoansvarige. </p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront-plattform</p></td>
   <td>
<p>Din organisations instans av Workfront måste vara registrerad i Adobe Unified Experience för att kunna komma åt Workfront Planning.</p>
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience för Workfront</a>. </p>
   </td>
  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licens för Adobe Workfront*</p></td>
   <td>
   <p>Standard</p>
   <p>Workfront Planning är inte tillgängligt för äldre Workfront-licenser</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Konfiguration av åtkomstnivå</p></td>
   <td> <p>Visa eller högre åtkomst till projekt, program och portföljer</p>  
   <p>Det finns ingen konfiguration av åtkomstnivå för Workfront Planning. </p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Behörigheter för objekt</p></td>
   <td>
   <p>I Workfront kan du visa eller ha högre behörighet till ett projekt, en portfölj eller ett program</a> </p> 
   <p>I Workfront Planning:
   <ul><li>
   Visa behörigheter till en arbetsyta och posttyp för att visa alla anslutna poster </li>
   eller
   <li> Bidra eller högre behörigheter till en arbetsyta och posttyp för att ansluta eller koppla från poster</a></li></ul> </p>  
   <p>Systemadministratörer har behörighet till alla Workfront Planning-arbetsytor, även de som de inte har skapat</p> 
  </td>
  </tr>
 </tbody>
</table>

*Mer information om åtkomstkrav för Workfront finns [i Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Hantera poster i avsnittet Planering

Du kan använda avsnittet Planering i ett Workfront-objekt för att visa alla posttyper och deras respektive poster som är anslutna till Workfront-objektet.
Avsnittet Planering är tillgängligt för följande Workfront-objekt:

* Projekt
* Portfölj
* Program
<!--* Group
* Company-->

### Att tänka på när det gäller avsnittet Planering av Workfront-objekt

Tänk på följande när du visar Workfront Planning-poster från avsnittet Planning i ett Workfront-objekt:

* Posttyper för Workfront Planning måste först anslutas till Workfront-objekttyper.

  Mer information finns i följande artiklar:

   * [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [Koppla poster](/help/quicksilver/planning/records/connect-records.md)
* Du kan visa avsnittet Planering från ett Workfront-objekt, även om det inte finns några poster som är associerade med Workfront-objektet.

### Hantera postanslutningar från avsnittet Planering

{{step1-to-planning}}

1. Klicka på kortet för en arbetsyta.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på kortet för en posttyp som är kopplad till ett Workfront-projekt, en portfölj eller ett program.
1. Gå till ett anslutet postfält som har en anslutning till ett Workfront-objekt, antingen i tabellvyn eller från en posts informationssida. Mer information finns i [Ansluta poster](/help/quicksilver/planning/records/connect-records.md).
1. Klicka på namnet på ett Workfront-objekt i fältet för den anslutna posten.
Objektets sida öppnas i Workfront.

   >[!NOTE]
   >
   >  Om du känner till ett Workfront-objekt som redan är anslutet till en planeringspost kan du navigera till avsnittet Planering från Workfront-objektet.

1. Klicka på **Planering** i den vänstra panelen.

   >[!NOTE]
   >
   >   Workfront- eller gruppadministratören måste lägga till avsnittet Planering i layoutmallen innan det visas för ett Workfront-projekt, en portfölj eller ett program.

   Avsnittet Planering visas med följande information:

   * De anslutna posterna visas på enskilda kort som innehåller följande information:
      * Namn på posten
      * Miniatyrbilden för posten
      * Namnet på det anslutna postfältet så som det visas i Workfront Planning.
   * Poster visas under respektive arbetsyta och posttyp.

   ![Planeringsavsnitt om projekt](assets/planning-section-on-project.png)

1. (Valfritt) Klicka på **Visa alla anslutningar** för att visa alla anslutna posttyper, inklusive de som inte har anslutna poster. Som standard visas inte posttyper utan anslutna poster.
1. Klicka på ett postkort om du vill visa mer information om posten. Rutan för förhandsgranskning av post visas.
1. (Valfritt) Börja ändra fält i postens förhandsgranskningsruta. Dina ändringar sparas automatiskt.
1. (Valfritt) **Klicka på ikonen**&#x200B;Öppna i en ny flik![ i ikonen Öppna i en ny flik](assets/open-details-in-a-new-tab-icon.png) i det övre högra hörnet av förhandsgranskningsrutan för att öppna postens informationssida. Informationssidan för posten öppnas i Workfront Planning.
1. (Valfritt) Håll muspekaren över ett inspelningskort, klicka sedan på ikonen **för att koppla från post -** och klicka sedan på **Koppla från**.
Följande saker händer:
   * Posten är inte längre kopplad till Workfront-objektet.
   * Workfront-objektet tas också bort från postens anslutna fält från Workfront Planning.
   * Värdena för Workfront-uppslagsfält som är anslutna till planeringsposten tas också bort.
1. Klicka på **Anslut** om du vill ansluta fler poster för de anslutna posttyperna.

   Mer information finns i [Ansluta poster](/help/quicksilver/planning/records/connect-records.md).
1. (Valfritt) Om du inte hittar en post att ansluta och du vill lägga till den klickar du på **+ Lägg** till för att lägga till en ny post. Mer information finns i avsnittet &quot;Skapa poster när du kopplar dem från andra poster&quot; i artikeln [Skapa poster](/help/quicksilver/planning/records/create-records.md).

   Följande saker händer:

   * Posterna kopplas omedelbart till Workfront-objektet och visas i avsnittet Planering.
   * Workfront-objektet läggs till i Workfront Planning-postens anslutna fält.
   * Värdena för de Workfront-uppslagsfält som är kopplade till planeringsposten fylls i i Workfront Planning.

## Hantera poster i fälttypen Planeringsanslutning

Du kan använda ett anpassat fält för planeringsanslutning på ett Workfront-objekt för att visa en posttyp och dess respektive poster som är anslutna till Workfront-objektet.

Du kan styra vilka typer av planeringsposter som visas för Workfront-objektet när du skapar anpassade fält för planeringsanslutning.

* I fältet Planeringsanslutning visas planeringsposter efter att en anslutning har upprättats och när fältet är kopplat till formulär för följande Workfront-objekt:

   * Projekt
   * Portfölj
   * Program
   * Grupp
   * Företag

Mer information finns i [Skapa ett formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Att tänka på när det gäller fälttypen Planeringsanslutning

Tänk på följande när du visar Workfront Planning-poster från ett Planning-anslutningsfält för ett Workfront-objekt:

* Ett planeringsanslutningsfält visas på följande sätt i ett Workfront-objekts anpassade formulär, efter att planeringsposter har kopplats till Workfront-objektet:

   * Om endast det primära fältet i den anslutna posten är markerat, visas fältet Planeringsanslutning som ett fält med flera värden, om anslutningen tillåter att flera poster länkas. Mer information finns i [Översikt över](/help/quicksilver/planning/architecture/connect-record-types-overview.md) Anslut posttyper.
   * Om Workfront- eller gruppadministratören har lagt till ytterligare uppslagsfält från den anslutna posten i det anpassade formuläret visas fältet Planeringsanslutning som en tabell. Upp till 7 fält kan väljas för fältet Planeringsanslutning. Tabellvyn är skrivskyddad.

* Du kan bara koppla en posttyp till ett planeringsanslutningsfält. Det finns ingen gräns för hur många planeringsanslutningsfält du har i ett formulär.
* Du måste ha rätt åtkomst och behörighet till objektet, posten och Workfront Planning för att kunna koppla ett anpassat formulär med ett anpassat fält för planeringsanslutning till ett Workfront-objekt.
* Du måste ha behörigheten Delta för en arbetsyta i Workfront Planning för att kunna ansluta eller koppla från poster från fältet Planning connection för ett Workfront-objekt.
* Posttyper för Workfront Planning måste först anslutas till Workfront-objekttyper. Mer information finns i [Ansluta posttyper](/help/quicksilver/planning/architecture/connect-record-types.md). Detta gör Workfront Planning-posterna tillgängliga från Workfront.
* Du kan endast ansluta eller koppla bort poster från fältet Planeringsanslutning för ett Workfront-objekt för objekt som kan ha Workfront Planning-anslutningar.

  Du kan till exempel koppla ett anpassat formulär med ett planeringsanslutningsfält till uppgifter, men du kan inte koppla Workfront Planning-objekt till uppgifter.
* Du kan inte redigera ett planeringsanslutningsfält när du redigerar flera Workfront-objekt samtidigt.

### Hantera postanslutningar från fälttypen Planeringsanslutning

1. Gå till en av följande objekttyper som har kopplats till en Workfront Planning-posttyp:

   * Projekt
   * Portfölj
   * Program
   * Företag
   * Grupp

1. Klicka på **&lt; Object > Detaljer** i den vänstra panelen.
1. (Villkorligt) Lägg till ett anpassat formulär med minst ett planeringsanslutningsfält för det objekt du har valt, om det inte finns något sådant.

   >[!NOTE]
   >
   >Din Workfront- eller gruppadministratör måste först skapa formuläret och lägga till ett planeringsanslutningsfält i det innan du kan lägga till det i ett objekt.


1. Klicka i fältet för att lägga till kopplade poster och klicka sedan på den nedåtpekande pilen i fältet för att välja poster i listan.

   ![Planeringsanslutningsfält på projekt med postlista öppen](assets/planning-connection-field-on-project-with-record-list-open.png)

   >[!TIP]
   >
   >Du kan inte lägga till poster i planeringsanslutningsfält som är associerade med andra Workfront-objekt än det objekt som du valde när fältet konfigurerades.
   >
   >Du kan till exempel inte lägga till poster i ett planeringsanslutningsfält som skapats för en portföljanslutning från ett projekts anpassade formulär.
   >
   >Det finns en indikation på att objektet i fältet och det objekt som du har valt inte matchar.
   >
   >![Varning för att objektet Planeringsanslutning inte stöds i formuläret](assets/warning-unsupported-object-planning-connection-field-on-form.png)

1. Klicka utanför listan för att stänga den.

   Följande saker händer:

   * Posterna kopplas omedelbart till Workfront-objektet och de visas i fältet Planeringsanslutning samt i avsnittet Planering i Workfront-objektet.
   * Workfront-objektet läggs till i Workfront Planning-postens anslutna fält.
   * Värdena för de Workfront-uppslagsfält som är kopplade till planeringsposten fylls i i Workfront Planning.
   * Om Workfront- eller gruppadministratören lade till uppslagsfält för poster när de skapade det anpassade formuläret, fylls postens uppslagsfält i automatiskt i en tabellvy. Tabellvyn i fältet Planeringsanslutning är skrivskyddad.

     ![Anpassat formulär för planeringsanslutning med tabell i projekt Detaljer](assets/planning-connection-field-with-table-on-project-details-custom-form.png)

     >[!NOTE]
     >
     >Tabellvyn visas endast när uppslagsfält har lagts till i fältet Planeringsanslutningar i det anpassade formuläret.


1. (Valfritt) Klicka på namnet på en post eller håll muspekaren över namnet på posten i tabellen och klicka sedan på **ikonen**&#x200B;Öppna post![ Öppna post i det anpassade formuläret](assets/open-record-icon-on-planning-connection-custom-form.png) Planeringsanslutning i fältet Planeringsanslutning för att öppna den i Workfront Planning.
Förhandsgranskningsrutan för Workfront Planning-postinformation öppnas.
1. Granska eller redigera information om posten, eller klicka på **ikonen**&#x200B;Öppna i en ny flik![ Öppna post i ny flik](assets/open-details-in-a-new-tab-icon.png) för att öppna sidan med postinformation.

1. (Valfritt) Från det anpassade formuläret i Workfront klickar du på **ikonen Ta bort** ![](assets/remove-icon.png) på en post för att ta bort den från fältet Planeringsanslutning och koppla bort den från Workfront-objektet.
Workfront-objektet kopplas bort från planeringsposten och all sökinformation från Workfront tas bort från posten.

1. Klicka på **Save Changes** för att spara det anpassade formuläret och andra ändringar som du har gjort i Workfront-objektet.

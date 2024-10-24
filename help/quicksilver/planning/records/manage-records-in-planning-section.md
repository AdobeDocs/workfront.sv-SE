---
title: Hantera poster i planeringsavsnittet för Adobe Workfront-objekt
description: Du kan visa de Workfront Planning-poster som är kopplade till Adobe Workfront-objekt i Planning-delen av ett Workfront-objekt i den vänstra panelen.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: e82cf1b586ea3b08f419802bd1e88c6567b61b95
workflow-type: tm+mt
source-wordcount: '1493'
ht-degree: 0%

---


<!--add also Group and Company when they are available-->

# Hantera postanslutningar från Workfront-objekt

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

{{planning-important-intro}}

Du kan visa Workfront Planning-poster och deras respektive poster som är kopplade till Adobe Workfront-objekt i följande områden i Workfront:

* Avsnittet Planning för ett Workfront-objekt: Visar alla posttyper som är kopplade till ett objekt och deras respektive anslutna poster.
* <span class="preview">Ett anpassat fält för planeringsanslutning: Visar en posttyp och dess respektive anslutna poster. </span>

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven för Workfront Planning.

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
   <td role="rowheader"><p>Adobe Workfront Planning*</p></td>
   <td>
<p>Alla</p>
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
   <td>
   <p>Standard</p>
   <p>Workfront Planning är inte tillgängligt för tidigare Workfront-licenser</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td>
   <td> <p>Visa eller ge senare åtkomst till projekt, program och Portfolio</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Objektbehörigheter</p></td>
   <td>
   <p>I Workfront: Visa eller högre behörigheter för ett projekt, en portfölj eller ett program </a> </p> 
   <p>I Workfront Planning kan du visa behörigheter till en arbetsyta om du vill visa anslutna poster eller Contribute eller högre behörigheter till en arbetsyta för att ansluta till eller koppla från poster.</a> </p>  
   <p>Systemadministratörer har behörighet till alla Workfront Planning-arbetsytor, inklusive de som de inte skapade</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Om du vill visa Planning-området eller Planning-avsnittet för ett Workfront-objekt måste alla användare, inklusive Workfront-administratörer, tilldelas en layoutmall som innehåller Planning-området på Main Menu (Huvudmeny) och Planning-området för projekt, portföljer och program. </p> Mer information finns i <a href="/help/quicksilver/planning/access/access-overview.md">Åtkomstöversikt för Adobe-planering</a>. </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Hantera poster i planeringsavsnittet

Du kan använda Planning-avsnittet för ett Workfront-objekt för att visa alla posttyper och deras respektive poster som är kopplade till Workfront-objektet.
Planeringsavsnittet är tillgängligt för följande Workfront-objekt:

* Projekt
* Portfolio
* Program
<!--* Group
* Company-->

### Att tänka på när det gäller planeringsavsnittet för Workfront-objekt

Tänk på följande när du visar Workfront Planning-poster från Planning-delen av ett Workfront-objekt:

* Workfront Planning-posttyper måste först anslutas till Workfront-objekttyper.

  Mer information finns i följande artiklar:

   * [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [Koppla poster](/help/quicksilver/planning/records/connect-records.md)
* Du kan visa Planning-avsnittet från ett Workfront-objekt, även när det inte finns några poster kopplade till Workfront-objektet.

### Hantera postanslutningar från planeringsavsnittet

{{step1-to-planning}}

1. Klicka på kortet för en arbetsyta.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på kortet för en posttyp som är kopplad till ett Workfront-projekt, en portfölj eller ett program.
1. Gå till ett anslutet postfält som har en anslutning till ett Workfront-objekt, antingen i tabellvyn eller från postens informationssida. Mer information finns i [Anslut poster](/help/quicksilver/planning/records/connect-records.md).
1. Klicka på namnet på ett Workfront-objekt i det anslutna postfältet.
Objektets sida öppnas i Workfront.

   >[!NOTE]
   >
   >  Om du känner till ett Workfront-objekt som redan är anslutet till en Planning-post kan du navigera till Planning-avsnittet från Workfront-objektet.

1. Klicka på **Planering** i den vänstra panelen.

   >[!NOTE]
   >
   >   Workfront- eller gruppadministratören måste lägga till planeringsavsnittet i layoutmallen innan den visas för ett Workfront-projekt, en portfölj eller ett program.

   Planeringsavsnittet visas med följande information:

   * De kopplade posterna visas på enskilda kort som innehåller följande information:
      * Postens namn
      * Postens miniatyrbild
      * Namnet på det anslutna postfältet så som det visas i Workfront Planning.
   * Poster visas under respektive arbetsyta och posttyp.

   ![](assets/planning-section-on-project.png)

1. (Valfritt) Klicka på **Visa alla anslutningar** om du vill visa alla anslutna posttyper, inklusive de utan anslutna poster. Som standard visas inte posttyper utan kopplade poster.
1. Klicka på ett postkort om du vill visa mer information om posten. Postens förhandsvisningsruta visas.
1. (Valfritt) Börja ändra fält i postens förhandsvisningsruta. Ändringarna sparas automatiskt.
1. (Valfritt) Klicka på ikonen **Öppna på en ny flik** ![](assets/open-details-in-a-new-tab-icon.png) i det övre högra hörnet av förhandsvisningsrutan för att öppna postens informationssida. Postens informationssida öppnas i Workfront Planning.
1. (Valfritt) Hovra över ett postkort, klicka på ikonen för att koppla från post **-** och klicka sedan på **Koppla från**.
Följande saker händer:
   * Posten är inte längre ansluten till Workfront-objektet.
   * Workfront-objektet tas också bort från postens anslutna fält från Workfront Planning.
   * Värdena för Workfront sökfält som är kopplade till Planning-posten tas också bort.
1. Klicka på **Anslut** för att ansluta fler poster för de anslutna posttyperna. Mer information finns i [Anslut poster](/help/quicksilver/planning/records/connect-records.md).

   Följande saker händer:

   * Posterna är omedelbart kopplade till Workfront-objektet och visas i planeringsavsnittet.
   * Workfront-objektet läggs till i Workfront Planning-postens anslutna fält.
   * Värdena för Workfront sökfält som är kopplade till Planning-posten fylls i i Workfront Planning.

<div class="preview">

## Hantera poster i fältet Planering-anslutning

Du kan använda ett anpassat fält för planeringsanslutning på ett Workfront-objekt för att visa en posttyp och dess respektive poster som är kopplade till Workfront-objektet.

Du kan styra vilka Planning-posttyper som ska visas för Workfront-objektet när du skapar anpassade fält för Planning-anslutningen.

* I fältet Planering-anslutning visas Planning-poster när en anslutning har upprättats och när fältet är kopplat till formulär för följande Workfront-objekt:

   * Projekt
   * Portfolio
   * Program
   * Grupp
   * Företag

Mer information finns i [Skapa ett formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Överväganden om typen av anslutningsfält för planering

Tänk på följande när du visar Workfront Planning-poster från ett Planning-anslutningsfält för ett Workfront-objekt:

* Du kan bara associera en posttyp med ett Planning-anslutningsfält.
* Du måste bifoga ett anpassat formulär med ett anpassat fält för planeringsanslutning till ett Workfront-objekt som kan anslutas från Workfront Planning, om du har rätt åtkomst.
* Workfront Planning-posttyper måste först anslutas till Workfront-objekttyper. Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).
* Du kan ansluta till eller koppla från poster från planeringsanslutningsfältet för ett Workfront-objekt endast för objekt som kan ha Workfront Planning-anslutningar.
* Du måste ha Contribute-behörighet för en arbetsyta i Workfront Planning för att kunna ansluta till eller koppla från poster från planeringsanslutningsfältet för ett Workfront-objekt.
* Du kan inte redigera ett planeringsanslutningsfält när du redigerar flera Workfront-objekt samtidigt.

### Hantera postanslutningar från anslutningstypen Planering

1. Gå till någon av följande objekttyper som har kopplats till en Workfront Planning-posttyp:

   * Projekt
   * Portfolio
   * Program
   * Företag
   * Grupp

1. Klicka på **&lt; Objekt > Detaljer** i den vänstra panelen.
1. (Villkorligt) Lägg till ett anpassat formulär med minst ett Planning-anslutningsfält för det markerade objektet, om det inte finns något.

   >[!NOTE]
   >
   >Workfront- eller gruppadministratören måste först skapa formuläret och lägga till ett planeringsanslutningsfält innan du kan lägga till det i ett objekt.


1. Klicka i fältet för att lägga till kopplade poster och klicka sedan på nedåtpilen i fältet för att välja poster från listan.

   ![](assets/planning-connection-field-on-project-with-record-list-open.png)

   >[!TIP]
   >
   >Du kan inte lägga till poster i planeringsanslutningsfält som är kopplade till andra Workfront-objekt än det objekt som du markerade när fältet konfigurerades.
   >
   >Du kan till exempel inte lägga till poster i ett Planning-anslutningsfält som har skapats för en Portfolio-anslutning från ett projekts anpassade formulär.
   >
   >Det finns en indikation på att objektet i fältet och det markerade objektet inte matchar.
   >
   >![](assets/warning-unsupported-object-planning-connection-field-on-form.png)

1. Klicka utanför listan för att stänga den.

   Följande saker händer:

   * Posterna är omedelbart kopplade till Workfront-objektet och visas i anslutningsfältet Planning samt planeringsavsnittet för Workfront-objektet.
   * Workfront-objektet läggs till i Workfront Planning-postens anslutna fält.
   * Värdena för Workfront sökfält som är kopplade till Planning-posten fylls i i Workfront Planning.
1. (Valfritt) Klicka på namnet på en post i anslutningsfältet Planning för att öppna den i Workfront Planning.
Fliken med postinformation öppnas i Workfront Planning.
Du kan granska information om posten eller navigera till posttypssidan.

1. (Valfritt) Klicka på ikonen **Ta bort** ![](assets/remove-icon.png) för en post i det anpassade formuläret i Workfront för att ta bort den från anslutningsfältet Planning och koppla bort den från Workfront-objektet.
Workfront-objektet kopplas bort från Planning-posten och all sökinformation från Workfront tas bort från posten.

</div>
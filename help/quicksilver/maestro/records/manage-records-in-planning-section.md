---
title: Hantera poster i Planning-delen av Adobe Workfront-objekt
description: Du kan visa posterna som är kopplade till Adobe Workfront-objekt i Planning-delen av ett Workfront-objekt på den vänstra panelen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 9b1b8d8661917946230033b661ca652f5edef734
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

<!--add this to the main TOC and the mini TOC-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--add also Group and Company when they are available-->


# Hantera poster i Planning-delen av Adobe Workfront-objekt

{{maestro-important-intro}}

Du kan visa posterna som är kopplade till Adobe Workfront-objekt i Planning-delen av ett Workfront-objekt på den vänstra panelen.

Planeringsavsnittet är tillgängligt för följande Workfront-objekt:

* Projekt
* Portfolio
* Program
<!--* Group
* Company-->

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
<p>Din organisation måste vara registrerad i betaprogrammet Adobe Workfront Planning. Kontakta din kontorepresentant om du vill veta mer om det nya erbjudandet. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront</p></td>
   <td>
<p>Alla</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td>
   <td>
   <p>Nytt: Standard</p>
   eller
   <p>Aktuell: Planera</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td>
   <td> <p>Visa eller ge senare åtkomst till projekt, program och Portfolio</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>I Workfront: Visa eller högre behörigheter för ett projekt, en portfölj eller ett program</a> </p> 
   <p>I Workfront Planning kan du visa eller högre behörigheter för en arbetsyta</a> </p>  
   <p>Systemadministratörer har behörighet till alla Workfront Planning-arbetsytor, inklusive de som de inte skapade</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Din Workfront- eller gruppadministratör måste lägga till planeringsområdet i huvudmenyn och planeringsavsnittet i den vänstra panelen i layoutmallen. Mer information finns i <a href="../access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Mer information finns på [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Att tänka på när det gäller planeringsavsnittet för Workfront-objekt

* Först måste du koppla posttyper till Workfront-objekttyper och poster till Workfront-objekt för att kunna visa dem i Workfront.

  Mer information finns i följande artiklar:

   * [Koppla posttyper](/help/quicksilver/maestro/architecture/connect-record-types.md)
   * [Koppla poster](/help/quicksilver/maestro/records/connect-records.md)
* Du kan visa Planning-avsnittet i ett Workfront-objekt, även när det inte finns några poster kopplade till Workfront-objektet.
* Du kan koppla planeringsposter till Workfront-objekt från Workfront i planeringsavsnittet.

## Hantera poster i planeringsavsnittet

{{step1-to-maestro}}

Den senast öppnade arbetsytan öppnas som standard.

1. Klicka på kortet för en posttyp som är kopplad till ett Workfront-projekt, en portfölj eller ett program.
1. Välj en tabellvy på menyn **Visa** listruta.
1. (Villkorligt) Gå till det anslutna postfältet i tabellen och lägg till ett Workfront-objekt. Klicka sedan på namnet på Workfront-objektet i fältet. Mer information finns i [Koppla poster](/help/quicksilver/maestro/records/connect-records.md).
Objektets sida öppnas i Workfront Planning.
1. Klicka **Gå till källa**, längst upp till höger på skärmen.

   Objektets sida öppnas i Workfront.
1. Klicka **Planering** till vänster.

   >[!NOTE]
   >
   >   Workfront- eller gruppadministratören måste lägga till planeringsavsnittet i layoutmallen innan den visas för ett Worfront-projekt, en portfölj eller ett program.

   Planeringsavsnittet visas med följande information:

   * De kopplade posterna visas på enskilda kort som innehåller följande information:
      * Postens namn
      * Postens miniatyrbild
      * Namnet på det anslutna postfältet så som det visas i Workfront Planning.
   * Poster visas under deras respektive arbetsyta.

   ![](assets/planning-section-on-project.png)

1. Klicka på ett postkort om du vill visa mer information om posten. Postens förhandsvisningsruta visas.
1. (Valfritt) Börja ändra fält i postens förhandsvisningsruta. Ändringarna sparas automatiskt.
1. (Valfritt) Klicka på **Öppna på en ny flik** icon ![](assets/open-details-in-a-new-tab-icon.png) i det övre högra hörnet av förhandsvisningsrutan för att öppna postens informationssida.
1. Håll muspekaren över ett minneskort och klicka sedan på ikonen för att koppla från post **-** och sedan klicka **Koppla från**.
Följande saker händer:
   * Posten är inte längre ansluten till Workfront-objektet.
   * Workfront-objektet tas också bort från postens anslutna fält från Workfront Planning.
   * Värdena för de Workfront-fält som är kopplade till Planning-posten tas också bort.
1. Klicka **Anslut** för att ansluta fler poster.

   <!--checking with the team on the below note - not sure if if should stay Manage or be changed to Contribute??-->

   >[!NOTE]
   >
   >   Knappen Anslut visas bara för de arbetsytor där du har behörigheten Hantera.

1. Klicka på de poster som du vill ansluta. Följande saker händer:

   * Posterna är omedelbart kopplade till Workfront-objektet och visas i planeringsavsnittet.
   * Workfront-objektet läggs till i Workfront Planning-postens anslutna fält.
   * Värdena för de Workfront-fält som är kopplade till Planning-posten fylls i i Workfront Planning.

<!--add more steps here for what happens after clicking Connect-->



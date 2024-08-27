---
title: Hantera poster i planeringsavsnittet för Adobe Workfront-objekt
description: Du kan visa de Workfront Planning-poster som är kopplade till Adobe Workfront-objekt i Planning-delen av ett Workfront-objekt i den vänstra panelen.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: cf42511263ec1cffd90d1e4bdcd43521b7fe6a30
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---


<!--add also Group and Company when they are available-->

# Hantera poster i Planning-delen av Adobe Workfront-objekt

{{planning-important-intro}}

Du kan visa de Workfront Planning-poster som är kopplade till Adobe Workfront-objekt i Planning-delen av ett Workfront-objekt i den vänstra panelen.

Planeringsavsnittet är tillgängligt för följande Workfront-objekt:

* Projekt
* Portfolio
* Program
<!--* Group
* Company-->

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven för Workfront Planning.

Du måste ha följande för att kunna komma åt Workfront Planning:

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
<p>Mer information om vad som ingår i varje Workfront Planning-plan finns i <a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfront priser och paketering</a>. </p>
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
   <p>I Workfront Planning, Contribute eller högre behörigheter till en arbetsyta </a> </p>  
   <p>Systemadministratörer har behörighet till alla Workfront Planning-arbetsytor, inklusive de som de inte skapade</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn och planeringsområdet för projekt, portföljer och program. </p> Mer information finns i <a href="/help/quicksilver/planning/access/access-overview.md">Åtkomstöversikt</a>. </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på när det gäller planeringsavsnittet för Workfront-objekt

* Workfront Planning-posttyper måste vara anslutna till Workfront objekttyper.

  Mer information finns i följande artiklar:

   * [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [Koppla poster](/help/quicksilver/planning/records/connect-records.md)
* Du kan visa Planning-avsnittet i ett Workfront-objekt, även när det inte finns några poster kopplade till Workfront-objektet.
* Du kan koppla planeringsposter till Workfront-objekt från Workfront, i planeringsavsnittet, när det finns minst en post kopplad till Workfront-objektet.

## Hantera poster i planeringsavsnittet

{{step1-to-planning}}

1. Klicka på kortet för en arbetsyta.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på kortet för en posttyp som är kopplad till ett Workfront-projekt, en portfölj eller ett program.
1. Gå till ett anslutet postfält som har en anslutning till ett Workfront-objekt, antingen i tabellvyn eller från postens informationssida. Mer information finns i [Anslut poster](/help/quicksilver/planning/records/connect-records.md).
1. Klicka på namnet på ett Workfront-objekt i det anslutna postfältet.
Objektets sida öppnas i Workfront.

1. Klicka på **Planering** i den vänstra panelen.

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

1. (Valfritt) Klicka på **Visa alla anslutningar** om du vill visa alla anslutna posttyper, inklusive de utan anslutna poster. Som standard visas inte posttyper utan kopplade poster.
1. Klicka på ett postkort om du vill visa mer information om posten. Postens förhandsvisningsruta visas.
1. (Valfritt) Börja ändra fält i postens förhandsvisningsruta. Ändringarna sparas automatiskt.
1. (Valfritt) Klicka på ikonen **Öppna på en ny flik** ![](assets/open-details-in-a-new-tab-icon.png) i det övre högra hörnet av förhandsvisningsrutan för att öppna postens informationssida. Postens informationssida öppnas i Workfront Planning.
1. Håll muspekaren över ett postkort, klicka på ikonen för att koppla från post **-** och klicka sedan på **Koppla från**.
Följande saker händer:
   * Posten är inte längre ansluten till Workfront-objektet.
   * Workfront-objektet tas också bort från postens anslutna fält från Workfront Planning.
   * Värdena för Workfront sökfält som är kopplade till Planning-posten tas också bort.
1. Klicka på **Anslut** för att ansluta fler poster för de anslutna posttyperna. Mer information finns i [Anslut poster](/help/quicksilver/planning/records/connect-records.md).

   Följande saker händer:

   * Posterna är omedelbart kopplade till Workfront-objektet och visas i planeringsavsnittet.
   * Workfront-objektet läggs till i Workfront Planning-postens anslutna fält.
   * Värdena för Workfront sökfält som är kopplade till Planning-posten fylls i i Workfront Planning.



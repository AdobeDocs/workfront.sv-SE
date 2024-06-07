---
title: Redigera arbetsytor
description: Du kan redigera informationen om en befintlig arbetsyta, som att byta namn på den.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 374b6d9c-69a9-4a73-8708-51c14a78c7c9
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Redigera arbetsytor

{{planning-important-intro}}

I Adobe Workfront Planning är arbetsytorna centraliserade platser där team kan planera arbetet.

En arbetsyta är en samling posttyper som används av ett team och representerar teamets arbetslivscykel. Du kan anpassa arbetsytorna helt i Adobe Workfront Planning.

Mer information om hur du skapar arbetsytor finns i [Skapa arbetsytor](/help/quicksilver/planning/architecture/create-workspaces.md).

Alla ändringar du gör på en arbetsyta är synliga för alla som har minst behörigheten Visa på arbetsytan.

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
<p>Din organisation måste vara registrerad på Workfront Planning i ett tidigt skede </p>
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
   <p>Aktuell: Planera</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td>
   <td> <p>Det finns inga åtkomstnivåkontroller för Workfront Planning</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Hantera behörigheter på arbetsytan </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Du måste lägga till planeringsområdet i layoutmallen. Mer information finns i <a href="/help/quicksilver/planning/access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>

</tbody>
</table>

Mer information om åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Redigera en arbetsyta

{{step1-to-planning}}

1. Klicka på ett arbetsytekort för att öppna arbetsytan.
1. Klicka inuti arbetsytans namn i arbetsytans sidhuvud för den nya arbetsytan och tryck sedan på **Retur**.
1. Klicka på **Mer** meny ![](assets/more-menu.png)till höger om arbetsytans namn i sidhuvudet och klicka sedan på **Redigera**.

   ![](assets/edit-workspace-box.png)

   Uppdatera följande information i **Arbetsytan Redigera** box:

   * Lägg till ett namn för arbetsytan. <!--did they add a label for this field?-->
   * **Beskrivning**: Lägg till information om arbetsytan.
   * Välj en ikon som du vill associera med arbetsytan.

1. Klicka **Spara** om du vill stänga arbetsytan Editor och tillämpa ändringarna.

1. (Valfritt) Gör något av följande om du vill lägga till ett nytt avsnitt i arbetsytan:

   * Klicka **Lägg till avsnitt** längst ned på arbetsytan.
   * Håll muspekaren över namnet på ett avsnitt och klicka på **Mer** meny ![](assets/more-menu.png)och sedan klicka **Lägg till avsnittet ovan** eller **Lägg till avsnitt nedan**.

1. (Valfritt) Gör något av följande om du vill ändra platsen för ett avsnitt:

   * Håll muspekaren över namnet på ett avsnitt och klicka på **ta** icon ![](assets/grab-icon.png)och sedan dra och släpp den på den högra platsen.
   * Håll muspekaren över namnet på ett avsnitt och klicka på **Mer** meny ![](assets/more-menu.png)och sedan klicka **Flytta uppåt** eller **Flytta nedåt**. Avsnittet flyttas uppåt eller nedåt i arbetsytan.

1. (Valfritt) Så här tar du bort ett avsnitt på arbetsytan:

   1. Håll muspekaren över namnet på ett avsnitt och klicka sedan på **Mer** meny ![](assets/more-menu.png)och sedan klicka **Ta bort**. <!--add screen shot when UI is final?-->
   1. Markera ett nytt avsnitt som du vill flytta alla posttyper till och klicka sedan på **Ta bort**. <!--check the button name; logged a bug to change it to "Delete" from "Delete section".-->

      Alla posttyper flyttas till urvalssektionen och avsnittet tas bort.

1. (Valfritt) Klicka på **Lägg till posttyp** om du vill lägga till posttyper på arbetsytan.

   Mer information finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

1. (Valfritt) Håll muspekaren över ett posttypskort och klicka på **Mer** meny ![](assets/more-menu.png) i det övre högra hörnet och klicka sedan på **Redigera** om du vill ändra utseendet på en posttyp.

   Mer information finns i [Redigera posttyper](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Valfritt) Håll muspekaren över ett posttypskort och klicka på **Mer** meny ![](assets/more-menu.png) i det övre högra hörnet och klicka sedan på **Ta bort** om du vill ta bort en posttyp.

   Mer information finns i [Ta bort posttyper](/help/quicksilver/planning/architecture/delete-record-types.md).

1. (Valfritt) Tryck på ett posttypskort för att dra det och släppa det på en ny plats. Du kan dra och släppa posttyper från ett avsnitt på arbetsytan till ett annat.

   ![](assets/drag-and-drop-record-types-in-a-workspace.png)

1. (Valfritt) Klicka på **Dela** i det övre högra hörnet av arbetsytan om du vill dela arbetsytan med andra.

   Mer information finns i [Dela arbetsytor](/help/quicksilver/planning/access/share-workspaces.md).

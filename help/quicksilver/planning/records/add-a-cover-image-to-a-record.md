---
title: Lägga till en omslagsbild till en post
description: Du kan anpassa poster genom att lägga till en omslagsbild på postsidan i Adobe Workfront Planning när du redigerar en post.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: 8a4da96562b18977f56567f0fc5f72b369078432
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---


<!--update the metadata with real information-->

# Lägga till en omslagsbild till en post

{{planning-important-intro}}

Du kan anpassa poster genom att lägga till en omslagsbild på postsidan i Adobe Workfront Planning när du redigerar en post.

Mer information om hur du redigerar poster finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

Du måste skapa posttyper innan du kan börja skapa och redigera poster.

Mer information finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

## Åtkomstkrav

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding cover images-->

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
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td>
   <td> <p>Det finns inga åtkomstkontroller för Workfront Planning </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Hantera behörigheter till en arbetsyta </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td>  <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn. </p> <p>Mer information finns i <a href="/help/quicksilver/planning/access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Mer information finns på [Åtkomstkrav i Workforts dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Att tänka på när det gäller omslagsbilder för postsidor

Du kan anpassa postens sida genom att lägga till en omslagsbild.

Tänk på följande:

* En omslagsbild är unik för en post och gäller inte för alla poster av samma typ.
* Du kan bara lägga till bildfiler som omslagsbilder.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* Du kan lägga till en omslagsbild till enskilda poster från postförhandsvisningen i valfri vy eller från postsidan.
* Du kan inte lägga till omslagsbilder från en postvy.
* Workfront laddar automatiskt upp en omslagsbild varje gång du skapar en post. Du kan ändra den här bilden senare.

## Lägga till en omslagsbild till en post

Du kan anpassa en post genom att lägga till en omslagsbild högst upp i postens förhandsvisning eller sida.

{{step1-to-planning}}

1. Klicka på arbetsytan vars poster du vill anpassa,

   eller

   Utöka den nedåtriktade pilen till höger om namnet på en befintlig arbetsyta i en arbetsyta, sök efter en arbetsyta och markera den när den visas i listan.

   Arbetsytan öppnas och posttyperna visas.

1. Klicka på ett posttypskort.

   Posttypssidan öppnas.

1. Klicka på en post i en vy av valfri typ

   eller

   I tabelltabellvyn klickar du på **Öppna detaljer** icon ![](assets/open-details-icon-in-table-name-field.png) i den första kolumnen.

   Postens förhandsgranskning öppnas i vyn.

   ![](assets/details-box.png)

1. (Valfritt) Klicka på **Öppna på ny flik** icon ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> i det övre högra hörnet av postförhandsgranskningen om du vill öppna postens sida på en ny flik.

   Postsidan öppnas.

   ![](assets/details-page.png)

1. Klicka på Förhandsgranska post eller på en sida **Lägg till omslag**


   eller

   Hovra över en befintlig omslagsbild, klicka på **Mer** meny ![](assets/more-menu.png) och sedan klicka **Överför**. <!--check the casing here; I logged a bug for this-->
The **Postomslag** öppnas i **Överför** -fliken.

   ![](assets/record-cover-box-for-upload.png)

1. Klicka **Bläddra bland bilder** och bläddra efter en bild på datorn för att markera och lägga till den.

1. (Valfritt) Om du vill ta bort bilden innan den sparas klickar du på **Överför ny bild** icon ![](assets/upload-new-image-icon.png) och överför en ny bild.

1. (Valfritt) Klicka på **Galleri** och sedan klicka på en bild i bildgalleriet. Det går inte att ändra bildgalleriet.

   ![](assets/record-cover-box-for-gallery.png)

1. Klicka **Använd bild**.

   Bilden överförs högst upp i postens förhandsgranskning eller sida och ändringarna sparas automatiskt.

   ![](assets/record-page-with-cover-image.png)

1. (Valfritt) Hovra över bilden och klicka sedan på **Mer** meny ![](assets/more-menu.png) i det nedre högra hörnet av omslagsbilden gör du något av följande:

   * Klicka **Överför** om du vill ersätta omslagsbilden och upprepa steg 6 för att ladda upp och spara en ny bild.
   * Klicka **Flytta** och använder **Flytta** verktyg ![](assets/reposition-tool-icon.png) för att centrera omslagsbilden och sedan klicka **Spara** när det är klart.
   * Klicka **Ta bort** för att ta bort omslagsbilden.

   Workfront sparar automatiskt ändringarna.

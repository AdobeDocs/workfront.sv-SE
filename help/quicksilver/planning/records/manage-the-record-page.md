---
title: Hantera postsidans layout
description: Du kan redigera layouten för postförhandsgranskning och -sida i Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 869a1f9e4fd7e3b65591050530b96d6dae9e230c
workflow-type: tm+mt
source-wordcount: '1066'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Hantera postsidans layout

{{planning-important-intro}}

Du kan redigera layouten för postförhandsgranskning och -sida i Adobe Workfront Planning.

Förhandsgranskningen av posten är en mindre vy av postsidan som visas i vyn av en posttyp.

När du ändrar layouten för en postförhandsgranskning och sida påverkar ändringarna förhandsvisningsrutorna och informationssidorna för alla poster av samma typ.

I den här artikeln beskrivs hur du kan ändra layouten och utseendet på en postförhandsvisningsruta eller en postsida. Mer information om hur du redigerar poster finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

Du måste skapa posttyper och poster innan du kan börja redigera postsidor.

Mer information finns i följande artiklar:

* [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md)

* [Skapa poster](/help/quicksilver/planning/records/create-records.md)

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
   <p>Nytt: Ljus eller högre</p>
   eller
   <p>Aktuell: Arbete eller högre</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td>
   <td> <p>Det finns inga åtkomstkontroller för Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Hantera eller högre behörigheter på en arbetsyta</a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Workfront- eller gruppadministratören måste lägga till planeringsområdet i layoutmallen. Mer information finns i <a href="/help/quicksilver/planning/access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Mer information finns på [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Att tänka på när du redigerar postsidor

* Som standard visas alla fält som är kopplade till posten på information- och förhandsvisningssidorna för en post.

* Du kan inte lägga till nya fält för en post på förhandsgransknings- eller informationssidan. Du måste lägga till nya fält i tabellvyn för att kunna visa dem på förhandsgransknings- och informationssidorna.

* Du kan lägga till avsnitt på en förhandsgransknings- eller informationssida för att ordna informationen utifrån vanliga kriterier och göra den lättare att hitta.

* Följande ändringar påverkar alla poster av samma typ och är synliga för alla användare som använder dessa poster:

   * Ordna om fält
   * Lägga till eller ta bort avsnitt

* Visningsändringar som du gör i postförhandsgranskningen visas direkt på postinformationssidan. Ändringar som görs på postsidan visas också i rutan Förhandsgranska post.

* Att lägga till en omslagsbild eller en miniatyrbild i en post ingår inte i den övergripande layouten för postförhandsvisningen eller -sidan. Du kan lägga till unika omslagsbilder eller miniatyrbilder till varje post. Mer information finns i [Lägga till en omslagsbild till en post](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) och [Lägga till en miniatyrbild i en post](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

## Lägga till avsnitt i en postförhandsgranskning eller sida

Tänk på följande när du lägger till avsnitt på en postsida:

* Det finns ingen gräns för hur många avsnitt du kan ha på en sida.
* Du kan inte ha ett tomt avsnitt. Du måste ha minst ett fält i ett avsnitt.
* Du kan dra och släppa fält från ett avsnitt till ett annat. Mer information finns i avsnittet [Ordna om fält på sidan för postförhandsgranskning eller detaljer](#rearrange-fields-in-the-record-preview-or-details-page) i den här artikeln.
* När du tar bort alla fält från ett avsnitt tas avsnittet automatiskt bort och kan inte återställas.

Så här lägger du till ett avsnitt i en postförhandsgranskning eller sida:

{{step1-to-planning}}

1. Klicka på kortet för en arbetsyta.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett posttypskort.

   Posttypssidan öppnas.

1. Klicka på en post i en vy av valfri typ

   eller

   I tabelltabellvyn klickar du på **Öppna detaljer** icon ![](assets/open-details-icon-in-table-name-field.png) i den första kolumnen.

   Postens förhandsgranskning öppnas i vyn.

   ![](assets/details-box.png)

1. (Valfritt) Klicka på **Öppna på ny flik** icon ![](assets/open-details-in-a-new-tab-icon.png) i det övre högra hörnet av postförhandsgranskningen om du vill öppna postens sida på en ny flik.

   Postsidan öppnas.

   ![](assets/details-page.png)

1. Håll markören över det tomma utrymmet till vänster om fälten och klicka sedan på **Lägg till avsnitt** icon ![](assets/add-section-icon.png) för att lägga till ett avsnitt.
1. Klicka i avsnittets namn och ersätt **Namnlöst avsnitt** med ett namn och klicka sedan på Enter. Fälten som visas under avsnittet är automatiskt en del av det nya avsnittet.
1. Börja dra och släppa fält till det nya avsnittet, vilket beskrivs i avsnittet [Ordna om fält på sidan för postförhandsgranskning eller detaljer](#rearrange-fields-in-the-record-preview-or-details-page) i den här artikeln.

1. (Valfritt) Håll pekaren över namnet på ett avsnitt och klicka på knappen **Mer** meny ![](assets/more-menu.png).

   ![](assets/more-menu-options-for-section-on-record-page.png)
1. (Valfritt) Gör något av följande om du vill redigera avsnittet:

   * Klicka **Byt namn** för att byta namn på avsnittet

     >[!TIP]
     >
     > Du kan byta namn på ett avsnitt genom att klicka på namnet.

   * Klicka **Flytta uppåt** för att flytta avsnittet uppåt en position

     eller

     Klicka **Flytta nedåt** om du vill flytta avsnittet nedåt en position.
Alla fält i avsnittet flyttas tillsammans med avsnittet.

   * Klicka **Ta bort** för att ta bort avsnittet. Avsnittet tas bort och kan inte återställas. Alla användare som har åtkomst till poster av den här typen kommer inte längre att visa det borttagna avsnittet.

1. Klicka på den nedåtriktade pilen till vänster om avsnittsnamnet för att komprimera det, eller på den högerriktade pilen för att expandera det.
Alla avsnitt expanderas som standard.

1. (Valfritt) Klicka på **ta** icon ![](assets/grab-icon.png) till vänster om ett avsnittsnamn och dra och släpp det på en önskad plats.

   Avsnittets nya position uppdateras både i förhandsgranskningen och på sidan med alla poster av samma typ för alla användare som visar posterna.

   Alla ändringar i avsnitt och fältordning sparas automatiskt.

## Ordna om fält på sidan för postförhandsgranskning eller detaljer

{{step1-to-planning}}

1. Klicka på kortet för en arbetsyta.

   Arbetsytan öppnas och posttyperna visas som kort.

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

1. Klicka på knappen **ta** icon ![](assets/grab-icon.png) till vänster om ett fältnamn och sedan dra och släppa det på önskad plats. <!--You can drag and drop fields to another section. You must have at least one field in a section.-->

   Den nya positionen för fältet uppdateras både i förhandsvisningen och på sidan med alla poster av samma typ för alla användare som visar posterna.

   Alla ändringar av layouten för postförhandsgranskningen eller sidan sparas automatiskt.


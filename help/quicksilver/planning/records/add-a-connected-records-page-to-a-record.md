---
title: Lägg till en sida med kopplade poster i en post
description: Du kan visa information från anslutna poster eller objekt genom att lägga till en flik för en sida med kopplade poster till en post. Då läggs de kopplade posterna i en tabellvy till på fliken.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 54ba4509269784ebe25fb5283b539c440454362a
workflow-type: tm+mt
source-wordcount: '1577'
ht-degree: 0%

---


# Lägga till en sida med kopplade poster i en post

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Du kan visa information från anslutna poster eller objekt genom att lägga till en flik för en sida med kopplade poster till en post i Adobe Workfront Planning. Då läggs de kopplade posterna i en tabellvy till på fliken.

Tänk på följande när du lägger till en sida med kopplade poster till en post:

* Du kan lägga till en sida med kopplade poster till en post efter att du har kopplat post- eller objekttyper till posttypen från tabellvyn för en posttyp.

* Du kan lägga till en sida med kopplade poster från en posts förhandsgranskningsområde eller postens sida.

* Anslutna postsidor visar endast anslutna objekt eller poster från ett objekt eller en posttyp. På sidan visas inte alla poster av den typen.

* Du kan visa objekten på en sida med kopplade poster i tabellvyn.

<!--replace the above bullet with this: 

* You can display the objects in a connected records page in the following types of views:

   * Table
   * <span class="preview">Timeline</span>
   * <span class="preview">Calendar</span>

* <span class="preview">You can create one page per one object or record type. For example, you cannot create two connected record pages for connected projects or tactics.</span>

-->

* Du kan lägga till sidor med kopplade poster för följande anslutna post- eller objekttyper:

   * Workfront Planning - posttyper
   * Workfront-projekt

     Du kan visa de anslutna Workfront-projekten även om du inte har behörighet att komma åt dem i Workfront.

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
<td> 
   <p> Ytterligare produkter</p> </td> 
   <td> 
   <p> Förutom Adobe Workfront måste du ha följande om du vill lägga till en ansluten postsida för objekt från följande program:</p>
   <ul><li><p>En Adobe Experience Manager Assets-licens och en integrering mellan AEM Assets och Workfront för att koppla AEM-material till posttyperna Planning.</p>
   <p>Mer information finns i <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront för Experience Manager Assets och Assets Essentials: artikelindex</a>. </p></li>
   <li><p> En Adobe GenStudio for Performance Marketing-licens för att koppla posttyper till GenStudio Brands</p>
   <p>Mer information finns i <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started">Kom igång med Adobe GenStudio for Performance Marketing</a>.</p></li></ul>
   </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Objektbehörigheter</p></td>
   <td>
   <p>Contribute eller högre behörighet för en arbetsyta och en posttyp </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p> 
  </td>
  </tr>   
</tbody> 
</table>

Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Lägga till en sida med kopplade poster i en post

Du måste först koppla posttyper till andra posttyper eller Workfront-projekt innan du lägger till en ansluten postsida till en post.

1. Klicka på postens namn för att öppna den från en vy av en posttypssida.
1. Klicka på **Lägg till sida** i något av följande områden:

   * Postens förhandsgranskningsfönster
   * Postens informationssida när du har klickat på ikonen **Öppna på ny flik** ![Öppna information på en ny flikikon](assets/open-details-in-a-new-tab-icon.png) i det övre högra hörnet på förhandsvisningssidan.

   Rutan **Skapa sida** öppnas.

   ![Sidan Lägg till kopplade poster modal](assets/add-connection-view-page-modal.png)

1. Lägg till **sidnamnet**, klicka på sidan **Anslutna poster** och klicka sedan på **Skapa**.

   En ny sida med kopplade poster läggs till som en ny flik på postens sida.

   Posterna som är kopplade till den aktuella posten visas i tabellvyn.

   >[!TIP]
   >
   >Du måste lägga till kopplade poster i tabellen eller i området Detaljer för en post innan du kan visa dem på en ansluten postsida.

   <!--All fields of the connected record display in the table view of the connected record's tab.-->

   De första fem fälten i de anslutna posterna visas som standard. <!--No lookup fields display by default.-->

   ![Målgruppsansluten tabellvy under kampanjinformation](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Valfritt) Klicka på namnet på en ansluten post eller objekttyp i listan eller sök efter den och klicka sedan på den när den visas i listan för att skapa sidan för den posten eller objekttypen.

1. (Valfritt och villkorligt) Om mer än ett anslutet fält av den posttyp som du skapar sidan för visas, klickar du på det fält vars poster du vill visa på sidan med anslutna poster.

   En av följande sidor läggs till på sidan med anslutna poster:

   * Registervyn för en posttyp
   * Listvyn för en projektobjekttyp

1. (Valfritt och villkorligt) Gör något av följande när du skapar en ansluten postsida för anslutna planeringsposter: <!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

   * Klicka på namnet på en post. Posten öppnas på en ny flik.
   * Klicka på **Anslut** längst ned i tabellvyn om du vill ansluta befintliga poster, markera dem i anslutningsrutan och klicka sedan utanför rutan för att stänga den. Posterna läggs automatiskt till i tabellen. Posterna måste finnas innan du kan lägga till dem.

     Mer information finns i [Anslut poster](/help/quicksilver/planning/records/connect-records.md).
   * Redigera all information från de anslutna posterna i tabellvyn.

   * Håll muspekaren över namnet på en ansluten post och klicka sedan på menyn **Mer** ![Mer](assets/more-menu.png)

     eller

     Markera en av posterna och klicka sedan på något av följande alternativ i det blå fältet längst ned i listan:

      * **Visa** om du vill öppna postsidan på en ny flik
      * **Kopiera länk** för att kopiera en länk till postsidan
      * **Redigera miniatyrbild** för att öppna rutan **Spela in miniatyrbild** och redigera postens miniatyrbild
      * **Duplicera** om du vill duplicera den anslutna posten. Den duplicerade posten är även ansluten till den aktuella posten.
      * **Infoga posten ovanför eller under** om du vill lägga till nya poster till den anslutna posttypen. Nya poster som läggs till här är också kopplade till den aktuella posten. Det här alternativet är inte tillgängligt i det blå fältet när du markerar en post i tabellen.
      * **Ta bort** om du vill ta bort posten. Om du tar bort en ansluten post tas den bort från sin posttyp och från alla ställen där posten är ansluten.

        Mer information om hur du redigerar poster i tabellvyn finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

        >[!TIP]
        >
        >Du kan markera flera poster eller objekt som du vill ta bort.

   * Du kan redigera alla planeringsposter i tabellen på den anslutna postsidan.
   * Använd något av följande vyelement i verktygsfältet på en ansluten postsida för att hantera tabellvyn:

   * **Filter**
   * **Sortera**. Inte tillgängligt för projekt.
   * **Gruppering**. Inte tillgängligt för projekt.
   * **Fält**, för att visa, dölja eller ordna om fält
   * **Radhöjd**. Inte tillgängligt för projekt.
   * **Sök**

     Mer information finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md).

     >[!NOTE]
     >
     >Du kan inte skapa, redigera eller ta bort fält i tabellvyn på fliken för en ansluten post.

   <!--No longer possible: 1. (Optional and conditional) When you create a connected records page for the following Workfront object types:
         * Portfolios
         * Programs
         * Groups
         * Companies
      Do any of the following in the table view of the connected records page: 
      * Click the name of a object. This opens the object's page in a new tab. 
      * Click **Connect** at the bottom of the table view to connect existing objects, select them from the connection box, then click outside the box to close it. The objects are automatically added to the table. The objects must exist before you can add them.
      For more information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).
      * Select one of the objects in the table view, then click one of the following options in the blue bar at the bottom of the list: 
      * **View** to open the record page in a new tab
      * **Copy link** to copy a link to the record page
      * **Disconnect** to disconnect the object from the record you are viewing. 
      >[!TIP]
      >
      >You can select more than one record or object to disconnect them.
      -->
1. (Valfritt och villkorligt) Gör något av följande när du skapar en ansluten postsida för anslutna Workfront-projekt:

   * Klicka på **Anslut poster** i det övre högra hörnet på den anslutna postsidan om du vill ansluta befintliga projekt.

     Mer information finns i [Anslut poster](/help/quicksilver/planning/records/connect-records.md).
   * Inline redigera projektinformation i registret.
   * Klicka på **Ny rad** om du vill skapa ett projekt utan en mall. Det nya projektet ansluts direkt till den aktuella posten.

     Mer information finns i [Skapa Workfront-objekt från Workfront Planning när du ansluter dem till poster](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)
   * Hovra över ett projekt och klicka på menyn **Mer** [Mer](assets/more-menu.png)

     eller

     Markera ett eller flera projekt och lägg märke till det blå fältet längst ned i listan. Klicka sedan på något av följande:

      * **Ta bort** om du vill ta bort projektet. Om du tar bort ett projekt kopplas det från posten och flyttas till Workfront papperskorg.
      * **Koppla från** om du vill koppla från projektet från posten. När du kopplar från ett projekt tas det bort och alla värden i sökfälten tas bort från den aktuella posten.

     >[!TIP]
     >
     >Du kan markera flera projekt som ska kopplas från eller tas bort.
   * Klicka på listrutan Vyer och sedan på **Ny vy** för att lägga till en ny vy för sidan. Gör sedan följande:
      1. Lägg till ett **visningsnamn**.
      1. Välj **Lista** i området **Visningstyp**.
      1. Klicka på **Skapa**.
En ny listvy läggs till i listrutan Vyer.
      1. (Valfritt) Håll muspekaren över namnet på en vy som du har skapat och klicka på menyn **Mer** ![Mer](assets/more-menu.png). Klicka sedan på något av följande alternativ:

         * **Byt namn på** om du vill lägga till ett nytt namn för vyn.
         * <span class="preview">**Dela**</span>
Mer information finns i [Dela vyer &#x200B;](/help/quicksilver/planning/access/share-views.md) .
         * **Ta bort**
Mer information finns i [Ta bort postvyer](/help/quicksilver/planning/views/delete-record-views.md).

           ![](assets/view-more-menu-projects-connected-records-page.png)
   * Klicka på ikonen **Filter** ![Filter &#x200B;](assets/filter-icon.png) och använd filtret för att visa specifika projekt.

     >[!TIP]
     >
     ><span class="preview">För persontypsfält, som **Ägare** eller **Sponsorn**, kan du använda ett jokertecken för att visa projekt där den inloggade användaren har tilldelats rollerna.</span>
     >
     >![Filtrera med användarens jokertecken för projektanslutna poster &#x200B;](assets/filter-with-user-wildcard-project-connected-records-page.png)
     >
   * Klicka på ikonen **Kolumner** ![Kolumner](assets/columns-icon.png) om du vill dölja eller visa kolumner i listan.
   * Klicka på ikonen **+** i tabellvyns övre högra hörn för att lägga till befintliga fält i tabellen. Fälten måste finnas innan du kan lägga till dem.

     Rutan **Kolumnhanteraren** öppnas. Gör följande:

      1. Sök efter ett befintligt objektfält i kolumnen **Tillgängligt** och klicka sedan på **+** till höger om fältnamnet för att lägga till det i kolumnen **Markerat**.

         De fält som du väljer läggs till i tabellvyn på sidan för anslutna poster.
      1. Klicka på **-** till höger om ett fält i kolumnen **Markerad** för att ta bort det från tabellvyn.
      1. Klicka på **Spara** för att spara den anslutna postsidans tabellvy.
1. (Valfritt) Dubbelklicka på namnet på fliken **Anslutna poster**

   eller

   Håll muspekaren över flikens namn, klicka sedan på **Mer** ![Mer-menyn](assets/more-menu.png) och klicka sedan på **Byt namn** för att byta namn till den nya fliken Ansluten vy.


   <!--1. <span class="preview">(Optional) Click the dropdown menu to the right of the view name, then click **New view** to add a view. For more information, see the section [Manage multiple views from the connected records page](#manage-multiple-views-from-the-connected-records-page) in this article. </span>-->

1. (Valfritt) Håll pekaren över namnet på fliken Anslutna poster, klicka på **Mer** ![Mer-menyn](assets/more-menu.png) och klicka sedan på **Ta bort** för att ta bort fliken.

<!--
<div class="preview">

## Manage multiple views from the connected records page

You can add and manage multiple view types from the connected records page of a record. 

The views you create in the Connected records page of a record type are available everywhere in Workfront Planning where that record type page displays. Views created for the same record type anywhere else in Workfront Planning are also accessible in all connected records pages of that record type. 

To manage multiple views from the connected records page: 

1. From the connected records page of a record, click the dropdown menu to the right of the view name, then click **New view** to add a view, then select from the following options: 

   * **Table**. For more information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 
   * **Timeline**. For more information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).
   * **Calendar**. For more information, see [Manage the calendar view](/help/quicksilver/planning/views/manage-the-calendar-view.md). 

1. (Optional) Hover over the name of a view in the Connected records page, then click the **More** menu ![More menu](assets/more-menu.png), then click one of the following: *************check to make sure these are all possible*********

   * **Rename**
   * **Share**. For more information, see [Share views](/help/quicksilver/planning/access/share-views.md).

   >[!TIP]
   >
   >Sharing views from Connected records pages makes them accessible to users in all areas of Workfront Planning where the view displays. 
   >Also, if a view is shared from any other area of Workfront Planning, it is also available to the same users in Connected records pages. 

   * **Export** 
   * **Duplicate**. For more information, see [Duplicate record views](/help/quicksilver/planning/views/duplicate-record-views.md).

      >[!TIP]
      >
      >Duplicating a view from Connected records pages makes it available in all other areas of Workfornt planning, when viewing the same record types. 

</div> -->
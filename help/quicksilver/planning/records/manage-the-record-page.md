---
title: Hantera postsidans layout
description: Du kan redigera layouten för postförhandsgranskning och -sida i Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '2262'
ht-degree: 0%

---


# Hantera postsidans layout

<!--
<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

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


<!--Old:
<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Products</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront Planning<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront plan*</p></td>
   <td>
<p>Any of the following Workfront plans:</p>
<ul><li>Select</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning is not available for legacy Workfront plans</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td>
   <td>
<p>Any</p>
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>

  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Object permissions</p></td>
   <td>
   <p>Contribute or higher permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> 
  </td>
  </tr>
 </tbody>
</table>-->

## Att tänka på när du redigerar postsidor

* Som standard visas alla fält som är kopplade till posten på information- och förhandsvisningssidorna för en post.

* Du kan inte lägga till nya fält för en post på förhandsgransknings- eller informationssidan. Du måste lägga till nya fält i tabellvyn för att kunna visa dem på förhandsgransknings- och informationssidorna.

* Du kan lägga till avsnitt på en förhandsgransknings- eller informationssida för att ordna informationen utifrån vanliga kriterier och göra den lättare att hitta.

* Följande ändringar påverkar alla poster av samma typ och är synliga för alla användare som använder dessa poster:

   * Ordna om fält
   * Lägga till eller ta bort avsnitt

* Visningsändringar som du gör i postförhandsgranskningen visas direkt på postinformationssidan. Ändringar som görs på postsidan visas också i rutan Förhandsgranska post.

* Att lägga till en omslagsbild eller en miniatyrbild i en post ingår inte i den övergripande layouten för postförhandsvisningen eller -sidan. Du kan lägga till unika omslagsbilder eller miniatyrbilder till varje post. Mer information finns i [Lägga till en omslagsbild i en post](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) och [Lägga till en miniatyrbild i en post](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

## Lägga till avsnitt i en postförhandsgranskning eller sida

Tänk på följande när du lägger till avsnitt på en postsida:

* Det finns ingen gräns för hur många avsnitt du kan ha på en sida.
* Du kan inte ha ett tomt avsnitt. Du måste ha minst ett fält i ett avsnitt.
* Du kan dra och släppa fält från ett avsnitt till ett annat. Mer information finns i avsnittet [Ordna om fält på sidan för postförhandsgranskning eller information](#rearrange-fields-in-the-record-preview-or-details-page) i den här artikeln.
* När du tar bort alla fält från ett avsnitt tas avsnittet automatiskt bort och kan inte återställas.

Så här lägger du till ett avsnitt i en postförhandsgranskning eller sida:

{{step1-to-planning}}

1. Klicka på kortet för en arbetsyta.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett posttypskort.

   Posttypssidan öppnas.

1. Klicka på en post i en vy av valfri typ

   eller

   I tabelltabellvyn klickar du på ikonen **Öppna detaljer** ![Öppna detaljikonen i tabellnamnsfältet](assets/open-details-icon-in-table-name-field.png) i den första kolumnen.

   Postens förhandsgranskning öppnas i vyn.

   ![Informationsruta](assets/details-box.png)

1. (Valfritt) Klicka på ikonen **Öppna på ny flik** ![Öppna information på en ny flikikon](assets/open-details-in-a-new-tab-icon.png) i det övre högra hörnet av postförhandsvisningen för att öppna postens sida på en ny flik.

   Postsidan öppnas. Fliken Detaljer öppnas som standard.

   ![Informationssida](assets/details-page.png)

1. På fliken **Detaljer** i postförhandsgranskningen eller på sidan för du pekaren över det tomma utrymmet till vänster om fälten och klickar sedan på ikonen **Lägg till avsnitt** ![Lägg till avsnitt](assets/add-section-icon.png) för att lägga till ett avsnitt.
1. Klicka i avsnittets namn och ersätt **Namnlöst avsnitt** med ett namn. Klicka sedan på Retur. Fälten som visas under avsnittet är automatiskt en del av det nya avsnittet.
1. Börja dra och släppa fält till det nya avsnittet, så som beskrivs i avsnittet [Ordna om fält i postförhandsgranskningen eller informationssidan](#rearrange-fields-in-the-record-preview-or-details-page) i den här artikeln.

1. (Valfritt) Håll pekaren över namnet på ett avsnitt och klicka på menyn **Mer** ![Mer](assets/more-menu.png).

   ![Fler menyalternativ för avsnittet på postsidan](assets/more-menu-options-for-section-on-record-page.png)
1. (Valfritt) Gör något av följande om du vill redigera avsnittet:

   * Klicka på **Byt namn på** om du vill byta namn på avsnittet

     >[!TIP]
     >
     > Du kan byta namn på ett avsnitt genom att klicka på namnet.

   * Klicka på **Flytta upp** för att flytta avsnittet uppåt en position

     eller

     Klicka på **Flytta nedåt** om du vill flytta avsnittet nedåt en position.
Alla fält i avsnittet flyttas tillsammans med avsnittet.

   * Klicka på **Ta bort** för att ta bort avsnittet. Avsnittet tas bort och kan inte återställas. Alla användare som har åtkomst till poster av den här typen kommer inte längre att visa det borttagna avsnittet.

1. Klicka på den nedåtriktade pilen till vänster om avsnittsnamnet för att komprimera det, eller på den högerriktade pilen för att expandera det.
Alla avsnitt expanderas som standard.

1. (Valfritt) Klicka på ikonen **Ta** ![Ta ögonblicksbild](assets/grab-icon.png) till vänster om ett avsnittsnamn och dra och släpp den på önskad plats.

   Avsnittets nya position uppdateras både i förhandsgranskningen och på sidan med alla poster av samma typ för alla användare som visar posterna.

   Alla ändringar i avsnitt och fältordning sparas automatiskt.

1. (Valfritt) Klicka på **Exportera**-menyn ![Exportikonen på informationssidan](assets/export-icon-in-record-details-page.png) för att exportera detaljfliken till en Word- eller PDF-fil. Mer information finns i [Exportera information för en post](/help/quicksilver/planning/records/export-the-record-page.md).

1. (Valfritt) Klicka på fliken **Anslutningar** bredvid fliken **Detaljer** . Du kan behöva klicka på **Mer** innan du klickar på fliken **Anslutningar**.

   Alla poster eller objekt som är kopplade till den valda posten visas under namnen på posttypen, eller i det program de tillhör.

   ![Fliken Anslutningar på posten i Workfront Planning](assets/connections-tab-on-record-in-workfront-planning.png)

1. (Valfritt) Välj inställningen **Visa alla poster** i det övre högra hörnet på fliken Anslutningar. Alla anslutna posttyper visas, inklusive de som ännu inte har några kopplade poster. Som standard är alternativet avmarkerat och posttyper utan kopplade poster är dolda.

1. (Valfritt) Klicka på **Anslut** för att lägga till fler poster till de anslutna posttyperna. Mer information finns i [Anslut poster](/help/quicksilver/planning/records/connect-records.md).

1. (Valfritt) Hovra över ett postkort, klicka på ikonen för att koppla från post **-** och klicka sedan på **Koppla från**. <!--this is copied to the Manage the Planning page in Workfront article; update in both articles-->
Följande saker händer:
   * Posten är inte längre ansluten till Workfront-objektet.
   * Workfront-objektet tas också bort från postens anslutna fält från Workfront Planning.
   * Värdena för Workfront sökfält som är kopplade till Planning-posten tas också bort.

## Ordna om fält på postens flik Detaljer

{{step1-to-planning}}

1. Klicka på kortet för en arbetsyta.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett posttypskort.

   Posttypssidan öppnas.

1. Klicka på en post i en vy av valfri typ

   eller

   I tabelltabellvyn klickar du på ikonen **Öppna detaljer** ![Öppna detaljikonen i tabellnamnsfältet](assets/open-details-icon-in-table-name-field.png) i den första kolumnen.

   Postens förhandsgranskning öppnas i vyn.

   ![Informationsruta](assets/details-box.png)

1. (Valfritt) Klicka på ikonen **Öppna på ny flik** ![Öppna informationsrutan i en ny flikikon](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> i det övre högra hörnet av postens förhandsgranskning för att öppna postens sida på en ny flik.

   Fliken **Detaljer** i posten öppnas som standard.

   ![Informationssida](assets/details-page.png)

1. På fliken **Detaljer** klickar du på ikonen **Ta** ![Ta tag i ](assets/grab-icon.png) till vänster om fältnamnet och drar och släpper den på önskad plats.

   >[!TIP]
   >
   >Du kan dra och släppa fält till ett annat avsnitt.
   >Du måste ha minst ett fält i ett avsnitt.
   >

   Den nya positionen för fältet uppdateras både i förhandsvisningen och på sidan med alla poster av samma typ för alla användare som visar posterna.

   Alla ändringar av layouten för postförhandsgranskningen eller sidan sparas automatiskt.

## Lägga till en sida med kopplade poster i en post

Du kan visa information från anslutna poster eller objekt genom att lägga till en flik för en sida med kopplade poster till en post. Då läggs de kopplade posterna i en tabellvy till på fliken.

Tänk på följande när du lägger till en sida med kopplade poster till en post:

* Du kan lägga till en sida med kopplade poster till en post efter att du har kopplat post- eller objekttyper till posttypen från tabellvyn för en posttyp.

* Du kan lägga till en sida med kopplade poster från en posts förhandsgranskningsområde eller postens sida.

* Anslutna postsidor visar endast anslutna objekt eller poster från ett objekt eller en posttyp i en tabellvy. På sidan visas inte alla poster av den typen.

* Du kan lägga till sidor med kopplade poster för följande anslutna post- eller objekttyper:

   * Workfront Planning - posttyper
   * Workfront projekt, program, portfolior, grupper eller företag. Du kan visa de anslutna Workfront-objekten även när du inte har åtkomstbehörighet till dem i Workfront.

  >[!NOTE]
  >
  > Du kan inte lägga till en sida med kopplade poster för anslutna AEM Assets-poster.

Så här lägger du till en sida med anslutna poster:

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

1. (Valfritt) Sök efter eller klicka på namnet på en ansluten post eller objekttyp i listan.

1. (Valfritt och villkorligt) Gör något av följande i tabellvyn på den anslutna postsidan när du visar anslutna Planning-poster eller andra Workfront-objekt, förutom för projekt: <!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

   * Klicka på namnet på en post. Posten öppnas på en ny flik.

   * Klicka på **Anslut** längst ned i tabellvyn om du vill ansluta fler poster och klicka sedan utanför anslutningsrutan för att stänga den. De nya posterna läggs automatiskt till i tabellen.

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
     
   * Redigera alla planeringsposter i tabellen på sidan Anslutna poster.

     Alla andra Workfront-objekt visas i en skrivskyddad tabellvy och du kan inte redigera dem.

1. (Valfritt och villkorligt) Gör något av följande i tabellvyn på den anslutna postsidan när du visar anslutna Workfront-projekt:

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

1. (Valfritt) Dubbelklicka på namnet på fliken **Anslutna poster**

   eller

   Håll muspekaren över flikens namn, klicka sedan på **Mer** ![Mer-menyn](assets/more-menu.png) och klicka sedan på **Byt namn** för att byta namn till den nya fliken Ansluten vy.
1. (Valfritt) Använd något av följande vyelement i verktygsfältet på en ansluten postsida för att hantera tabellvyn:

   * Filter
   * Sortera
   * Gruppering
   * Fält, för att visa, dölja eller ordna om fält
   * Radhöjd
   * Sök

   Mer information finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md).

   >[!NOTE]
   >
   >Du kan inte skapa, redigera eller ta bort fält i tabellvyn på fliken för en ansluten post.

1. (Valfritt) Håll pekaren över namnet på fliken Anslutna poster, klicka på **Mer** ![Mer-menyn](assets/more-menu.png) och klicka sedan på **Ta bort** för att ta bort fliken.

<!--
## Add a Brief page to a record's page

You can add a Brief page to the record's preview or pages. 

Brief pages contain the same information as the Details tab, in a read-only format. <!--edit this when we can remove fields from this page-->

<!--
1. From a record's page view, click the name of a record to open its preview or page.
1. Click **Add page** > **Brief**. 
1. Add the **Page name**, then click **Create**. 
-->




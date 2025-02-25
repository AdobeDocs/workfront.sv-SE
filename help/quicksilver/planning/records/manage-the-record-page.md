---
title: Hantera postsidans layout
description: Du kan redigera layouten för postförhandsgranskning och -sida i Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: f3f33d870859408db5ec3dc306cf1d4209c126a3
workflow-type: tm+mt
source-wordcount: '1772'
ht-degree: 0%

---


# Hantera postsidans layout

<!--<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

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
   <td role="rowheader"><p>Adobe Workfront Planning-paket*</p></td>
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
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Objektbehörigheter</p></td>
   <td>
   <p>Hantera behörigheter till en arbetsyta </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn och planeringsområdet för projekt, portföljer och program. </p> Mer information finns i <a href="/help/quicksilver/planning/access/access-overview.md">Åtkomstöversikt för Adobe Planning</a>. </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

   <!--<div class="preview">

    ![Details box](assets/details-box.png)  

    </div>-->

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

   <!--<div class="preview">

    ![Details box](assets/details-box.png) 

    </div>-->

1. (Valfritt) Klicka på ikonen **Öppna på ny flik** ![Öppna informationsrutan i en ny flikikon](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> i det övre högra hörnet av postens förhandsgranskning för att öppna postens sida på en ny flik.

   Fliken **Detaljer** i posten öppnas som standard.

   <!--<div class="preview">

   ![Details page](assets/details-page.png)

   </div>-->

1. På fliken **Detaljer** klickar du på ikonen **Ta** ![Ta tag i ](assets/grab-icon.png) till vänster om fältnamnet och drar och släpper den på önskad plats. <!--You can drag and drop fields to another section. You must have at least one field in a section.-->

   Den nya positionen för fältet uppdateras både i förhandsvisningen och på sidan med alla poster av samma typ för alla användare som visar posterna.

   Alla ändringar av layouten för postförhandsgranskningen eller sidan sparas automatiskt.

## Lägga till en sida i Anslutningsvyn på en postsida

<!--suggested a new name for this type of page: "Connected records details" - check to see if this changed-->

Tänk på följande när du lägger till en anslutningsvy på en postsida:

* Du kan lägga till en sida i Anslutningsvyn på en postsida.

* Du kan inte lägga till en sida i Anslutningsvyn i en posts förhandsvisningsområde.

* På sidor i anslutningsvyn visas en kopplad postsida i tabellvyn. Tabellvyn är skrivskyddad. <!--more views might be added in the future-->

* Du kan lägga till en sida i Anslutningsvyn för varje ansluten posttyp.  <!--edit this when we can remove fields from this page-->

* När du har lagt till en sida i Anslutningsvyn på en postsida visas sidfliken från postens förhandsvisningsområde. Du måste gå till den fullständiga sidan för att se tabellvyn för den anslutna posten. <!--this might have changed? check and take disclaimer out-->

Så här lägger du till en sida i Anslutningsvyn:

1. I en postsidvy klickar du på namnet på en post för att öppna den. Klicka sedan på ikonen **Öppna på ny flik** ![Öppna information på en ny flikikon](assets/open-details-in-a-new-tab-icon.png) i det övre högra hörnet på förhandsvisningssidan.
1. Klicka på **Lägg till sida** > **Anslutningsvy**.

   ![Lägg till spärrad sida för anslutningsvy](assets/add-connection-view-page-modal.png)
1. Lägg till **sidnamnet**, klicka på **Anslutningsvyn** och klicka sedan på **Skapa**.

   En ny flik läggs till på postens sida.
1. Sök efter eller klicka på namnet på en ansluten post eller objekttyp i listan.
Tabellvyn för den posttyp du valde visas och de kopplade posterna visas i tabellvyn.
Alla fält i den anslutna posten visas i tabellvyn på den anslutna postens flik.

   <!--<span class="preview">When you access Workfront Planning from the Preview environment, the first five fields from the connected record table display by default. No lookup fields display by default. -->

   Tabellvyn är skrivskyddad.

   <!--replace screen shot below when additional capabilities come to the table view - Fields, etc-->

   ![Målgruppsansluten tabellvy under kampanjinformation](assets/audience-connected-table-view-under-campaign-details-page.png)
1. (Valfritt) Dubbelklicka på flikens namn

   eller

   Håll muspekaren över flikens namn, klicka sedan på **Mer** ![Mer-menyn](assets/more-menu.png) och klicka sedan på **Byt namn** för att byta namn till den nya fliken Ansluten vy.
1. (Valfritt) Använd något av följande vyelement i verktygsfältet för att hantera tabellvyn

   * Filter
   * Sortera
   * Gruppering

   <!--Add to the list above from the list below - and condition these for Preview only: Hide fields, rearrange fields-->

   Mer information finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md).

   >[!NOTE]
   >
   >   Du kan inte göra något av följande i tabellvyn på fliken för en ansluten post:
   >
   >   * Dölj fält
   >   * Skapa, redigera eller ta bort fält
   >   * Ordna om fält
   >
1. (Valfritt) Håll pekaren över namnet på fliken och klicka sedan på **Mer** ![Mer-menyn](assets/more-menu.png). Klicka sedan på **Ta bort** för att ta bort från den nya fliken Ansluten vy.


<!--
## Add a Brief page to a record's page

You can add a Brief page to the record's preview or pages. 

Brief pages contain the same information as the Details tab, in a read-only format. <!--edit this when we can remove fields from this page-->

<!--
1. From a record's page view, click the name of a record to open its preview or page.
1. Click **Add page** > **Brief**. 
1. Add the **Page name**, then click **Create**. 
-->




---
title: Skapa poster
description: När du använder Adobe Workfront Planning är en post en instans av en posttyp. Du kan skapa unika poster för varje posttyp i Workfront Planning genom att manuellt lägga till dem i tabellvyn, importera dem från en lista, duplicera dem eller skapa dem när du ansluter dem till andra poster.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: 5bccad02f90fd99135b50c5a929913b16cc5b809
workflow-type: tm+mt
source-wordcount: '3240'
ht-degree: 0%

---


# Skapa poster

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

{{planning-important-intro}}

I Adobe Workfront Planning är en post en instans av en posttyp.

Du kan skapa poster genom att göra något av följande:

* [Använd knappen Ny post eller Begär post från valfri posttypsvy](#create-records-using-the-new-record-or-request-record-button-from-any-record-type-view)
* [Lägg till dem textbundet från posttypstabellvyn](#create-records-by-adding-them-inline-from-the-record-type-table-view)
* [Lägg till dem i tidslinjevyn för posttypen](#create-records-by-adding-them-in-the-record-type-timeline-view)
* [Lägg till dem i posttypens kalendervy](#create-records-by-adding-them-in-the-record-type-calendar-view)
* [Kopiera och klistra in en lista med poster från en extern lista](#create-records-by-copying-and-pasting-them-from-an-external-list)
* [Duplicera poster från en tabellvy](#create-records-by-duplicating-them)
* [Koppla dem från andra poster](#create-records-as-you-connect-them)
* [Skicka ett begärandeformulär till en posttyp](#create-records-by-submitting-a-request-form-to-a-record-type)
* [Importera information från en CSV- eller Excel-fil](#create-records-by-importing-records-from-a-csv-or-excel-file)
* [Använd automatisering](#create-records-by-using-automations)

Mer information om hur du hanterar poster i tabell- och tidslinjevyer finns i följande artiklar:

* [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md)
* [Hantera tidslinjevyn](/help/quicksilver/planning/views/manage-the-timeline-view.md)

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
<p>Alla Workfront- och Planning-paket</p> <p>Alla arbetsflöden och alla planeringsdokument</p>
<p>Mer information om vad som ingår i respektive Workfront Planning-paket får du av Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td> <p>Contribute eller högre behörigheter på arbetsytan och den posttyp där du vill lägga till poster. </p>
   <p>Visa eller högre behörigheter på arbetsytan och posttypen för att skapa poster med hjälp av knappen Begär post på postsidan</p>
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>
   <p>Hantera behörigheter för Workfront-objekt (portföljer) för att lägga till underordnade objekt (projekt).</p>
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
<p>Any </p> 
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
   <td> Standard
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p> 
   <p>Edit access in Workfront for the object types that you want to create (projects, programs, and portfolios) as you connect the records to them. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Contribute or higher permissions to the workspace and record type where you want to add records. </p>
   <p>View or higher permissions to the workspace and record type to create records using the Request record button on the record page</p>
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 

</tbody> 
</table> -->

## Att tänka på när du skapar poster

* Beroende på vilken arbetsyta de läggs till från visas poster som lagts till i globala posttyper av följande typer av användare:

   * Poster som läggs till på den ursprungliga arbetsytan för en global posttyp visas från den ursprungliga arbetsytan.
   * Poster som läggs till på en sekundär arbetsyta av en global posttyp visas bara från den arbetsyta som de skapades på och den ursprungliga arbetsytan för den globala posttypen.
Mer information finns i [Posttypöversikt för arbetsytan över &#x200B;](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).

* Beroende på deras behörigheter för arbetsytan och posttyperna kan användarna skapa poster på följande sätt:

   * Användare med behörigheten Visa på arbetsytan och posttypen kan bara skapa poster med hjälp av knappen Begär post på posttypsidan.
   * Användare med behörigheterna Contribute och Hantera på arbetsytan och i posttypen kan skapa poster med knappen Ny post på posttypssidan.

  >[!IMPORTANT]
  >
  >En arbetsytehanterare måste skapa ett begärandeformulär för posttypen för att användare med behörigheten Visa ska kunna lägga till poster med hjälp av ett begärandeformulär. Annars kan inte användare med behörigheten Visa skapa poster.


## Skapa poster med knappen Ny post eller Begär post från vilken posttyp som helst

{{step1-to-planning}}

1. Klicka på arbetsytan där du vill lägga till poster.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett posttypskort. Mer information om hur du skapar en posttyp finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

   Posttypssidan öppnas i den vy som du senast använde. Som standard öppnas en posttypssida i tabellvyn.
Alla poster av den valda typen visas i vyn.

1. (Villkorligt) I valfri vy kan du klicka på följande i skärmens övre högra hörn, beroende på arbetsytan och behörigheter för posttyp:

   * Klicka på **Ny post** om du har Contribute eller högre behörighet på arbetsytan och posttypen

     eller

   * Klicka på **Begär post** om du har behörigheten Visa på arbetsytan och posttypen.

1. (Villkorligt) Gör följande om du klickade på **Ny post**:

   1. Klicka på något av följande sätt för att skapa en post och klicka sedan på **Fortsätt**:

      * **Lägg till manuellt**. Postens förhandsvisningsruta öppnas.\
        Lägg till information om posten, enligt beskrivningen i avsnittet [Skapa poster genom att lägga till dem textbundet från posttyptabellvyn](#create-records-by-adding-them-inline-from-the-record-type-table-view) i den här artikeln, med början från steg 6. <!--insure this stays accurate-->
      * **Överför från fil**
Lägg till poster enligt beskrivningen i artikeln [Skapa poster genom att importera information från en CSV- eller Excel-fil &#x200B;](/help/quicksilver/planning/records/import-file-to-create-records.md), med början i steg 6. <!--ensure this stays accurate-->
      * **Skicka en begäran**
Formuläret med förfrågningar av posttyp öppnas.

        En arbetsytehanterare måste skapa ett begärandeformulär för att kunna lägga till en post med hjälp av ett begärandeformulär.

        >[!TIP]
        >
        >Vissa posttyper kan ha flera formulär. Klicka på en för att öppna den.

        Lägg till posten enligt beskrivningen i artikeln [Skicka Adobe Workfront Planning-begäranden för att skapa poster](/help/quicksilver/planning/requests/submit-requests.md), med början i steg 6. <!--ensure this stays accurate-->

      ![Tre sätt att skapa valfria poster](assets/three-ways-to-create-records-choice-modal.png)

1. (Villkorligt) Gör följande om du klickade på **Begär post**:

   1. (Villkorligt) Om posttypen har fler än ett begärandeformulär klickar du på ett för att välja det.
   2. Fortsätt lägga till information i formuläret för att skapa posten, så som beskrivs i artikeln [Skicka Adobe Workfront Planning-begäranden för att skapa poster](/help/quicksilver/planning/requests/submit-requests.md), med början från steg 6. <!--ensure this stays accurate-->

1. (Villkorligt) Granska de nya posterna.

   Beroende på hur du väljer att lägga till posten kan följande saker hända:

   * En ny post läggs till posttypen, såvida du inte väljer att lägga till den med ett begärandeformulär med en godkännandeprocess. Godkännandet måste beviljas av alla godkännare innan posten skapas.
   * Flera poster läggs till posttypen om du har lagt till poster med hjälp av ett CSV- eller Excel-kalkylblad.
   * En ny begäran läggs till i området för Workfront-förfrågningar om du lade till den genom att skicka ett begärandeformulär.

<!-- this is not possible anymore: 

## Create records by connecting them from another application

You can import records from other applications by linking them to existing records. This creates a linked record for the other application's connected object. 

1. Create a record type, as described in the [Create record types](/help/quicksilver/planning/architecture/create-record-types.md).

1. Create records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a connection to an object type from another application for the record type you created. For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Add objects from another application to the records you created above using the linked record field you created in the previous step. For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 

    The following items are created in Workfront Planning:

    * A read-only record type that refers to the other application's record type you linked to in the connected record field. 

      For example, if you connect a Planning record type to Workfront project, a read-only record type named "Workfront project" is created in the same workspace. You can access the read-only Workfront record types from the table view of the Planning records you're linking from. 
   
-->

## Skapa poster genom att lägga till dem textbundet från registervyn för posttyp

Du kan skapa poster i tabellvyn för en posttypsida när du lägger till dem textbundet.

Mer information om hur du redigerar postinformation finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

{{step1-to-planning}}

1. Klicka på arbetsytan där du vill lägga till poster.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett posttypskort. Mer information om hur du skapar en posttyp finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

   Posttypssidan öppnas i den vy som du senast använde. Som standard öppnas en posttypssida i tabellvyn.
Poster av den valda typen visas i vyn.

1. (Villkorligt) Gör något av följande i tabellvyn:

   * Klicka på **Ny post** på den sista raden i tabellen eller efter den sista posten i en gruppering

     >[!TIP]
     >
     >När du lägger till en ny post efter den sista posten i en gruppering eller delgruppering, fyller Workfront automatiskt i de fält som ingår i grupperingarna. Du kan redigera dessa fält manuellt om det behövs och posterna kan tas bort från grupperingen.

   * Klicka på **Skift + Retur** på tangentbordet från valfri kolumn eller rad i tabellen. Då läggs en tom rad till under den post du börjar från.
   * Håll markören över en posts primära fält, klicka på menyn **Mer** ![Mer](assets/more-menu.png) till höger om fältet och klicka sedan på **Infoga post ovanför** eller **Infoga post nedanför**.

   ![Lägger till en ny kampanj i tabellraden](assets/adding-a-new-campaign-in-table-row.png)

   Workfront överför automatiskt en miniatyrbild till varje ny post. Du kan ändra dessa bilder senare. Mer information finns i [Lägga till en omslagsbild till en post](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md).

   En ny post läggs till i tabellen.

1. Klicka på den nya postens primära fält

   eller

   Klicka på ikonen **Öppna detaljer** ![Öppna detaljikonen i tabellnamnsfältet](assets/open-details-icon-in-table-name-field.png) till vänster om postnamnet.

   Förhandsvisningsrutan öppnas i tabellen.

1. Börja skriva information om den nya posten i de fält som visas i förhandsvisningsrutan.

   >[!NOTE]
   >
   >  * Det finns inga obligatoriska fält för poster. Vi rekommenderar dock att du lägger till information för det primära fältet i en post, eftersom det är praktiskt att identifiera poster när du länkar poster till varandra. Mer information om primära fält finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md) och [Översikt över primära fält](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >  * Fält som refererar till andra posttyper eller beräknade fält är skrivskyddade fält.

1. (Villkorligt) När du lägger till poster i tabellen fortsätter du att lägga till information på varje rad innan du öppnar postens förhandsvisningsruta. Klicka sedan på **Retur** på tangentbordet för att spara ändringarna.

   eller

   Klicka på den nya postens namn eller på ikonen **Öppna detaljer** ![Öppna informationsikonen i tabellnamnsfältet](assets/open-details-icon-in-table-name-field.png) till vänster om postens namn för att öppna förhandsvisningsrutan och redigera postens information i informationsområdet.

   >[!TIP]
   >
   >Du kan bara komma åt ikonen **Öppna detaljer** från postens namnfält när fältet Namn är ett primärt fält.

1. (Valfritt) I postens förhandsvisningsruta klickar du på ikonen **Öppna på ny flik** ![Öppna detaljer i en ny flikikon](assets/open-details-in-a-new-tab-icon.png) i det övre högra hörnet för att öppna postens sida på en ny flik. Fortsätt redigera posten på postsidan. Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

   Workfront sparar automatiskt ändringarna.

1. (Valfritt) Stäng förhandsvisningsrutan eller klicka på bakåtpilen till vänster om postens namn om du öppnade postens sida.

1. (Valfritt) I tabellvyn använder du följande kortkommandon för att ångra eller göra om tillägg av nya poster eller deras information när du lägger till dem i tabellvyn:

   * CTRL + Z (⌘ + Z för Mac) för att ångra en ändring
   * CTRL + Skift + Z (⌘ + Skift + Z för Mac) för att göra om en ändring


## Skapa poster genom att lägga till dem i posttypens tidslinjevy

Du kan skapa poster i tidslinjevyn på en posttypsida genom att dubbelklicka på tidslinjen.

Mer information om hur du skapar en tidslinjevy finns i [Hantera tidslinjevyn](/help/quicksilver/planning/views/manage-the-timeline-view.md).

{{step1-to-planning}}

1. Klicka på arbetsytan där du vill lägga till poster.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett posttypskort.

   Posttypssidan öppnas i den vy som du senast använde.

1. Klicka för att öppna en tidslinjevy eller skapa en tidslinjevy först.

   >[!NOTE]
   >
   >Du kan bara skapa en tidslinjevy om det finns minst två datumfält associerade med posttypen.
1. Dubbelklicka var som helst i tidslinjen.

   Rutan **Ny post** öppnas. <!--might need a new screen shot for Production - might add a title etc-->

   ![Ny postruta på tidslinjen med namnlöst postfält](assets/new-record-small-box-on-timeline.png)

   >[!NOTE]
   >
   >Du kan inte skapa poster i tidslinjevyn när postfälten visas i en namngiven gruppering.
1. Uppdatera följande information:


   * **Namn**: Ange postens namn. Om du lämnar den tom namnges den som **Namnlös** som standard av Workfront.

     >[!TIP]
     >
     >Om du visar namnet på posten i postfälten enligt tidslinjeinställningarna, visas inte namnet i postfältet om det inte finns något.

   * **Registrera datumfält**: Uppdatera postens datum.

     Namnen på datumfälten anpassas efter de fält som valts för start- och slutdatum när tidslinjevyn skapades.

     Som standard är datumvärden förinställda beroende på hur du visar tidslinjevyn. Följande scenarier finns:

      * Efter **År**: Postens start- och slutdatum sträcker sig över en månad.
      * Efter **Kvartal**: Postens start- och slutdatum sträcker sig över en vecka.
      * Efter **månad**: Postens start- och slutdatum sträcker sig över tre dagar.

1. (Valfritt) Klicka på en av följande ikoner:

   * **Expandera** ![Expandera ikonen](assets/expand-icon.png) om du vill öppna postinformationen i förhandsvisningsfönstret.
   * **Ta bort** ![Ta bort ikon](assets/delete-icon.png) om du vill ta bort posten.
   * **Stäng** ![Stäng ikonen](assets/close-icon.png) för att stänga den nya postrutan.

   Posten läggs till på tidslinjen samt i tabell- och kalendervyerna direkt, om du inte har klickat på ikonen **Ta bort** .

1. (Valfritt) Håll markören över en av postfältets marginaler på tidslinjen och dra och släpp sedan fältets ändar till ett annat datum. Detta ändrar automatiskt postens start- och slutdatum.

   Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

1. (Valfritt) Klicka på postfältet på tidslinjen för att öppna postens informationsfönster och uppdatera informationen, ta bort den eller lägga till kommentarer.

   >[!TIP]
   >
   >Som standard associerar Workfront posten med en miniatyrbild och en omslagsbild.
   >
   >Miniatyrbilden visas bara i tidslinjevyn när den är aktiverad i vyinställningarna.



## Skapa poster genom att lägga till dem i posttypens kalendervy

Du kan skapa poster i kalendervyn på en posttypsida genom att dubbelklicka var som helst i kalendern.

Mer information om hur du skapar en kalendervy finns i [Hantera kalendervyn](/help/quicksilver/planning/views/manage-the-calendar-view.md).

{{step1-to-planning}}

1. Klicka på arbetsytan där du vill lägga till poster.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett posttypskort.

   Posttypssidan öppnas i den vy som du senast använde.

1. Klicka för att öppna en kalendervy eller skapa en kalendervy.

   >[!NOTE]
   >
   >Du kan bara skapa en kalendervy om det finns minst två datumfält associerade med posttypen.
1. Dubbelklicka någonstans i kalendern.

   Rutan **Ny post** öppnas. <!--(********might need a new screen shot for Production - might add a title etc*********ALSO CHECK IF THE SAME ONE NEEDS REPLACING FOR TIMELINE?????)-->

   ![Ny postruta i kalendern med namnlöst postfält](assets/new-record-small-box-on-calendar.png)

1. Uppdatera följande information:

   * **Namn**: Ange postens namn. Om du lämnar den tom namnges den som **Namnlös** som standard av Workfront.

     >[!TIP]
     >
     >Om du visar namnet på posten i postfälten enligt kalenderinställningarna, visas inte namnet i postfältet om det inte finns något.

   * **Registrera datumfält**: Uppdatera postens datum.

     Namnen på datumfälten anpassas efter de fält som valdes för start- och slutdatumen när kalendervyn skapades.

     Som standard är datumvärden förinställda beroende på hur du visar kalendervyn. Följande scenarier finns:

      * Efter **månad**: Postens start- och slutdatum sträcker sig över en dag.
      * Efter **Vecka**: Postens start- och slutdatum sträcker sig över två dagar.

1. (Valfritt) Klicka på en av följande ikoner:

   * **Expandera** ![Expandera ikonen](assets/expand-icon.png) om du vill öppna postinformationen i förhandsvisningsfönstret.
   * **Ta bort** ![Ta bort ikon](assets/delete-icon.png) om du vill ta bort posten.
   * **Stäng** ![Stäng ikonen](assets/close-icon.png) för att stänga den nya postrutan.

   Posten läggs till i kalendern samt i tabell- och tidslinjevyerna direkt, om du inte har klickat på ikonen **Ta bort** .
1. (Valfritt och villkorligt) Välj **Månad** i listrutan i det övre hörnet, håll markören över en av postfältets marginaler i kalendern och dra och släpp fältets ändar till ett annat datum. Detta ändrar automatiskt postens start- och slutdatum.

   Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).
1. (Valfritt) Klicka på postfältet i kalendern för att öppna postens informationsfönster och uppdatera informationen, ta bort den eller lägga till kommentarer.

   >[!TIP]
   >
   >Som standard associerar Workfront posten med en miniatyrbild och en omslagsbild.
   >
   >Miniatyrbilden visas bara i kalendervyn när den är aktiverad i vyinställningarna.

   <!--(*********when this is available in both monthly and weekly, add more steps to show resizing the timeline and dragging and dropping the record in the calendar*******)-->

## Skapa poster genom att kopiera och klistra in dem från en extern lista

1. Börja skapa poster i tabellvyn, enligt beskrivningen i avsnittet [Skapa poster genom att manuellt lägga till dem till en posttyp](#create-records-by-manually-adding-them-to-a-record-type) i den här artikeln.

   Se till att tabellvyn innehåller kolumnerna (eller fälten) som du vill fylla med den nya postinformationen.

1. Klicka på **Nytt &lt; posttypnamn >** i den sista raden i tabellen om du vill lägga till så många nya rader i tabellen som du vill att de nya posterna ska vara.

   Lägg till exempel till 10 rader i tabellvyn om du vill klistra in informationen för 10 nya poster från ett annat program.

1. Skapa en lista med poster som du vill importera i ett annat program.

   Du kan t.ex. använda ett Excel-kalkylblad för att skapa en lista.

   Listan bör innehålla information i tabellformat.

   >[!TIP]
   >
   > Kolumnerna i listan bör innehålla information om de fält du har i Workfront.
   >
   > Kontrollera att du redan har skapat de önskade fälten i Workfront och att informationen i bladet visas i rätt format, som matchar fälten i Workfront.

1. I ett annat program markerar du flera rader och kolumner och klistrar sedan in informationen i posttypstabellvyn, med början från den första nya posten.

   Följande information importeras till Workfront Planning:

   * Raderna innehåller de nya posterna
   * Kolumnerna fyller i information för posternas fält.

## Skapa poster genom att duplicera dem

Mer information om att duplicera poster finns i [Duplicera poster](/help/quicksilver/planning/records/copy-or-duplicate-records.md).

## Skapa poster när du kopplar dem

Du kan skapa följande objekttyper när du kopplar dem från andra poster:

* Workfront Planning - poster
* Workfront-objekt

I det här avsnittet beskrivs hur du skapar Workfront Planning-poster när du kopplar dem från andra poster.

>[!NOTE]
>
>Att skapa Workfront-projekt och portföljer när du kopplar dem till Workfront Planning-poster liknar att skapa Planning-poster när du kopplar dem från andra poster.
>
>Mer information om hur du skapar Workfront-objekt från Workfront Planning finns i [Skapa Workfront-objekt från Workfront Planning när du ansluter dem till poster](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md).

Du måste ha följande innan du kan lägga till nya poster genom att koppla dem från befintliga poster:

* Anslutna posttyper. Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).
* Poster.
* Rätt åtkomst och behörigheter i Workfront Planning och Workfront, enligt beskrivningen i avsnittet [Åtkomstkrav](#access-requirements) i den här artikeln.

Så här skapar du poster när du kopplar dem från andra poster:

1. Börja ansluta Workfront Planning-poster enligt beskrivningen i artikeln [Anslut poster](/help/quicksilver/planning/records/connect-records.md). Du kan koppla poster från följande områden:

   * Ett anslutningsfält i följande områden av Workfront Planning:

      * Tabellvyn
      * Informationssidan eller förhandsvisningsrutan för en post

   * Ett anslutningsfält i planeringsavsnittet för ett projekt, en portfölj eller ett program i Workfront.

     Mer information finns i [Hantera postanslutningar från Workfront-objekt](/help/quicksilver/planning/records/manage-records-in-planning-section.md).

1. (Villkorligt) Om du inte kan hitta en post när du försöker ansluta den klickar du på **+ Lägg till**

   eller
Börja skriva ett namn och klicka sedan på **+ Lägg till**. Knappen **+ Lägg till** följs av namnet på den posttyp som du ansluter till. Exempel:&quot;Lägg till varumärken&quot; när du lägger till ett varumärke i en befintlig kampanj. Namnet som du skrev följer även knappen Lägg till.

   ![Lägg till knapp för att skapa poster i kontextmarkerad](assets/add-button-to-create-records-in-context-highlighted.png)

   Posten skapas och läggs till i det anslutna postfältet.

   >[!IMPORTANT]
   >
   >* Du kan bara skapa projekt, portföljer och program i Workfront när du kopplar dem från en post.
   >
   >* Du kan inte skapa grupper eller företag när du kopplar dem från en post i Workfront Planning.
   > 

1. (Valfritt) Gå till tabellvyn för den posttyp vars post du skapade. En ny post visas på den sista raden i vyn.
1. (Valfritt) Börja lägga till information för den nya posten i tabellvyn
eller
Klicka på namnet för att öppna informationssidan och lägga till information där.

## Skapa poster genom att skicka ett begärandeformulär till en posttyp

När någon skapar ett begärandeformulär för en posttyp och delar en länk till den med dig, kan du skicka en begäran som skapar en post för den posttypen.

Mer information finns i [Skapa och hantera ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

Både Workfront-användare och användare utanför din organisation kan skicka begäranden till posttyperna Planning och skapa poster, om de har en länk till förfrågningsformuläret.

Mer information finns i [Skicka Adobe Workfront Planning-begäranden för att skapa poster](/help/quicksilver/planning/requests/submit-requests.md).

## Skapa poster när du importerar posttyper från en CSV- eller Excel-fil

Du kan importera poster när du importerar posttyper med hjälp av en CSV- eller Excel-fil.

Mer information finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

## Skapa poster genom att importera poster från en CSV- eller Excel-fil

Du kan importera poster för befintliga posttyper när du importerar information från en CSV- eller Excel-fil.

Mer information finns i [Skapa poster genom att importera information från en CSV- eller Excel-fil](/help/quicksilver/planning/records/import-file-to-create-records.md).

## Skapa poster med hjälp av automatisering

Du kan konfigurera automatisering i Workfront Planning som, när den aktiveras, skapar poster när de aktiveras från en Planning-post. De skapade posterna kopplas automatiskt till de poster som du aktiverar automatiseringen från.

Du kan konfigurera och aktivera automatiseringen på postens sida i Workfront Planning. Den anslutna post som skapas placeras i det anslutna fältet för den posttyp som du kör automatiseringen från.

Mer information finns i [Skapa objekt med hjälp av postautomatisering för Adobe Workfront Planning &#x200B;](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).




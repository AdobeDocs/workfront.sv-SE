---
title: Skapa poster
description: När du använder Adobe Workfront Planning är en post en instans av en posttyp. Du kan skapa unika poster för varje posttyp i Workfront Planning genom att manuellt lägga till dem i tabellvyn, importera dem från en lista, duplicera dem eller skapa dem när du ansluter dem till andra poster.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: 597d8db034269e673dbe46e8c0f4934bf9509e2f
workflow-type: tm+mt
source-wordcount: '1593'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Skapa poster

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

I Adobe Workfront Planning är en post en instans av en posttyp.

Du kan skapa poster genom att göra något av följande:

* [Lägga till poster från posttypsidan i tabellvyn](#create-records-by-adding-them-to-a-record-type-in-a-record-type-table)
* [Kopiera och klistra in en lista med poster från en extern lista](#create-records-by-copying-and-pasting-them-from-an-external-list)
* [Duplicera poster från en tabellvy](#create-records-by-duplicating-them)
* [Skapa poster när du kopplar dem från andra poster](#create-records-as-you-connect-them)
* [Skapa poster genom att skicka ett begärandeformulär till en posttyp](#create-records-by-submitting-a-request-form-to-a-record-type)
* [Skapa poster när du importerar posttyper från en CSV- eller Excel-fil](#create-records-when-importing-record-types-from-a-csv-or-excel-file)

<!--* <span class="preview">[Create records by using automations](#create-records-by-using-automations)</span>-->


Mer information om hur du hanterar poster i tabell- och tidslinjevyer finns i följande artiklar:

* [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md)
* [Hantera tidslinjevyn](/help/quicksilver/planning/views/manage-the-timeline-view.md)

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
<p>Alla </p> 
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
   <td> Standard
   <p>Workfront Planning är inte tillgängligt för tidigare Workfront-licenser</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p> 
   <p>Redigera åtkomst i Workfront för de objekttyper som du vill skapa (projekt och portföljer) när du kopplar posterna till dem. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td> <p>Hantera behörigheter för den arbetsyta som du vill lägga till poster i. </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>
   <p>Hantera behörigheter för Workfront-objekt (portföljer) för att lägga till underordnade objekt (projekt).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutmall</p></td> 
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn </p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa poster genom att lägga till dem till en posttyp i en posttypstabell

Du kan skapa poster i tabellvyn för en posttypssida.

Mer information om hur du redigerar postinformation finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

{{step1-to-planning}}

1. Klicka på arbetsytan där du vill lägga till poster.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett posttypskort. Mer information om hur du skapar en posttyp finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

   Posttypssidan öppnas i den vy som du senast använde. Som standard öppnas en posttypssida i tabellvyn.
Alla poster av den valda typen visas i vyn.

1. (Villkorligt) Beroende på vilken vy du visar gör du något av följande:

   * Från tabellvyn:

      * Klicka på **Ny post** i den sista raden i tabellen

      * Klicka på **Skift + Retur** på tangentbordet från valfri kolumn eller rad i tabellen. Då läggs en tom rad till under den post du börjar från.
      * Håll markören över en posts primära fält, klicka på menyn **Mer** ![Mer](assets/more-menu.png) till höger om fältet och klicka sedan på **Infoga post ovanför** eller **Infoga post nedanför**.

     ![Lägger till en ny kampanj i tabellraden](assets/adding-a-new-campaign-in-table-row.png)

   * Från alla vyer:

      * Klicka på **Ny post** i det övre högra hörnet på sidan. Förhandsgranskningsrutan för posten öppnas.

     Workfront överför automatiskt en miniatyrbild och en omslagsbild till varje ny post. Du kan ändra dessa bilder senare. Mer information finns i följande artiklar:

      * [Lägga till en omslagsbild till en post](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
      * [Lägga till en miniatyrbild i en post](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

1. Börja skriva information om den nya posten i de fält som visas i förhandsvisningsrutan.

   >[!NOTE]
   >
   >  * Det finns inga obligatoriska fält för poster. Vi rekommenderar dock att du lägger till information för det primära fältet i en post, eftersom det är praktiskt att identifiera poster när du länkar poster till varandra. Mer information om primära fält finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md) och [Översikt över primära fält](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >  * Fält som refererar till andra posttyper eller beräknade fält är skrivskyddade fält.

1. (Villkorligt) När du lägger till poster i tabellen fortsätter du att lägga till information på varje rad och klickar sedan på **Retur** på tangentbordet för att spara ändringarna.

   eller

   Klicka på den nya postens namn eller på ikonen **Öppna detaljer** ![Öppna informationsikonen i tabellnamnsfältet](assets/open-details-icon-in-table-name-field.png) till vänster om postens namn. En förhandsgranskning med postens detaljerade information öppnas i tabellen.

   >[!TIP]
   >
   >Du kan bara komma åt ikonen **Öppna detaljer** från postens namnfält när fältet Namn är ett primärt fält.

1. Börja redigera postens information i postens förhandsgranskning. Workfront sparar automatiskt ändringarna.
1. (Valfritt) Klicka på ikonen **Öppna på ny flik** ![Öppna information på en ny flikikon](assets/open-details-in-a-new-tab-icon.png) i det övre högra hörnet av postens förhandsgranskning för att öppna postens sida på en ny flik. Fortsätt redigera posten på postsidan. Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

1. (Valfritt) Använd följande kortkommandon om du vill ångra eller göra om tillägg av nya poster eller deras information när du lägger till dem i tabellvyn:

   * CTRL + Z ( ⌘ + Z för Mac) för att ångra en ändring
   * CTRL + Skift + Z ( ⌘ + Skift + Z för Mac) för att göra om en ändring

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
>Mer information om hur du skapar Workfront-objekt från Workfront Planning finns i [Skapa Workfront-objekt från Workfront Planning](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md).

Du måste ha följande innan du kan lägga till nya poster genom att koppla dem från befintliga poster:

* Anslutna posttyper. Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).
* Poster.
* Rätt åtkomst och behörigheter i Workfront Planning och Workfront, enligt beskrivningen i avsnittet [Åtkomstkrav](#access-requirements) i den här artikeln.

Så här skapar du poster när du kopplar dem från andra poster:

1. Börja ansluta Workfront Planning-poster enligt beskrivningen i artikeln [Anslut poster](/help/quicksilver/planning/records/connect-records.md). Du kan koppla poster från ett anslutningsfält i följande områden i Workfront Planning:

   * Tabellvyn
   * Informationssidan eller förhandsvisningsrutan för en post

1. (Villkorligt) Om du inte kan hitta en post när du försöker lägga till den från det anslutna postfältet för en annan post söker du efter en post och klickar sedan på **+ Lägg till**. Knappen **+ Lägg till** följs av namnet på den posttyp som du ansluter till. Exempel:&quot;Lägg till varumärken&quot; när du lägger till ett varumärke i en befintlig kampanj. Namnet som du skrev följer även knappen Lägg till.

   <!--remove the first part of the step above to say just Click Add when the button will be persistent, for preview and production-->

   ![Lägg till knapp för att skapa poster i kontextmarkerad](assets/add-button-to-create-records-in-context-highlighted.png)

   Posten skapas och läggs till i det anslutna postfältet.

   <!--
    >[!IMPORTANT]
    >
    >* You can create only projects and portfolios in Workfront when connecting them from a record. 
    >
    >* You cannot create programs, groups, or companies when connecting them from a record in Workfront Planning. 
    >
    >* You cannot create a project from a template when when you create projects by connecting them from a record. You must manually add tasks and project information or a template to the new project after you add it to the record. -->

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

<!--
<div class="preview">

## Create records by using automations

You can configure automations in Workfront Planning that, when activated, create records when triggered from a Planning record. The created records are automatically connected to the records you are triggering the automation from.

You can configure and activate the automation in the record's page in Workfront Planning. The connected record that is created is placed in the connected field of the record type you run the automation from.

For information, see [Create objects using Adobe Workfront Planning record automations](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md). 

</div>

-->

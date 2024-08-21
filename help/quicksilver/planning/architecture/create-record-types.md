---
title: Skapa posttyper
description: Posttyperna är objekttyperna för Adobe Workfront Planning. I Workfront Planning kan du skapa anpassade posttyper som illustrerar de arbetsuppgifter som behövs i organisationens livscykel.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: f713e8fa72c98b6df2509e71acd7080d4df46a3a
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->
<!--this is linked to the UI in an empty workspace screen-->

# Skapa posttyper

{{planning-important-intro}}

Posttyperna är objekttyperna för Adobe Workfront Planning. I Workfront Planning kan du skapa anpassade posttyper som illustrerar de arbetsrelaterade objekt som behövs i organisationens livscykel.

Mer information om posttyper finns i [Översikt över posttyper](/help/quicksilver/planning/architecture/overview-of-record-types.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven för Workfront Planning.

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
   <td> Adobe Workfront
   </td>
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
   <p>Aktuell: Planera</p>
   eller
   <p>Nytt: Standard </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td>
   <td> <p>Det finns inga åtkomstnivåkontroller för Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Workfront- eller gruppadministratören måste lägga till planeringsområdet i layoutmallen. Mer information finns i <a href="/help/quicksilver/planning/access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Hantera behörigheter till en arbetsyta </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade
</td>
  </tr>
 </tbody>
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Att tänka på när du skapar posttyper

* Du kan skapa posttyper på en arbetsyta på följande sätt:

   * Automatiskt:
      * När du skapar en arbetsyta med hjälp av en mall.

        Mer information finns i [Skapa arbetsytor](/help/quicksilver/planning/architecture/create-workspaces.md).

     <!--* When you import them using an Excel or CSV file. 

            >[!IMPORTANT]
            >
            >This functionality has been temporarily removed since March 21, 2024. It will be enabled at a later date.-->

     <!--this should not ne known anymore: * When you add objects from another application to a linked record field of a record. This creates a read-only record type in Workfront Planning which is connected to object types from the original application. 
        For information about connecting record types with object types from another application, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).
        For information about connecting objects with records, see [Connect records](/help/quicksilver/planning/records/connect-records.md). -->
   * Manuellt:

      * Från scratch.

        I den här artikeln beskrivs hur du skapar posttyper från grunden.

* Du kan flytta posttyper inom ett avsnitt och från ett avsnitt på en arbetsyta till ett annat. Du kan inte flytta posttyper från en arbetsyta till en annan.

## Skapa posttyper med hjälp av en arbetsytemall

Du kan skapa posttyper automatiskt när du skapar en arbetsyta med en Workfront Planning-mall. Varje mall innehåller exempelposttyper.

När du skapar en arbetsyta från en mall grupperas posttyperna i följande avsnitt:

* Operativa posttyper
* Taxonomier

Du kan lägga till posttyper manuellt i avsnitten Driftposttyper och Taxonomier.

Mer information om hur du skapar arbetsytor finns i [Skapa arbetsytor](/help/quicksilver/planning/architecture/create-workspaces.md).

Mer information om vilka posttyper som ingår i varje mall finns i [Lista över arbetsytemallar](/help/quicksilver/planning/architecture/workspace-templates.md).

## Skapa en posttyp från grunden

{{step1-to-planning}}

1. Klicka på arbetsytan där du vill skapa en posttyp,

   eller

   Utöka den nedåtriktade pilen till höger om namnet på en befintlig arbetsyta i en arbetsyta, sök efter en arbetsyta och markera den när den visas i listan.
1. (Valfritt) Klicka på **Lägg till avsnitt** om du vill lägga till ett nytt avsnitt på arbetsytan.
1. Klicka på **Lägg till posttyp**.

   Rutan Lägg till posttyp öppnas.
   <!--1. (Conditional) When creating record types by importing an Excel or CSV file is enabled, click **From scratch**. Otherwise, the **Add record type** box opens. -->

   ![](assets/add-record-type-box-with-appearance-options.png)

1. Uppdatera följande information:

   * Ersätt&quot;Namnlös posttyp&quot; med namnet på din framtida posttyp. <!--did they bring back the field label here and did they rename it to "Name"-->
   * **Beskrivning**: Lägg till mer information om posttypen.
   * Välj en färg och form för den ikon som är associerad med posttypen. Gör följande:
      * Välj en färg som identifierar den nya posttypen. Det här är färgen på ikonen för posttyp. Grått är markerat som standard.
      * Välj en ikon i listan eller börja skriva namnet på en ikon för att beskriva vad den representerar och markera den sedan när den visas. Det här är ikonen för posttypen. Som standard är en filikon markerad.

1. Klicka på **Skapa**.

   Posttypkortet läggs till i avsnittet och på den arbetsyta som du har valt.
Beskrivning av posttypen visas på kortet.

   ![](assets/record-type-card-with-description.png)

1. (Valfritt) Håll markören över posttypskortet, klicka på ikonen **Mer** ![](assets/more-menu.png) i det övre högra hörnet och klicka sedan på **Redigera** för att ändra information om posttypen.
1. (Valfritt) Klicka på posttypskortet för att öppna posttypssidan.

   ![](assets/operational-record-type-blank.png)

   Posttypssidan visas som standard i tabellvyn. Kolumnerna i tabellen är fält som är kopplade till den nya posttypen. Varje rad är en unik post som du måste lägga till.

   <!--TIP: If you import a record type from an Excel or CSV file, records are also imported.-->

   Som standard visas följande fält i tabellvykolumnerna för en operativ posttyp:

   * Namn
   * Beskrivning
   * Startdatum
   * Slutdatum
   * Status

1. (Valfritt) Uppdatera posttypens namn i sidhuvudet

   eller

   Klicka på ikonen **Mer** ![](assets/more-menu.png) till höger om posttypens namn och klicka på **Redigera** för att byta namn på den eller ändra informationen om den. Mer information finns i [Redigera posttyper](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Valfritt) Klicka på **+ Ny post** om du vill lägga till poster av den valda posttypen. Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).
1. (Valfritt) Klicka på ikonen **+** i tabellens övre högra hörn för att lägga till fler fält i posttypen.

   Mer information om hur du skapar fält finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

1. (Valfritt) Klicka på vänsterpilen till vänster om posttypens namn i sidhuvudet för att gå tillbaka till den valda arbetsytan.

1. (Valfritt) Klicka på och håll ned ett posttypskort på arbetsytan om du vill dra och släppa posttypen på en önskad plats, eller om du vill flytta den till ett annat avsnitt.

   Ändringarna sparas automatiskt.

   Mer information om hur du lägger till poster, tar bort eller redigerar posttyper eller uppdaterar vyn på posttypsidan finns i följande artiklar:

   * [Skapa poster](/help/quicksilver/planning/records/create-records.md)
   * [Ta bort posttyper](/help/quicksilver/planning/architecture/delete-record-types.md)
   * [Redigera posttyper](/help/quicksilver/planning/architecture/edit-record-types.md)
   * [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md)

<!--
## Create record types by importing an Excel or CSV file

>[!IMPORTANT]
>
>This functionality has been temporarily removed since March 21, 2024. It will be enabled at a later date.

Consider the following when importing record types using an Excel or CSV file: 

* Each sheet of the Excel file becomes a record type. 
* The columns of each sheet become the fields associated with each record type. 
* Fields are unique for their respective record types. 
* Each row in each sheet becomes a unique record associated with its respective record type. 
* Each sheet of the Excel file should not exceed the following: 
    * 50,000 rows
    * 500 columns
* The Excel file should not be larger than 5MB.
* Empty sheets are not supported. 

To import record types using an Excel file: 

{{step1-to-planning}}

1. Click the workspace where you want to create record types, 

    Or

    From a workspace, expand the downward-pointing arrow to the right of an existing workspace name, search for a workspace, then select it when it displays in the list.
1. Click **Add record type**. 
1. Click **Excel/CSV**.
1. Drag and drop an Excel or CSV file previously saved on your computer, or click **Select a CSV or Excel file** to browse for one. 
1. Click **Review your data**.
    
    The Preview and edit box displays with the following information: 

    * The names of the sheets or of the future record types display in the left panel. Workfront Planning selects an icon and a color for each new record type by default.
    * The first sheet or record type is selected and the names of the fields associated with it display as the column headers. The type of each field is selected by default. 
    * Each row represents a new record. Only the first 10 records display in the Preview and edit box. 

    ![](assets/preview-and-edit-box.png)

1. (Optional) Click the name of each sheet in the left panel to review the information it contains. 

    >[!NOTE]
    >
    >    Sheets that are empty are not supported and are dimmed. 


1. (Optional) Click the **Select sheets to import** drop-down menu and deselect the sheets that you don't want to import. 

    ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

    Sheets you deselected display with a gray background. 

1. Click **Import** when you are ready to import your file. 

    The following information imports in to Workfront Planning:

    * New record types
    * New fields associated with each record type
    * New records associated with each record type

    You can start managing fields and records on the record types pages. 
    
    Everyone with access to Workfront Planning can now view and edit the imported record types and their information.-->


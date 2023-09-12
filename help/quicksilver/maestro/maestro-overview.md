---
title: Adobe Maestro - översikt
description: Adobe Maestro är ett nytt erbjudande från Adobe Workfront. Du kan skapa anpassningsbara arbetsytor för att definiera arbetsflöden som uppfyller behoven för varje organisationsenhet i företaget.
hidefromtoc: true
hide: true
source-git-commit: 71ce412ead1590b8511ec4219d3ba72fbf32b98d
workflow-type: tm+mt
source-wordcount: '1805'
ht-degree: 0%

---


# Adobe Maestro - översikt

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!--see the separate article I wrote to have the PMs vet it for this: https://adobe-my.sharepoint.com/personal/alinaw_adobe_com/_layouts/15/doc.aspx?sourcedoc={79f94807-3d73-4015-afc0-5c016fc63cfc}&action=edit-->

<!--all the links are hidden for now, so I can share this with customer zero. Activate the links before making this public. -->

<!-- remove the references to closed beta from the entire article-->

>[!IMPORTANT]
>
>För närvarande ingår Adobe Maestro i ett slutet betaprogram som är öppet för ett begränsat antal kunder.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.

## Introduktion till Adobe Maestro

Adobe Maestro är ett nytt erbjudande från Adobe Workfront. Syftet med Maestro är att ge en heltäckande inblick i en organisations operativa detaljer och besvara viktiga affärsfrågor i varje fas av arbetshanteringens livscykel.

Team och ledarskap behöver tydliga svar på frågor som:

* Hur många kampanjer anordnar vi i EMEA för fjärde kvartalet?
* Finns det någon publiköverlappning mellan samtidiga kampanjer?
* Hur bra fungerar medvetandeprogrammen just nu?
* Hur ser resurserna ut för en viss kampanj? Vilka av dem måste fortfarande godkännas?

För att svara på dessa frågor behöver ledningen en lösning som ger en helhetsbild av alla arbetsmoment, från planering till genomförande, från leverans till mätning av resultaten. För närvarande har organisationer verktyg som kan täcka vissa delar av processen, men många har inte bra kopplingar till alla faser av arbetet och kan inte heller ge resultat på ett tillförlitligt sätt.

Här följer några av huvudfunktionerna i Maestro:

* Lös problemet med att hantera arbetet i alla faser och för alla intressenter som deltar i arbetsprocessen.
* Anpassa arbetsflödena helt och hållet, från att bestämma vilka objekttyper (eller posttyper) organisationen använder till att konfigurera hur dessa objekt länkar till varandra.
* Länka till objekttyper från andra system och skapa ett sammanhängande ramverk för alla era processer.

## Åtkomst krävs för att använda Maestro under det avslutade betaprogrammet

>[!IMPORTANT]
>
>För närvarande finns det inga åtkomstnivåer eller behörigheter kopplade till användare eller informationen i Maestro. Alla användare kan visa, redigera och ta bort all information som andra användare lägger till i Maestro.

Mer information om vilken åtkomst som krävs för att använda Maestro finns i [Översikt över åtkomst till Adobe Maestro](../maestro/access/access-overview.md).

<!-- hidden the table after I moved the content to the Access overview article: 

You must have the following access to use Adobe Maestro: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader">Access level</td>
   <td> <p>Any</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Layout template</td>
   <td> <p>Your system administrator must add the Maestro area in your layout template. For information, see <a href="../maestro/access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

************* Activate note when going to GA: 

>[!NOTE]
>
>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). 
-->

## Maestro-terminologi

Även om Maestro är en del av Workfront innehåller det egna koncept och terminologi. Se till att du känner till Maestro-koncepten innan du startar Maestro för din organisation.

Ramverket för Maestro är helt anpassningsbart. Du kan skapa alla posttyper, deras attribut och alla fält som är kopplade till dem för att passa din organisations behov.

Nedan följer de viktigaste Maestro-objekten och begreppen:

* **Arbetsyta**: En samling posttyper och taxonomier som definierar den operativa livscykeln för en viss organisation. En arbetsyta är en arbetsyta i en organisationsenhet.

  En Workfront-instans kan ha högst 1 000 arbetsytor.

  ![](assets/marketing-workspace-with-record-type-taxonomies-opening-page.png)

  Mer information finns i [Skapa arbetsytor](../maestro/architecture-and-fields/create-workspaces.md).

* **Posttyp**: Huvudobjekttypen för Maestro.

  Till skillnad från Workfront där objekttyperna är fördefinierade kan du skapa egna objekttyper i Maestro.

  I Workfront har till exempel objekttyperna Program, Portfolio, Projekt, Uppgift eller Utgåva redan skapats.

  I Maestro kan du skapa alla posttyper som passar din organisations arbetsflöden. Senare kan du definiera hur posttyperna relaterar till varandra eller formulärberoenden.

  Mer information finns i [Översikt över driftsposttyper och taxonomier](../maestro/architecture-and-fields/overview-of-record-types-and-taxonomies.md).

  Maestro har följande posttyper:

   * **Driftposttyp**: En posttyp som representerar strategiska planer, initiativ eller utfört arbete.

     ![](assets/operational-record-type-blank.png)

     Exempel: Campaign, Activity, Program kan vara driftsposttyper.

     Mer information finns i [Skapa posttyper](../maestro/architecture-and-fields/create-record-types.md).

   * **Taxonomi**: En posttyp som samlar in attribut om en operativ posttyp.

     ![](assets/taxonomy-record-type-blank.png)

     Även om det är samma sak att skapa taxonomier som att skapa operativa posttyper, skiljer Maestro mellan en operativ posttyp och en taxonomiposttyp. Syftet med taxonomier är att förbättra den operativa registertypen. <!--this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.-->

     Till exempel kan Audience, Region eller Address vara posttyper av taxonomintyp.

     Mer information finns i [Skapa taxonomiposttyper](../maestro/architecture-and-fields/create-a-taxonomy.md).

* **Post**: En instans av en Maestro-posttyp. En post kan referera till en driftsposttyp eller till en taxonomi.

  ![](assets/records-highlighted-in-campaign-record-type-list.png)
  ![](assets/records-highlighted-in-region-taxonomy-type-list.png)

  När du har lagt till en posttyp på en arbetsyta kan du börja lägga till poster av den typen på posttypens sida.

  Exempel:&quot;Campaign&quot; kan vara en operativ posttyp och&quot;Sommarkampanj för EMEA&quot; är ett register över posttypen Campaign

  eller

  &quot;Region&quot; är en posttyp av taxonomisk typ, medan &quot;Amerika-Latinamerika&quot; eller &quot;EMEA - Centraleuropa&quot; är taxonomiposter.

  Mer information finns i [Skapa poster](../maestro/records/create-records.md).

* **Arbetsytemall**: Du kan skapa en arbetsyta med fördefinierade mallar. Du kan använda de fördefinierade posttyperna, taxonomierna och fälten som finns i en mall eller lägga till egna.

  ![](assets/workspaces-page-with-templates-thumbnails.png)

  Maestro levereras med en arbetsyta för försäljning, marknadsföring och produkthantering.

  Mer information finns i [Skapa arbetsytor](../maestro/architecture-and-fields/create-workspaces.md).

* **Fält**: Fält är attribut som du kan lägga till i användnings- eller taxonomiposttyper som innehåller information om posttypen. <!--check the shot below, "Connection" needs to be in lowercase-->

  ![](assets/drop-down-list-of-record-fields.png)

  Att tänka på när det gäller Maestro-fält:

   * De fält som du lägger till för en posttyp kopplas automatiskt till alla poster av den typen och kan användas för att samla in data om dessa poster.

   * Fält visas som kolumner i tabellvyn som används på en posttypssida. De visas även på postens detaljsida.

   * Fält är unika för en posttyp och överförs inte från en posttyp till en annan.

   * Maestro-fälten är helt anpassningsbara och är bara tillgängliga i Maestro. Du har inte åtkomst till Maestro-fält från Workfront.

  Mer information finns i [Skapa fält](../maestro/architecture-and-fields/create-fields.md)

  En ny operativ posttyp är som standard associerad med följande fördefinierade fält:

   * Namn
   * Beskrivning
   * Startdatum
   * Slutdatum
   * Status

  En ny taxonomiposttyp är som standard associerad med ett namnfält.

  Du kan skapa anpassade fält av följande typer:

   * Enkelradig text
   * Stycke
   * Flera val
   * Enkelval
   * Datum
   * Nummer
   * Procent
   * Valuta
   * Kryssruta

* **Länkade posttyper**, **Länkade poster** och **Länkade postfält**: Du kan skapa en anslutning mellan följande enheter:

   * Två Maestro-posttyper
   * En Maestro-posttyp och en Workfront projekt-, program-, portfölj-, företag- eller gruppobjekttyp.

  ![](assets/new-connection-tab-with-workfront-option.png)

  När du har upprättat en anslutning mellan posttyperna kan du koppla enskilda poster av dessa typer till varandra. Anslutningen mellan posterna visas som ett länkat postfält.

* **Länkade fält** (eller sökfält): När du har upprättat anslutningen mellan två posttyper och länkar samman enskilda poster kan du referera till de länkade posternas fält i den post du ansluter från.

  ![](assets/add-lookup-fields-modal.png)

  Mer information om hur du länkar posttyper, poster och skapar länkade fält finns i följande artiklar:

   * [Koppla posttyper](../maestro/architecture-and-fields/connect-record-types.md)
   * [Koppla poster](../maestro/records/connect-records.md)

<!--not yet:* Fields are reusable across Record Types.  -->

* **Vyer**: Poster visas under sina respektive posttypssidor i olika typer av vyer.

  ![](assets/view-types-drop-down-from-record-type-list.png)

  Vyer innehåller anpassade inställningar för en viss vytyp, till exempel listan med fält (kolumner), en lista med poster (rader), deras ordning (sortering), ett tillämpat eller tillämpligt filter och gruppering.

  Här följer några vytyper som du kan använda på posttypssidan:

   * **Tabellvy**: Visar poster och deras fält i ett tabellformat. Raderna i tabellen är de enskilda posterna och kolumnerna är postfälten. Det här är standardvyn.

     ![](assets/table-view-example.png)

   * **Tidslinjevy**: Visar poster som har minst två datumfält på en kronologisk tidslinje.

     ![](assets/grouping-applied-in-timeline-view.png)

  Mer information finns i [Hantera postvyer](../maestro/views/manage-record-views.md).


## Begränsningar för Maestro-objekt

I följande tabell visas gränserna för hur många objekt du kan skapa i Maestro. Begränsningarna kan komma att ändras när vi går vidare till nästa fas i Maestro:s utveckling.

| Maestro-objekt | Gräns |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| Antal arbetsytor för en Workfront-instans | 1,000 |
| Antal posttyper för en arbetsyta | 1 000 (inkluderar taxonomier för arbetsytan eller objekt som du importerar från tredjepartsprogram) |
| Antal poster för en posttyp | 10,000 |
| Antal fält för en posttyp eller taxonomi | 500 |
| Antal tecken för ett textfält | 1 000 tecken |
| Storlek på fil som du kan klistra in i en posttypstabell | 1MB |
| Storlek på fil som du kan importera via API för en posttypstabell | 1.5MB |
| Frekvensen med vilken API-begäranden kan göras | 200 begäranden per minut |
| Storlek på Excel-fil som du kan importera i en tabell | 5MB |

## Aktivera Maestro för användare i din Workfront-instans

Din organisation måste registrera sig i det slutna betaprogrammet för Adobe Maestro innan du kan komma åt Maestro. Kontakta din kontorepresentant om du vill ha information om hur du registrerar dig i betaprogrammet.

Mer information om att bevilja åtkomst till och göra det möjligt för andra att använda Maestro finns i [Ge åtkomst till Adobe Maestro](../maestro/access/grant-access.md).

<!--hidden this after moved it to a separate article

After your organization has been enrolled in the Maestro beta program, you can add the Maestro area for other users by using a layout template. 

To share the Maestro area using a layout template: 

1. Log in to Workfront as a system administrator.  

1. Add the Maestro icon to the Main Menu using a Layout Template. For information, see [Customize the Main Menu using a layout template](../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md). 

1. Assign the  layout template to the users that you want to have access to Maestro.For information, see [Assign users to a layout template](../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

    All users who can access Maestro in their Main Menu can start creating workspaces, records types, records, and fields.  
  -->


## Hitta maestro

Kontrollera att din organisation har fått tillgång till Maestro och att din system- eller gruppadministratör har lagt till Maestro-området på huvudmenyn.

Så här hittar du Maestro:

1. Logga in på Adobe Workfront.

1. Klicka på **Huvudmeny** ![](assets/main-menu-workfront.png) i det övre högra hörnet eller klicka på **Huvudmeny** ![](assets/main-menu-shell.png) i det övre vänstra hörnet, om det är tillgängligt.

1. Klicka **Maestro** ![](assets/maestro-icon.png).

   Området Maestro Workspaces öppnas.

1. (Valfritt och rekommenderas) Fortsätt med några av följande åtgärder för att skapa din arbetsstruktur i Maestro:

   1. Skapa en arbetsyta från grunden eller med en mall.

   1. Lägg till posttyper på den nya arbetsytan.

   1. Lägg till taxonomier i de nya arbetsytorna.

   1. Klicka på namnet på en posttyp för att öppna postens sida. Postsidan öppnas som standard i tabellvyn.

   1. Anpassa tabellvyn genom att göra något av följande:

      * Lägg till fler fält till posttypen genom att klicka på **+** i det övre högra hörnet. Kolumnerna i vyn är fält som är associerade med posttypen.
      * Lägg till poster genom att klicka på **+** i det nedre vänstra hörnet. Raderna i vyn är unika poster av den valda posttypen.
      * Klicka **Filter** för att filtrera den information som visas på posttypssidan.

   1. Klicka på namnet på en post för att visa mer information på postens informationssida.

   1. Skapa en tidslinjevy från **Visa** nedrullningsbar meny i det övre högra hörnet på posttypssidan.

   1. Anpassa tidslinjevyn genom att uppdatera filter, grupperingar eller inställningar.

## Aktuella funktioner i Maestro

I följande tabell visas huvudfunktionerna som kommer att vara tillgängliga i Maestro och en tidslinje för deras tillgänglighet. Listan innehåller inte alla funktioner.

| Funktion | Ute nu | Tillgänglig snart | Forskning |
|----------------------------------------------------|:-----------------------------:|:--------------------------------:|:----------------:|
| Skapa arbetsytor | ✓ |                                  |                  |
| Skapa driftsposttyper | ✓ |                                  |                  |
| Skapa taxonomier | ✓ |                                  |                  |
| Skapa personliga, namngivna poster och taxonomier | ✓ |                                  |                  |
| Skapa anpassade postfält | ✓ |                                  |                  |
| Importera posttyper och fält med en Excel- eller CSV-fil | ✓ |                                  |                  |
| Länka poster | ✓ |                                  |                  |
| Visa poster i en tabell | ✓ |                                  |                  |
| Visa poster på en tidslinje | ✓ |                                  |                  |
| Filtrera poster | ✓ |                                  |                  |
| Gruppera poster i tidslinjevyn | ✓ |                                  |                  |
| Gruppera poster i tabellvyn |                               | ✓ |                  |
| Sortera poster i tabellvyn | ✓ |                                 |                  |
| Sortera poster i tidslinjevyn |                               | ✓ |                  |
| Sortera grupperingar i tabellvyn |                               | ✓ |                  |
| Sortera grupperingar i tidslinjevyn |                               | ✓ |                  |
| Ansluta arbetsytor |                               | ✓ |                  |
| Koppla ihop Maestro-poster och taxonomier | ✓ |
| Koppla ihop Maestro-poster till Workfront projekt, program, portfolior, företag, grupper | ✓ |                                 |                  |
| Sidan med postinformation | ✓ |                                  |                  |
| Uppdatera layouten på sidan med postinformation |                               | ✓ |                  |
| Åtkomstnivåer och behörigheter | | ✓ |  |
| Skicka begäranden |                               |                                  | ✓ |
| Kreativ översikt |                               |                                  | ✓ |
| Anpassa färg och ikon för en post | ✓ |                                  |                 |

## Aktivitet för lansering av Maestro

Vi släpper regelbundet nya funktioner till Maestro. En uppdaterad lista över funktioner som släppts finns på [Adobe Maestro-lansering](../maestro/release-activity.md).

<!--moved the contents of this whole section to its own article: release-activity.md, in the same folder

This section lists the features and patches that have been released after the launch of the Maestro closed beta program, on May 22, 2023. 

The features are released weekly and are listed in the order of their release, with the most recent first. Customers who are participating in the Maestro closed beta program can access all features in their Preview and Production environments. 

### Week of September 4, 2023

#### Connect Maestro records with Workfront companies and groups

Preview and production: September 5, 2023  

You can now connect a Maestro record with Workfront companies and groups. You must first create a connection between a Maestro record type and the Workfront companies and groups object types. Then, you can connect a single Maestro record of the selected record type to individual Workfront companies and groups.  

Consider the following:  

* You must create a connection between Maestro record types and Workfront companies and groups for each Workspace.  

* You cannot connect taxonomy record types with Workfront object types. 

* You can connect multiple Maestro records to the same Workfront company or group, and multiple companies or groups to the same Maestro record.  

* You cannot edit companies or groups in Maestro. All company or group changes performed in Workfront are visible in Maestro, when reviewing the Maestro linked records.  

#### URL support for single-line text fields 

Preview and production: September 7, 2023 

For better visibility when working with links in the Table view, we have added support for URLs in single-line text fields. Using URLs to other websites or external drives when updating a single-line text field, now identifies them as links and allows you to click them from the table.  

### Week of August 28, 2023

#### Field visibility menu for the Table View toolbar

Preview and production: August 31, 2023

To display the right information on a given set of records, especially if you intend to share the view with others who need to see some but not all fields of a record type, you can now select which fields (or columns) to display and which to hide in the Table view.  

You can hide or show individual fields, from each header of the field columns, or you can manage all fields of the record type from a setting in the table view toolbar.  

### Week of August 21, 2023

#### Connect Maestro records to programs and portfolios 

Preview and production: August 24, 2023

You can now connect a Maestro record with Workfront programs and portfolios. You must first create a connection between a Maestro record type and a program or portfolio which creates a connected field. Then, you can connect any Maestro records from all other record types within the same workspace to specific programs and portfolios which will create a read-only Workfront Program or Workfront Portfolio record type in the same workspace. Consider the following:

* Workfront connector record types are unique for each workspace. 
* You can connect multiple Maestro records to the same Workfront program or portfolio, and multiple programs and portfolios to the same Maestro record. 
* You cannot edit programs and portfolios in Maestro. All program and portfolio changes performed in Workfront are visible in Maestro, when reviewing the linked records. 

#### New sorting functionality for the table view

Preview and production: August 24, 2023

You can now sort records in the table view of a record type page. 
The following capabilities are now available: 

* Sorting at the table-level, where you can sort by multiple fields at the same time. 
* Sorting at the column or field-level, where you can sort by an individual field at a time.

#### Improvements to the timeline view: new look-and-feel for groupings and the Compact/ Standard view switch

Preview and production: August 24, 2023

We have introduced the following improvements to the timeline view: 

* You can now display the timeline view in the following modes:

    * Standard: Displays records in separate lines.
    * Compact: Display the records whose dates don't intersect on the same line. 

* We have changed the look-and-feel of the grouping lines in the timeline view to display above the timeline of the records they contain. Prior to this improvement, the grouping lines displayed across the entire length of the timeline.

### Week of August 14, 2023

#### Reorder columns in the table view

You can now reorder columns in the Maestro table view. Consider the following when reordering columns: 

* The Name field is always the first field in the table view of a record type page 

* You cannot move the Name field to another position 

* The Name field is frozen and is not part of the horizontal scroll. 

#### Horizontal scroll for timeline view

You can now scroll horizontally in the timeline view of a record type. 

### Week of August 7, 2023

#### Import record types from an Excel file 

Preview and production: August 10, 2023

You can now import an Excel file to create record types in a workspace. The sheets of the file become the record types, and the columns of the file become their respective fields.  

#### Improved experience for connecting record types and projects 

Preview and production: August 10, 2023

We have improved the way you connect record types, including connecting to Workfront projects. As part of this improvement, we made the following changes when adding a field for a record type from the table view:  

* Removed the Relationship-type field from the "New field" tab.  

* Add a "New connection" tab where you can directly select the record or object type you want to connect to, eliminating the need for a Relationship-type field. 

### Week of July 10, 2023

#### Update the appearance of a record type

Preview and production: July 13, 2023

You can now select a custom icon for a record type, as well as a custom color for the record type icon.  

#### New Checkbox field type

Preview and production: July 13, 2023 

You can now add a Checkbox field type to Maestro record types. You can use the Checkbox field type to add a single checkbox option to a record. You can use this field to indicate a specific attribute or status for that particular record. For example, you can use it as a flag for tracking completion, approval, or any other binary attribute for each record.  

### Week of June 26, 2023

#### Quick activation of the contextual menu in a table

Preview and production: June 28, 2023
 
We have enabled the ability to activate the contextual menu by right-clicking anywhere in a record row, when viewing the records in the table view or a record type. You can now quickly view, delete, or copy a link to the record's Details page when you access the contextual menu from anywhere in the table view of a record type. Prior to this enhancement, the contextual menu was accessible only from the More menu in the Name column of a record.  

### Week of June 19, 2023

#### Record field names are unique

We have introduced a requirement now that the field names of a Maestro record type should have unique names. Fields that belong to different record types do not have to have unique names.  

### Week of June 5, 2023

#### Connect Maestro records with Workfront projects

Preview and production: June 5, 2023

You can now connect a Maestro record with Workfront projects. You must first create a connector Maestro record type to establish the connection between Maestro records and Workfront projects. Then, you can connect any Maestro records from all other record types to the connector record using the Relationship field. Consider the following:

* You must have a connector record type for Workfront for each Workspace. 
* You can connect multiple Maestro records to the same Workfront project, and multiple projects to the same Maestro record. 
* You cannot edit projects in Maestro. All project changes performed in Workfront are visible in Maestro, when reviewing the linked records. 

### Week of May 29, 2023

#### Two-date requirement for creating a Timeline view

Preview and production: May 31, 2023  

You must have at least two date fields associated with a record type in order to create a Timeline view. 
-->





---
title: Skapa posttyper
description: Posttyperna är objekttyperna för Adobe Workfront Planning. I Workfront Planning kan du skapa anpassade posttyper som illustrerar de arbetsuppgifter som behövs i organisationens livscykel.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 1369269bcb64bd32f26603608782dc996b079cb9
workflow-type: tm+mt
source-wordcount: '1259'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->
<!--this is linked to the UI in an empty workspace screen-->

# Skapa posttyper

{{planning-important-intro}}

Posttyperna är objekttyperna för Adobe Workfront Planning. I Workfront Planning kan du skapa anpassade posttyper som illustrerar de arbetsrelaterade objekt som behövs i organisationens livscykel.

Mer information om posttyper finns i [Översikt över posttyper](../architecture/overview-of-record-types-and-taxonomies.md).

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
   <td role="rowheader"><p>Adobe Workfront-licens</p></td>
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
   <td> <p>Workfront- eller gruppadministratören måste lägga till planeringsområdet i layoutmallen. Mer information finns i <a href="../access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Hantera behörigheter till en arbetsyta</a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Att tänka på när du skapar posttyper

* Du kan skapa posttyper på en arbetsyta på följande sätt:

   * Automatiskt:
      * När du skapar en arbetsyta med hjälp av en mall.

        Mer information finns i [Skapa arbetsytor](../architecture/create-workspaces.md).

      * När du importerar dem med en Excel- eller CSV-fil.

        >[!IMPORTANT]
        >
        >Den här funktionen har tillfälligt inaktiverats sedan 21 mars 2024. Den aktiveras vid ett senare tillfälle.

     <!--this should not ne known anymore: * When you add objects from another application to a linked record field of a record. This creates a read-only record type in Workfront Planning which is connected to object types from the original application. 
        For information about connecting record types with object types from another application, see [Connect record types](/help/quicksilver/maestro/architecture/connect-record-types.md).
        For information about connecting objects with records, see [Connect records](/help/quicksilver/maestro/records/connect-records.md). -->
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

Mer information om hur du skapar arbetsytor finns i [Skapa arbetsytor](../architecture/create-workspaces.md).

Mer information om vilka posttyper som ingår i respektive mall finns i [Lista över arbetsytemallar](../architecture/workspace-templates.md).

## Skapa en posttyp från grunden

{{step1-to-maestro}}

Den senast använda arbetsytan bör öppnas som standard.

1. (Valfritt) Expandera den nedåtriktade pilen till höger om namnet på en befintlig arbetsyta och markera den arbetsyta som du vill skapa posttyper för.
1. (Valfritt) Klicka på **Lägg till avsnitt** om du vill lägga till ett nytt avsnitt på arbetsytan.
1. Klicka **Lägg till posttyp**.
1. (Villkorligt) När du skapar posttyper genom att importera en Excel- eller CSV-fil, klickar du på **Från början**. I annat fall **Lägg till posttyp** öppnas.

   ![](assets/add-record-type-box-with-appearance-options.png)

1. Uppdatera följande information:

   * Ersätt&quot;Namnlös posttyp&quot; med namnet på din framtida posttyp. <!--did they bring back the field label here and did they rename it to "Name"-->
   * **Beskrivning**: Lägg till mer information om posttypen.
   * Välj en färg och form för den ikon som är associerad med posttypen. Gör följande:
      * Välj en färg som identifierar den nya posttypen. Det här är färgen på ikonen för posttyp. Grått är markerat som standard.
      * Välj en ikon i listan eller börja skriva namnet på en ikon för att beskriva vad den representerar och markera den sedan när den visas. Det här är ikonen för posttypen. Som standard är en filikon markerad.

1. Klicka **Skapa**.

   Posttypkortet läggs till i avsnittet och på den arbetsyta som du har valt.
Beskrivning av posttypen visas på kortet.

   ![](assets/record-type-card-with-description.png)

1. (Valfritt) Håll markören över posttypskortet och klicka på knappen **Mer** icon ![](assets/more-menu.png) i det övre högra hörnet och klicka sedan på **Redigera** om du vill ändra information om posttypen.
1. (Valfritt) Klicka på posttypskortet för att öppna posttypssidan.

   ![](assets/operational-record-type-blank.png)

   Posttypssidan visas som standard i tabellvyn. Kolumnerna i tabellen är fält som är kopplade till den nya posttypen. Varje rad är en unik post som du måste lägga till.

   >[!TIP]
   >
   >    Om du importerar en posttyp från en Excel- eller CSV-fil importeras också poster.

   Som standard visas följande fält i tabellvykolumnerna för en operativ posttyp:

   * Namn
   * Beskrivning
   * Startdatum
   * Slutdatum
   * Status

1. (Valfritt) Uppdatera posttypens namn i sidhuvudet

   eller

   Klicka på **Mer** icon ![](assets/more-menu.png) till höger om posttypens namn och klicka på **Redigera** om du vill byta namn på den eller ändra informationen om den. Mer information finns i [Redigera posttyper](/help/quicksilver/maestro/architecture/edit-record-types.md).

1. (Valfritt) Klicka på **+ Ny post** om du vill lägga till poster av den valda posttypen. Mer information finns i [Skapa poster](../records/create-records.md).
1. (Valfritt) Klicka på **+** i tabellens övre högra hörn om du vill lägga till fler fält i posttypen.

   Mer information om hur du skapar fält finns i [Skapa fält](../fields/create-fields.md).

1. (Valfritt) Klicka på vänsterpilen till vänster om posttypens namn i sidhuvudet för att gå tillbaka till den valda arbetsytan.

1. (Valfritt) Klicka på och håll ned ett posttypskort på arbetsytan om du vill dra och släppa posttypen på en önskad plats, eller om du vill flytta den till ett annat avsnitt.

   Ändringarna sparas automatiskt.

   Mer information om hur du lägger till poster, tar bort eller redigerar posttyper eller uppdaterar vyn på posttypsidan finns i följande artiklar:

   * [Skapa poster](../records/create-records.md)
   * [Ta bort posttyper](../architecture/delete-record-types.md)
   * [Redigera posttyper](../architecture/edit-record-types.md)
   * [Hantera postvyer](../views/manage-record-views.md)

## Skapa posttyper genom att importera en Excel- eller CSV-fil

>[!IMPORTANT]
>
>Den här funktionen har tillfälligt inaktiverats sedan 21 mars 2024. Den aktiveras vid ett senare tillfälle.

Tänk på följande när du importerar posttyper med en Excel- eller CSV-fil:

* Varje blad i Excel-filen blir en posttyp.
* Kolumnerna i varje blad blir de fält som är kopplade till varje posttyp.
* Fält är unika för respektive posttyp.
* Varje rad i varje blad blir en unik post som är kopplad till respektive posttyp.
* Varje blad i Excel-filen får inte överskrida följande:
   * 50 000 rader
   * 500 kolumner
* Excel-filen får inte vara större än 5 MB.
* Tomma blad stöds inte.

Så här importerar du posttyper med en Excel-fil:

{{step1-to-maestro}}

Den senast använda arbetsytan bör öppnas som standard.

1. (Valfritt) Expandera den nedåtriktade pilen till höger om namnet på en befintlig arbetsyta och markera den arbetsyta som du vill skapa posttyper för.
1. Klicka **Lägg till posttyp**.
1. Klicka **Excel/CSV**.
1. Dra och släpp en Excel- eller CSV-fil som tidigare sparats på datorn eller klicka på **Välj en CSV- eller Excel-fil** för att hitta en.
1. Klicka **Granska dina data**.

   Rutan Förhandsgranska och redigera visas med följande information:

   * Namnen på arken eller de framtida posttyperna visas på den vänstra panelen. I Workfront Planning väljs en ikon och en färg för varje ny posttyp som standard.
   * Den första arks- eller posttypen markeras och namnen på de fält som är kopplade till den visas som kolumnrubriker. Som standard väljs typen för varje fält.
   * Varje rad representerar en ny post. Endast de första 10 posterna visas i rutan Förhandsgranska och redigera.

   ![](assets/preview-and-edit-box.png)

1. (Valfritt) Klicka på namnet på varje blad i den vänstra panelen för att granska informationen som det innehåller.

   >[!NOTE]
   >
   >    Blad som är tomma stöds inte och är nedtonade.


1. (Valfritt) Klicka på **Välj ark att importera** och avmarkera de blad som du inte vill importera.

   ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

   Blad som du avmarkerat visas med grå bakgrund.

1. Klicka **Importera** när du är redo att importera filen.

   Följande information importeras till Workfront Planning:

   * Nya posttyper
   * Nya fält som är associerade med varje posttyp
   * Nya poster associerade med varje posttyp

   Du kan börja hantera fält och poster på posttypssidorna.

   Alla som har tillgång till Workfront Planning kan nu visa och redigera de importerade posttyperna och deras information. <!--this will change with permissions-->

<!--## Connect record types with object types from another application

You can connect a record type and an object type from another application. This creates a read-only record type in Workfront Planning that corresponds to the object type in the other application. 

For example, you can create record types by connecting Workfront Planning record types with Workfront projects. As a result, the Workfront project object type is imported into Workfront Planning as a read-only record type. By default, the record type is named "Workfront Project." (********************)has this name changed? Lusine wanted to change it at some point***********)
    
You can import the following objects from the following applications: 

* From Workfront:

    * Projects
    * Portfolios
    * Programs
    * Company
    * Group

For more information, see [Connect record types](../architecture/connect-record-types.md). 
-->
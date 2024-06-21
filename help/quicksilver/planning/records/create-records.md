---
title: Skapa poster
description: När du använder Adobe Workfront Planning är en post en instans av en posttyp.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: f5430d81f1914a3717130de3af54b4b84e0e2d06
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Skapa poster

{{planning-important-intro}}

I Adobe Workfront Planning är en post en instans av en posttyp.

Du kan skapa poster genom att göra något av följande:

* Skapa dem manuellt för posttyper
* Skapa poster genom att kopiera och klistra in information från en extern lista.

I den här artikeln beskrivs hur du skapar poster. Mer information om hur du hanterar poster i tabell- och tidslinjevyer finns i följande artiklar:

* [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md)
* [Hantera tidslinjevyn](/help/quicksilver/planning/views/manage-the-timeline-view.md)

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
   <p>Nytt: Standard</p>
   <p>Aktuell: Planera</p>  
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td>
   <td> <p>Det finns inga åtkomstkontroller för Adobe Workfront Planning </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Contribute eller högre behörighet till en arbetsyta</a> </p>  
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

*Mer information finns på [Åtkomstkrav för Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/planning/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Skapa poster genom att lägga till dem manuellt till en posttyp <!--in a record type table (I don't think you can create them elsewhere right now)-->

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

      * Klicka **Ny post** i tabellens sista rad

      * Klicka **Skift + Retur** på tangentbordet från en kolumn eller rad i tabellen. Det här annonserar en tom rad.

     ![](assets/adding-a-new-campaign-in-table-row.png)

   * Från alla vyer:

      * Klicka **Ny post** i det övre högra hörnet på sidan. Förhandsgranskningsrutan för posten öppnas.

     Workfront överför automatiskt en miniatyrbild och en omslagsbild till varje ny post. Du kan ändra dessa bilder senare. Mer information finns i följande artiklar:

      * [Lägga till en omslagsbild till en post](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
      * [Lägga till en miniatyrbild i en post](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

1. Börja skriva information om den nya posten i de fält som visas i förhandsvisningsrutan.

   >[!NOTE]
   >
   >  * Det finns inga obligatoriska fält för poster. Vi rekommenderar dock att du lägger till information för det primära fältet i en post, eftersom det är praktiskt att identifiera poster när du länkar poster till varandra. Mer information om primära fält finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md) och [Översikt över primärt fält](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >  * Fält som refererar till andra posttyper eller beräknade fält är skrivskyddade fält.

1. (Villkorligt) När du lägger till poster i tabellen fortsätter du att lägga till information på varje rad och klickar sedan på **Retur** på tangentbordet för att spara ändringarna.

   eller

   Klicka på den nya postens namn eller på **Öppna detaljer** icon ![](assets/open-details-icon-in-table-name-field.png) till vänster om postens namn. En förhandsgranskning med postens detaljerade information öppnas i tabellen.

   >[!TIP]
   >
   >Du kommer åt **Öppna detaljer** -ikonen från postens namnfält när fältet Namn är ett primärt fält.

1. Börja redigera postens information i postens förhandsgranskning. Workfront sparar automatiskt ändringarna.
1. (Valfritt) Klicka på **Öppna på ny flik** icon ![](assets/open-details-in-a-new-tab-icon.png) i det övre högra hörnet av postens förhandsgranskning för att öppna postens sida på en ny flik. Fortsätt redigera posten på postsidan. Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

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

## Skapa poster genom att kopiera och klistra in information från en extern lista

1. Börja skapa poster i tabellvyn enligt beskrivningen i avsnittet [Skapa poster genom att lägga till dem manuellt till en posttyp](#create-records-by-manually-adding-them-to-a-record-type) i den här artikeln.

   Se till att tabellvyn innehåller kolumnerna (eller fälten) som du vill fylla med den nya postinformationen.

1. Klicka **Nytt &lt; Posttypnamn >** i den sista raden i tabellen för att lägga till så många nya rader i tabellen som du vill att de nya posterna ska vara.

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

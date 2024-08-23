---
title: Redigera poster
description: Du kan redigera postinformation i Adobe Workfront Planning. Du måste skapa posttyper innan du kan börja skapa och redigera poster.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 61cad7dc76ba04ea84ff0bd5052182f040f7b4d9
workflow-type: tm+mt
source-wordcount: '1833'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Redigera poster

{{planning-important-intro}}

Du kan redigera postinformation i Adobe Workfront Planning genom att redigera värdena i fälten som är kopplade till posterna.

Du måste skapa posttyper innan du kan börja skapa och redigera poster.

Mer information finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

Mer information om hur du skapar poster finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).

&lt;!— här anger du att fälten i detaljvyn är desamma som fälten i tabellvyn - den här artikeln är länkad från vyerna Hantera post för att referera till den här informationen—>

## Åtkomstkrav

<!--Updated for GA-->

+++ Expandera om du vill visa åtkomstkraven för Workfront Planning.

Du måste ha följande för att kunna komma åt Workfront Planning:

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
   <td role="rowheader"><p>Adobe Workfront Planning*</p></td> 
   <td> 
<p>Alla </p> 
<p>Mer information om vad som ingår i varje Workfront Planning-plan finns i <a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfront priser och paketering</a>. </p> 
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
   <td> <p>Standard</p> 
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
   <td>  <p>Contribute eller högre behörighet till en arbetsyta </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutmall</p></td> 
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn. </p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   Or
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Att tänka på när du redigerar poster

* Du kan redigera poster som du har skapat eller poster som har skapats av andra, om du har fått behörighet till arbetsytan.
* Du kan redigera postfält från följande områden:

   * Postens förhandsgranskning i en postvy
   * Postens sida
   * Textbunden i en tabellvy.

* När en användare redigerar en post i en vy visas ändringarna omedelbart i alla vyer och postsidorna för alla andra användare.

* Följande typer av fält uppdateras automatiskt och du kan inte redigera deras värden manuellt:
   * Länkade fält från andra poster
   * Formelfält
   * Systemfält (Skapat av, Skapat den, Senast ändrat den, Senast ändrat den)
* Om de poster som du visar är länkade till andra poster, återspeglas den nya informationen om de poster som du redigerar på de länkade posterna.
* Du kan inte redigera flera poster samtidigt. <!--this will probably change-->
* URL-adresser känns bara igen som länkar i enradiga textfält när de börjar med följande: http://, https://, ftp:// eller www. .
* Du kan lägga till en omslagsbild till varje post. Bilden är unik för varje post och gäller inte för alla poster samtidigt.
* Du kan redigera fältordningen på en postsida och lägga till en omslagsbild för en post. Mer information finns i [Hantera postsidans layout](/help/quicksilver/planning/records/manage-the-record-page.md).

## Redigera poster

Du kan redigera en post i följande områden:

* [Från tabellvyn för en posttyp](#edit-a-record-inline-in-the-table-view-of-a-record-type)
* [Från postens förhandsgranskning i en vy](#edit-a-record-from-the-records-preview-in-a-view)
* [Från postens sida](#edit-a-record-from-the-records-page)
* [Från ett Workfront-objekt i Planning-avsnittet](#edit-a-record-from-a-workfront-object-in-the-planning-section)

### Redigera en post textbundet i tabellvyn för en posttyp

{{step1-to-planning}}

1. Klicka på arbetsytan vars poster du vill redigera

   Arbetsytan öppnas och posttyperna visas som kort.
1. Klicka på ett posttypskort.

   Posttypssidan öppnas.
1. (Villkorligt) Klicka på fliken i en tabellvy eller klicka på **+-vy** för att skapa en tabellvy. Tabellvyn ska vara standardvy, såvida du inte har visat posttypen i en annan typ av vy när du senast öppnade den.

   Posterna som är associerade med den valda posttypen visas i tabellvyn.
1. Klicka inuti en post för att börja redigera information om den infogade posten.

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)

   >[!TIP]
   >
   >  Du kan inte redigera information för följande fält eftersom de är skrivskyddade och Workfront uppdaterar dem automatiskt:
   >  
   >  * Länkade fält som skapas genom att koppla posttyper. Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).
   >  * Fält av följande typer: Skapat av, Skapat den, Senast ändrat av, Senast ändrat den, Formelfält.

1. (Valfritt och villkorligt) Använd följande formateringsalternativ för **RTF** när du redigerar ett stycketextfält:

   * Fet
   * Kursiv
   * Understruken
   * Lägg till en länk
   * Lägga till en punktlista
   * Lägga till en numrerad lista

   ![](assets/rich-text-toolbar-on-paragraph-field.png)

1. (Valfritt) Dubbelklicka på ett kopplat postfält för att lägga till kopplade poster eller objekt till en annan post. Mer information finns i [Anslut poster](/help/quicksilver/planning/records/connect-records.md).
1. Tryck på **Enter** på tangentbordet eller klicka utanför en rad för att spara ändringarna. Ändringarna sparas automatiskt. En **sparad**-indikator visas kort i tabellvyns övre högra hörn för att visa att ändringarna sparades.


1. (Valfritt) Om du vill kopiera och klistra in information från ett fält till ett annat gör du något av följande:

   * Kopiera ett eller flera befintliga värden för ett fält och klistra sedan in dem i ett fält av samma typ på en annan post
   * Klicka på kolumnrubriken för en kolumn för att markera den och kopiera den, klicka sedan på kolumnrubriken för en annan kolumn och klistra in innehållet i den kopierade kolumnen. Kolumnerna måste innehålla liknande fälttyper.
   * Med Skift-tangenten nedtryckt klickar du för att markera flera rader i en tabell, kopierar informationen i de markerade raderna, klickar på en annan rad och klistrar in den markerade informationen på den nya raden och efterföljande rader.
   * Kopiera informationen från en cell, markera flera celler och klistra in samma information i flera celler. Du kan markera flera celler och klistra in samma information i flera celler från närliggande rader och kolumner.
   * Markera det nedre högra hörnet i en befintlig cell som innehåller den information som du vill kopiera och dra och släpp den sedan över de angränsande cellerna där du vill klistra in samma information. Alla celler måste innehålla samma typ av information.

     ![](assets/dragable-lower-right-corner-for-copy-paste-in-table-view.png)

   >[!NOTE]
   >
   >Tänk på följande:
   >
   >* Använd följande kortkommandon för att kopiera och klistra in information:
   >   * Copy: CTRL + C ( ⌘ + C för Mac)
   >   * Klistra in: CTRL + V ( ⌘ + V för Mac)
   >
   >* Du kan inte kopiera och klistra in fältvärden på postsidan. Den här funktionen stöds bara i tabellvyn för en posttyp.
   >* Du kan inte kopiera och klistra in fältvärden för följande fälttyper:
   >
   >
   >    * Länkade fält (eller uppslagsfält) som skapas genom att koppla posttyper. Du kan kopiera och klistra in länkade postfält. Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).
   >    * Fält av följande typer: Skapad av, Skapad, Senast ändrad av, Senast ändrad

1. (Valfritt) Använd följande kortkommandon för att ångra eller göra om redigering eller kopiering och inklistring av postinformation:

   * CTRL + Z ( ⌘ + Z för Mac) för att ångra en ändring
   * CTRL + Skift + Z ( ⌘ + Skift + Z för Mac) för att göra om en ändring

   >[!TIP]
   >
   >    Du kan använda kortkommandona flera gånger i rad för att ångra flera ändringar.

1. (Valfritt) Lägg till en miniatyrbild till en post. Mer information finns i [Lägga till en miniatyrbild i en post](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

### Redigera en post från postens förhandsgranskning i en vy

{{step1-to-planning}}

1. Klicka på arbetsytan vars poster du vill redigera

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett posttypskort.

   Posttypssidan öppnas.

1. Klicka på posten i en vy av valfri typ

   eller

   Klicka på ikonen **Öppna detaljer** ![](assets/open-details-icon-in-table-name-field.png) i den första kolumnen i tabellvyn. Postens förhandsgranskning öppnas i vyn.

   ![](assets/details-box.png)

1. (Valfritt) Klicka på menyn **Mer** till höger om postens titel och klicka sedan på **Byt namn**. Detta uppdaterar fältet som visas som postens titel.

   Postens rubrik är det primära fältet i posten när den visas i en tabellvy. Mer information finns i [Översikt över primärt fält](/help/quicksilver/planning/fields/primary-field-overview.md).

1. Börja redigera fältinformationen i postens förhandsgranskning.

   >[!TIP]
   >
   >  Du kan inte redigera information för följande fält eftersom de är skrivskyddade och Workfront uppdaterar dem automatiskt:
   >  
   >  * Sök efter fält från andra poster som har skapats genom att koppla posttyper. Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).
   >  * Fält av följande typer: Skapat av, Skapat den, Senast ändrat av, Senast ändrat den, Formelfält.

1. (Valfritt) Klicka på **Lägg till omslag** om du vill lägga till en omslagsbild i posten. Mer information finns i [Lägga till en omslagsbild till en post](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md).

1. (Valfritt) Håll pekaren över miniatyrbildikonen och klicka sedan på **Mer** ![](assets/more-menu.png) > **Redigera miniatyrbild** för att lägga till en miniatyrbild. Mer information finns i [Lägga till en miniatyrbild i en post](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

   Workfront sparar automatiskt ändringarna.

1. (Valfritt) Klicka på ikonen **Exportera** ![](assets/export-icon-in-record-details-page.png) om du vill exportera postens information. Mer information finns i [Exportera information för en post](/help/quicksilver/planning/records/export-the-record-page.md).

1. (Valfritt) Klicka på ikonen **Öppna på ny flik** ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> i det övre högra hörnet av postens förhandsgranskning för att öppna postens sida på en ny flik. Fortsätt redigera posten enligt beskrivningen i [Redigera en post från postens sidavsnitt](#edit-a-record-from-the-records-page) i den här artikeln.

### Redigera en post från postens sida

{{step1-to-planning}}

1. Klicka på arbetsytan vars poster du vill redigera

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett posttypskort.

   Posttypssidan öppnas.

1. Gör något av följande:

   * Från vilken vy som helst öppnar du postens förhandsgranskning enligt beskrivningen i [Redigera en post från postens förhandsgranskning i en vy](#edit-a-record-from-the-records-preview-in-a-view) i den här artikeln och klickar sedan på ikonen **Öppna på ny flik** ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> i det övre högra hörnet av postens förhandsgranskning för att öppna postens sida på en ny flik.

   * I vyn **Tabell** för du muspekaren över namnet på en post, klickar på menyn **Mer** ![](assets/more-menu.png) och sedan på **Visa**

     ![](assets/contextual-menu-for-record-row.png)

     Postsidan öppnas.

     ![](assets/details-page.png)

1. (Valfritt) Klicka på menyn **Mer** till höger om postens titel och klicka sedan på **Byt namn**. Detta uppdaterar fältet som visas som postens titel.

   Postens rubrik är det primära fältet i posten när den visas i en tabellvy. Mer information finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md).

1. Klicka på ett redigerbart fält på postsidan för att redigera det.

   >[!TIP]
   >
   >  Du kan inte redigera information för följande fält eftersom de är skrivskyddade och Workfront uppdaterar dem automatiskt:
   >  
   >  * Länkade fält som skapas genom att koppla posttyper. Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).
   >  * Fält av följande typer: Skapat av, Skapat den, Senast ändrat av, Senast ändrat den, Formelfält.

1. (Valfritt) Klicka på **Lägg till omslag** om du vill lägga till en omslagsbild i posten

   eller

   Håll pekaren över den befintliga omslagsbilden och klicka sedan på menyn **Mer** ![](assets/more-menu.png) > **Överför** för att lägga till en ny omslagsbild för posten.

   Mer information finns i [Lägga till en omslagsbild till en post](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md).

1. (Valfritt) Hovra över en befintlig miniatyrbild eller ikonen **miniatyrbild** ![](assets/record-thumbnail-icon-on-details-page.png) och klicka sedan på menyn **Mer** ![](assets/more-menu.png) > **Redigera miniatyrbild** för att lägga till en miniatyrbild för posten.

   Mer information finns i [Lägga till en miniatyrbild i en post](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

   Workfront sparar automatiskt ändringarna.

1. (Valfritt) Klicka på ikonen **Exportera** ![](assets/export-icon-in-record-details-page.png) om du vill exportera postens information. Mer information finns i [Exportera information för en post](/help/quicksilver/planning/records/export-the-record-page.md).


## Redigera en post från ett Workfront-objekt i planeringsavsnittet

När du har kopplat poster till Workfront-objekt kan du redigera Workfront Planning-poster i Workfront från objektets Planning-avsnitt.

Mer information finns i [Hantera poster i planeringsavsnittet för Adobe Workfront-objekt](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
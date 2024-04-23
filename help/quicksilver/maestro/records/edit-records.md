---
title: Redigera poster
description: Du kan redigera postinformation i Adobe Workfront Planning. Du måste skapa posttyper innan du kan börja skapa och redigera poster.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 6bea34403e45c2b50986f79272f7a46959d67c6d
workflow-type: tm+mt
source-wordcount: '1495'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Redigera poster

{{maestro-important-intro}}

Du kan redigera postinformation i Adobe Workfront Planning genom att redigera värdena i fälten som är kopplade till posterna.

Du måste skapa posttyper innan du kan börja skapa och redigera poster.

Mer information finns i [Skapa posttyper](../architecture/create-record-types.md).

Mer information om hur du skapar poster finns i [Skapa poster](/help/quicksilver/maestro/records/create-records.md).

&lt;!— här anger du att fälten i detaljvyn är desamma som fälten i tabellvyn - den här artikeln är länkad från vyerna Hantera post för att referera till den här informationen—>

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
<p>Din organisation måste vara registrerad i betaprogrammet Adobe Workfront Planning. Kontakta din kontorepresentant om du vill veta mer om det nya erbjudandet. </p>
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
   <p>Nytt: Ljus eller högre</p>
   eller
   <p>Aktuell: Arbete eller högre</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td>
   <td> <p>Det finns inga åtkomstkontroller för Adobe Workfront Planning</p>  
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
   <td> <p>Workfront- eller gruppadministratören måste lägga till planeringsområdet i layoutmallen. Mer information finns i <a href="../access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Mer information finns på [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Att tänka på när du redigerar poster

* Du kan redigera poster som du har skapat eller poster som har skapats av andra, om du har fått behörighet till arbetsytan.
* Du kan redigera postfält från följande områden:

   * Postens ruta i en postvy
   * Postens sida
   * Textbunden i en tabellvy.

* Följande typer av fält uppdateras automatiskt och du kan inte redigera deras värden manuellt:
   * Länkade fält från andra poster
   * Formelfält
   * Systemfält (Skapat av, Skapat den, Senast ändrat den, Senast ändrat den)
* Om de poster som du visar är länkade till andra poster, återspeglas den nya informationen om de poster som du redigerar på de länkade posterna.
* Du kan inte redigera flera poster samtidigt. <!--this will probably change-->
* URL-adresser känns bara igen som länkar i enradiga textfält när de börjar med följande: http://, https://, ftp:// eller www. .
* Du kan lägga till en omslagsbild till varje post. Bilden är unik för varje post och gäller inte för alla poster samtidigt.
* Du kan redigera fältordningen på en postsida och lägga till en omslagsbild för en post. Mer information finns i [Hantera postsidan](/help/quicksilver/maestro/records/manage-the-record-page.md).

## Redigera poster

Du kan redigera en post i följande områden:

* [Från tabellvyn för en posttyp](#edit-a-record-from-the-table-view-of-a-record-type)
* [Från postens ruta i en vy](#edit-a-record-from-the-records-box-in-a-view)
* [Från postens sida](#edit-a-record-from-the-records-page)

### Redigera en post textbundet i tabellvyn för en posttyp

{#step1-to-maestro}

Arbetsytan som du senast öppnade öppnas.

1. (Valfritt) Klicka på nedåtpilen till höger om arbetsytans namn för att markera arbetsytan vars poster du vill uppdatera.
1. Klicka på ett posttypskort.

   Posttypssidan öppnas.
1. (Villkorligt) Klicka på fliken i en tabellvy eller klicka på **+ Visa** för att skapa en tabellvy. Tabellvyn ska vara standardvy, såvida du inte har visat posttypen i en annan typ av vy när du senast öppnade den.

   Posterna som är associerade med den valda posttypen visas i tabellvyn.
1. Klicka inuti en post för att börja redigera information om den infogade posten.

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)

   >[!TIP]
   >
   >  Du kan inte redigera information för följande fält eftersom de är skrivskyddade och Workfront uppdaterar dem automatiskt:
   >  
   >  * Länkade fält som skapas genom att koppla posttyper. Mer information finns i [Koppla posttyper](../architecture/connect-record-types.md).
   >  * Fält av följande typer: Skapat av, Skapat den, Senast ändrat av, Senast ändrat den, Formelfält.

1. (Valfritt och villkorligt) Använd följande när du redigerar ett stycketextfält **RTF** formateringsalternativ:

   * Fet
   * Kursiv
   * Understruken
   * Lägg till en länk
   * Lägga till en punktlista
   * Lägga till en numrerad lista

   ![](assets/rich-text-toolbar-on-paragraph-field.png)

1. (Valfritt) Dubbelklicka på ett kopplat postfält för att lägga till kopplade poster eller objekt till en annan post. Mer information finns i [Koppla poster](/help/quicksilver/maestro/records/connect-records.md).
1. Tryck **Retur** på tangentbordet eller klicka utanför en rad för att spara ändringarna. Ändringarna sparas automatiskt. A **Sparad** indikator visas kort i tabellvyns övre högra hörn för att visa att ändringarna sparades.


1. (Valfritt) Om du vill kopiera och klistra in information från ett fält till ett annat gör du något av följande:

   * Kopiera ett eller flera befintliga värden för ett fält och klistra sedan in dem i ett fält av samma typ på en annan post
   * Klicka på kolumnrubriken för en kolumn för att markera den och kopiera den, klicka sedan på kolumnrubriken för en annan kolumn och klistra in innehållet i den kopierade kolumnen. Kolumnerna måste innehålla liknande fälttyper.
   * Med Skift-tangenten nedtryckt klickar du för att markera flera rader i en tabell, kopierar informationen i de markerade raderna, klickar på en annan rad och klistrar in den markerade informationen på den nya raden och efterföljande rader.
   * Kopiera informationen från en cell, markera flera celler och klistra in samma information i flera celler. Du kan markera flera celler och klistra in samma information i flera celler från närliggande rader och kolumner.

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
   >    * Länkade fält (eller uppslagsfält) som skapas genom att koppla posttyper. Du kan kopiera och klistra in länkade postfält. Mer information finns i [Koppla posttyper](../architecture/connect-record-types.md).
   >    * Fält av följande typer: Skapad av, Skapad, Senast ändrad av, Senast ändrad

1. (Valfritt) Använd följande kortkommandon för att ångra eller göra om redigering eller kopiering och inklistring av postinformation:

   * CTRL + Z ( ⌘ + Z för Mac) för att ångra en ändring
   * CTRL + Skift + Z ( ⌘ + Skift + Z för Mac) för att göra om en ändring

   >[!TIP]
   >
   >    Du kan använda kortkommandona flera gånger i rad för att ångra flera ändringar.

1. (Valfritt) Lägg till en miniatyrbild till en post. Mer information finns i [Lägga till en miniatyrbild i en post](/help/quicksilver/maestro/records/add-thumbnails-to-records.md).

### Redigera en post från postens ruta i en vy

{{step1-to-maestro}}

Arbetsytan som du öppnar senast öppnas.

1. (Valfritt) Klicka på nedåtpilen till höger om arbetsytans namn för att markera arbetsytan vars poster du vill uppdatera.

1. Klicka på ett posttypskort.

   Posttypssidan öppnas.

1. Klicka på en post i en vy av valfri typ

   eller

   I tabellvyn klickar du på **Öppna detaljer** icon ![](assets/open-details-icon-in-table-name-field.png) till vänster om ett postnamn. Postens ruta öppnas i vyn.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >Du kan visa **Öppna detaljer** ikonen till vänster om fältet Namn för en post i en tabellvy enbart när fältet Namn är primärt.

1. Börja redigera fältinformationen i postens ruta.

   >[!TIP]
   >
   >  Du kan inte redigera information för följande fält eftersom de är skrivskyddade och Workfront uppdaterar dem automatiskt:
   >  
   >  * Länkade fält som skapas genom att koppla posttyper. Mer information finns i [Koppla posttyper](../architecture/connect-record-types.md).
   >  * Fält av följande typer: Skapat av, Skapat den, Senast ändrat av, Senast ändrat den, Formelfält.

1. (Valfritt) Klicka på **Lägg till omslag** om du vill lägga till en omslagsbild i posten. Mer information finns i [Lägga till en omslagsbild till en post](/help/quicksilver/maestro/records/add-a-cover-image-to-a-record.md).

   Workfront sparar automatiskt ändringarna.

1. (Valfritt) Klicka på **Öppna på ny flik** icon ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> i det övre högra hörnet av postens ruta för att öppna postens sida på en ny flik. Fortsätt redigera posten enligt beskrivningen i [Redigera en post från postens sida](#edit-a-record-from-the-records-page) i den här artikeln.

### Redigera en post från postens sida

{{step1-to-maestro}}

Arbetsytan som du öppnar senast öppnas.

1. (Valfritt) Klicka på nedåtpilen till höger om arbetsytans namn för att markera arbetsytan vars poster du vill uppdatera.

1. Klicka på ett posttypskort.

   Posttypssidan öppnas.

1. Gör något av följande:

   * I alla vyer öppnar du postens ruta enligt beskrivningen i [Redigera en post från postens ruta i en vy](#edit-a-record-from-the-records-box-in-a-view) i den här artikeln klickar du på **Öppna på ny flik** icon ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> i det övre högra hörnet av postrutan för att öppna postens sida på en ny flik.

   * Från **Tabell** visa, hovra över namnet på en post och klicka sedan på **Mer** meny ![](assets/more-menu.png)och sedan klicka **Visa**

     ![](assets/contextual-menu-for-record-row.png)

     Postsidan öppnas.

     ![](assets/details-page.png)

1. Klicka på ett redigerbart fält på postsidan för att redigera det.

   >[!TIP]
   >
   >  Du kan inte redigera information för följande fält eftersom de är skrivskyddade och Workfront uppdaterar dem automatiskt:
   >  
   >  * Länkade fält som skapas genom att koppla posttyper. Mer information finns i [Koppla posttyper](../architecture/connect-record-types.md).
   >  * Fält av följande typer: Skapat av, Skapat den, Senast ändrat av, Senast ändrat den, Formelfält.

1. (Valfritt) Klicka på **Lägg till omslag** om du vill lägga till en omslagsbild i posten. Mer information finns i [Lägga till en omslagsbild till en post](/help/quicksilver/maestro/records/add-a-cover-image-to-a-record.md).

   Workfront sparar automatiskt ändringarna.


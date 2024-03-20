---
title: Redigera poster
description: Du kan redigera postinformation i Adobe Workfront planeringsfunktioner. Du måste skapa posttyper innan du kan börja skapa och redigera poster.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: e881aa57b5175ce5b559180a2713de0c607b3b1d
workflow-type: tm+mt
source-wordcount: '1337'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Redigera poster

{{maestro-important-intro}}

Du kan redigera postinformation i Adobe Workfront planeringsfunktioner genom att redigera värdena i fälten som är kopplade till posterna.

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
<p>Din organisation måste vara registrerad i det slutna betaprogrammet för Adobe Workfront planeringsfunktioner. Kontakta din kontorepresentant om du vill veta mer om det nya erbjudandet. </p>
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
   <td> <p>Det finns inga åtkomstkontroller för Adobe Workfront planeringsfunktioner </p>  
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
   <td> <p>Din Workfront- eller gruppadministratör måste lägga till Maestro-området i layoutmallen. Mer information finns i <a href="../access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Mer information finns på [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Att tänka på när du redigerar poster

* Du kan redigera poster som du har skapat eller poster som har skapats av andra, om du har fått behörighet till arbetsytan.
* Du kan redigera postfält från följande områden:

   * Rutan Detaljer för en post från en postvy.
   * Sidan Information för en post.
   * Textbunden i en tabellvy.

* Följande typer av fält uppdateras automatiskt och du kan inte redigera deras värden manuellt:
   * Länkade fält från andra poster
   * Formelfält
   * Systemfält (Skapat av, Skapat den, Senast ändrat den, Senast ändrat den)
* Om de poster som du visar är länkade till andra poster, återspeglas den nya informationen om de poster som du redigerar på de länkade posterna.
* Du kan inte redigera flera poster samtidigt. <!--this will probably change-->
* URL-adresser känns bara igen som länkar i enradiga textfält när de börjar med följande: http://, https://, ftp:// eller www. .

## Redigera poster

Du kan redigera en post i följande områden:

* [Från tabellvyn för en posttyp](#edit-a-record-from-the-table-view-of-a-record-type)
* [Från detaljsidan för en post](#edit-a-record-from-the-records-details-page)

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

   >[!NOTE]
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

   >[!NOTE]
   >
   >Tänk på följande:
   >
   >* Använd följande kortkommandon för att kopiera och klistra in information:
   >   * Copy: CTRL + C ( ⌘ + C för Mac)
   >   * Klistra in: CTRL + V ( ⌘ + V för Mac)
   >* Du kan inte kopiera information från en annan källa, förutom ett postfält av samma typ som det fält som du klistrar in informationen i.
   >
   >* Du kan inte kopiera och klistra in fältvärden i området Detaljer för en post. Den här funktionen stöds bara i tabellvyn för en posttyp.
   >* Du kan inte kopiera och klistra in fältvärden för följande fälttyper:
   >
   >
   >    * Länkade fält som skapas genom att koppla posttyper. Du kan kopiera och klistra in länkade postfält. Mer information finns i [Koppla posttyper](../architecture/connect-record-types.md).
   >    * Fält av följande typer: Skapad av, Skapad, Senast ändrad av, Senast ändrad

1. (Valfritt) Använd följande kortkommandon för att ångra eller göra om redigering eller kopiering och inklistring av postinformation:

   * CTRL + Z ( ⌘ + Z för Mac) för att ångra en ändring
   * CTRL + Skift + Z ( ⌘ + Skift + Z för Mac) för att göra om en ändring

   >[!TIP]
   >
   >    Du kan använda kortkommandona flera gånger i rad för att ångra flera ändringar.

1. (Valfritt) Lägg till en miniatyrbild till en post. Mer information finns i [Lägga till en miniatyrbild i en post](/help/quicksilver/maestro/records/add-thumbnails-to-records.md).

### Redigera en post från postens informationsruta i en vy

Du kan redigera en post i rutan Detaljer för vilken vy som helst.

{{step1-to-maestro}}

Arbetsytan som du öppnar senast öppnas.

1. (Valfritt) Klicka på nedåtpilen till höger om arbetsytans namn för att markera arbetsytan vars poster du vill uppdatera.

1. Klicka på ett posttypskort.

   Posttypssidan öppnas.

1. Klicka på en post i en vy av valfri typ

   eller

   I tabelltabellvyn klickar du på **Öppna detaljer** icon ![](assets/open-details-icon-in-table-name-field.png) till vänster om ett postnamn eller klicka på ett postnamn. The **Information** öppnas i vyn.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >Du kan visa **Öppna detaljer** ikonen till vänster om fältet Namn för en post i en tabellvy enbart när fältet Namn är primärt.

1. Börja redigera fältinformationen i **Information** box. Workfront sparar automatiskt ändringarna.

1. (Valfritt) Klicka på **Öppna på ny flik** icon ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> i det övre högra hörnet av **Information** för att öppna postens **Information** på en ny flik. Fortsätt redigera posten enligt beskrivningen i [Redigera en post från postens informationssida](#edit-a-record-from-the-records-details-page) i den här artikeln.

### Redigera en post från postens informationssida

Du kan redigera en post på detaljsidan.

{{step1-to-maestro}}

Arbetsytan som du öppnar senast öppnas.

1. (Valfritt) Klicka på nedåtpilen till höger om arbetsytans namn för att markera arbetsytan vars poster du vill uppdatera.

1. Klicka på ett posttypskort.

   Posttypssidan öppnas.

1. Gör något av följande:

   * Från vilken vy som helst öppnar du rutan Detaljer, som beskrivs i [Redigera en post från postens informationsruta i en vy](#edit-a-record-from-the-records-details-box-in-a-view)i den här artikeln. Klicka sedan på **Öppna på ny flik** icon ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> i det övre högra hörnet av **Information** för att öppna postens **Information** på en ny flik.

   * Från **Tabell** visa, hovra över namnet på en post och klicka sedan på **Mer** meny ![](assets/more-menu.png)och sedan klicka **Visa**

     ![](assets/contextual-menu-for-record-row.png)

     Posten **Information** sidan öppnas.

     ![](assets/details-page.png)

1. Klicka på **Mer** meny ![](assets/more-menu.png) till höger om postnamnet och klicka sedan på **Redigera**

   eller

   Klicka i ett redigerbart fält på detaljsidan för att redigera informationen.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->

1. Klicka **Spara ändringar**.
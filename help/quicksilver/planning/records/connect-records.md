---
title: Anslut poster
description: När du har skapat anslutningar mellan posttyper kan du koppla enskilda poster till varandra. Du kan visa information från en post på en annan post när du ansluter dem.
recommendations: noDisplay, noCatalog
feature: Workfront Planning
role: User, Admin
author: Alina
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '3306'
ht-degree: 0%

---


# Koppla poster

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>  -->

{{planning-important-intro}}

Du kan koppla Adobe Workfront Planning-poster till varandra eller till objekt från andra program. Du kan visa information från en post på en annan post när du ansluter dem.

I den här artikeln beskrivs hur du kan ansluta poster. Mer allmän information om hur du ansluter poster finns i [Översikt över](/help/quicksilver/planning/records/connected-records-overview.md) anslutna poster.

Du måste först koppla två posttyper till varandra, eller en posttyp till en objekttyp från ett annat program. Detta skapar sammanhängande postfält. Du kan sedan koppla poster till varandra eller poster till andra objekt från andra program i de anslutna postfälten.

Att koppla poster liknar att koppla poster till objekt från ett annat program.

Information om hur du ansluter posttyper till varandra eller till objekttyper från andra program finns i [Ansluta posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).

Ett exempel på hur du ansluter posttyper finns i [Exempel på anslutning av posttyper och poster](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md).

Du kan ansluta följande:

* Adobe Workfront Planera poster med varandra
* Adobe Workfront Planning-poster med objekt från andra program.

  Du kan koppla poster med objekt av de typer som anges nedan från följande program:

   * Adobe Workfront

      * Projekt
      * Portföljer
      * Program
      * Företag
      * Grupper

   * Adobe Experience Manager-resurser

      * Bildfiler
      * Mappar

  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

## Krav för åtkomst

+++ Expandera för att visa åtkomstkrav.

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
   <li><p> Planering av Adobe Workfront<p></li>
   <li><p>Adobe Experience Manager Assets, om du vill koppla AEM resurser till planeringsposter<p>
   <p>Du måste ha en Adobe Experience Manager Assets-licens och en integrering mellan AEM Assets och Workfront.    Mer information finns i <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront för Experience Manager Assets och Assets Essentials: artikelindex</a>. </p>
   </li>  
   </ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-plan*</p></td> 
   <td> 
<p>Någon av följande Workfront-planer:</p> 
<ul><li>Utvald</li> 
<li>Primtal</li> 
<li>Sist</li></ul> 
<p>Workfront Planning är inte tillgängligt för äldre Workfront-planer</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planeringspaket*</p></td> 
   <td> 
<p>Någon </p> 
<p>Om du vill ha mer information om vad som ingår i varje Workfront Planning-plan kontaktar du din Workfront-kontoansvarige. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-plattform</p></td> 
   <td> 
<p>Din organisations instans av Workfront måste vara registrerad i Adobe Unified Experience för att kunna komma åt Workfront Planning.</p> 
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience för Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licens för Adobe Workfront*</p></td> 
   <td> Standard
   <p>Workfront Planning är inte tillgängligt för äldre Workfront-licenser</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration av åtkomstnivå</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning-objekt</p> 
   <p>Visa eller högre behörigheter till de objekttyper som du vill länka från Workfront.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Behörigheter för objekt</p></td> 
   <td>   <p>Bidra eller högre behörigheter till en arbetsyta och posttyp för att ansluta poster </p>  
   <p>Visa eller högre behörigheter till en arbetsyta och posttyp för att visa alla anslutningar till objekt och fält från andra applikationer, oavsett din åtkomst i den andra applikationen. </p>
   <p>Visa eller högre behörigheter till de objekt som du vill länka från Workfront eller Experience Manager Assets. </p>
   <p>Systemadministratörer har behörighet till alla arbetsytor, även de som de inte har skapat.</p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om åtkomstkrav för Workfront finns [i Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på vid anslutning av poster

* För att koppla poster med andra poster eller objekt måste du ha följande:

   * Minst en arbetsyta, posttyp och post.

     Mer information finns i följande artiklar:

      * [Skapa arbetsytor](/help/quicksilver/planning/architecture/create-workspaces.md)
      * [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md)
      * [Skapa poster](/help/quicksilver/planning/records/create-records.md)

   * Anslutningar mellan posttyper, eller mellan posttyper och objekt från andra program. Mer information finns i [Ansluta posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).

* Du kan koppla en eller flera poster eller objekt till varandra. Detta beror på vilken anslutningstyp du valde när du anslöt post- eller objekttyperna. Mer information finns i [Översikt över](/help/quicksilver/planning/architecture/connect-record-types-overview.md) Anslut posttyper.

## Koppla poster från Workfront Planning

Du kan koppla poster från Workfront Planning i följande områden i en planeringspost:

* De anslutna postfälten i tabellvyn.
* Postens förhandsgranskningsruta eller sida i de anslutna postfälten på fliken Detaljer.
* Postens förhandsgranskningsruta eller sida på fliken Anslutningar.
* Postens sida på sidan Anslutna poster.

### Anslut Workfront Planning-poster från tabellvyn eller detaljområdet i en post

{{step1-to-planning}}

1. Klicka på den arbetsyta vars poster du vill koppla.

   Arbetsytan öppnas och posttyperna visas som kort.
1. Klicka på kortet för en posttyp för att öppna sidan för posttypen.
1. Klicka på namnet på en tabellvy för att öppna den.
1. (Valfritt) Lägg till poster i den posttyp som du har valt genom att lägga till en ny rad i tabellen. Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).
1. (Villkorligt) När du har kopplat den valda posttypen till en annan posttyp går du till det anslutna fältet i en post och klickar i fältet eller klickar på **Anslut** för att lägga till post.

   ![Koppla ihop andra poster i tabellvyn](assets/connect-other-records-smaller-box-in-table-view.png)

1. Gör något av följande:

   * Klicka på namnet på en ansluten post i listan för att lägga till den i den valda posten. Posten läggs till automatiskt.
   * Börja skriva namnet på en post och klicka på den när den visas i listan. Posten läggs till automatiskt.

   >[!TIP]
   >
   >Om endast bilden av posten valdes för att visas när posttyperna var anslutna, visas endast miniatyrbilden eller ikonen för posten i det anslutna fältet. Mer information finns i [Ansluta posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).
   >

1. (Villkorligt) Om du valde En till många eller En till en som Anslutningstyp när du anslöt posttyperna, och du försöker ansluta en post eller ett objekt som redan är anslutet någon annanstans, får du en varning om att om du ansluter den igen kommer den att tas bort från den ursprungliga anslutningen. Klicka på Anslut **om du vill tillåta borttagning och koppla posten, eller** på **Avbryt** om du vill gå tillbaka till fältet och välja en annan post.
1. (Valfritt) Om du inte kan hitta ett objekt att ansluta och vill lägga till det klickar du på **+ Lägg till**

   Eller

   Börja skriva ett namn för objektet och klicka sedan på **+ Lägg** till för att skapa och lägga till det.

   Mer information finns i avsnittet &quot;Skapa poster när du kopplar dem från andra poster&quot; i artikeln [Skapa poster](/help/quicksilver/planning/records/create-records.md).

   >[!TIP]
   >
   >    Du kan öppna sidan för en post och koppla ihop andra poster genom att göra följande i tabellvyn:
   >1. Klicka på namnet på posten i vyn.
   >1. Leta reda på det länkade postfältet och dubbelklicka på fältet (om det redan finns anslutna poster)
   >Eller
   >Klicka på **Koppla poster** (om fältet är tomt) för att lägga till poster från den kopplade posten eller objekttypen.
   >
   >![Koppla poster från postsidans fält](assets/connect-records-from-record-page-field.png)

1. (Valfritt) Klicka på **Visa alla** om du vill visa alla poster.

1. (Villkorligt) Om du klickade på Visa alla **i föregående steg** visas rutan Anslut objekt **.**

   ![Tabell över anslutna objekt för poster](assets/connected-objects-table-for-records.png)

1. Börja skriva namnet på en post i sökrutan och välj den sedan när den visas i listan

   Eller

   Markera namnet på en eller flera poster i rutan och klicka sedan på **Koppla objekt**.

   Följande skall läggas till:

   * De länkade posterna visas i fältet för den länkade posten som du valde i ett tidigare steg.
   * De länkade fälten fylls i med informationen från de länkade posterna, om du lade till länkade uppslagsfält när du kopplade posttyperna.

   När du uppdaterar de länkade posterna uppdateras de länkade fälten för de poster som du länkar från automatiskt. Du kan inte redigera länkade fält manuellt.

   >[!TIP]
   >
   >* Vi använder &quot;länkade fält&quot; och &quot;uppslagsfält&quot; omväxlande.
   >
   >* När du väljer att koppla flera poster när du kopplar ihop posttyperna, visas fältvärdena från de olika objekten antingen separerade med kommatecken eller aggregeras enligt den aggregator du valde när du anslöt posttyperna.
   >* Du kan inte lägga till Workfront typeahead-fält (inklusive fält som Projektägare eller Projektsponsor) som uppslagsfält.
   >
   >* Workfront-objektens datumfältsinformation visas i 24-timmarsformat i Workfront Planning, oavsett hur den visas i Workfront.
   >
   >   Om ett projekts planerade startdatum till exempel visas som 15:00 :00 i Workfront visas det som 15:00 i Workfront Planning i ett importerat uppslagsfält.

1. (Valfritt) Stäng sidan för posttyp och gå till den arbetsyta som du har valt.
1. Klicka på kortet för den posttyp som du har länkat till.

   Om du till exempel har kopplat **kampanjposten** till produktposten klickar du på produktkortet **&#x200B;**.

   Kortet för posttyp ska öppnas i tabellvyn. Om inte, välj en tabellvy.

   Observera att **fältet Länkad post för kampanj** visar namnen på de kampanjer som du har länkat till produkter på sidan Typ av produktpost. När du uppdaterar kampanjinformationen uppdateras automatiskt fältet Länkad kampanjpost för posttypen Produkt.

### Koppla Workfront Planning-poster till Workfront-objekt från tabellvyn eller detaljområdet för en post

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

När du har skapat en anslutning mellan en posttyp och en Workfront-objekttyp kan du koppla enskilda poster till objekt i Workfront. De Workfront-fält som du har anslutit fylls i automatiskt i de poster som du länkar objekten från.

>[!NOTE]
>
>Du kan inte koppla Workfront-objekttyper med Workfront Planning-posttyper från Workfront.


{{step1-to-planning}}

1. Klicka på den arbetsyta vars poster du vill koppla.

   Arbetsytan öppnas och posttyperna visas som kort.
1. Klicka på kortet för en posttyp för att öppna sidan för posttypen.
1. Välj en **tabellvy** i **listrutan Visa** .

1. Klicka på **Ny post**  om du vill lägga till enskilda poster i den posttyp som du har valt. Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).

1. (Villkorligt) När du har kopplat den valda posttypen till en Workfront-objekttyp går du till det anslutna fältet på en post och klickar antingen på fältet eller klickar på **Anslut** för att lägga till Workfront-objekt.

   ![Koppla ihop projekt i tabellvyn](assets/connect-projects-smaller-box-in-table-view.png)

1. Gör något av följande:

   * Klicka på ett objekt i listan för att lägga till det i den markerade posten. Objekten listas i alfabetisk ordning. Objektet läggs till automatiskt.
   * Börja skriva namnet på ett objekt och klicka på det när det visas i listan. Objektet läggs till automatiskt.

   >[!TIP]
   >
   >Du kan öppna sidan för en post från vyn, dubbelklicka på det länkade postfältet eller klicka på **Koppla** i fältet för att lägga till objekt från den anslutna objekttypen.

1. (Valfritt) Om du inte kan hitta ett objekt att ansluta och vill lägga till det klickar du på **+ Lägg till**

   Eller

   Börja skriva ett namn för objektet och klicka sedan på **+ Lägg** till för att skapa och lägga till ett nytt projekt, portfölj eller program.

   Mer information finns i [Skapa Workfront-objekt från Workfront Planning](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)

1. (Valfritt) Klicka på **Visa alla** om du vill visa alla objekt som du har minst behörighet att visa.

   Om du klickade på Visa alla **i föregående steg** visas rutan Anslut objekt **.**

   ![Rutan Koppla objekt för att välja projekt](assets/connect-objects-box-to-select-projects.png)

1. Börja skriva namnet på ett Workfront-objekt i sökrutan och välj det sedan när det visas i listan

   Eller

   Markera namnet på ett eller flera objekt i rutan och klicka sedan på **Koppla ihop objekt**.

   >[!IMPORTANT]
   >
   >* Du kan bara lägga till Workfront-objekt som du har tillgång till att visa.
   >
   >* När du lägger till Workfront-objekt kan alla med visningsbehörighet eller högre behörighet till arbetsytan visa Workfront-objekten och deras fältinformation, oavsett deras behörigheter eller åtkomst i Workfront.

   Följande skall läggas till:

   * De markerade Workfront-objekten läggs till i det länkade postfältet.
   * Om du lade till dem när du kopplade posttypen till Workfront fylls de länkade fälten (eller uppslagsfälten) i Workfront-objekten automatiskt med information från Workfront.

   Mer information om hur du ansluter posttyper till objekt från ett annat program finns i [Ansluta posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).

1. (Valfritt) Klicka på namnet på ett Workfront-objekt som är kopplat till en Workfront Planning-post antingen i det länkade fältet i en tabellvy eller från det länkade fältet på postsidan.

   Då öppnas Workfront-objektet i Workfront, om du har minst visningsbehörighet till objektet.

   >[!TIP]
   >
   >* När du väljer att koppla flera poster när du ansluter posttyperna visas värdena i uppslagsfälten antingen separerade med kommatecken eller aggregeras enligt den aggregator du har valt.
   >
   >* Ett länkat postfält skapas inte för de länkade Workfront-objekten i Workfront.

1. (Valfritt) Från tabellvyn för posttypen håller du muspekaren över kolumnrubriken för det länkade Workfront-objektet och klickar på rullgardinsmenyn och klickar sedan på **Redigera uppslagsfält**.

1. Lägg till Workfront-objektfält från området Omarkerade **fält**

   Eller

   Ta bort Workfront-objektfält från **området Valda fält** .

   Detta lägger till eller tar bort länkade fält från Workfront Planning-posterna. Informationen som är kopplad till de borttagna fälten finns kvar i Workfront.


### Anslut Workfront Planning-poster till Adobe Experience Manager-objekt från tabellvyn eller området Detaljer i en post

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

>[!IMPORTANT]
>
>Du måste ha en Adobe Experience Manager Assets-licens och din organisations instans av Workfront måste vara registrerad på Adobe Business Platform eller Adobe Admin Console för att kunna ansluta Workfront Planning-poster till Adobe Experience Manager Assets.
>
>Om du har frågor om hur du kommer igång med Adobe Admin Console kan du läsa Vanliga frågor och svar[ om ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md)Adobe Unified Experience.

När du har skapat en anslutning mellan en posttyp och Adobe Experience Manager Assets kan du koppla enskilda poster till Experience Manager-resurser. De resursfält som du anslöt från Experience Manager Assets när du skapade anslutningen fylls automatiskt i den posttyp som du länkade från.

>[!NOTE]
>
>Planeringsposter och deras fält är tillgängliga från Experience Manager Assets när Workfront-administratören konfigurerar metadatamappningen genom integreringen mellan Workfront och Adobe Experience Manager Assets. Mer information finns i [Konfigurera mappning av resursmetadata mellan Adobe Workfront och Experience Manager Assets](https://experienceleague.adobe.com/sv/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).

Så här kopplar du poster till Experience Manager-resurser:

{{step1-to-planning}}

1. Klicka på den arbetsyta vars poster du vill koppla.

   Arbetsytan öppnas och posttyperna visas.
1. Klicka på kortet för en posttyp för att öppna sidan för posttypen.
1. Välj en **tabellvy** i listrutan Visa **&#x200B;**&#x200B;i det övre högra hörnet på sidan för posttyp.

1. (Valfritt) Klicka på **Ny post** om du vill lägga till nya poster i den posttyp som du har valt. Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).
1. (Villkorligt) När du har kopplat den valda posttypen till Experience Manager Assets går du till det anslutna fältet på en post och klickar antingen på fältet eller klickar på **Connect** för att lägga till Experience Manager-resurser i posten och klickar sedan på +**-ikonen**.

   >[!TIP]
   >
   >  Du kan lägga till att klicka på **+** -ikonen i det länkade objektfältet på postsidan för att koppla tillgångar till posten.

   Rutan Välj **tillgångar** visas. <!--we might change this to Connect assets-->

   ![Rutan Välj resurser för AEM postanslutningar](assets/select-assets-box-for-aem-record-connections.png)

1. Klicka för att välja några av följande typer av tillgångar:

   * Bilder
   * Mappar

   Du kan välja flera tillgångar.

   >[!IMPORTANT]
   >
   > Du kan bara ansluta resurser som du har tillgång till i Experience Manager. När de är anslutna kan alla Workfront Planning-användare visa resurserna i Workfront Planning, oavsett om de har åtkomst till Experience Manager Assets.

1. Klicka på **Välj**. <!-- we might change this to Connect-->

   Följande skall läggas till:

   * De valda Experience Manager-resurserna läggs till i det länkade postfältet.
   * De länkade fälten (eller uppslagsfälten) fylls i med information från de Experience Manager-anslutna resurserna.

     All befintlig information från fälten i Experience Manager-resurserna visas automatiskt i de länkade fälten eller uppslagsfälten.

     >[!TIP]
     >
     >* När du väljer att ansluta flera poster när du ansluter posttyperna visas värdena för de olika objekten antingen avgränsade med kommatecken eller aggregerade enligt den aggregator du väljer.
     >
     >* Ett länkat postfält till de länkade Workfront Planning-posterna skapas inte för de länkade Experience Manager-resurserna i Experience Manager Assets-programmet.

1. (Valfritt) Gå till den posttyp som du länkade till Experience Manager Assets från och klicka på namnet på en resurs i det länkade postfältet. Experience Manager-information om resursen visas i ett popup-fönster.

   ![Popup-fönster för resurser med AEM information och miniatyrbild](assets/asset-pop-up-window-with-aem-details-and-thumbnail.png)

   Följande fält visas för en bildfil:

   * En miniatyrbild av bilden
   * Namnet på bildfilen
   * Mått
   * Storlek
   * Beskrivning
   * Filsökvägen i Experience Manager
   * Typ av tillgång
   * Skapad den
   * Ändrad datum

1. (Valfritt) Om du vill öppna postsidan för Experience Manager-resurser i Experience Manager går du till posttypssidan för den post som du länkar från, klickar på namnet på en resurs i det länkade postfältet för att öppna popup-fönstret och klickar sedan på **ikonen Öppna i AEM** ![Öppna resurs i AEM](assets/open-asset-icon.png) för att öppna resursen.

   Då öppnas Experience Manager-resursen i Adobe Experience Manager Assets.

1. (Valfritt) Håll muspekaren över kolumnrubriken för den länkade Experience Manager-resursen i tabellvyn för posttypen, klicka på rullgardinsmenyn och klicka sedan på **Redigera uppslagsfält**.

1. Lägg till Experience Manager Assets-objektfält från området **Omarkerade fält**

   Eller

   Ta bort Workfront-objektfält från **området Valda fält** .

   Detta lägger till eller tar bort länkade fält från posterna. Informationen som är kopplad till de borttagna fälten finns kvar i Adobe Experience Assets.

### Koppla Workfront Planning-poster till andra poster eller objekt från fliken Anslutningar på postsidan

1. Gå till en vy av en posttyp som har kopplats till andra planeringsposttyper eller objekttyper från andra program.
1. Följ stegen som beskrivs i föregående underavsnitt för att hitta en post i vyn som du vill koppla ihop med andra poster eller objekt.
1. Klicka på namnet på en post.

   Förhandsgranskningssidan öppnas.
1. (Valfritt) **Klicka på ikonen**&#x200B;Öppna i ny flik![ Öppna information i en ny flik](assets/open-details-in-a-new-tab-icon.png) för att öppna postens sida.
1. **Klicka på fliken Anslutningar** i postens förhandsgranskning eller på sidan.

   ![Fliken Anslutningar på posten i Workfront Planning](assets/connections-tab-on-record-in-workfront-planning.png)

   Alla post- eller objekttyper som är länkade till den valda posttypen visas som avsnitt. Kopplade poster eller objekt visas under sina post- eller objekttypsnamn på kort.

   >[!TIP]
   >
   >    Endast anslutna poster som har enskilda poster anslutna visas som standard.

1. (Valfritt) Klicka på **Visa alla anslutningar** för att visa alla anslutna posttyper, inklusive de som inte har anslutna poster.

1. (Valfritt) Klicka på den nedåtpekande pilen till vänster om ett avsnitt för att komprimera det.

1. (Villkorligt) Klicka på **Anslut** om du vill lägga till fler poster eller objekt av samma typ.
1. (Valfritt) Om du inte kan hitta en post eller ett objekt att koppla och du vill lägga till det klickar du på **+ Lägg till**

   Eller

   Börja skriva ett namn för objektet och klicka sedan på **+ Lägg** till för att skapa och lägga till det i posten.

   Mer information finns i avsnittet &quot;Skapa poster när du kopplar dem från andra poster&quot; i artikeln [Skapa poster](/help/quicksilver/planning/records/create-records.md).
1. Följ stegen som beskrivs i föregående avsnitt för att koppla poster från Workfront Planning eller objekt från Workfront eller Experience Manager Assets.
Posterna och objekten läggs till direkt.
1. (Valfritt) Håll muspekaren över det anslutna kortet för en post eller ett objekt och klicka sedan på **ikonen** Koppla från post![ för att koppla bort post för att koppla bort den](assets/disconnect-icon-with-tooltip.png) från den valda posten.

   ![Koppla från inspelningsikonen med verktygstipset på fliken anslutningar](assets/disconnect-record-icon-with-tooltip-on-connections-tab.png)

   Posten kopplas omedelbart bort från alla områden i Workfront Planning eller från andra program där den kan visas som ansluten. Alla uppslagsfältsvärden tas också bort.

### Koppla poster från sidan Anslutna poster för en post

1. Gå till en vy av en posttyp som har kopplats till andra planeringsposttyper eller objekttyper från andra program.
1. Följ stegen som beskrivs i föregående underavsnitt för att hitta en post i vyn som du vill koppla ihop med andra poster eller objekt.
1. Klicka på namnet på en post.

   Förhandsgranskningssidan öppnas.
1. **Klicka på ikonen**&#x200B;Öppna i ny flik![ Öppna information i en ny flik](assets/open-details-in-a-new-tab-icon.png) för att öppna postens sida.
1. Klicka på en befintlig flik för sidan Anslutna poster på postens sida. Du måste först skapa sidan Anslutna poster. Mer information finns i [Hantera postsidans layout](/help/quicksilver/planning/records/manage-the-record-page.md).

   En ansluten posttypssida visas i tabellvyn.

   Alla anslutna poster av en typ visas i tabellen.
1. Klicka på **Anslut** för att lägga till eller ta bort poster.

   ![Knappen Anslut är markerad på fliken Information om ansluten post](assets/connect-button-highlighted-in-connected-record-details-tab.png)
1. (Valfritt) Om du inte hittar en ansluten post klickar du på **+ Lägg** till för att skapa och ansluta dem.

## Koppla ihop poster från Workfront-objekt

Du måste ha följande för att kunna ansluta Workfront Planning-poster från Workfront-objekt:

* Anslutningar mellan posttyper och Workfront-objekttyper som upprättas i Workfront Planning.
* Din Workfront- eller gruppadministratör måste lägga till något av följande i en Workfront-objekttyp:

   * Avsnittet Planering till Workfront-projekt, portföljer och program i layoutmallen.

   * Det anpassade fältet Planeringsanslutningar till ett anpassat formulär för något av följande objekt:

      * Projekt
      * Portfölj
      * Program
      * Grupp
      * Företag

  Mer information finns i [Hantera postanslutningar från Workfront-objekt](/help/quicksilver/planning/records/manage-records-in-planning-section.md).

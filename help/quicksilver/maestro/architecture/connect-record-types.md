---
title: Koppla posttyper
description: Ett sätt att ange hur enskilda posttyper relaterar till varandra är att koppla dem. Du kan även koppla Maestro-posttyper till objekttyper från andra program för att förbättra användarupplevelsen och behålla fokus i ett program.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 6f026590f0030b564f0d110afead9ade1acd7896
workflow-type: tm+mt
source-wordcount: '2020'
ht-degree: 0%

---

<!-----
title: Connect record types
description: A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Maestro record types with object types from other applications to enhance your users' experience and keep their focus in one application.
hidefromtoc: yes
hide: yes
feature: Work management
role: User
author: Alina
--->

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->
<!--************ THIS MIGHT NO LONGER BE A 'RELATIONSHIP' TYPE FIELD, BECAUSE THEY WILL SHOW IT IN THE CONNECTION TAB*****************************-->


# Koppla posttyper

>[!IMPORTANT]
>
>Informationen i den här artikeln handlar om Adobe Maestro, ett nytt erbjudande från Adobe Workfront.
>
>För närvarande ingår Adobe Maestro i ett betaprogram som är öppet för ett begränsat antal kunder. Du måste vara Workfront-kund för att kunna använda Maestro-funktionerna.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.
>
>Mer information finns i [Adobe Maestro - översikt](../maestro-overview.md).

Du kan använda Adobe Maestro för att utforma anpassningsbara arbetsytor som innehåller de posttyper som behövs i organisationen. Ett sätt att ange hur enskilda posttyper relaterar till varandra är att koppla dem. Du kan även koppla Maestro-posttyper till objekttyper från andra program för att förbättra användarupplevelsen och behålla fokus i ett program.

Du kan ansluta följande:

* Posttyper i maestro operativt
* Maestro taxonomier mot varandra
* Posttyper och taxonomier för Maestro operativt
* Posttyper och taxonomier med objekttyper från andra program.

På så sätt kan du visa fält från den länkade posten eller objekttypen på en annan Maestro-post.

I den här artikeln beskrivs hur du kan koppla två Maestro-posttyper eller en Maestro-posttyp till ett objekt från ett annat program.

När anslutningen mellan post- eller objekttyper har upprättats kan du koppla enskilda poster till varandra.

Mer information om hur du ansluter en Maestro-post till ett objekt från ett annat program finns i [Koppla poster](../records/connect-records.md).

Ett exempel på hur du ansluter posttyper finns i [Exempel på att ansluta posttyper och poster](../architecture/example-connect-record-types-and-records.md).

<!--ensure this last linked article is right; the title and the link should have changed-->

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
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p><b>ANMÄRKNING</b></p>
   <p>Om du vill ansluta Maestro-posttyper till Experience Manager Assets måste du ha en Adobe Experience Manager Assets-licens och din organisations instans av Workfront måste vara registrerad på Adobe Business Platform eller Adobe Admin Console. </p>
   </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-avtal</p></td>
   <td>
<p>Din organisation måste vara registrerad i det betaprogram som Adobe Maestro stängt. Kontakta din kontorepresentant om du vill veta mer om det nya erbjudandet. </p>
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
   <p>Alla</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Åtkomstnivå</td>
   <td> <p>Alla</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Layoutmall</td>
   <td> <p>Systemadministratören måste lägga till Maestro-området i layoutmallen. Mer information finns i <a href="../access/grant-access.md">Ge åtkomst till Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permssions - replace the table with: 

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
   <p> Adobe Workfront</p> <p>To connect Maestro record types with Experience Manager Assets, you must have an Adobe Experience Manager Assets license and your organization's instance of Workfront must be onboarded to the Adobe Business Platform or the Adobe Admin Console.</p> </td>
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
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create
</td>
  </tr>
 </tbody>
</table>

-->

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->


## Att tänka på när du ansluter posttyper

Tänk på följande:

* Du kan ansluta följande enheter i Maestro:

   * Två driftsposttyper
   * Två taxonomier
   * En driftsposttyp och en taxonomi
   * En operativ posttyp eller en taxonomi och en objekttyp från ett annat program.

* Du kan koppla följande objekt från följande program till posttyper i Maestro:

   * Adobe Workfront:

      * Projekt
      * Portfolio
      * Program
      * Företag
      * Grupper

   * Adobe Experience Manager Assets:

      * Bilder
      * Mappar

     >[!IMPORTANT]
     >
     >Du måste ha en Adobe Experience Manager Assets-licens och din organisations instans av Workfront måste vara registrerad på Adobe Business Platform eller Adobe Admin Console för att kunna ansluta Maestro-poster till Adobe Experience Manager Assets.
     >
     >Om du har frågor om hur du kommer igång med Adobe Admin Console kan du läsa [Adobe - frågor och svar om enhetliga upplevelser](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* När du har kopplat en posttyp till en annan posttyp eller till en objekttyp från ett annat program finns följande scenarier:

   * **När du ansluter två posttyper**: Ett länkat postfält skapas för den posttyp som du ansluter från. Ett liknande länkat postfält skapas för den posttyp som du ansluter till.

     Om du till exempel ansluter posttypen&quot;Campaign&quot; till posttypen&quot;Product&quot; skapas ett länkat postfält som du kallar&quot;Linked Product&quot; för posttypen Campaign, och en länkad posttyp som automatiskt kallas&quot;Campaign&quot; skapas för posttypen Produkt.

   * **När du ansluter en posttyp med en objekttyp från ett annat program**: Ett länkat postfält skapas för den posttyp som du ansluter från. Inget länkat postfält skapas automatiskt i tredjepartsprogramobjektet.

     En ny Maestro-posttyp skapas för tredjepartsprogramobjektet endast när faktiska objekt är kopplade till Maestro-posterna.

     Mer information finns i [Koppla poster](../records/connect-records.md).

   * **När du lägger till uppslagsfält från posten eller objektet som du ansluter till**: Länkade fält läggs till i den post som du ansluter från som visar de uppslagsfält som du har valt att hämta från den länkade posten till de poster som du länkar från. Postfälten är alltid skrivskyddade och fylls i automatiskt med värden för tredjepartsobjektet.

     Om du till exempel kopplar posttypen&quot;Campaign&quot; till ett Workfront-projekt och du väljer att överföra fältet Planerat slutförandedatum för projektet till Maestro-posten, skapas ett länkat fält med namnet Planerat slutförandedatum (från projekt) automatiskt för den post du länkar från.

* Länkade postfält föregås av en relationsikon ![](assets/relationship-field-icon.png).

  Länkade fält föregås av en ikon som anger fälttypen. Till exempel ikoner som anger att ett fält är ett tal, ett stycke eller ett datum.

* När du har skapat enskilda poster för en posttyp kan du välja de poster som du ansluter till från det länkade posttypsfältet. Mer information finns i [Koppla poster](../records/connect-records.md).

## Koppla posttyper

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-maestro}}

Den senast använda arbetsytan bör öppnas som standard.

1. (Valfritt) Expandera den nedåtriktade pilen till höger om namnet på en befintlig arbetsyta och markera den arbetsyta som du vill koppla posttyper från.
1. Klicka på kortet för en posttyp för att öppna posttypssidan.
1. Klicka på **+** i tabellvyns övre högra hörn och klicka sedan på **Ny anslutning** -fliken.

   ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. I **Posttyp** väljer du något av följande: <!--is the field name spelled right? lowercase "t"?-->

   * En annan operativ posttyp eller en taxonomi från arbetsytan som du valde

     >[!TIP]
     >
     >Det är bara posttyper och taxonomier från den arbetsyta som du har valt som är tillgängliga att ansluta till.
     > 
     >Om du inte har andra posttyper på den valda arbetsytan visas inte arbetsytans namn.

   * A **Projekt, Portfolio, Program, Företag**, eller **Grupp** från **Workfront-objekttyper** -avsnitt.
   * **Experience Manager Assets** från **Adobe-program** -avsnitt.

   ![](assets/new-connection-tab-fields-with-another-record-selected.png)


1. Uppdatera följande information:

   * **Namn**: Namnet på det anslutna fältet, så som det kommer att visas i tabellvyn eller på detaljsidan för den ursprungliga posttypen. Då skapas den länkade postkolumnen i tabellvyn för den ursprungliga posttypen eller det länkade postfältet för de ursprungliga posterna. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->

   >[!TIP]
   >
   >Vi rekommenderar att du tar med namnet på den post som du länkar till i namnet på det anslutna postfältet för att ta reda på vilken posttyp det nya fältet kommer från. Namnet på den länkade posten visas inte i det nya länkade postfältet eller i dess länkade fält.

   * **Beskrivning**: Ytterligare information om det anslutna postfältet. Beskrivningen av ett fält visas när du hovrar över fältets kolumn i en tabell.
   * **Tillåt flera poster**: Välj det här alternativet för att ange att du tillåter att användare kan lägga till flera poster när fältet för länkad posttyp visas på de ursprungliga posterna. Detta är markerat som standard.
   * **Välj sökfält**: Välj det här alternativet om du vill lägga till fält från den valda posttypen. Detta är markerat som standard.

1. (Villkorligt och valfritt) Om du valt att ansluta ett Workfront-objekt väljer du en **Eget formulär** från **Länka endast projekt som uppfyller dessa villkor** -avsnitt. <!--this needs to be updated for each object when they fix this UI.--> Det är bara objekt som har de markerade anpassade formulären kopplade som kan länkas till den valda Maestro-posttypen. Du kan markera flera formulär.

   ![](assets/workfront-project-connection-selection.png)

1. (Villkorligt) Om du valt att ansluta till Experience Manager Assets väljer du en databas i dialogrutan **Experience Manager-databas** nedrullningsbar meny i **Länka resurser från följande databas** -avsnitt. Detta är ett obligatoriskt fält. Endast databaser som du har åtkomst till i Experience Manager Assets visas i det här fältet.

   ![](assets/aem-assets-connection-selection.png)

1. Klicka **Skapa**.

1. (Villkorligt) Om du markerade **Välj sökfält** inställning, **Lägg till sökfält** öppnas.

   Klicka på **+** ikon för att lägga till fält från **Omarkerade fält** område.

   eller

   Klicka på **-** ikonen för att ta bort fält från **Markerade fält** area

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)


1. (Valfritt) Klicka på **Hoppa över** och lägg inte till några fält från den länkade posten eller objektet. The **Namn** av den länkade posten är det enda synliga fältet i den ursprungliga postens tabellvy.

1. (Valfritt och villkorligt) Om du väljer att länka ett tal, en valuta, en procentandel eller ett datumtypsfält, ska du även välja ett aggregeringsvärde. Värdena för de länkade fälten visas antingen avgränsade med kommatecken eller som ett aggregeringsvärde enligt den aggregator du väljer, när användare markerar mer än en länkad post i det länkade postfältet.

   ![](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > Aggregatorer är inte tillgängliga när du ansluter posttyper till Experience Manager Assets.

   Välj bland följande:

   * **Ingen**: Visar värden som kommer från flera poster avgränsade med kommatecken. Det här är standardvalet.
   * **MAX**: Visar det högsta värdet från alla värden som kommer från flera markerade poster i det länkade postfältet.
   * **MIN**: Visar det lägsta värdet från alla värden som kommer från flera poster som är markerade i det länkade postfältet.
   * **SUM**: Visar summan av alla värden som kommer från flera markerade poster i det länkade postfältet.
   * **AVG**: Visar medelvärdet av alla värden som kommer från flera markerade poster i det länkade postfältet.

   >[!NOTE]
   >
   >Du kan till exempel länka produktposten (den länkade posten) från Campaign-posten (den ursprungliga posten) och ge den namnet&quot;Produktfält&quot;. Du kan också välja att länka produktpostens budgetfält från kampanjposten och kalla det&quot;Produktbudget&quot;. Om du tillät att välja flera poster i fältet&quot;Produkt&quot; kan du välja Produkt 1 med en budget på 120 000 och Produkt 2 med en budget på 100 000 USD. Du kan visa följande budgetinformation i det länkade fältet från den ursprungliga posten, beroende på vilken aggregator du väljer:
   >
   >* **Ingen**: 120 000 dollar, 100 000 dollar
   >* **MAX**: 120 000 dollar
   >* **MIN**: 100 000 dollar
   >* **SUM**: 220 000 dollar
   >* **AVG**: 110 000 dollar
   >

1. (Valfritt) Använd **sök** icon ![](assets/search-icon.png) om du vill söka efter ett fält.

1. Klicka **Lägg till fält** för att spara ändringarna.

   Följande objekt läggs till:

   * Det länkade postfältet som visar posterna från den länkade posttypen efter att du har lagt till dem manuellt. Namnet på det länkade postfältet är det namn du valde i steg 5. <!--accurate-->

   * Det eller de länkade fält som visar information från fälten för den länkade posttypen efter att du manuellt har lagt till posterna i det länkade postfältet. De länkade fälten skapas endast när **Välj sökfält** inställningen är markerad när anslutningen skapas. De länkade fälten namnges enligt det här mönstret:

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

   * När du länkar Maestro-posttyper till varandra läggs ett länkat postfält till i den posttyp som du länkar till . Namnet på det länkade postfältet på den länkade posttypen är namnet på den posttyp som du länkar från.

     Om du t.ex. länkar posttypen &quot;Produkt&quot; från posttypen &quot;Kampanj&quot; och namnger det anslutna fältet för Campaign &quot;Länkad produkt&quot;, skapas ett &quot;Kampanjlänkat&quot; postfält för posttypen Produkt.

1. (Valfritt) Klicka på nedåtpilen i huvudet för de länkade postfälten i den ursprungliga posttypen eller i tabellvyn för den länkade posttypen och klicka sedan på något av följande:

   * **Redigera fält**: Du kan bara uppdatera **Namn** och **Beskrivning** information om fältet.
   * **Redigera sökfält**: Lägg till eller ta bort fält för den länkade posten.

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   Följ instruktionerna i steg 9-13 ovan för att lägga till eller ta bort uppslagsfält. <!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > Du kan inte lägga till sökfälten för den post som du länkar från till den länkade posttypen som anger ett objekt i ett tredjepartsprogram.
   >
   > Du kan till exempel inte lägga till sökfältet för ett Campaign-maestro-objekt från det länkade fältet Campaign som visas i posttypen Maestro-projekt när du länkar till Workfront-projekt.


1. (Valfritt) Klicka på nedåtpilen i huvudet på det länkade postfältet från den posttyp som du länkar från och klicka sedan på **Ta bort**.

   Postfältet och eventuella ytterligare länkade sökfält tas bort och fälten och deras information kan inte återställas.

   >[!TIP]
   >
   >    Det länkade postfältet för den posttyp som du länkar till tas inte bort. <!-- is this still accurate?! -->

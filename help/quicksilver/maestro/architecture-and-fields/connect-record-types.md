---
title: Koppla posttyper
description: Ett sätt att ange hur enskilda posttyper relaterar till varandra är att koppla dem. Du kan även koppla Maestro-posttyper till objekttyper från andra program för att förbättra användarupplevelsen och behålla fokus i ett program.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '1739'
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
>Informationen i den här artikeln handlar om Adobe Maestro, ett nytt erbjudande från Adobe.
>
>För närvarande ingår Adobe Maestro i ett betaprogram som är öppet för ett begränsat antal kunder.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.
>
>Mer information finns i [Adobe Maestro - översikt](../maestro-overview.md).

Du kan använda Adobe Maestro för att utforma anpassningsbara arbetsytor som innehåller de posttyper som behövs i organisationen. Ett sätt att ange hur enskilda posttyper relaterar till varandra är att koppla dem. Du kan även koppla Maestro-posttyper till objekttyper från andra program för att förbättra användarupplevelsen och behålla fokus i ett program.

Du kan ansluta följande:

* Posttyper för operationsmaestro
* Posttyper för maestro-operationer till taxonomiposttyper
* Magnettaxonomityper till driftsposttyper
* Posttyper och objekttyper från andra program.

På så sätt kan du visa fält från den länkade posten eller objekttypen på en annan Maestro-post.

I den här artikeln beskrivs hur du kan koppla två Maestro-posttyper eller en Maestro-posttyp till ett objekt från ett annat program.

När anslutningen mellan post- eller objekttyper har upprättats kan du koppla enskilda poster till varandra.

Mer information om hur du ansluter en Maestro-post till ett objekt från ett annat program finns i [Koppla poster](../records/connect-records.md).

Ett exempel på hur du ansluter posttyper finns i [Exempel på att ansluta posttyper och poster](../architecture-and-fields/example-connect-record-types-and-records.md).

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
   <p> Adobe Workfront</p> </td>
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

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Att tänka på när du ansluter posttyper

* Du kan ansluta följande enheter i Maestro:

   * Två driftsposttyper
   * Två taxonomier
   * En driftsposttyp och en taxonomi
   * En operativ posttyp och en objekttyp från ett annat program.

     >[!TIP]
     >
     >    Du kan inte ansluta en taxonomiposttyp till en operativ posttyp eller till en objekttyp från ett annat program.

* Du kan koppla följande objekt från följande program till posttyper i Maestro:

   * Adobe Workfront:

      * Projekt
      * Portfolio
      * Program
      * Företag
      * Grupper

* När du har kopplat en posttyp till en annan posttyp eller till en objekttyp från ett annat program finns följande scenarier:

   * När du ansluter två posttyper: Ett länkat postfält skapas för den posttyp som du ansluter från. Ett liknande länkat postfält skapas för den posttyp som du ansluter till.

     Om du till exempel ansluter posttypen&quot;Campaign&quot; till posttypen&quot;Product&quot; skapas ett länkat postfält som du kallar&quot;Linked Product&quot; för posttypen Campaign, och en länkad posttyp som automatiskt kallas&quot;Campaign&quot; skapas för posttypen Produkt.

   * När du kopplar ett posttypsfält till en taxonomi: Ett länkat postfält skapas för den posttyp som du ansluter från. Inget länkat postfält skapas i den taxonomi som du ansluter till.

     Om du till exempel kopplar posttypen&quot;Campaign&quot; till posttypen&quot;Audience&quot; skapas ett länkat postfält som du kallar&quot;Linked Audience&quot; i posttypen Campaign. Inget länkat postfält som automatiskt heter Campaign skapas i posttypen Audience taxonomy. <!--this might be temporary-->

   * När du ansluter ett posttypsfält med en objekttyp från ett annat program skapas ett länkat postfält för den posttyp som du ansluter från. Inget länkat postfält skapas automatiskt i Workfront-projektet i Workfront. Ett länkat postfält skapas endast i objekttypen i Workfront när de faktiska objekten är kopplade till Maestro-posterna.

     Mer information finns i [Koppla poster](../records/connect-records.md).

* När du har anslutit posttyperna kan du koppla flera fält från en posttyp till en annan posttyp. Dessa fält kommer att refereras som&quot;länkade fält&quot; eller&quot;sökfält&quot;.
* Länkade postfält föregås av en relationsikon ![](assets/relationship-field-icon.png).
* När du har skapat enskilda poster för en posttyp kan du välja de poster som du ansluter till från det länkade posttypsfältet. Mer information finns i [Koppla poster](../records/connect-records.md).
* Du kan inte redigera informationen i de länkade fälten från den posttyp som du länkar från, eftersom de automatiskt fylls i från den ursprungliga posttypen som de tillhör så fort du markerar de länkade posterna.

## Koppla posttyper

<!--when changes here, also update the article for "Connect records"-->

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-workfront.png) i Workfront övre högra hörn, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> klicka sedan på **Maestro** ![](assets/maestro-icon.png).

   Den senast använda arbetsytan bör öppnas som standard.

1. (Valfritt) Expandera den nedåtriktade pilen till höger om namnet på en befintlig arbetsyta och markera den arbetsyta som du vill koppla posttyper från.
1. Klicka på kortet för en posttyp för att öppna posttypssidan.
1. Klicka på **+** i tabellvyns övre högra hörn och klicka sedan på **Ny anslutning** -fliken.

   ![](assets/new-connection-tab-with-workfront-option.png)
1. I **Posttyp** väljer du något av följande: <!--is the field name spelled right? lowercase "t"?-->

   * En annan operativ posttyp
   * En taxonomi
   * Ett Workfront-projekt, Portfolio, Program, Company eller Group.

   ![](assets/new-connection-tab-fields-with-another-record-selected.png)

   >[!TIP]
   >
   > Det går bara att välja posttyper och taxonomier från den valda arbetsytan.

1. Uppdatera följande information:

   * **Namn**: Namnet på det anslutna fältet, så som det kommer att visas i tabellvyn eller på detaljsidan för den ursprungliga posttypen. Då skapas den länkade postkolumnen i tabellvyn för den ursprungliga posttypen eller det länkade postfältet för de ursprungliga posterna. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->

   >[!TIP]
   >
   >Vi rekommenderar att du tar med namnet på den post som du länkar till i namnet på det anslutna postfältet för att ta reda på vilken posttyp det nya fältet kommer från. Namnet på den länkade posten visas inte i det nya länkade postfältet eller i dess länkade fält.

   * **Beskrivning**: Ytterligare information om det anslutna postfältet. Beskrivningen av ett fält visas när du hovrar över fältets kolumn i en tabell.
   * **Tillåt flera poster**: Välj det här alternativet för att ange att du tillåter att användare kan lägga till flera poster när fältet för länkad posttyp visas på de ursprungliga posterna. Detta är markerat som standard.
   * **Välj sökfält**: Välj det här alternativet om du vill lägga till fält från den valda posttypen. Detta är markerat som standard.

1. Klicka **Skapa**.

1. (Villkorligt) Om du valde inställningen Välj uppslagsfält i föregående steg visas **Lägg till sökfält** öppnas.

   Klicka på **+** ikon för att lägga till fält från **Omarkerade fält** område.

   eller

   Klicka på **-** ikonen för att ta bort fält från **Markerade fält** area

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   >[!NOTE]
   >
   >Om du inte markerar något av fälten visas **Namn** av den länkade posten är det enda synliga fältet i den ursprungliga postens tabellvy. The **Namn** kan inte tas bort.

1. (Valfritt och villkorligt) Om du väljer att länka ett tal, en valuta, en procentandel eller ett datumtypsfält, ska du även välja ett aggregeringsvärde. Värdena för de länkade fälten visas antingen avgränsade med kommatecken eller som ett aggregeringsvärde enligt den aggregator du väljer, när användare markerar mer än en länkad post i det länkade postfältet.

   ![](assets/aggregator-drop-down-for-number-linked-field.png)

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

1. (Valfritt) Klicka på **Hoppa över** om du inte vill lägga till några fält från den anslutna posttypen.

1. Klicka **Lägg till fält** för att spara ändringarna.

   Följande objekt läggs till:

   * Det länkade postfält som visar posterna från den länkade posttypen efter att du har lagt till dem manuellt. Namnet på det länkade postfältet är det namn du valde i steg 6. <!-- ensure this is still accurate-->

   * Det eller de länkade fält som visar information från fälten av den länkade posttypen efter att du manuellt har lagt till posterna i det länkade postfältet. De länkade fälten skapas endast när **Välj sökfält** inställningen är markerad när anslutningen skapas. De länkade fälten namnges enligt det här mönstret:

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

   * Ett länkat postfält på den posttyp som du länkar till. Namnet på det länkade postfältet på den länkade posttypen är namnet på den posttyp som du länkar från.

     Om du t.ex. länkar posttypen &quot;Produkt&quot; från posttypen &quot;Kampanj&quot; och namnger det anslutna fältet för Campaign &quot;Länkad produkt&quot;, skapas ett &quot;Kampanjlänkat&quot; postfält för posttypen Produkt.

1. (Valfritt) Klicka på nedåtpilen i huvudet för de länkade postfälten i den ursprungliga posttypen eller i tabellvyn för den länkade posttypen och klicka sedan på något av följande:

   * **Redigera fält**: Du kan bara uppdatera **Namn** och **Beskrivning** information om fältet.
   * **Redigera sökfält**: Lägg till eller ta bort fält för den länkade posten.

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   Följ instruktionerna i steg 7-12 ovan för att lägga till eller ta bort fält. <!--ensure these step numbers stay accurate-->

1. (Valfritt) Klicka på nedåtpilen i huvudet på det länkade postfältet från den posttyp som du länkar från och klicka sedan på **Ta bort**.

   Postfältet och eventuella ytterligare länkade sökfält tas bort och fälten och deras information kan inte återställas.

   >[!TIP]
   >
   >    Det länkade postfältet för den posttyp som du länkar till tas inte bort. <!-- is this still accurate?! -->

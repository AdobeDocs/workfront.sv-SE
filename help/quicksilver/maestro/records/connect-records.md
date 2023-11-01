---
title: Koppla poster
description: När du har skapat anslutningar mellan posttyper kan du koppla enskilda poster till varandra.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: 1dcc267f04242782efea4a219410380ca5a01e1d
workflow-type: tm+mt
source-wordcount: '1964'
ht-degree: 0%

---

<!--when you make this live, update the metadata above to this: 
---
title: Connect records and objects
description: In addition to connecting Maestro records to one another, you can also connect Maestro records to objects from other applications.  
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->
<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

<!--if you change steps here, also update steps in the "Connect records" article-->

# Koppla poster

>[!IMPORTANT]
>
>Informationen i den här artikeln handlar om Adobe Maestro, ett nytt erbjudande från Adobe.
>
>För närvarande ingår Adobe Maestro i ett betaprogram som är öppet för ett begränsat antal kunder.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.
>
>Mer information finns i [Adobe Maestro - översikt](../maestro-overview.md).

Du kan ansluta Adobe Maestro-poster till varandra eller till objekt från andra program.

Du måste först koppla ihop två posttyper eller en posttyp till en objekttyp från ett annat program, och sedan kan du använda posttypens tabellvy för att koppla poster till varandra eller poster till andra objekt.

Mer information om hur du ansluter posttyper till varandra eller till objekttyper från andra program finns i [Koppla posttyper](../architecture-and-fields/connect-record-types.md).

Ett exempel på hur du ansluter posttyper finns i [Exempel på att ansluta posttyper och poster](../architecture-and-fields/example-connect-record-types-and-records.md).

Du kan ansluta följande:

* Mejsarkiv
* Mejsel operationsregister till taxonomiposter
* Arkiv och objekt från andra program.

  Du kan koppla Maestro-poster till objekt av den typ som listas nedan från följande program:

   * Adobe Workfront

      * Projekt
      * Portfolio
      * Program
      * Företag
      * Grupp

  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto">
 <col>
<tbody>
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
   <td><p>Valfritt, för att skapa Maestro-poster</p> 
<p>Arbeta eller högre för att visa projekt i Workfront</p>
  <p>Mer information finns i <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Översikt över Adobe Workfront-licenser</a>.</p> 
  </td>
  </tr>
  <tr>
   <td role="rowheader">Åtkomstnivå</td>
   <td> <p>Valfritt, för att skapa Maestro-poster</p>
<p>Visa eller ge högre åtkomst till projekt, Portfolio, program</p> 
<p>Ytterligare åtkomst till grupper och företag när användare visar grupper eller företag tillhör de inte</p>   
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Objektbehörigheter</p></td>
   <td> <p>Visa eller ange högre behörighet för de objekt som du vill länka till Maestro-poster  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Systemadministratören måste lägga till Maestro-området i layoutmallen. Mer information finns i <a href="../access/grant-access.md">Ge åtkomst till Adobe Maestro</a>. </p></td>
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

## Koppla poster

### Att tänka på när det gäller att ansluta poster

* När anslutningen mellan posttyperna har upprättats visas de kopplade posttyperna som länkade postfält i tabellen med de posttyper som de är länkade från.
* Du kan bläddra bland och lägga till poster och objekt för den länkade posten och objekttyperna från de länkade postfälten.
* Du kan lägga till fält från de länkade posttyperna i tabellen med den posttyp som du länkar från.
* Du kan inte uppdatera värdena för länkade fält manuellt på de poster som du länkar från.

  Värdena för de länkade fälten från de länkade posterna fyller i den Maestro-post som du länkar från automatiskt.

* Alla som har tillgång till Maestro kan se kopplingarna mellan Maestro-posterna eller mellan Maestro-poster och Workfront-objekt. Du kan även visa och redigera alla andras anslutningar. <!--add that this is based on your permissions in both Maestro and Workfront (or, later, any other application)-->
* Du kan koppla en Maestro-post till ett eller flera objekt från ett annat program.
* Du kan inte ansluta taxonomier till posttyper eller till objekt från ett annat program. <!-- this is temporary; there will be certain objects (teams, etc) that will be linked to taxonomies, per Lilit-->
* Om du vill länka Maestro-poster till Workfront-objekt måste du ha följande:

   * Workfront-objekt. Du måste till exempel först skapa projekt, portföljer, program, företag eller grupper i Workfront.
   * Makroarbetsytor, posttyper och poster. Mer information finns i följande artiklar:

      * [Skapa arbetsytor](../architecture-and-fields/create-workspaces.md)
      * [Skapa posttyper](../architecture-and-fields/create-record-types.md)
      * [Skapa poster](../records/create-records.md)

   * Kopplingar mellan posttyper eller mellan posttyper och objekt från andra program. Mer information finns i [Koppla posttyper](../architecture-and-fields/connect-record-types.md).

### Connect Maestro-poster

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-workfront.png) i det övre högra hörnet av Workfront eller **Huvudmeny** icon ![](assets/main-menu-shell.png)  i det övre vänstra hörnet, om det är tillgängligt, klickar du på **Maestro** ![](assets/maestro-icon.png).

   Den senast använda arbetsytan bör öppnas som standard.

1. (Valfritt) Expandera den nedåtriktade pilen till höger om namnet på en befintlig arbetsyta och markera den arbetsyta som du vill koppla poster från.
1. Klicka på kortet för en posttyp för att öppna posttypssidan.
1. Välj en **Tabell** visa från **Visa** nedrullningsbar meny i det övre högra hörnet på posttypssidan.
1. Lägg till en anslutning till en annan post eller objekttyp från den valda posttypen. Mer information finns i [Koppla posttyper](../architecture-and-fields/connect-record-types.md).

   En ny kolumn läggs till i tabellen för att visa den länkade posttypen.

1. Lägg till poster till den posttyp du valde genom att lägga till en ny rad i tabellen. Mer information finns i [Skapa poster](../../maestro/records/create-records.md).
1. Gå till kolumnen för den länkade posten från en post som visas i tabellvyn och hovra över cellen för den post som du vill länka till andra Maestro-poster. Klicka sedan på **+** -ikon.

   The **Koppla objekt** visas.

   ![](assets/connected-objects-table-for-records.png)

1. Börja skriva namnet på en post i sökrutan och markera den när den visas i listan

   eller

   Markera namnet på en eller flera poster i rutan och klicka sedan på **Koppla objekt** i det övre högra hörnet av rutan Anslut objekt.

   Följande ska läggas till:

   * De länkade posterna visas i det länkade postfältet för den post som du valde i steg 3. När du uppdaterar de länkade posterna uppdateras automatiskt de länkade postfälten för de poster som du länkar från. <!--ensure the number of the step stays accurate-->
   * De länkade fält som tillhör de länkade posterna fylls automatiskt i med informationen från de ursprungliga länkade posterna. Du kan inte redigera länkade fält manuellt.

     >[!TIP]
     >
     >* Vi använder länkade fält och sökfält omväxlande.
     >
     >* Om du har aktiverat inställningen Tillåt flera poster när du har anslutit posttyperna, visas fältvärdena för de flera markerade objekten antingen separerade med kommatecken eller aggregeras enligt den aggregator du har valt.

1. (Valfritt) Stäng sidan för posttypen Maestro och gå till den arbetsyta du valde.
1. Klicka på kortet för den posttyp som du länkade till.

   Om du till exempel har anslutit Campaign-posten till produktposten klickar du på **Produkt** kort.

   Posttypkortet ska öppnas i tabellvyn.

   Observera att det länkade postfältet för Campaign visar namnen på de kampanjer som du länkade till produkter på sidan Produktposttyp. Om du uppdaterar Campaign-informationen uppdateras automatiskt det Campaign-länkade postfältet för produktposttypen.

### Koppla Maestro-poster till Workfront-objekt

<!--when we will have more applications to link to from Maestro, change the title to soemthing like: Connect Maestro records to objects from other applications-->

När du har skapat en anslutning mellan en Maestro-posttyp och en Workfront-objekttyp kan du koppla enskilda Maestro-poster till objekt i Workfront. Du kan också koppla fält från Workfront-objektet till Maestro-posttypen.

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-workfront.png) i det övre högra hörnet av Workfront eller **Huvudmeny** icon ![](assets/main-menu-shell.png)  i det övre vänstra hörnet, om det är tillgängligt, klickar du på **Maestro** ![](assets/maestro-icon.png).

   Den senast använda arbetsytan bör öppnas som standard.

1. (Valfritt) Expandera den nedåtriktade pilen till höger om namnet på en befintlig arbetsyta och markera den arbetsyta som du vill koppla poster från.
1. Klicka på kortet för en posttyp för att öppna posttypssidan.
1. Välj en tabellvy på menyn **Visa** nedrullningsbar meny i det övre högra hörnet på posttypssidan.
1. Lägg till en ny anslutning till en objekttyp från Workfront för den valda posttypen. Välj bland följande objekt under avsnittet Workfront:

   * Projekt
   * Portfolio
   * Program
   * Företag
   * Grupp

   Mer information finns i [Koppla posttyper](../architecture-and-fields/connect-record-types.md).

   En ny kolumn läggs till i tabellen för att visa den länkade objekttypen.

1. Lägg till enskilda poster till den posttyp du valde genom att lägga till en ny rad i tabellen. Mer information finns i [Skapa poster](../../maestro/records/create-records.md).
1. Gå till kolumnen för det länkade objektet från en post som visas i tabellvyn och hovra över cellen för den post som du vill länka till andra objekt från Workfront. Klicka sedan på **+** -ikon. <!--change Workfront to other applications, when this will be possible-->

   The **Koppla objekt** visas.

   ![](assets/connect-objects-box-to-select-projects.png)

1. Börja skriva namnet på ett Workfront-objekt i sökrutan och markera det sedan när det visas i listan

   eller

   Markera namnet på ett eller flera objekt i rutan och klicka sedan på **Koppla objekt** i det övre högra hörnet av rutan Anslut objekt.

   Följande har lagts till i Maestro:

   * De markerade Workfront-objekten läggs till i det länkade postfältet.
   * Ett nytt länkat fält (eller ett uppslagsfält) skapas för varje länkat fält som du markerade när du lade till fälten i den länkade posten.
   * En ny posttyp med namnet&quot;Workfront-objekt&quot; skapas på samma arbetsyta som den maestro-post som du länkar från. Objektets namn är en del av den här posttypens namn. Om du till exempel länkar till Workfront-projekt skapas Workfront projekttyp i Maestro.

     Detta är en skrivskyddad posttyp och visar Workfront-objekt som är markerade i det nya länkade objektfältet som du skapade från Maestro-posten. De länkade fälten för det länkade objektet visas även på de skrivskyddade länkade Workfront-posterna.

     >[!IMPORTANT]
     >
     > Den skrivskyddade posttypen för Workfront-objekt skapas bara när enskilda projekt läggs till i Maestro-poster. Workfront-posttypen skapas inte om du skapar en anslutning mellan en Maestro-posttyp och en Workfront-objekttyp.

     All befintlig information från fälten i Workfront-objekten visas i de länkade fälten eller sökfälten.

     >[!TIP]
     >
     >
     >* Om du har aktiverat inställningen Tillåt flera poster visas värdena för de olika objekten antingen avgränsade med kommatecken eller aggregeras enligt den aggregator du har valt.
     >
     >* Ett länkat postfält till de länkade dataposterna skapas inte för de länkade Workfront-objekten.


1. (Valfritt) Stäng sidan för posttypen Maestro och gå till den arbetsyta du valde.
1. Klicka på kortet för posttypen för Workfront-objekt. Klicka till exempel på **Workfront-projekt** om du har länkat till Workfront-projekt. Skrivskyddat posttypskort för Workfront ska öppnas i tabellvyn.

   >[!NOTE]
   >
   >    * Posterna som visas på posttypssidan i Workfront är skrivskyddade Workfront-objekt. De fält som är länkade från posttypen för Workfront visas också som skrivskyddade kolumner, och de fylls i automatiskt när de fylls i i Workfront.
   >    * Du kan inte uppdatera Workfront-fält manuellt i Maestro. Workfront objektfält måste fyllas i i Workfront och fältvärdena visas automatiskt på Workfront-posten i Maestro.
   >
   >    * Om du vill visa posttypen för Workfront-objektet i tidslinjevyn måste det finnas minst två datumfält i tabellvyn på den skrivskyddade Workfront-posttypsidan.

1. (Valfritt) Gör något av följande om du vill öppna Workfront objektpostinformationssida i Maestro:

   * Gå till det länkade postfältet för Workfront-objektet från den posttyp du länkade från och klicka på namnet på Workfront-objektet.
   * Från **Tabell** vy över posttypssidan för Workfront, klicka på namnet på Workfront-objektet

     eller

     Klicka på **Mer** till höger om Workfront-objektnamnet och klicka sedan på **Visa**.

     ![](assets/workfront-object-more-menu-in-table-with-go-to-source-link.png)

   Då öppnas sidan Maestro Details (Maestro-information) för det länkade Workfront-objektet. Det här är en skrivskyddad sida.

1. (Valfritt) Gör något av följande om du vill öppna det länkade Workfront-objektet i Workfront:

   * Från **Tabell** visa Workfront posttypsida, klicka på namnet på Workfront-objektet,

   eller

   Klicka på **Mer** till höger om Workfront-objektnamnet och klicka sedan på **Gå till källa**.

   ![](assets/workfront-project-maestro-details-page-with-go-to-source-link.png)

   Då öppnas Workfront objektsida. Du kan redigera information om Workfront-objektet om du har behörighet att göra det.

1. (Valfritt) Klicka på **Lägg till fält** icon ![](assets/add-fields-icon.png) i tabellvyns övre högra hörn på posttypssidan för Workfront om du vill lägga till eller ta bort Workfront-fält från posttypen för Workfront.

   >[!NOTE]
   >
   >  De fält som du lägger till eller tar bort på Workfront objektposttypsida läggs inte till och tas inte bort från Maestro-posttypen som länkar till Workfront-objekttypen. Fälten visas bara på den skrivskyddade posttypssidan för Workfront, så du kan granska dem i Maestro.

1. (Valfritt och villkorligt) Om du har lagt till minst två datumfält i Workfront-objektet klickar du på **Visa** nedrullningsbar meny på posttypssidan för Workfront-objekt och välj **Tidslinje** vy. De länkade Workfront-objekten visas i tidslinjevyn.

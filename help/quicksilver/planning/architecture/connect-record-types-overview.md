---
title: Översikt över posttyper för anslutning
description: Ett sätt att ange hur enskilda posttyper relaterar till varandra är att koppla dem. Du kan även koppla posttyperna Adobe Workfront Planning till objekttyper från andra program för att förbättra användarupplevelsen och behålla fokus i ett program.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: d5d517a0c9a1292c37e66db07f7ed17d0a9a59e1
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 0%

---


<!--update metadata at GA-->
<!--add mini TOC when live, already added to big TOC to get the link-->

# Översikt över posttyper för anslutning

<!--REMOVE THE CONTENT BELOW FROM THE "CONNECT RECORD TYPES" ARTICLE WHEN YOU TURN THIS ARTICLE LIVE- THIS IS THE SAME CONTENT AS THERE, DUPLICATED-->

Du kan ange att enskilda posttyper relaterar till varandra eller till objekt från andra program genom att koppla dem.

Den här artikeln innehåller en översikt över hur posttyper ansluter och beskriver de typer av anslutningar som du kan upprätta mellan post- och objekttyper.

Mer information om hur du ansluter posttyper finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).

## Att tänka på när du ansluter posttyper

* Du kan ansluta följande enheter i Adobe Workfront Planning:

   * Två posttyper

     Posttyperna måste tillhöra samma arbetsyta.
   * En posttyp och en objekttyp från ett annat program.

* Du kan koppla posttyper för Workfront Planning till följande objekttyper från följande program:

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
     >Du måste ha en Adobe Experience Manager Assets-licens och din organisations instans av Workfront måste vara registrerad på Adobe Business Platform eller Adobe Admin Console för att kunna ansluta Workfront Planning-poster till Adobe Experience Manager Assets.
     >
     >Om du har frågor om hur du kommer igång med Adobe Admin Console kan du läsa [Adobe Unified Experience FAQ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* När du har skapat enskilda poster för en posttyp kan du välja de poster som du ansluter till från det länkade posttypsfältet. Mer information finns i [Anslut poster](/help/quicksilver/planning/records/connect-records.md).

* När du har kopplat en posttyp till en annan posttyp eller till en objekttyp från ett annat program finns följande scenarier:

   * **När du ansluter två posttyper**: Ett länkat postfält skapas för den posttyp som du ansluter från. Ett liknande länkat postfält skapas för den posttyp som du ansluter till.

     Om du till exempel kopplar posttypen&quot;Campaign&quot; till posttypen&quot;Product&quot; skapas ett länkat postfält som du kallar&quot;Linked Product&quot; i posttypen Campaign. En länkad posttyp som automatiskt heter&quot;Campaign&quot; skapas på produktposttypen.

   * **När du ansluter en posttyp med en objekttyp från ett annat program**:

      * Ett länkat postfält skapas för den posttyp som du ansluter från. Inget länkat postfält skapas automatiskt i det andra programmets objekttyp.

      * Planeringspostfält är inte tillgängliga från Workfront-objekt.
      * Du kan planera postfält från Experience Manager-resurser när Workfront-administratören konfigurerar metadatamappningen genom integrationen mellan Workfront och Adobe Experience Manager Assets. Mer information finns i [Konfigurera mappning av metadata för resurser mellan Adobe Workfront och Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).

   * **När du lägger till länkade (eller uppslag) fält från posten eller objektet som du ansluter till**: Ett länkat (eller uppslagsfält) med information från posten som du ansluter till visas på posten som du ansluter från.

     Du kan koppla fält från andra posttyper eller objekt från andra program till posttypen Workfront Planning.

     Länkade fält är skrivskyddade och visar automatiskt information från kopplade poster eller objekt när du kopplar posterna eller objekten.

     Om du t.ex. kopplar posttypen&quot;Campaign&quot; till ett Workfront-projekt och väljer att överföra fältet Planerat slutförandedatum för projektet till Workfront Planning-posten, skapas automatiskt ett länkat fält med namnet Planerat slutförandedatum (från projekt) för kampanjen. Du kan inte redigera det här länkade fältet manuellt. I fältet Planerat slutförandedatum (från projekt) visas det planerade slutförandedatumet för de länkade projekten.

     >[!IMPORTANT]
     >
     >Alla som har behörighet att visa eller högre på arbetsytan kan visa informationen i de länkade fälten, oavsett behörighet eller åtkomstnivå i programmet för de länkade objekttyperna.

* Länkade postfält föregås av en relationsikon ![](assets/relationship-field-icon.png).

  Länkade fält föregås av en ikon som anger fälttypen. Länkade (eller uppslag) fält föregås av ikoner som anger att ett fält är ett tal, ett stycke eller ett datum.

* Uppslagsfält föregås av en ikon som anger vilken typ av information som visas i fältet.

## Anslutningstyper

När du har upprättat en anslutning mellan två posttyper eller mellan en post och en objekttyp från ett annat program, kan du lägga till poster i de anslutna postfälten.

Beroende på hur många poster du kan lägga till i en anslutning kan du välja mellan följande anslutningstyper vid anslutning av posttyper:

* [En till många](#one-to-many-connection-type)
* [En till en](#many-to-one-connection-type)
* [Många till ett](#many-to-one-connection-type)
* [Många till många](#many-to-many-connection-type)

<!-- add screen shots for each type of connection below-->

### Anslutningstyp en till många

När du väljer en-till-många-anslutningstyp mellan posttyper kan du senare ansluta en post med flera poster som du ansluter till.

Om ni till exempel kopplar ihop kampanjer med projekt kan ni koppla samman en kampanj med flera projekt. Men ett projekt kan bara kopplas till en kampanj.

När du väljer den här anslutningstypen kan du senare bara ändra den till en många-till-många-anslutningstyp.

### En-till-en-anslutningstyp

När du väljer en-till-en-anslutningstyp mellan posttyper kan du senare ansluta en post med en annan post som du ansluter till.

Om ni till exempel kopplar ihop kampanjer med projekt kan ni koppla samman en kampanj med ett projekt. Ett projekt kan bara kopplas till en kampanj.

När du väljer den här anslutningstypen kan du ändra den senare till en annan anslutningstyp.

### Anslutningstyp för många-till-ett

När du väljer anslutningstypen många-till-en mellan posttyper kan du senare ansluta många poster med bara en post som du ansluter till.

Om ni till exempel kopplar ihop kampanjer med projekt kan ni koppla samman flera kampanjer med ett projekt. Ett projekt kan kopplas till flera kampanjer.

När du väljer den här anslutningstypen kan du senare bara ändra den till en många-till-många-anslutningstyp.

### Anslutningstyp för många-till-många

När du väljer anslutningstypen många-till-många mellan posttyper kan du senare ansluta många poster med flera poster som du ansluter till.

Om ni till exempel kopplar ihop kampanjer med projekt kan ni koppla samman flera kampanjer med flera projekt. Du kan också koppla samman flera projekt med flera kampanjer.

När du väljer den här anslutningstypen kan du inte ändra anslutningstypen efter att du har sparat den.
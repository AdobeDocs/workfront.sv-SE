---
title: Översikt över anslutna poster
description: När du har skapat anslutningar mellan posttyper kan du koppla enskilda poster till varandra. I den här artikeln beskrivs överväganden som du måste ta hänsyn till när du ansluter poster i Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: d56a4721353f8b7db856eab5a3ae3b53396bd079
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---


<!--update metadata at GA-->

# Översikt över anslutna poster

{{planning-important-intro}}

Du kan ansluta Adobe Workfront Planning-poster till varandra eller till objekt från andra program.

I den här artikeln beskrivs överväganden som du måste ta hänsyn till när du ansluter poster i Adobe Workfront Planning.

Mer information om hur du kan ansluta poster till varandra eller till ett annat objekt finns i [Koppla poster](/help/quicksilver/planning/records/connect-records.md).


## Att tänka på när det gäller att ansluta poster

* När du har anslutit posttyper visas de kopplade posttyperna som länkade postfält i tabellen med de posttyper som de är länkade från och på posternas sidor.
* Du kan bläddra bland och lägga till poster och objekt för den länkade posten och objekttyperna från de länkade postfälten.
* Du kan lägga till fält (sökfält) för de länkade posttyperna i tabellen med den posttyp som du länkar från.

  Du kan lägga till fält (uppslagsfält) för de posttyper som du länkar från i tabellen med den posttyp som du länkar till.

  Om du till exempel länkar posttypen för Produkt från posttypen för Campaign kan du visa produktfält för kampanjer samt kampanjfält för Produkter.
* Du kan inte uppdatera värdena för uppslagsfält manuellt på de poster som du länkar från.

  Värdena för sökfälten fyller i den Workfront Planning-post som du länkar från automatiskt när de har uppdaterats på den ursprungliga posten eller objektet.

* Alla som har åtkomst till Workfront Planning och View eller högre behörighet till arbetsytan kan se anslutningarna mellan posterna eller mellan poster och andra programobjekt. De kan visa anslutna poster och objekt oavsett deras behörigheter i de program du ansluter till.
* Du kan visa och redigera alla andras anslutningar om du har behörigheten Hantera på arbetsytan där de anslutna posterna finns.
* Du kan koppla en post till ett eller flera objekt från ett annat program. <!--For more information, see the "Connections types" section in the article [Connected record types overview](/help/quicksilver/planning/architecture/connect-record-types-overview.md). -->

## Områden där du kan koppla poster

Du kan koppla poster till andra poster eller till objekt från andra program i följande områden:

* Du kan koppla poster från Workfront Planning till Workfront-objekt inom följande områden:
   * Från en planeringspost i Workfront Planning i de anslutna fälten i tabellvyn.
   * Från en planeringspost i Workfront Planning i postförhandsgranskningen eller på sidan i de anslutna postfälten.
  <!--
  * From a Planning record in Workfront Planning in the record preview or page in the connected record fields on the Details tab.
  * From a Planning record in the record's preview or page on the Connections tab.  -->

* Du kan ansluta Workfront Planning-poster till Experience Manager Assets inom följande områden:

   * Från en planeringspost i Workfront Planning i tabellvyn.
  <!--* From a Planning record in the Connections tab on the record's preview or page.  -->

* Du kan koppla Workfront-objekt till Workfront Planning-poster i följande områden:

   * Under Planning för ett Workfront-objekt.


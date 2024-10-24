---
title: Översikt över anslutna poster
description: När du har skapat anslutningar mellan posttyper kan du koppla enskilda poster till varandra. I den här artikeln beskrivs överväganden som du måste ta hänsyn till när du ansluter poster i Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: be51023c-8e11-42e7-aa4f-34484c30eb03
source-git-commit: e82cf1b586ea3b08f419802bd1e88c6567b61b95
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 0%

---

# Översikt över anslutna poster

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

{{planning-important-intro}}

Du kan ansluta Adobe Workfront Planning-poster till varandra eller till objekt från andra program.

I den här artikeln beskrivs överväganden som du måste ta hänsyn till när du ansluter poster i Adobe Workfront Planning.

Mer information om hur du kan ansluta poster till varandra eller till ett annat objekt finns i [Koppla poster](/help/quicksilver/planning/records/connect-records.md).


## Att tänka på när det gäller att ansluta poster

* När du har anslutit posttyper visas de kopplade posttyperna som länkade postfält i tabellen med de posttyper som de är länkade från och på posternas sidor.
* Du kan bläddra bland och lägga till poster och objekt för den länkade posten och objekttyperna från de länkade postfälten.
* Du kan lägga till fält (sökfält) för de länkade posttyperna i tabellen med den posttyp som du länkar från.

  Du kan också lägga till fält (uppslagsfält) för de posttyper som du länkar från i tabellen med den posttyp som du länkar till.

  Om du till exempel länkar posttypen för Produkt från posttypen för Campaign kan du visa produktfält för kampanjer samt kampanjfält för produkter.
* Du kan inte uppdatera värdena för uppslagsfält manuellt på de poster som du länkar från.

  Värdena för sökfälten fyller i den Workfront Planning-post som du länkar från automatiskt när de har uppdaterats på den ursprungliga posten eller objektet.

* Alla som har åtkomst till Workfront Planning och View eller högre behörighet till arbetsytan kan se anslutningarna mellan posterna eller mellan poster och andra programobjekt. De kan visa anslutna poster och objekt oavsett deras behörigheter i de program du ansluter till.
* Du kan visa och redigera alla andras anslutningar om du har behörigheten Hantera på arbetsytan där de anslutna posterna finns.
* Du kan koppla en post till ett eller flera objekt från ett annat program. Mer information finns i avsnittet Anslutningstyper i artikeln [Översikt över anslutna posttyper](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Områden där du kan koppla poster

Du kan koppla poster till andra poster eller till objekt från andra program i följande områden:

* Du kan koppla poster från Workfront Planning till Workfront-objekt eller Experience Manager Assets-objekt i följande områden i en Planning-post:

   * De kopplade postfälten i tabellvyn för en posttyp i Planning.
   * Postens förhandsgranskning eller sida i de anslutna postfälten på fliken Information.
   * Postens förhandsgranskning eller sida på fliken Anslutningar.

* Du kan koppla Workfront-objekt till Workfront Planning-poster i följande områden:

   * Under Planning för ett Workfront-objekt.
   * <span class="preview">Från ett Planning-anslutningsfält på ett Workfront-objekts anpassade formulär. </span>

  Mer information finns i [Hantera postanslutningar från Workfront-objekt](/help/quicksilver/planning/records/manage-records-in-planning-section.md)
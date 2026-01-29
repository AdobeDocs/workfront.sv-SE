---
title: Översikt över anslutna poster
description: När du har skapat anslutningar mellan posttyper kan du koppla enskilda poster till varandra. I den här artikeln beskrivs överväganden som du måste ta hänsyn till när du ansluter poster i Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: be51023c-8e11-42e7-aa4f-34484c30eb03
source-git-commit: 11d856aeee3bd9edcdc1dbca3964f37bdf83bd00
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---

# Översikt över anslutna poster

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->

{{planning-important-intro}}

Du kan ansluta Adobe Workfront Planning-poster till varandra eller till objekt från andra program.

I den här artikeln beskrivs överväganden som du måste ta hänsyn till när du ansluter poster i Workfront Planning.

Mer information om hur du kan ansluta poster till varandra eller till ett annat objekt finns i [Koppla poster](/help/quicksilver/planning/records/connect-records.md).

## Förutsättningar

Du måste ansluta följande innan du kan ansluta poster i Workfront Planning:

* Två posttyper
* En posttyp med ett objekt från ett annat program

Mer information finns i [Översikt över anslutna posttyper](/help/quicksilver/planning/architecture/connect-record-types-overview.md).


## Att tänka på när det gäller att ansluta poster

* När du har anslutit posttyper visas de anslutna posttyperna som anslutningsfält i tabellen med de posttyper som de är länkade från och på posternas sidor.
* Du kan bläddra bland och lägga till poster och objekt för den länkade posten och objekttyperna från de länkade postfälten.
* Du kan lägga till fält (sökfält) för de länkade posttyperna i tabellen med den posttyp som du länkar från.

  Du kan också lägga till fält (uppslagsfält) för de posttyper som du länkar från i tabellen med den posttyp som du länkar till.

  Om du till exempel länkar posttypen för Produkt från posttypen för Campaign kan du visa produktfält för kampanjer samt kampanjfält för produkter.
* Du kan inte uppdatera värdena för uppslagsfält manuellt på de poster som du länkar från.

  Värdena för sökfälten fyller i den Workfront Planning-post som du länkar från automatiskt när de har uppdaterats på den ursprungliga posten eller objektet.

* Alla som har åtkomst till Workfront Planning och View eller högre behörighet till arbetsytan och en posttyp kan se anslutningarna mellan posterna eller mellan poster och andra programs objekt. De kan visa anslutna poster och objekt oavsett deras behörigheter i de program du ansluter till.
* Du kan visa och redigera alla andras anslutningar om du har behörigheten Hantera på arbetsytan och posttypen där de anslutna posterna finns.
* Du kan ansluta en post till en eller flera objekt från ett annat program, beroende på vilken typ av anslutning du valde när du kopplade posttyperna. Mer information finns i avsnittet Anslutningstyper i artikeln [Översikt över anslutna posttyper](/help/quicksilver/planning/architecture/connect-record-types-overview.md).
* När anslutna posttyper ingår i hierarkier kan du komma åt alla objekttyper i hierarkin från posternas sidor. Mer information finns i [Översikt över hierarki och vägbeskrivningar](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).
* När anslutna posttyper ingår i hierarkier kan du koppla en post från en underordnad posttyp till upp till 10 poster från en överordnad posttyp. Mer information finns i [Översikt över hierarki och vägbeskrivningar](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

## Områden där du kan koppla poster

Du kan koppla poster manuellt eller automatiskt i Workfront.

### Koppla poster manuellt

Du kan koppla poster till andra poster eller till objekt från andra program manuellt i följande områden:

* Du kan koppla poster från Workfront Planning till Workfront-objekt, Experience Manager Assets-objekt eller GenStudio Brands i följande områden i en Planning-post:

   * De kopplade postfälten i tabellvyn för en posttyp i Planning.
   * De kopplade postfälten på en posts förhandsgransknings- eller informationssida.
   * Postens förhandsgransknings- eller informationssida på sidan Anslutna poster i en post.

* Du kan ansluta Workfront-objekt till Workfront Planning-poster i följande områden i Workfront:

   * Planeringsdelen av ett Workfront-objekt.
   * Ett Planning-anslutningsfält i ett Workfront-objekts anpassade formulär.

  Mer information finns i [Hantera postanslutningar från Workfront-objekt](/help/quicksilver/planning/records/manage-records-in-planning-section.md).

### Koppla ihop poster automatiskt

När du har kopplat posttyper till varandra eller en posttyp till en objekttyp från ett annat program kan du automatiskt koppla poster och objekt på följande sätt:

* Använda automatisering

  Du kan skapa poster eller Workfront-objekt från en planeringspost där du konfigurerar automatisering.

  När ett villkor som du definierar uppfylls skapas en post eller ett objekt och den ansluts automatiskt till den post som du utlöser automatiseringen från.

  Mer information finns i [Konfigurera Adobe Workfront Planning Automations](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

* Skapa poster med hjälp av frågeformulär

  Du kan skapa poster när du skickar en planeringsförfrågan. Begäran och posten kopplas automatiskt samman.

  >[!NOTE]
  >
  >Du kan inte koppla bort en post från den ursprungliga begäran.

  Mer information finns i [Skicka Adobe Workfront Planning-begäranden för att skapa poster](/help/quicksilver/planning/requests/submit-requests.md).

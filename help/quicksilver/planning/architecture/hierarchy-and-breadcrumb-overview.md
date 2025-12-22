---
title: Översikt över hierarki och vägbeskrivningar
description: Du kan skapa flera arbetsytehierarkier mellan posttyperna på en arbetsyta.
hide: true
hidefromtoc: true
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '887'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Hierarchy and Breadcrumb Overview
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---
-->

# Översikt över hierarki och vägbeskrivningar

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Som arbetsytehanterare kan du definiera flexibla men strukturerade hierarkier mellan posttyper och andra objekttyper i Adobe Workfront Planning.

Hierarkier är anslutningar mellan posttyper eller mellan posttyper och ett Workfront-projekt.

Mer information om hur du skapar hierarkier finns i [Skapa arbetsytehierarkier](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).

Nedan följer några fördelar med att använda hierarkier i dina arbetsytor:

* Organisera arbetet på ett sätt som återspeglar hur era team faktiskt planerar, arbetar och levererar.
* För att användarna ska förstå var de är, hur posttyperna ansluter och hur strategin flödar in i körningen genom att referera till en uppsättning vägbeskrivningar som anger deras plats i systemet.
* För att ge bättre navigering och skapa tydlighet och kontinuitet i alla arbetsflöden.
* För att definiera flöden som passar hur organisationen fungerar, med stöd för både flexibilitet och konsekvens i alla arbetsfaser.

## Att tänka på när du arbetar med hierarkier

* Du kan skapa flera hierarkier för en arbetsyta.
* Du kan ha upp till fyra post- och objekttyper anslutna i en hierarki.
* Du kan bara ansluta följande objekttyper i en arbetsytehierarki:
   * Posttyper som tillhör den arbetsyta som du skapar hierarkierna i.
   * Workfront-projekt. Det går inte att lägga till Workfront-projekt som överordnade för andra posttyper. De är alltid den sista objekttypen i en hierarki.
* Du kan inte lägga till följande objekttyper i en hierarki:
   * Posttyper från andra arbetsytor, även när de är inställda som kopplingsbara eller globala posttyper. Du kan bara lägga till globala posttyper i hierarkier när de har lagts till på arbetsytan som du skapar hierarkin från.
   * Alla andra Workfront-objekt.
   * AEM Assets.
* Hierarkier kan innehålla både Planning-posttyper och Workfront-projekt samtidigt.

      Du kan till exempel ha en Campaign-posttyp med Planning Tactics och Workfront Projects som underordnade i samma arbetsytehierarki.
  * Om det redan finns en anslutning mellan de valda posttyperna återanvänds den befintliga anslutningen.
* Om det inte finns någon anslutning skapar Workfront en sådan i hierarkiinställningarna.
* Inställningen **Skapa motsvarande fält för den länkade posttypen** måste aktiveras för det anslutna fältet för poster och objekttyper som du vill ta med i en hierarki.
* Följande är regler för hierarkiinställningar:
   * En posttyp kan bara ha en överordnad posttyp på en angiven arbetsyta.

     En taktisk posttyp kan till exempel inte ha både en Campaign- och en målobjekttyp som överordnad på samma arbetsyta.
   * En posttyp kan vara överordnad i flera hierarkier.

     Du kan till exempel ha tre olika hierarkier på en arbetsyta, och var och en av dem kan ha kampanjer som överordnad posttyp.
   * En post kan kopplas till flera överordnade poster av samma typ när du kopplar en till många eller flera posttyper.

     Taktik A kan till exempel tillhöra både Campaign X och Campaign Y.
   * En posttyp kan bara ansluta till en underordnad posttyp åt gången. En underordnad posttyp kan också vara överordnad en annan posttyp.

     En Campaign-posttyp kan till exempel vara överordnad till endast en annan posttyp i samma hierarki (Tactics), och Tactics kan i sin tur vara överordnad Program som kan vara överordnad till Projekt.
   * En posttyp kan inte vara överordnad i en hierarki och underordnad i en annan hierarki i samma arbetsyta.
   * Globala posttyper kan visas i flera arbetsytor i flera hierarkier efter att de har lagts till på dessa arbetsytor.

     Om en Campaign till exempel är en global posttyp och en del av en hierarki i Workspace 1, kan den läggas till som en befintlig posttyp i Workspace 2 och ingå i en hierarki där. Men den kan inte ingå i en hierarki i Workspace 2 endast när den har angetts som en global posttyp i Workspace 1, men inte läggas till i Workspace 2.

## Att tänka på när du visar vägbeskrivningar

<!-- this might be incomplete, because I have no UI for this yet-->

När du skapar hierarkier mellan posttyper genereras vägbeskrivningar för poster som tillhör de posttyperna.

Om du t.ex. skapar en hierarki och kopplar ihop kampanjer med taktik, sedan med Aktiviteter, och sedan med Projekt, när du navigerar till en post av någon av de typer som är kopplade till hierarkin, kan du visa var i hierarkin posten placeras.

Tänk på följande:

* Om en posttyp ingår i flera hierarkier kan du växla mellan hierarkier från postens vägbeskrivningar på postens sida.
* Brödraperier fungerar i Workfront och Planning.

  Om du till exempel tittar på ett projekt som är kopplat till Planering-kampanjer och taktik, och även till Workfront portfolior och program, kan du växla mellan både Planning och Workfront objekttyper från den stora mängden.

  Mer information finns i [Skapa arbetsytehierarkier](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).
* När du redigerar en post visas ändringarna från alla arbetsytor och alla hierarkier som posten är en del av.



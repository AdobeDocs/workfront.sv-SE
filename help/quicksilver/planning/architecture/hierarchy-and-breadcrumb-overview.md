---
title: Översikt över hierarki och vägbeskrivningar
description: Du kan skapa flera arbetsytehierarkier mellan posttyperna på en arbetsyta.
hide: true
hidefromtoc: true
source-git-commit: 1f1db1c9184a6a8a2abcd3139e4e4e61d2f08bc4
workflow-type: tm+mt
source-wordcount: '612'
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

Som arbetsytehanterare kan du definiera flexibla men strukturerade hierarkier mellan posttyper och andra objekttyper i Adobe Workfront Planning.

Hierarkier är anslutningar mellan posttyper. Du kan ha upp till fyra post- och objekttyper anslutna i en hierarki.

Mer information om hur du skapar hierarkier finns i [Skapa arbetsytehierarkier](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).

Nedan följer några fördelar med att använda hierarkier i dina arbetsytor:

* Organisera arbetet på ett sätt som återspeglar hur era team faktiskt planerar, arbetar och levererar.
* För att användarna ska förstå var de är, hur posttyperna ansluter och hur strategin flödar in i körningen genom att referera till en uppsättning vägbeskrivningar som anger deras plats i systemet.
* För att ge bättre navigering och skapa tydlighet och kontinuitet i alla arbetsflöden.
* För att definiera flöden som passar hur organisationen fungerar, med stöd för både flexibilitet och konsekvens i alla arbetsfaser.

## Att tänka på när du arbetar med hierarkier

* Som arbetsytehanterare kan du skapa flera hierarkier för en arbetsyta.
* Om det redan finns en anslutning mellan de valda posttyperna återanvänds den befintliga anslutningen.
* Om det inte finns någon anslutning skapas en automatiskt i Workfront som en del av hierarkiinställningarna.
* Följande är regler för hierarkiinställningar:
   * En posttyp kan bara ha en överordnad posttyp på en angiven arbetsyta.

     En taktisk posttyp kan till exempel inte ha både en Campaign- och en målobjekttyp som överordnad på samma arbetsyta.
   * En post kan kopplas till flera överordnade poster av samma typ när du kopplar en till många eller flera posttyper.
Taktik A kan till exempel tillhöra både Campaign X och Campaign Y.
   * En posttyp kan ansluta till flera underordnade posttyper.

     En Campaign-posttyp kan till exempel vara överordnad flera andra posttyper, som Tactics, Tests och andra posttyper.
   * Hierarkier kan innehålla både Planning-posttyper och Workfront-objekttyper.

     Du kan till exempel ha en Campaign-posttyp med Planning Tactics och Workfront Projects som underordnade.

     <!--asking if ONLY projects are supported here in slack; if yes, make a note to say that only Projects are supported; also add a note about AEM -->
   * Globala posttyper kan förekomma i flera arbetsytor i flera hierarkier. <!--not sure if this AFTER they were added to another workspace; right now, I can see only the current workspace when building one??-->
   * Workfront objekttyper kan också visas i flera hierarkier och i olika arbetsytor.
   * Globala posttyper kan inte ingå i hierarkier på en annan arbetsyta.

     Om en Campaign till exempel är en global posttyp och en del av en hierarki i Workspace 1, kan den läggas till som en befintlig posttyp i Workspace 2, men inte som en del av en hierarki där. <!--verifying that this is not connectable RT and it is about global ones - checking in slack-->
   * Posttyperna med anslutningar som inte skapar ett motsvarande fält på sina länkade posttyper kan också ingå i hierarkier. Nya anslutningar som skapas under hierarkiinställningar skapar som standard alltid ett motsvarande fält på de länkade posttyperna.

## Att tänka på när du visar vägbeskrivningar

När du skapar hierarkier mellan posttyper genereras vägbeskrivningar för poster som tillhör de posttyperna.

Om du till exempel skapar en hierarki och kopplar ihop kampanjer med taktik med program och sedan Projekt, kan du visa var i hierarkin posten placeras när du navigerar till en post med någon av de typer som är kopplade till den.

Tänk på följande:

* Om en posttyp ingår i flera hierarkier på flera arbetsytor kan du växla mellan hierarkier från postens synliga del på postens sida.
* Brödraperier fungerar i Workfront och Planning.

  Om du till exempel tittar på ett projekt som är kopplat till Planering-kampanjer och taktik, och även till Workfront portfolior och program, kan du växla mellan både Planning och Workfront hierarkier från den stora mängden.

  Mer information finns i [Skapa arbetsytehierarkier](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).



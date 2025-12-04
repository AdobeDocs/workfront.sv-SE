---
title: Översikt över hierarki och vägbeskrivningar
description: Du kan skapa flera arbetsytehierarkier mellan posttyperna på en arbetsyta.
hide: true
hidefromtoc: true
source-git-commit: f345cc0d41dc1bd62e7361fa0755cb7ba72465a0
workflow-type: tm+mt
source-wordcount: '405'
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

Nedan följer några fördelar med att använda hierarkier i dina arbetsytor:

* Organisera arbetet på ett sätt som återspeglar hur era team faktiskt planerar, arbetar och levererar.
* Användarna förstår var de är, hur posttyper ansluter och hur strategin flödar in i körningen genom att referera till en uppsättning vägbeskrivningar som anger deras plats i systemet.
* Erbjud bättre navigering och skapa tydlighet och kontinuitet i alla arbetsflöden.
* Hierarkier tillämpar inte en fast, systemdefinierad struktur, utan låter er i stället definiera flöden som passar hur organisationen fungerar, med stöd för både flexibilitet och enhetlighet i alla steg av arbetet.

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
   * Globala posttyper kan förekomma i flera arbetsytor i flera hierarkier.
   * Workfront objekttyper kan också visas i flera hierarkier och i olika arbetsytor.
     <!--Not sure what this means: * Shared record can't be part of hierarchies.-->
   * Posttyperna med anslutningar som inte skapar ett motsvarande fält på sina länkade posttyper kan också ingå i hierarkier. Nya anslutningar som skapas under hierarkiinställningar skapar som standard alltid ett motsvarande fält på de länkade posttyperna.

## Att tänka på när du visar vägbeskrivningar



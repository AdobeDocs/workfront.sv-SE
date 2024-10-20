---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 Beta 1 - versionsaktivitet
description: Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i 2018.2 Beta 1. Funktionerna gjordes tillgängliga i förhandsvisningsmiljön den 22 mars 2018. Den kommer att göras tillgänglig i produktionsmiljön i juni 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: cbe98ee2-f155-4d31-88c4-7f41b6f91eb2
source-git-commit: 51b8e474cefe63b4db8c42e480990ca0ba431a4d
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 0%

---

# 2018.2 Beta 1 - versionsaktivitet

Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i 2018.2 Beta 1. Funktionerna gjordes tillgängliga i förhandsvisningsmiljön den 22 mars 2018. Den kommer att göras tillgänglig i produktionsmiljön i juni 2018.

>[!IMPORTANT]
>
>Funktionerna som beskrivs på den här sidan kan ändras innan de är tillgängliga i produktionsmiljön.

En lista över alla ändringar som gjorts under 2018.2 finns i [Översikt över versionsaktivitet för 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

2018.2 Beta 1 innehåller följande förbättringar:

* [Ändra aktivitetsdatum i Gantt-schemat](#modify-task-dates-in-the-gantt-chart)
* [Gå till Project Gantt-schemat från fliken Uppdateringar](#access-the-project-gantt-chart-from-the-updates-tab) (tillfälligt borttagen)

* [Olika länkar återinfördes till dokument i dokumentlistan](#various-links-re-introduced-to-documents-on-the-document-list)
* [Förbättringar av användarvyn i resursplaneraren](#user-view-improvements-in-the-resource-planner)
* [Ny projektlisteupplevelse](#new-project-list-experience)
* [Ny sökning efter uppdateringsfliken](#new-look-for-updates-tab)
* [Mobilförbättringar](#mobile-improvements)

## Ändra aktivitetsdatum i Gantt-schemat {#modify-task-dates-in-the-gantt-chart}

Nu kan du dra aktivitetsbubblan för att ändra planerad start- och planerad slutförandedatum i Gantt-schemat. Med den här ändringen kan du använda konsekvensscenarier i ditt projekt utan att tidslinjen påverkas.

Före den här ändringen kan du bara ändra aktivitetsdatum i uppgiftslistan eller på aktivitetsnivå.

Mer information finns i [Uppdatera information i Gantt-schemat för uppgiftslistan](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Gå till Project Gantt-schemat från fliken Uppdateringar {#access-the-project-gantt-chart-from-the-updates-tab}

>[!NOTE]
>
>Den här funktionen har tillfälligt tagits bort från förhandsvisningsmiljön.

Du kan nu komma åt det nya Gantt-schemat för projekt på fliken Uppdateringar. När en användare ändrar implementeringsdatumet för en aktivitet på ett sätt som påverkar projekttidslinjen kan du visa effekten i projektets Gantt-schema.

Före den här ändringen öppnades det äldre Gantt-schemat via länken Projekttidslinje.

Mer information finns i [Genomför datumöversikt](../../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

Mer information finns i [Översikt över Portfolio-optimering](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

## Olika länkar återinfördes till dokument i dokumentlistan {#various-links-re-introduced-to-documents-on-the-document-list}

I version 18.1 togs olika länkar bort från dokument i dokumentlistan och flyttades till andra delar av gränssnittet (vissa som en knapp bredvid dokumentnamnet och andra i en nedrullningsbar meny på knappen). Följande länkar återinförs under dokumentnamnet med den här versionen och är nu tillgängliga för enskilda dokument i dokumentlistan:

* Generera korrektur (tillgängligt när inget korrektur har genererats ännu)
* Öppna korrektur (tillgängligt när ett korrektur skapas)
* Dokumentinformation (tillgänglig när inget korrektur har genererats ännu)
* Korrekturinformation (tillgänglig när ett korrektur skapas)
* Skriv ut sammanfattning

Följande åtgärder återinförs inte som länkar i dokumentet i dokumentlistan:

* Dela (fortfarande tillgängligt som en knapp på menyn)
* Checka ut/Checka in (fortfarande tillgängligt i listrutan Mer på menyn)

Mer information finns i följande avsnitt:

*  in 

## Förbättringar av användarvyn i resursplaneraren {#user-view-improvements-in-the-resource-planner}

Resursplaneringens användarvy innehåller nu följande förbättringar:

* Användarvyn är nu standardvy och ersätter projektvyn.
* Förbättrade filter som hämtar information från hela databasen i stället för bara informationen på skärmen.
* Helskärmsläge.
* Prestanda är nu snabbare och effektivare.

   * Nya gränser för hur många användare, projekt, roller och uppgifter du kan visa.
   * Lazy loading, för snabbare inläsning av användare.

Följande funktioner har tillfälligt inaktiverats i resursplaneraren:

* Exportera data från resursplaneraren när du använder användarvyn.

Före dessa förbättringar har du rapporterat att resursplaneraren var långsam att läsa in och att du har upptäckt inkonsekvenser i de data som visas. Dessa förbättringar bör nu tas bort.

Mer information om områdena i resursplaneraren finns i [Navigeringsöversikt för resursplanering](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a></p>
-->

## Ny projektlisteupplevelse {#new-project-list-experience}

Nu finns det en ny upplevelse när du visar en lista över projekt. Den här upplevelsen innebär bättre prestanda och smidigare och snabbare listnavigering. Endast listorna på fliken Projekt i området Projekt i Workfront har uppdaterats till den nya upplevelsen.

För det mesta ändras listans hastighet och effektivitet. Följande synliga ändringar har också införts:

* I listan visas upp till 2 000 objekt som standard.

  Före den här förbättringen visades 100 objekt i listan.

* Grupperingar komprimeras som standard.

  Före den här ändringen expanderades grupperingarna som standard.

* Området för att markera en rad har utökats till hela raden.

Följande funktioner har tillfälligt inaktiverats i de angivna projektlistorna:

* Ändra storlek på kolumner (den här funktionen återinfördes i 2018.2 Beta 5)
* Ordna om kolumner
* Statusikonfält visas som tomma (den här funktionen återinfördes i 2018.2 Beta 5)
* Gantt-schemat är inte tillgängligt (den här funktionen återinfördes i version 2018.2 av Beta 3).

Mer information om hur du arbetar i listor finns i [Kom igång med listor i Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Ny sökning efter uppdateringsflik {#new-look-for-updates-tab}

>[!NOTE]
>
>För vissa användare kanske inte den nya uppdateringsfliken visas i förhandsvisningsmiljön. Vårt utvecklingsteam felsöker just nu problemet och arbetar för att lösa det så snart som möjligt.

Utseendet på fliken Uppdateringar har ändrats så att den bättre motsvarar andra delar av gränssnittet. Den här ändringen gäller projekt, uppgifter, utgåvor och dokument.

I följande tabell visas uppdateringarna på fliken Uppdateringar:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Aktivitet</strong> </p> </th> 
   <th> <p><strong>Tidigare användaråtgärd</strong> </p> </th> 
   <th> <p><strong>Ny användaråtgärd</strong> </p> </th> 
   <th> <p><strong>Mer information finns i..</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Loggningstid på en tidrapport</p> </td> 
   <td> <p>Klicka på länken Loggtid</p> </td> 
   <td> <p>Klicka på knappen Loggtid</p> </td> 
   <td> <p><a href="../../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Loggtid</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Filtrera ut systemuppdateringar på fliken Uppdateringar</p> </td> 
   <td> <p>Klicka på länken Filtrera systemuppdateringar</p> </td> 
   <td> <p>Inaktivera alternativet Visa aktivitetsloggen</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Uppdatera arbete</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Visa systemuppdateringar på fliken Uppdateringar</p> </td> 
   <td> <p>Klicka på Visa alla uppdateringar</p> </td> 
   <td> <p>Aktivera alternativet Visa aktivitetsloggen</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Uppdatera arbete</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tagga andra användare för en uppdatering eller kommentar</p> </td> 
   <td> <p>Klicka på ikonen Inkludera andra i den här uppdateringen</p> </td> 
   <td> <p>Lägga till användare och team i fältet Meddela</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Uppdatera arbete</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tillåt endast användare i företaget att visa ett objekt</p> </td> 
   <td> <p>Klicka på låsikonen</p> </td> 
   <td> <p>Aktivera alternativet Privat till mitt företag</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tagga andra för uppdateringar</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tillåt användare utanför företaget att visa ett objekt</p> </td> 
   <td> <p>Klicka på låsikonen</p> </td> 
   <td> <p>Inaktivera alternativet Privat till mitt företag</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tagga andra för uppdateringar</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Lägga till ett svar eller en uppdatering till en kommentar eller uppdatering</p> </td> 
   <td> <p>Klicka på knappen Kommentar</p> </td> 
   <td> <p>Klicka på knappen Svara eller Uppdatera</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Uppdatera arbete</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Uppdatera aktivitetsstatus</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Uppdatera villkor för aktiviteter och problem</a> </p> <p> </p> <p><a href="../../../../documents/managing-documents/add-update-documents.md" class="MCXref xref">Lägg till en uppdatering i ett dokument</a> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Mobilförbättringar {#mobile-improvements}

Mobilappen innehåller följande förbättringar:

* Länkar som delas med dig i andra mobilprogram öppnas nu i Workfront mobilapp.

  Mer information om delning av länkar finns i .

  Uppdateringen kommer ibland att släppas på iOS den här veckan och Android-uppdateringen kommer snart.

* Vi har uppdaterat våra supportkrav för iOS-plattformen för iPhone X.

  Mer information om vilka mobila enheter och operativsystem som stöds finns i .

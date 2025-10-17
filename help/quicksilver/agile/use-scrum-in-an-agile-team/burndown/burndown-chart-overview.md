---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: Översikt över Agile Burndown Chart
description: Nedbrytningsdiagrammet ger en visuell representation av hur artiklar fortskrider genom iteration eller projekt. Den faktiska nedbränningsgraden mäts mot den ideala nedladdningsfrekvensen för tidslinjen för iteration eller projekt.
author: Jenny
feature: Agile
exl-id: 414e3315-35ed-4aa4-a2d8-be42ec585f29
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 0%

---

# Översikt över Agile-nedladdningsdiagram

Nedbrytningsdiagrammet ger en visuell representation av hur artiklar utvecklas genom upprepningen. Den faktiska nedbränningsgraden mäts mot den ideala nedladdningsfrekvensen för tidslinjen i iteration.

Nedbrytningsdiagrammet justeras baserat på den valda dagen. Den aktuella dagen är standarddatum. När en föregående dag har valts beräknas alla data i nedladdningsdiagrammet och alla värden i avsnittet [!UICONTROL completion status] ovanför nedladdningsdiagrammet om för att representera data som de var i slutet av den valda dagen. (Du kan välja föregående dagar eller den aktuella dagen. Du kan inte välja dagar i framtiden.)

![](assets/agile-iteration-burndown-350x88.png)

## Visuella indikatorer

Nedladdningsschemat innehåller följande visuella indikatorer:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-dottedblue.png" alt="Idealisk nedladdningsränta - början"> </td> 
   <td> <p>Idealisk nedbränningsgrad baserad på när iterationen påbörjades.</p> <p>Den här raden visas inte om upprepningens omfattning aldrig ändras (timmar eller punkter läggs aldrig till eller tas bort).</p> <p>Den här raden visas som platt när arbete utförs en ledig dag. Mer information finns i <a title="Använda Agile Burndown Chart" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">Hur dagar kvar påverkar nedladdningsschemat</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-solidblue.png" alt="Idealisk nedladdningsgrad för artiklar och uppgifter"> </td> 
   <td> <p>Idealisk nedladdningsfrekvens baserad på aktuella artiklar eller uppgifter.</p> <p>Den aktuella idealiska nedladdningsfrekvensen (helblå linje) skiljer sig från den ursprungliga idealiska nedladdningsfrekvensen (prickad blå linje) när timmar eller punkter läggs till eller tas bort från iterationen efter att iterationen påbörjats.</p> <p>Den här raden visas som platt när arbete utförs en ledig dag.</p> <p>Mer information finns i <a title="Använda Agile Burndown Chart" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">Hur dagar kvar påverkar nedladdningsschemat</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-red.png" alt="Faktisk nedbränningsgrad i rött"> </td> 
   <td> <p>Faktisk nedladdningsfrekvens visas i rött när nedladdningsfrekvensen är lägre än den ideala (fler punkter eller timmar återstår per dag än den idealiska nedladdningsberäkningen).</p> <p>Följande formel används för att beräkna den faktiska nedladdningsgraden:</p> <p>[SUM(Point or Hour Value of In-Progress Work * Percent Complete) + Point or Hour Value of Completed Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-green.png" alt="Faktisk nedbränningsgrad i grönt"> </td> 
   <td> <p>Faktisk nedbränningsgrad visas i grönt när nedladdningsgraden är lika med eller bättre än det ideala (lika med eller färre punkter återstår per dag än den ideala nedladdningsberäkningen).</p> <p>Följande formel används för att beräkna den faktiska nedladdningsgraden:</p> <p>[SUM(Point or Hour Value of In-Progress Work * Percent Complete) + Point or Hour Value of Completed Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt="Ändring i omfång"> </td> 
   <td> <p>Omfattningsändring (timmar eller punkter läggs till eller tas bort från iterationen).</p> <p>Omfångsändringar visas alltid som en lodrät linje mitt på dagen. Dessutom visas en blå punkt mitt under en dag när en omfångsändring har inträffat.</p> <p>Den lodräta axeln i nedladdningsdiagrammet visar artikelpunkterna eller timmarna.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt="Ändra i datumintervall"> </td> 
   <td> <p>Ändring i datumintervall (upprepningens varaktighet ökas eller minskas).</p> <p>En blå punkt visas mitt i en dag där upprepningens varaktighet ändrades.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt="Punktdiagram för nedbränt arbete"> </td> 
   <td> <p>En grön eller röd punkt visas i den faktiska nedladdningshastigheten när arbete bränns ned. (När den faktiska nedbränningsgraden den dagen är röd är punkten röd. När den faktiska nedladdningsfrekvensen den dagen är grön är punkten grön.)</p> <p>Arbetet bränns ned när något av följande inträffar:</p> 
    <ul> 
     <li> [!UICONTROL Percent Complete] utökas i artikeln.<br>[!UICONTROL Percent Complete] ökas när: 
      <ul> 
       <li> <p>Manuellt ändrad</p> </li> 
       <li> <p>Antalet poäng eller timmar uppdateras i artikeln</p> </li> 
      </ul></li>  
     <li>Artikelns status ändras till [!UICONTROL Complete]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Hur dagar ledigt påverkar nedladdningsschemat {#how-days-off-affect-the-burndown-chart}

Standardschemat som definieras i [!DNL Workfront] påverkar nedladdningsschemat genom att utesluta dagar utan (helger och helger) från nedladdningen. Nedladdningsschemat använder standardschemat för att definiera arbetsdagar (enligt beskrivningen i  [Skapa ett schema](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)).

Agile-team kan införliva teamspecifika, icke-arbetsrelaterade dagar genom att definiera ett alternativt schema (enligt beskrivningen i artikeln [Använd ett alternativt teamschema för nedladdningsscheman](../../../agile/use-scrum-in-an-agile-team/burndown/use-alt-team-schedule-burndown-charts.md)). Det alternativa schemat visas sedan i nedladdningsschemat för alla upprepningar som teamet har tilldelats. Det alternativa schemat påverkar bara nedladdningsschemat.

Lediga dagar visas endast i nedladdningsschemat om:

* Arbetet var tidigare loggat en ledig dag. (Den dag då arbetet loggades visas.)

  När arbete är utloggat en dag:

   * Alla loggade arbeten inkluderas inte vid beräkning av den idealiska nedladdningen eftersom teamet inte är schemalagt att utföra något arbete.
   * De idealiska nedtryckningslinjerna (den helfyllda blå linjen och den streckade blå linjen) visas som platta i nedladdningsdiagrammet för alla dagar som arbetet utfördes eller den dag du visar nedladdningsdiagrammet (om du visar på en ledig dag).
   * Arbete som loggas inkluderas vid beräkning av annan nedladdningsstatistik, t.ex. uppskattat slutförande och genomsnittspoäng eller timmar per dag.

* Du visar nedladdningsschemat en dag ledigt. (Den dag du visar visas i nedladdningsdiagrammet.)
* Du slutför det totala återstående arbetet för iterationen en dag bort.

  När en användare slutför det totala återstående arbetet för iterationen en dag bort, visar fältet [!UICONTROL Estimated Completion] datumet då iterationen slutfördes.

  Om du anger slutdatumet för upprepningen för en arbetsdag som inte är arbetsdag och upprepningen spåras till färdig i tid, anges datumet [!UICONTROL Estimated Completion] för den sista arbetsdagen före det slutdatum för upprepningen som du anger (eftersom arbetet inte schemalagts att brännas ned på arbetsdagar som inte är arbetsdag) när du planerar upprepningen.

  Slutdatumet för iteration anges när iteration planeras, vilket beskrivs i artikeln [Skapa en iteration](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

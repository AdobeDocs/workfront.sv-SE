---
title: Översikt över projektbegränsningar
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: Adobe Workfront har gränser för hur många objekt som kan kopplas till ett projekt. Projektbegränsningar finns för att förbättra produktprestanda och förbättra din upplevelse av Workfront.
author: Alina
feature: Work Management
exl-id: 60576107-89f1-4328-89e2-5b1e5e243fd9
source-git-commit: 809f1c3629c343a55305c0c617f4974dc05439bf
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# Översikt över projektbegränsningar

Adobe Workfront har gränser för hur många objekt som kan kopplas till ett projekt. Projektbegränsningar finns för att förbättra produktprestanda och förbättra din upplevelse av Workfront.

Följande objekt som är associerade med projekt har följande gränser:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Uppgifter</p></td> 
   <td>  <p>Det högsta antalet uppgifter per projekt är 5 000. Ett varningsmeddelande visas när antalet uppgifter närmar sig det maximala antalet. När det maximala antalet nås visas ett felmeddelande och ytterligare uppgifter kan inte läggas till i projektet.</p> <p>Flytta aktiviteter som är stängda till ett annat projekt som är avsett för stängda aktiviteter för att undvika att uppnå det maximala antalet. Rapporterna om dessa projekt kan behöva justeras.</p>

<b>VIKTIGT</b>

För projekt där aktiviteter har många beroenden rekommenderar vi att antalet uppgifter i projekten är mycket lägre än det högsta tillåtna antalet på 5 000 uppgifter.

Några exempel på aktivitetssamband som kan påverka eller förhindra omberäkning av projektets tidslinje är:

<ul><li>Antal underordnade</li>
   <li>Indrag för flera nivåer av uppgifter</li>
   <li>Antal föregångare</li>
   <li>Flera tilldelningar</li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Problem</p></td> 
   <td>  <p>Det högsta antalet utgåvor per projekt är 10 000. Ett varningsmeddelande visas när antalet problem närmar sig det maximala antalet. När det maximala antalet nås visas ett felmeddelande och ytterligare problem kan inte läggas till i projektet.</p> <p>Om du vill undvika att uppnå det maximala antalet flyttar du ärenden som är stängda till ett annat projekt som är avsett för stängda problem. Rapporterna om dessa projekt kan behöva justeras.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Varaktighet</p></td> 
   <td> <p>Ett projekt måste ha en varaktighet på högst 15 år för att Workfront automatiskt ska kunna beräkna tidslinjen. Ett varningsmeddelande visas när projektets längd närmar sig maxvärdet. När det maximala antalet nås visas ett varningsmeddelande och de automatiska tidslinjeberäkningarna inträffar inte längre.</p> <p>De automatiska tidslinjeberäkningarna återupptas så snart ett projekts längd minskar till under 15 år genom att datumen för uppgifterna i projektet justeras.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Beräkningar av tidslinje</p></td> 
   <td>Workfront utför inte automatiska tidslinjeberäkningar för projekt som inte har uppdaterats på sex månader och kommer inte att återupptas förrän en uppdatering har gjorts.<p>För projekt som inte har uppdaterats på tre månader utför Workfront tidslinjeberäkningar varje vecka i stället för varje natt.</p><p>Mer information om hur du beräknar projekttidslinjen finns i <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Beräkna om projekttidslinjer</a>. </p></td> 
  </tr> 
 </tbody> 
</table>

<!-- Notes from the table: 
     <p>For tasks limits: (This is NOT TRUE , but the PMs always wanted this to stay the way it is because they don't want customers creating projects bigger than this.)</p>
    <p>For issue limits: (this is true only for some clusters; according to Anna A., some clusters are set to a million.)</p>
    -->
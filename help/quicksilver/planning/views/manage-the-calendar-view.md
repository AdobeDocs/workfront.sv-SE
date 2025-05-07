---
title: Hantera kalendervyn
description: Du kan visa poster och deras fält i en kalendervy. I den här artikeln beskrivs hur du skapar en kalendervy och redigerar eller tar bort en befintlig.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: 3dfac5ada17248f5c67380b56b9a0969b10b73e6
workflow-type: tm+mt
source-wordcount: '859'
ht-degree: 0%

---

# Hantera kalendervyn

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Du kan visa poster och deras fält i en kalendervy från posttypssidan.

Mer information om Adobe Workfront Planning-vyer och hur du hanterar dem finns i [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produkter</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-plan*</p></td> 
   <td> 
<p>Något av följande Workfront-planer:</p> 
<ul><li>Välj</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning är inte tillgängligt för tidigare Workfront-planer</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning-paket*</p></td> 
   <td> 
<p>Alla </p> 
<p>Kontakta din kontoansvarige på Workfront om du vill ha mer information om vad som ingår i respektive Workfront Planning-plan. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront</p></td> 
   <td> 
<p>Din organisations instans av Workfront måste integreras med Adobe Unified Experience för att få tillgång till alla funktioner i Workfront Planning.</p> 
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning är inte tillgängligt för tidigare Workfront-licenser</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>   <p>Hantera behörigheter till en vy</p>  
   <p>Visa behörigheter till en vy om du tillfälligt vill ändra visningsinställningarna eller duplicera den</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutmall</p></td> 
   <td> <p>I produktionsmiljön måste alla användare, inklusive systemadministratörer, tilldelas en layoutmall som innehåller Planning.</p>
<p><span class="preview">I förhandsvisningsmiljön har standardanvändare och systemadministratörer Planering aktiverat som standard.</span></p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Hantera en kalendervy {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

Tänk på följande:

* Du kan bara skapa en kalendervy om du har minst två datumfält kopplade till en posttyp. När du har ett eller inga datumfält kopplade till en posttyp är alternativet Kalendervy nedtonat.

  Du kan välja från postdatumfält eller uppslagsdatumfält från anslutna post- eller objekttyper.
* Följande scenarier finns:

   * När både start- och slutdatum saknar värden visas inte posterna i kalendern
   * När start- eller slutdatumet saknar värde visas posten som en endagshändelse
   * När startdatumet är efter slutdatumet visas inte posten i kalendern.

Så här hanterar du en kalendervy:

1. Gå till den posttypssida som du vill visa kalendern för.
1. Skapa en kalendervy enligt beskrivningen i artikeln [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).

   ![Exempel på kalendervy](assets/calendar-view-example.png)

   Posterna som är associerade med den posttyp som du har valt visas som staplar i en kalender. Färgen på staplarna matchar färgen på postikonen.

1. Navigera i kalendern genom att göra något av följande:

   * Klicka på vänster- och högerikonerna eller använd den vågräta rullningen för att flytta bakåt och framåt i kalendern.
   * Klicka på **Idag** om du vill centrera kalendern till dagens datum.
   * Välj något av följande alternativ på den nedrullningsbara menyn för tidsram för att uppdatera tidsstegen:

      * **Månad**: Posterna visas i en månadskalender.


      * **Vecka**: Posterna visas i följande områden:

         * Poster som sträcker sig över flera dagar visas högst upp i kalendern.
         * Poster som varar en dag eller mindre visas i den nedre halvan av kalendervyn. Om du valde att visa timmen för Start- och slutdatum visas posten vid lämplig tidpunkt under dagen då den inträffar.


1. Uppdatera följande vyelement enligt beskrivningen i underavsnitten nedan:
   * [Filter](#add-filters)
   * [Inställningar](#edit-the-calendar-view-settings)
     <!--* [Grouping](#add-grouping)-->
     <!--* [Sort](#add-sort) not sure if this is present in calendar views?!; also check the anchor and make sure it's correct-->

### Lägg till filter

Du kan minska mängden information som visas på skärmen genom att använda filter.

Tänk på följande när du arbetar med filter i kalendervyn:

<!-- this list is almost identical to the one for the table view - update both-->

* De filter du skapar för en kalendervy fungerar oberoende av filtren i andra vyer som används för samma posttyp.

* Filtren är unika för den vy du väljer. Två kalendervyer av samma posttyp kan ha olika filter.

* Två användare som tittar på samma kalendervy ser samma filter som används för närvarande.

* Du kan inte namnge filtren som du skapar för en kalendervy.

* När du tar bort filter tas de bort från alla som använder samma posttyp som du och som visar samma vy som du.

* Att lägga till filter i kalendervyn är detsamma som att lägga till filter i tabellvyn.

  Mer information finns i avsnittet&quot;Lägg till filter&quot; i artikeln [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md).

* Du kan filtrera efter anslutna postfält eller uppslagsfält.

* Du kan filtrera efter uppslagsfält som visar flera värden.

### Redigera inställningar för kalendervyn

Att redigera kalendervyinställningarna liknar att redigera inställningarna för en tidslinjevy.

Mer information finns i avsnittet Redigera tidslinjevisningsinställningar i artikeln [Hantera tidslinjevyn](/help/quicksilver/planning/views/manage-the-timeline-view.md).

---
title: Hantera kalendervyn
description: Du kan visa poster och deras fält i en kalendervy.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: 402fb9d279fec258390535100e8f3d2c3c1b913b
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# Hantera kalendervyn

<!--
title: Manage the calendar view
description: You can display records in a calendar view.
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

Du kan visa poster och deras fält i en kalendervy från posttypssidan.

Mer information om Adobe Workfront Planning-vyer och hur du hanterar dem finns i [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).

<!--at GA the plan below will change to Prime, Select and Ultimate only-->

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produkt</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-avtal</p></td>
   <td>
<p>Din organisation måste vara registrerad på Workfront Planning i ett tidigt skede </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront</p></td>
   <td>
<p>Alla</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td>
   <td>
   <p>Nytt: Standard</p>
   eller
   <p>Aktuell: Planera </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td>
   <td> Det finns inga åtkomstkontroller för Adobe Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Hantera behörigheter till en vy</p>  
   <p>Visa behörigheter till en vy för att tillfälligt ändra visningsinställningarna</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn. </p> <p>Mer information finns i <a href="/help/quicksilver/planning/access/access-overview.md">Åtkomstöversikt</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

   ![](assets/calendar-view-example.png)

   Posterna som är associerade med den posttyp som du har valt visas som staplar i en kalender. Färgen på staplarna matchar färgen på postikonen.

1. Navigera i kalendern genom att göra något av följande:

   * Klicka på vänster- och högerikonerna eller använd den vågräta rullningen för att flytta bakåt och framåt i kalendern.
   * Klicka på **Idag** om du vill centrera kalendern till dagens datum.
   * Välj något av följande alternativ på den nedrullningsbara menyn för tidsram för att uppdatera tidsstegen:

      * Månad
1. Uppdatera följande vyelement enligt beskrivningen i underavsnitten nedan:
   * [Filter](#add-filters)
     <!--* [Grouping](#add-grouping)-->
     <!--* [Settings](#edit-the-calendar-view-settings)-->
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

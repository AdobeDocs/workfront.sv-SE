---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Hantera mål i mållistan för Adobe Workfront mål
description: När du eller andra användare har skapat mål kan du granska deras förlopp och information i mållistan. Mer information om hur du skapar mål finns i Skapa mål i Adobe Workfront-mål.
author: Alina
feature: Workfront Goals
exl-id: 2a2c1240-f796-4cb8-b8a6-2ad5853916b9
source-git-commit: 45c71a8106bdb8eeaa38f2fb83ff0312e48183d0
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# Hantera mål i mållistan för Adobe Workfront mål

<!-- printing or exporting goals is no longer possible, but see if they add it later-->

När du eller andra användare har skapat mål kan du granska deras förlopp och information i mållistan. Mer information om att skapa mål finns i [Skapa mål i Adobe Workfront-mål](../../workfront-goals/goal-management/create-goals.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra de åtgärder som beskrivs i den här artikeln:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> 
   <p>För den nya planen och licensstrukturen:
  <ul><li>En Ultimate-plan </li></ul>
   </p>
<p>För aktuell plan och licensstruktur: 
<ul><li> En Pro eller högre </li>
  <li>En Adobe Workfront Goals-licens förutom en Workfront-licens.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-licens*</td>
 <td>
 <p>Ny licens: Medarbetare eller högre</p>
 eller
 <p>Aktuell licens: Begär eller högre</p> <p>Mer information finns i <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Översikt över Adobe Workfront-licenser</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produkt*</td>
 <td>
 <p> Nytt produktkrav, något av följande: </p>
<ul>
<li>A Select- eller Prime Adobe Workfront-plan och en extra licens för Adobe Workfront Goals.</li>
<li>En Ultimate Workfront-plan som innehåller Workfront-mål som standard. </li></ul>
 <p>eller</p>
 <p>Aktuellt produktkrav: En Workfront-plan och ytterligare licens för Adobe Workfront-mål. </p> <p>Mer information finns i <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Krav för att använda Workfront-mål</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Åtkomstnivå</td>
 <td> <p>Redigera åtkomst till mål</p>  </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objektbehörigheter</td>
 <td>
  <div>
  <p>Visa eller högre behörigheter för målet för att visa det</p>
  <p>Hantera behörigheter till målet för att redigera det</p>
  <p>Mer information om delningsmål finns i <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Dela ett mål i Workfront-mål</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller området Mål på huvudmenyn. </p>  
</td>
  </tr>
</tbody>
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Hantera mål i mållistan

Du kan visa och hantera mål i följande avsnitt av Workfront-mål:

* Mållista
* Måljustering

Varje avsnitt visar mål i något olika format. Vilket avsnitt du använder beror på vilket syfte du vill uppnå när du arbetar med mål.

Mer information finns i [Översikt över avsnitten om Adobe Workfront-mål](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

I den här artikeln beskrivs hur du granskar mål i mållistan.

Tänk på följande när du granskar mållistan:

* Du kan visa mål som du eller någon annan i organisationen har skapat i mållistan. Du måste ha behörigheten Hantera för mål för att kunna redigera dem.

<!--

### Manage the Goal List in the Production environment

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **Goals**.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List section displays by default. You can view goals regardless of their status, period, or owner, by default.

   The list of goals contains the following columns with information about each goal, result, or activity: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> 
       <div> 
        <p role="rowheader">Name </p> 
       </div> </td> 
      <td>The name of the goal, result, or activity.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Owner</td> 
      <td>The name of the goal, result, or activity owner. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Period</td> 
      <td>The time period for which the goal is scheduled.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progress </td> 
      <td> <p>The progress indicator for the goal includes the following:</p> 
       <ul> 
      <li> <p>The progress label. </p> <p>For information, see <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Overview of goal progress and condition in Adobe Workfront Goals</a>. </p> </li> 
      <li> <p>The percent complete of the goal, activity, or result. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Status (includes alignment icon)</p> <p> <img src="assets/alignment-icon-large.png"> </p> </td> 
      <td> <p>The status of the goal which can be one of the following:</p> 
       <ul> 
        <li>Active</li> 
        <li>Draft</li> 
        <li>Inactive</li> 
        <li>Closed</li> 
       </ul> <p>For information about goal status, see <a href="../../workfront-goals/goal-management/goal-status-overview.md" class="MCXref xref">Goal status overview in Adobe Workfront Goals</a>. </p> <p>The alignment icon appears on goals that are aligned to other goals. For information about aligning goals, see <a href="../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md" class="MCXref xref">Align goals by connecting them in Adobe Workfront Goals</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Use the filters in the upper-right corner of the goal list to select only goals that are important to you. For information about using filters in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md)
1. Click any of the fields in the column headers to sort it by that field.

   An arrow displays to the right of the field by which the list is sorted.

   ![Goal list with goal expanded](assets/goal-list-with-goal-expanded-+-result-+-activity-350x117.png)

1. (Optional) Click the field in the column again to sort the same column in a descending order. 
1. Click the right-pointing arrow to the left of the goal name to expand a goal

   Or

   Click the right-pointing arrow ![Right-pointing arrow](assets/right-pointing-arrow.png) in the header of the list to expand all the goals in the list and view additional information about each goal, including any of the following:

   * Results names, owners, and progress

     For information about results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   
   * Activity names, owners, and progress

     For information about activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

1. Click the name of a goal to open the **Goal Details** panel on the right and review more information about the goal as well as manage it. For information about reviewing individual goals, see [Update goals in the Goal details section in Adobe Workfront Goals](../../workfront-goals/goal-management/update-goals-in-goal-details-panel.md).
1. (Optional) Expand the **Goals per page** drop-down menu and select from the following options to display additional goals:

   * 20  
      
      This is the default selection. 
   * 50
   * 100

1. Click **Print** to export a list of goals, results, and activities to a .pdf file.

   >[!TIP]
   >
   >* When printing a list of goals, the file produced contains only the information displayed on the screen. Items eliminated by filtering a list of goals do not display in the .pdf file.
   >* When you do not expand the goals in the list before printing the list, the .pdf file displays only goals without their results and activities.

   For more information, see [Print the Goal List in Adobe Workfront Goals](../../workfront-goals/goal-management/print-the-goal-list.md). 

1. Click the **Alignment icon** ![Alignment icon](assets/align-icon.png) next to an aligned to open the goal's card in the Goal Alignment section. For more information, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).
-->

Så här hanterar du mål i mållistan:

1. Klicka på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **Mål**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Avsnittet Mållista visas som standard. Som standard kan du visa mål oavsett status, period eller ägare.

   Listan med mål innehåller följande fält med information om varje mål:

   * **Namn**: Målets namn.
   * **Ägare**: Målägarens namn.
   * **Period**: Den tidsperiod för vilken målet har schemalagts.
   * **Status**: Målets status kan vara något av följande:
      * Aktiv
      * Utkast
      * Inaktiv
      * Stängd

     Mer information om målstatus finns i [Översikt över målstatus i Adobe Workfront-mål](../goal-management/goal-status-overview.md).

     Justeringsikonen visas för mål som är justerade mot andra mål. Mer information om att justera mål finns i [Justera mål genom att koppla dem i Adobe Workfront-mål](../goal-alignment/align-goals-by-connecting-them.md).

   * **Villkor**: En visuell representation av hur målet fortskrider inom den tidsperiod som har allokerats för att målet ska slutföras.

     Ett målvillkor kan vara något av följande:

      * Nytt
      * På mål
      * Risk
      * I problem

     Mer information om målvillkor finns i [Översikt över målstatus och villkor i Adobe Workfront-mål](../goal-management/calculate-goal-progress.md).

   * **Förlopp**: Förloppsindikatorn för målet i procent. Färgen på förloppsindikatorn matchar färgen på målets villkor.

     Mer information finns i [Beräkna målförlopp i Adobe Workfront-mål](../goal-management/calculate-goal-progress.md).

1. Klicka på filterikonen ![Filterikonen](assets/filter-icon.png) i det övre högra hörnet av mållistan och använd filter för att endast visa mål som är viktiga för dig.

   Mer information om hur du använder filter i Workfront-mål finns i [Filtrera information i Adobe Workfront-mål](../goal-management/filter-information-wf-goals.md).

1. Klicka på något av fälten i kolumnrubrikerna för att sortera listan efter det fältet.
En pil visas till höger om det fält som listan sorteras efter.

1. (Valfritt) Klicka på fältet i kolumnen igen om du vill sortera samma kolumn i fallande ordning.
1. Klicka på namnet på ett mål för att öppna målets sida.
1. Välj ett mål i listan och klicka sedan på något av följande alternativ högst upp i listan:
   * **Redigera** ikon ![Redigera ikon](assets/edit-icon.png) om du vill redigera information om målet. Mer information finns i [Redigera mål i Adobe Workfront-mål](../goal-management/edit-goals.md).
   * **Dela** ikon ![Dela ikon](assets/share-icon.png) om du vill dela målet med andra. Mer information finns i [Dela ett mål i Adobe Workfront-mål](../workfront-goals-settings/share-a-goal.md).
   * **Öppna justeringsikonen** ![Öppna justeringsikonen](assets/align-icon-unshimmed.png) för att öppna området för måljustering. Det här alternativet visas bara när det valda målet är justerat mot ett annat mål.
   * **Ta bort** ikon ![Ta bort ikon](assets/delete-icon.png) om du vill ta bort målet och klicka sedan på **Ta bort** för att bekräfta.  Mer information finns i [Ta bort och inaktivera mål i Adobe Workfront-mål](../goal-management/delete-and-deactivate-goals.md).






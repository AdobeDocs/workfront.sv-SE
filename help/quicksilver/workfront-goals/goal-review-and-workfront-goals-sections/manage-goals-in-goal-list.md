---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Hantera mål i mållistan för Adobe Workfront-mål
description: När du eller andra användare har skapat mål kan du granska deras förlopp och information i mållistan. Mer information om hur du skapar mål finns i Skapa mål i Adobe Workfront-mål.
author: Alina
feature: Workfront Goals
exl-id: 2a2c1240-f796-4cb8-b8a6-2ad5853916b9
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 0%

---

# Hantera mål i mållistan för Adobe Workfront-mål

<!-- printing or exporting goals is no longer possible, but see if they add it later-->

När du eller andra användare har skapat mål kan du granska deras förlopp och information i mållistan. Mer information om hur du skapar mål finns i [Skapa mål i Adobe Workfront-mål](../../workfront-goals/goal-management/create-goals.md).

## Åtkomstkrav

<!--drafted - replace the table below with this one when P&P releases: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>
-->

Du måste ha följande åtkomst för att kunna utföra de åtgärder som beskrivs i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Pro eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Begäran eller senare</p> <p>Mer information finns i <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Översikt över Adobe Workfront-licenser</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td> <p>Du måste köpa ytterligare en licens för Adobe Workfront Goals för att få tillgång till de funktioner som beskrivs i den här artikeln. </p> <p>Mer information finns i <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Krav för att använda Workfront-mål</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivå*</td> 
   <td> <p>Visa eller öka åtkomsten till mål</p> <p><b>ANMÄRKNING</b><p>Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra din åtkomstnivå finns i:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Bevilja åtkomst till Adobe Workfront-mål</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> 
    <div> 
     <p>Visa eller öka behörigheter för mål</p> 
     <p>Mer information om delningsmål finns i <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Dela ett mål i Workfront-mål</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Du måste ha följande innan du kan börja:

* En layoutmall som innehåller området Mål på huvudmenyn.

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

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner, then click **Goals**.

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

   ![](assets/goal-list-with-goal-expanded-+-result-+-activity-350x117.png)

1. (Optional) Click the field in the column again to sort the same column in a descending order. 
1. Click the right-pointing arrow to the left of the goal name to expand a goal

   Or

   Click the right-pointing arrow ![](assets/right-pointing-arrow.png) in the header of the list to expand all the goals in the list and view additional information about each goal, including any of the following:

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

1. Click the **Alignment icon** ![](assets/align-icon.png) next to an aligned to open the goal's card in the Goal Alignment section. For more information, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).
-->

Så här hanterar du mål i mållistan:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png)  i det övre högra hörnet och klicka sedan på **Mål**.

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

      Justeringsikonen visas för mål som är justerade mot andra mål. Mer information om hur du justerar mål finns i [Justera mål genom att koppla dem till Adobe Workfront mål](../goal-alignment/align-goals-by-connecting-them.md).

   * **Villkor**: En visuell representation av hur målet fortskrider inom den tidsperiod som har tilldelats för att målet ska slutföras.

      Villkoret för ett mål kan vara något av följande:

      * Nytt
      * På mål
      * Risk
      * I problem

      Mer information om målvillkor finns i [Översikt över målets förlopp och villkor i Adobe Workfront-mål](../goal-management/calculate-goal-progress.md).

   * **Förlopp**: Förloppsindikatorn för målet som ett procentvärde. Färgen på förloppsindikatorn matchar färgen på målets villkor.

      Mer information finns i [Beräkna målstatus i Adobe Workfront-mål](../goal-management/calculate-goal-progress.md).



1. Klicka på filterikonen ![](assets/filter-icon.png) i det övre högra hörnet av mållistan och tillämpa filter för att endast visa mål som är viktiga för dig.

   Mer information om hur du använder filter i Workfront-mål finns i [Filtrera information i Adobe Workfront mål](../goal-management/filter-information-wf-goals.md).

1. Klicka på något av fälten i kolumnrubrikerna för att sortera listan efter det fältet.
En pil visas till höger om det fält som listan sorteras efter.

1. (Valfritt) Klicka på fältet i kolumnen igen för att sortera samma kolumn i fallande ordning.
1. Klicka på namnet på ett mål för att öppna målets sida.
1. Välj ett mål i listan och klicka sedan på något av följande alternativ högst upp i listan:
   * **Redigera** icon ![](assets/edit-icon.png) om du vill redigera information om målet. Mer information finns i [Redigera mål i Adobe Workfront-mål](../goal-management/edit-goals.md).
   * **Dela** icon ![](assets/share-icon.png) för att dela målet med andra människor. Mer information finns i [Dela ett mål i Adobe Workfront-mål](../workfront-goals-settings/share-a-goal.md).
   * **Öppna justering** icon ![](assets/align-icon-unshimmed.png) för att öppna området Måljustering. Det här alternativet visas bara när det valda målet är justerat mot ett annat mål.
   * **Ta bort** icon ![](assets/delete-icon.png) för att ta bort målet och klicka sedan på **Ta bort** för att bekräfta.  Mer information finns i [Ta bort och inaktivera mål i Adobe Workfront-mål](../goal-management/delete-and-deactivate-goals.md).






---
product-previous: workfront-goals
navigation-topic: goal-management
title: Uppdatera mål på panelen Målinformation i Adobe Workfront-mål
description: Du kan uppdatera information för enskilda mål genom att gå till panelen Målinformation.
author: Alina
feature: Workfront Goals
exl-id: e9df0d98-05a1-4977-b7f1-426b8f5b3eae
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 0%

---

# Uppdatera mål i avsnittet Målinformation i Adobe Workfront-mål

<!--drafted for the goal redesign:
- change the title for Production to Update goals in the Goal details section in Adobe Workfront Goals. 
- update the description in the metadata above
-->

Du kan uppdatera information för enskilda mål genom att gå till panelen Målinformation.

>[!NOTE]
>
>Du kan inte uppdatera mål som har statusen Stängt.


## Åtkomstkrav

Du måste ha följande:

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
<li>A Select- eller Prime Adobe Workfront-plan och ytterligare licens för Adobe Workfront Goals.</li>
<li>En Ultimate Workfront-plan som innehåller Workfront-mål som standard. </li></ul>
 <p>eller</p>
 <p>Aktuellt produktkrav: En Workfront-plan och ytterligare licens för Adobe Workfront-mål. </p> <p>Mer information finns i <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Krav för att använda Workfront-mål</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Åtkomstnivå*</td>
 <td> <p>Redigera åtkomst till mål</p> </td>
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

## Uppdatera mål i avsnittet Målinformation

Du kan nå ett enskilt mål från en lista med mål.

<!--

Updating goals in the Goal Details panel differs depending on where you access the goal from. 

### Update goals in the Goal Details panel in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Goals area in Workfront. 

1. Click the name of a goal in the Goal List, then click the name of a goal.

   This opens the Goal Details panel on the right.
   ![](assets/goal-details-summary-tab-350x294.png)

   >[!TIP]
   >
   >You can also click the name of a goal in the Goal Alignment, Check-in, or Pulse sections. 
   >
   ><!-- drafted for goal redesign:
   >Add this to the TIP above with goal redesign: 
   >
   >The Check-in and Pulse sections have been removed from the Preview environment.
   >

1. On the Summary tab, click the **More icon** ![](assets/more-icon.png), then click any of the following options:

   1. **Edit**. For information about editing goals, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
   1. **Copy**. For information about copying goals, see [Copy goals in Adobe Workfront Goals](../../workfront-goals/goal-management/copy-goals.md).
   1. **Activate**. This option is available only for drafted and inactive goals.

      For information about activating goals, see [Access and open goals in Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md). 
   
   1. **Close**, then click**Close Goal**. This option is available only for active goals.

      For information about closing goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   
   1. **Deactivate**. This option is available only for active goals. This deactivates the goal immediately.

      For information about deactivating goals, see [Delete and deactivate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).
   
   1. **Delete**, then click **Yes, Delete**.

      For information about deleting goals, see [Delete and deactivate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

      >[!NOTE]
      >
      >Deleted goals cannot be recovered.

   1. **Reopen**, then click **Reopen**. This option is available only for closed goals that are from a current time period.

      For information about reopening goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   
   1. (Conditional) If you clicked any of the options between steps a-i above except Delete or Reopen, click **Save**.    
   
      (!--ensure this is accurate)--)

1. Click **Align to another goal** in the upper-right of the Summary tab, then specify the name of a goal in the **Align to** **another goal** field that you want to align the current goal to. The current goal becomes the child of the goal you align it to. For information about child and parent goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md). 
1. Click **Add results**. Results drive the progress of your goal. For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).

1. Click **Add activities**. Activities drive the progress of your goal. For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 

1. Click the **Updates** tab. Here, you can view goal comments and review the entire editing history of the goal, activities, and results, to understand who changed what and when.

   ![](assets/goal-details-updates-tab-350x280.png)

1. (Optional) Deselect any of the following options if you want to not display them in the Updates tab.&nbsp;They are selected by default: 

   | Option |Description  |
   |---|---|
   | Progress Updates |Displays information about the history of progress updates on results and activities.  |
   | Comments |Displays comments made by users on the goal.  |
   | Editing History |Displays information about creating and updating the goal, results, and activities.  |

1. (Optional) Click **Details** under a progress or an editing history update to display additional information about the update.

   ![](assets/update-details-in-updates-tab-expanded-highlighted-350x139.png)

-->



1. Klicka på namnet på ett mål i mållistan och klicka sedan på namnet på ett mål.

   Då öppnas avsnittet **Målinformation** till vänster.

   ![](assets/goal-page-unshimmed.png)

1. Klicka på ikonen **Redigera** ![](assets/edit-icon.png) i det övre högra hörnet och klicka sedan på **Redigera alla** eller **Översikt**

   eller

   Börja skriva information i ett av de redigerbara fälten i avsnittet Målinformation. Avsnittet kan redigeras.

   >[!IMPORTANT]
   >
   >Alla fält som visas i avsnittet Målinformation kan inte redigeras. Workfront beräknar några av fälten och de är skrivskyddade.

1. Uppdatera eller granska följande fält:

   * **Beskrivning**: Lägg till eller uppdatera information om målet.
   * **Förlopp**: Anger hur stor procentandel av målet som har slutförts hittills. Du kan inte uppdatera förloppet för ett mål manuellt. Målförloppet är en beräkning av alla förloppsindikatorer.
   * **Villkor**: Anger om målet är nytt och inte har uppdaterats ännu, om det är på målet att slutföras i tid eller om det ligger efter. Du kan inte uppdatera villkoret för ett mål. Målets villkor beräknas automatiskt av Worfront.\
     Mer information om målvillkor och -förlopp finns i
     [Översikt över målförlopp och villkor i Adobe Workfront-mål](../goal-management/calculate-goal-progress.md).
   * **Status**: Du kan inte uppdatera status för ett mål manuellt. Mer information finns i [Översikt över målstatus i Adobe Workfront-mål](../goal-management/goal-status-overview.md).
   * **Målägare**: Klicka för att uppdatera namnet på målets ägare. Börja skriva namnet på en användare, ett team, en grupp eller namnet på din organisation och markera den sedan när den visas i listan. Du kan bara ha en ägare för ett mål.
   * **Överordnat mål**: Börja skriva namnet på ett mål som du vill ange som överordnat mål för det mål som du har valt. Förloppet för det valda målet uppdaterar automatiskt förloppet för det överordnade målet.

     >[!TIP]
     >
     >Du kan inte uppdatera följande information om ett överordnat mål:
     >    * Överordnad målperiod
     >    * Förlopp för överordnat mål
     >    * Överordnad målägare.
     >      
     >Du måste uppdatera den här informationen om det överordnade målet.

   * **Period**: Klicka för att uppdatera tidsperioden för målet\
     eller\
     Välj **Aktivera anpassade datum** om du vill ange datum för målets **start**- och **slutdatum**.
   * **Stänger anteckningar**: Det här fältet visas bara för mål med statusen Stängt. Det går inte att redigera stängda mål. Om du öppnar ett stängt mål permanent tas slutkommentarerna bort.



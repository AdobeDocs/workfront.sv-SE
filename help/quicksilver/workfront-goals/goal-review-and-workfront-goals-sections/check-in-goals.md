---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Uppdatera målstatus i Adobe Workfront-mål
description: Ni måste regelbundet se över era mål och uppdatera deras framsteg för att se till att de inte hamnar på efterkälken eller riskerar att inte uppnås.
author: Alina
feature: Workfront Goals
exl-id: 5092f508-e52c-4934-a8c1-d0be04ecce13
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 0%

---

# Uppdatera målstatus i Adobe Workfront-mål

<!-- Audited for P&P only: 10/2025-->

Ni måste regelbundet se över era mål och uppdatera deras framsteg för att se till att de inte hamnar på efterkälken eller riskerar att inte uppnås.

<!--And: take this last sentence ^^ out when you update this for goal redesign production.-->

## Åtkomstkrav

>[!NOTE]
>
>Ditt företag kan välja att fortsätta använda Adobe Workfront-mål om de tidigare har köpt det här paketet. Du måste prata med din kontorepresentant för mer information.
>
>Adobe Workfront-mål går inte längre att köpa.

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Adobe Workfront package</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-licens</td>
 <td>
 <p>Medarbetare eller högre</p>
<p>Begäran eller senare</p></td>
 </tr>
  <tr>
 <td role="rowheader">Åtkomstnivåkonfiguration</td>
 <td> <p>Redigera åtkomst till mål</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objektbehörigheter</td>
 <td>
  <div>
  <p>Visa eller högre behörigheter för målet för att visa det</p>
  <p>Hantera behörigheter till målet för att redigera det</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Alla användare, inklusive systemadministratörer, måste tilldelas en layoutmall som innehåller området Mål på huvudmenyn. </p>  
</td>
  </tr>
</tbody>
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
   <p> New product requirement: Workfront</p>
   Or
   <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p></td>
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
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Förutsättningar

Du måste ha ett aktivt mål innan du kan börja.

Du kan inte uppdatera förloppet för mål som är utkast, inaktiva eller stängda.

## Att tänka på vid uppdatering av mål

Tänk på följande när du uppdaterar förloppet för mål:

* Workfront Target beräknar automatiskt förloppet för ett mål när du uppdaterar förloppet för dess förloppsindikatorer.

  >[!TIP]
  >
  >Du kan inte uppdatera förloppet direkt för ett mål. Du måste uppdatera förloppet för målets förloppsindikatorer (aktiviteter, resultat, sammankopplade projekt) som i sin tur uppdaterar förloppet för målet. Om du vill uppdatera förloppet för projekt måste du uppdatera uppgifterna i projektet.

  Se även följande artiklar:

   * Mer information om hur du lägger till aktiviteter i mål finns i [Lägga till aktiviteter i mål i Adobe Workfront-mål](../../workfront-goals/results-and-activities/add-activities-to-goals.md).
   * Mer information om hur du lägger till resultat i mål finns i [Lägga till resultat i mål i Adobe Workfront-mål](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   * Mer information om hur Workfront-mål beräknar förloppet för ett mål finns i [Översikt över målförloppet och villkoret i Adobe Workfront-mål](../../workfront-goals/goal-management/calculate-goal-progress.md).

* Du måste skapa mål och aktivera dem innan du kan uppdatera deras status.

  Se även följande artiklar:

   * Mer information om att skapa mål finns i [Skapa mål i Adobe Workfront-mål](../../workfront-goals/goal-management/create-goals.md).
   * Mer information om hur du aktiverar mål finns i [Aktivera mål i Adobe Workfront-mål](../../workfront-goals/goal-management/activate-goals.md).

  >[!IMPORTANT]
  >
  >Du kan inte uppdatera förloppet för mål som är skrivna, stängda eller inaktiva.

* Första gången du eller någon annan uppdaterar förloppet för ett resultat eller en aktivitet för ett mål, ändras målförloppet från Nytt och Workfront-mål börjar registrera förloppet och statusuppdateringar för förloppet för målet.

<!--

## Update goal progress by using Check-in in the Production environment

>[!IMPORTANT]
>
> <span class="preview"> The Check-in functionality has been removed from the Preview environment and will be removed from Workfront Goals with the 23.1 release. See the [Update goal progress in the Preview environment](#update-goal-progress-in-the-preview-environment) section in this article to update goal progress in Preview. </span>


You can check in on goals at the individual goal level, or you can check in on multiple goals from the Check-in section of Workfront Goals.

* [Update individual goals](#update-individual-goals) 
* [Update goals in the Check-in section](#update-goals-in-the-check-in-section)

### Update individual goals {#update-individual-goals}

When you check in on a goal at the goal level, you can update the progress of the results and activities that are assigned to you or other users.

For information about how to update additional information about results and activities, see [Edit results and activities in Adobe Workfront Goals](../../workfront-goals/results-and-activities/edit-results-and-activities.md).

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area.

   All goals display by default. 

1. (Optional) Click any of the following sections in the left panel to access a list of goals:

   * Goal Alignment 
   * Pulse 
   * Check-in

   Or

   From the Goal List, click the name of a goal to open the **Goal Details** panel on the right.

   >[!TIP]
   >
   >You must have Edit access to Goals in your Access Level to view the Check-in section or the Check in button.

1. Click **Check in**.

   ![Check in link](assets/check-in-link-inside-goal-details-highlighted-350x156.png)

   The progress of results and activities becomes editable.

1. Update the current progress on each of the results. Depending on what type of result you selected, you can do one of the following:

   * Update the quantity 
   * Update the currency amount
   * Update the percent complete

1. Update the percent complete on the Manual progress bar activity.

   >[!TIP]
   >
   >When you add projects as activities to your goals, you cannot manually update projects at the goal level. Workfront automatically updates project progress based on the project of their tasks. When the project percent complete updates in Workfront, the goal progress associated with the project also updates automatically.

1. Click **Back to Summary** to return to the Goal Details panel.

   Your goal progress updates as you update the results and activities of your goal. 

1. Click the **X icon** in the upper-right corner of the Goal Details panel to close it.

### Update goals in the Check-in section {#update-goals-in-the-check-in-section}

You can use the Check-in section to check in on goals when you want to quickly provide updates for several goals at the same time.

>[!TIP]
>
>You can access the Check-in section from any of the following sections:
>
>* Goal List 
>* Goal Alignment 
>* Pulse 
>

When you check in on a goal in the Check-in section, you can update the progress of the results and activities that are assigned only to you. You cannot update the progress of results and activities that are assigned to other users in this section.

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List section displays by default. 

1. Click Check-in in the left panel.

   Or

   (Conditional) If you are in the Goal List, Goal Alignment, or Pulse sections, click the **Check in** button in the upper-right of the screen. This opens the Check-in section.

   ![Check in button](assets/check-in-button-highlighted-350x102.png)

   Goals display in a list and results and activities are listed under each goal.

   ![Check in page](assets/check-in-page-with-show-all-aligned-goals-link-350x178.png)

1. (Optional) Click **Show all results**, **Show all activities**, or **Show all aligned goals** to the far right of the goal name to display all results, activities, and aligned goals of a goal whose progress you want to update.

   >[!CAUTION]
   >
   >You cannot directly update aligned goals, but you can update their results and activities.

1. Update the current progress on each of the results assigned to you. Depending on what type of result you selected, you can do one of the following:

   * Update the quantity 
   * Update the currency amount
   * Update the percent complete

   The result and the goal progress updated automatically and you receive a confirmation of your changes.

1. Update the percent complete on your Manual progress bar activity.

   >[!TIP]
   >
   >When you add projects as activities to your goals, you cannot manually update projects at the goal level. Workfront automatically updates project progress based on the project of their tasks. When the project percent complete updates in Workfront, the goal progress associated with the project also updates automatically.

   The activity and the goal progress updated automatically and you receive a confirmation of your changes.

1. (Optional) Add a comment for your goal, then click **Post** to save your comment.

-->

Så här uppdaterar du förloppet för mål:

1. Klicka på ikonen **Huvudmeny** ![Huvudmeny &#x200B;](assets/main-menu-icon.png) > **Mål** i det övre högra hörnet.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Detta öppnar mållistan. Alla mål som du har åtkomst till för att visa som standard.

   Du kan också klicka på Måljustering på den vänstra panelen.

1. Öppna målsidan genom att klicka på namnet på ett mål i mållistan.
1. Klicka på **Förloppsindikatorer** i den vänstra panelen.

   I listan med förloppsindikatorer visas alla förloppsindikatorer för det mål du valt.

   >[!NOTE]
   >
   >  * Du kan bara uppdatera resultat och aktiviteter.
   >  * Du måste uppdatera förloppsindikatorerna för barnens mål för att visa framsteg för barnens mål.
   >  * Du måste uppdatera uppgifterna i de anslutna projekten för att visa förloppet för projekten.
   >   
   >    De underordnade målens framsteg och projektens förlopp driver i sin tur förloppet för det valda målet.


1. Om du vill uppdatera förloppet för ett resultat eller en aktivitet klickar du på värdet i kolumnen **Faktiskt förlopp** för resultatet eller aktiviteten och skriver ett tal för att uppdatera värdet. Tryck sedan på Retur.

   ![Faktisk status](assets/actual-progress-result-updating-highlighted-unshimmed.png)

   Förloppsindikatorn för förloppsindikatorn i kolumnen Förlopp och förloppet för målet i målhuvudet uppdateras omedelbart.


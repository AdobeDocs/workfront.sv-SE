---
product-previous: workfront-goals
navigation-topic: goal-management
title: Stäng och öppna mål igen i Adobe Workfront-mål
description: Du kan stänga ett mål när du vill ange att du har slutfört det eller att du inte längre arbetar med det eftersom det blev föråldrat.
author: Alina
feature: Workfront Goals
exl-id: bbb549c1-aea6-4f5e-8a6b-01fc04cf06ef
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 0%

---

# Stäng och öppna mål igen i Adobe Workfront-mål

<!--Audited for P&P only: 4/2025-->

Du kan stänga ett mål när du vill ange följande:

* Målet är klart, antingen för att du uppnådde det eller för att tidsperioden gick ut.
* Ni arbetar inte längre på det och tänker inte heller göra det i den närmaste framtiden.

Du kan öppna mål som har stängts igen när de blir relevanta igen.

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
 <tr>
 <td role="rowheader">Adobe Workfront-licens</td>
 <td>
 <p>Medarbetare eller högre</p>
 <p>Begäran eller senare</p></td>
 </tr>
 <td role="rowheader">Åtkomstnivåkonfiguration</td>
 <td> <p>Redigera åtkomst till mål</p> </td>
 </tr>
 <tr>
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
 <p>Or</p>
  <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
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

## Överväganden när mål stängs eller öppnas igen

* Du måste ha tillgång till Redigera mål på åtkomstnivån innan du kan stänga och öppna mål igen. Mer information om att bevilja åtkomst till mål finns i [Bevilja åtkomst till Adobe Workfront-mål](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).
* Du kan bara stänga aktiva mål. Du kan inte stänga mål som har statusen Utkast.

  Mer information om målstatus finns i [Översikt över målstatus i Adobe Workfront-mål](../../workfront-goals/goal-management/goal-status-overview.md).

* Att stänga mål låser sig i utvecklingen och gör att du kan betygsätta hur bra du har lyckats med det.

  >[!CAUTION]
  >
  >När ett mål som har aktiva bidragande mål stängs ändras dess förlopp efter att det stängts för att ange förloppet för de bidragande aktiva målen. Mer information om att justera mål finns i [Justera mål genom att koppla dem i Adobe Workfront-mål](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

* Uppdatera målets förloppsindikatorer innan du stänger målet för att se till att det avslutas med ett korrekt förloppsvärde. Om alla förloppsindikatorer har uppnåtts bör målprocenten vara 100 % och ditt mål har uppnåtts. Mer information om hur du uppdaterar dina mål finns i [Uppdatera målförloppet i Adobe Workfront-mål](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).
* Lämna eventuella slutkommentarer som en uppdatering av de mål som du stänger. Mer information om hur du lägger till kommentarer i mål finns i [Hantera målkommentarer i Adobe Workfront-mål](../../workfront-goals/goal-management/manage-goal-comments.md).
* Du kan inte längre uppdatera förloppet för resultat och aktiviteter för ett mål som du stänger.
* Du kan öppna ett stängt mål igen om du vill fortsätta arbeta med det.
* Om målet inte har uppnåtts bör du överväga att kopiera merparten av informationen till nästa tidsperiod (kvartal eller år). Det här är ett bra alternativ för mål som är desamma från en tidsperiod till nästa eller mål som du kanske måste arbeta med att uppnå inom nästa tidsram. Mer information om kopieringsmål finns i [Kopiera mål i Adobe Workfront-mål](../../workfront-goals/goal-management/copy-goals.md). Du kan även uppdatera tidsperioden för målet i stället för att kopiera den till en annan period.
* Workfront tar bort kommentarerna för ett stängt mål när du öppnar det igen. Om du måste behålla kommentarerna rekommenderar vi att du kopierar det stängda målet inklusive eventuella resultat som är kopplade till det, i stället för att öppna det igen.


## Nära mål

<!--
Closing goals differs depending on what environment you use. 

### Close goals in the Production environment

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are active.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md). 

1. Click an active goal.

   The Goal Details panel displays on the right. 

1. (Optional and recommended) Click the **Updates** tab and add an update in the **Comment here** field about the reason you are closing the goal, then click **Post**. 

1. Click the **More icon** ![More icon](assets/more-icon.png) to the right of the goal name, then click **Close** > **Close Goal**.

   This closes the goal and saves the current progress on the goal and its results and activities.

   >[!IMPORTANT]
   >
   >If the goal has contributing goals that are still active, the progress of the goal continues to update based on the progress of the aligned goals.
   >
   >
   >![Closing goals with active aligned goals](assets/closing-goals-with-active-aligned-goals-warning-350x71.png)   >
   >

1. (Optional) Modify your filters again to display only closed goals. The goals you closed display on the screen.
-->

1. Klicka på ikonen **Huvudmeny** ![Huvudmeny &#x200B;](assets/main-menu-icon.png) > **Mål** i det övre högra hörnet.

   Mållistan öppnas.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Valfritt) Ändra filtren så att endast aktiva mål visas.

   Mer information om filtrering av information i Workfront-mål finns i [Filtrera information i Adobe Workfront-mål](../goal-management/filter-information-wf-goals.md).
1. Klicka på ett aktivt mål.

   Målsidan öppnas.

   ![Målsida](assets/goal-page-unshimmed.png)
1. Klicka på **Mer**-menyn ![Mer-ikonen](assets/more-icon.png) till höger om målnamnet och klicka sedan på **Stäng**.

   Målet stängs och du får en bekräftelse i skärmens övre högra hörn.

   ![Slutbekräftelse för mål](assets/goal-close-confirmation-with-add-closing-notes-link.png)

1. (Valfritt) Klicka på **Lägg till slutkommentarer** i bekräftelserutan om du vill lägga till kommentarer om det här målet och varför du måste stänga det.
1. Lägg till slutkommentarer och klicka sedan på **Lägg till anteckningar**.

   ![Lägg till slutkommentarsruta](assets/add-closing-notes-box-unshimmed.png)

   Kommentarerna visas i målinformationsavsnittet på målsidan i området Stäng anteckningar.

   >[!NOTE]
   >
   >Workfront tar bort slutkommentarerna om du senare öppnar ett stängt mål igen.


## Öppna mål igen

Du kan öppna stängda mål igen om du anser att de har blivit relevanta igen och att du måste fortsätta uppdatera deras framsteg.

<!--
Reopening goals differs depending on what environment you use.

### Reopen goals in the Production environment

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are closed.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).


1. Click a closed goal.

   This opens the Goal Details panel on the right. 

1. Click the **More icon** ![More icon](assets/more-icon.png) to the right of the goal name, then click **Reopen** > **Reopen**.

   This reopens the goal and places it in a status of Active. The progress of the goal is recalculated starting with the current date. 

1. (Optional) Modify your filters again to display only active goals. The goals you opened display on the screen.

-->

1. Klicka på ikonen **Huvudmeny** ![Huvudmeny &#x200B;](assets/main-menu-icon.png)> **Mål** i det övre högra hörnet.

   Mållistan öppnas.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Valfritt) Ändra filtren så att endast stängda mål visas.

   Mer information om filtrering av information i Workfront-mål finns i [Filtrera information i Adobe Workfront-mål](../goal-management/filter-information-wf-goals.md).
1. Klicka på namnet på ett stängt mål.

   Målsidan öppnas.
1. Klicka på ikonen **Mer** meny ![Mer](assets/more-icon.png) till höger om målnamnet och **Öppna** igen > **Öppna igen**.

   Följande saker händer:
   * Målet är nu öppet och har statusen Aktiv.
   * Förloppet för målet beräknas om med början på aktuellt datum.
   * Eventuella slutkommentarer tas bort från sidan Målinformation. Borttagna slutkommentarer kan inte återställas.

1. (Valfritt) Ändra filtren igen så att endast aktiva mål visas.

   De mål som du öppnade visas på skärmen.


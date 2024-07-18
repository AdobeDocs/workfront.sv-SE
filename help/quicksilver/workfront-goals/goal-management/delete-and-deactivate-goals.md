---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Ta bort och inaktivera mål i Adobe Workfront-mål
description: När du börjar arbeta med ett mål och det blir irrelevant i din organisation rekommenderar vi att du inaktiverar det i stället för att ta bort det. När du inaktiverar ett mål behålls den historiska informationen och du kan återaktivera den vid ett senare tillfälle. Det kan dock finnas tillfällen då det kan vara bra att ta bort ett mål så att mållistan hålls korrekt.
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 0%

---

# Ta bort och inaktivera mål i Adobe Workfront-mål

När du börjar arbeta med ett mål och det blir irrelevant i din organisation rekommenderar vi att du inaktiverar det i stället för att ta bort det. När du inaktiverar ett mål behålls den historiska informationen och du kan återaktivera den vid ett senare tillfälle. Det kan dock finnas tillfällen då det kan vara bra att ta bort ett mål så att mållistan hålls korrekt.

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
  <ul><li>En Ultimate-plan </li>
  eller
  <li>Ytterligare en licens för Adobe Workfront Goals för Prime- eller Select Adobe Workfront-planerna. </li></ul> </p>
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
 <p>Aktuell licens: Begär eller högre</p> </td>
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
 <td role="rowheader"><p>Åtkomstnivå</p></td>
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

## Inaktivera mål

Du kan inaktivera ett mål som inte längre är relevant och som du kanske vill återaktivera i framtiden.

* [Att tänka på när du inaktiverar mål](#considerations-when-deactivating-goals)
* [Inaktivera mål](#deactivate-goals)

### Att tänka på när du inaktiverar mål

Tänk på följande när du inaktiverar mål:

* Du kan bara inaktivera mål med statusen Aktiv. Mer information om hur du aktiverar ett mål finns i [Aktivera mål i Adobe Workfront-mål](../../workfront-goals/goal-management/activate-goals.md).

  >[!TIP]
  >
  >Du kan inte inaktivera mål med statusen Utkast.

* Workfront stoppar beräkningen av förloppet för inaktiverade mål.
* Inaktiva mål visas inte längre på eller tas med i diagramavsnittet för Workfront-mål. Mer information om Workfront-måldiagram finns i [Granska diagram för att förstå målförloppstrender i Adobe Workfront-mål](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goal-graphs.md).

  <!--* The Check-in section. For information about the Check-in page, see [Update goal progress in Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md). -->

* Du kan inte längre uppdatera inaktiverade mål.
* Du kan redigera information om målet och dess justering.
* Du kan återaktivera ett tidigare inaktiverat mål.

### Inaktivera mål

<!--
Deactivating goals differs depending on which environment you use.

### Deactivate goals in the Production environment


1. Go to the goal that you want to deactivate.

   For example, go to the Goal List and click the name of a goal.

   The Goal Details panel opens on the right.

   >[!TIP]
   >
   >You can open goals from any sections of Workfront Goals.

1. Click the **More icon** ![](assets/more-icon.png), then click **Deactivate**.

   ![](assets/deactivate-goal-highlighted.png)

   The goal status changes to Inactive. 

1. Click the **X** icon in the upper-right to close Goal Details.
-->

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **Mål**.

   Mållistan visas.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Valfritt) Ändra filtren så att endast aktiva mål visas.

   Mer information om filtrering av information i Workfront-mål finns i [Filtrera information i Adobe Workfront-mål](../goal-management/filter-information-wf-goals.md).

1. Klicka på ett aktivt mål.

   Målsidan öppnas.

   ![](assets/goal-page-unshimmed.png)

1. Klicka på menyn **Mer** ![](assets/more-icon.png) till höger om målnamnet och klicka sedan på **Inaktivera**.

1. Målet inaktiveras och dess status blir Inaktiv.

## Ta bort mål

Du kan ta bort mål som inte längre är eller aldrig är relevanta.

* [Saker att tänka på när du tar bort mål](#considerations-when-deleting-goals)
* [Ta bort mål](#delete-goals)

### Att tänka på när du tar bort mål {#considerations-when-deleting-goals}

* Du kan ta bort mål oavsett status, inklusive stängda mål.
* Du kan inte återställa borttagna mål.
* Resultat och manuella förloppsindikatoraktiviteter som är kopplade till målet tas också bort.
* Projekt som är kopplade till mål tas inte bort, men deras koppling till målet tas bort.

### Ta bort mål

<!--
Deleting  goals differs depending on which environment you use.

#### Delete goals in the Production environment

1. Go to the goal that you want to delete.

   For example, go to the Goal List and click a goal.

   The Goal Details panel opens on the right. 

1. Click the **More icon** ![](assets/more-icon.png), then click **Delete**.

   ![](assets/delete-goal-highlighted.png)

1. Click **Yes, delete**.

   The goal is removed from the Goal List and cannot be recovered.
-->

1. Klicka på ikonen Huvudmeny ![](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **Mål**.

   Mållistan visas.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. Klicka på namnet på ett mål. Målsidan öppnas.
1. Klicka på menyn **Mer** ![](assets/more-icon.png) till höger om målnamnet, klicka på **Ta bort mål** och sedan på **Ta bort**.

   Målet och dess aktiviteter och resultat tas också bort och kan inte återställas. Projekt som var associerade med målet eller de underordnade målen tas inte bort.



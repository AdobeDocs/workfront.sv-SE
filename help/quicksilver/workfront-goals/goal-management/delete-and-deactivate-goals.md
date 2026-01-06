---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Ta bort och inaktivera mål i Adobe Workfront-mål
description: När du börjar arbeta med ett mål och det blir irrelevant i din organisation rekommenderar vi att du inaktiverar det i stället för att ta bort det. När du inaktiverar ett mål behålls den historiska informationen och du kan återaktivera den vid ett senare tillfälle. Det kan dock finnas tillfällen då det kan vara bra att ta bort ett mål så att mållistan hålls korrekt.
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# Ta bort och inaktivera mål i Adobe Workfront-mål

<!--Audited for P&P only: 10/2025-->

När du börjar arbeta med ett mål och det blir irrelevant i din organisation rekommenderar vi att du inaktiverar det i stället för att ta bort det. När du inaktiverar ett mål behålls den historiska informationen och du kan återaktivera den vid ett senare tillfälle. Det kan dock finnas tillfällen då det kan vara bra att ta bort ett mål så att mållistan hålls korrekt.

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
 <tr>
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

1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Deactivate**.

   ![Deactivate goal](assets/deactivate-goal-highlighted.png)

   The goal status changes to Inactive. 

1. Click the **X** icon in the upper-right to close Goal Details.
-->

{{step1-to-goals}}

Mållistan visas.


1. (Valfritt) Ändra filtren så att endast aktiva mål visas.

   Mer information om filtrering av information i Workfront-mål finns i [Filtrera information i Adobe Workfront-mål](../goal-management/filter-information-wf-goals.md).

1. Klicka på ett aktivt mål.

   Målsidan öppnas.

   ![Målsida](assets/goal-page-unshimmed.png)

1. Klicka på **Mer**-menyn ![Mer-ikonen](assets/more-icon.png) till höger om målnamnet och klicka sedan på **Inaktivera**.

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

1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Delete**.

   ![Delete goal](assets/delete-goal-highlighted.png)

1. Click **Yes, delete**.

   The goal is removed from the Goal List and cannot be recovered.
-->

{{step1-to-goals}}

Mållistan visas.

1. Klicka på namnet på ett mål. Målsidan öppnas.
1. Klicka på ikonen **Mer** meny ![Mer](assets/more-icon.png) till höger om målnamnet, klicka på **Ta bort mål** och sedan på **Ta bort**.

   Målet och dess aktiviteter och resultat tas också bort och kan inte återställas. Projekt som var associerade med målet eller de underordnade målen tas inte bort.



---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Ta bort och inaktivera mål i Adobe Workfront-mål
description: När du börjar arbeta med ett mål och det blir irrelevant i din organisation rekommenderar vi att du inaktiverar det i stället för att ta bort det. När du inaktiverar ett mål behålls den historiska informationen och du kan återaktivera den vid ett senare tillfälle. Det kan dock finnas tillfällen då det kan vara bra att ta bort ett mål så att mållistan hålls korrekt.
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# Ta bort och inaktivera mål i Adobe Workfront-mål

När du börjar arbeta med ett mål och det blir irrelevant i din organisation rekommenderar vi att du inaktiverar det i stället för att ta bort det. När du inaktiverar ett mål behålls den historiska informationen och du kan återaktivera den vid ett senare tillfälle. Det kan dock finnas tillfällen då det kan vara bra att ta bort ett mål så att mållistan hålls korrekt.

## Åtkomstkrav

<!--drafted for P&P release: 

You must have the following:

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

Du måste ha följande:

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
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till mål eller högre</p> <p><b>ANMÄRKNING</b>

<p>Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra din åtkomstnivå finns i:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Bevilja åtkomst till Adobe Workfront-mål</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> 
    <div> 
     <p>Hantera behörigheter för målet</p> 
     <p>Mer information om delningsmål finns i <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Dela ett mål i Workfront-mål</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Du måste ha följande innan du kan börja:

* En layoutmall som innehåller området Mål på huvudmenyn.

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
* Inaktiva mål visas inte längre på eller tas med i diagramavsnittet för Workfront-mål. Mer information om Workfront-måldiagram finns i [Granska diagram för att förstå målutvecklingstrender i Adobe Workfront-mål](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goal-graphs.md).

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

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **Mål**.

   Mållistan visas.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Valfritt) Ändra filtren så att endast aktiva mål visas.

   Information om filtrering av information i Workfront-mål finns i [Filtrera information i Adobe Workfront mål](../goal-management/filter-information-wf-goals.md).

1. Klicka på ett aktivt mål.

   Målsidan öppnas.

   ![](assets/goal-page-unshimmed.png)

1. Klicka på **Mer** meny ![](assets/more-icon.png) till höger om målnamnet och klicka sedan på **Inaktivera**.

1. Målet inaktiveras och dess status blir Inaktiv.

## Ta bort mål

Du kan ta bort mål som inte längre är eller aldrig är relevanta.

* [Att tänka på när du tar bort mål](#considerations-when-deleting-goals)
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
1. Klicka på **Mer** meny ![](assets/more-icon.png) till höger om målnamnet och klicka sedan på **Ta bort mål** sedan **Ta bort**.

   Målet och dess aktiviteter och resultat tas också bort och kan inte återställas. Projekt som var associerade med målet eller de underordnade målen tas inte bort.



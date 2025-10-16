---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Ta bort förloppsindikatorer från mål i Adobe Workfront
description: Du kan ta bort resultat, aktiviteter och projekt från mål i Adobe Workfront när de inte längre är relevanta.
author: Alina
feature: Workfront Goals
exl-id: 0e064dbd-6168-47b4-98ab-b5c0481e839e
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Ta bort förloppsindikatorer från mål i Adobe Workfront

<!-- for goal redesign PRODUCTION RELEASE: Should this article be called "Remove or disconnect progress indicators from goals" when this is available to ALL progress indicators (including "disconnect goals")-- if yes, updte the title everywhere else where this is linked?
-->

Du kan ta bort resultat, aktiviteter och projekt från mål om de inte längre är relevanta.

Mer information om hur du skapar mål och lägger till resultat och aktiviteter till dem finns i följande artiklar:

* [Skapa mål i Adobe Workfront-mål](../../workfront-goals/goal-management/create-goals.md)
* [Lägg till aktiviteter i mål i Adobe Workfront-mål](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
* [Lägg till resultat i mål i Adobe Workfront ](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Redigera resultat och aktiviteter i Adobe Workfront-mål](../../workfront-goals/results-and-activities/edit-results-and-activities.md)

Mål kan också anpassas till överordnade mål och bli underordnade mål. Underordnade mål är också förloppsindikatorer för de överordnade målen.

Du kan ta bort justeringen mellan mål genom att ta bort kopplingen mellan dem. Mer information finns i [Ta bort måljustering i Adobe Workfront-mål](../goal-alignment/remove-goal-alignment.md).

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
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
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

## Förutsättningar

Du måste ha ett mål som är associerat med resultat, aktiviteter eller projekt.

## Att tänka på när du vill ta bort resultat, aktiviteter och koppla bort projekt från mål

* Du kan bara ta bort resultat och aktiviteter från aktiva mål.
* Du kan ta bort resultat och aktiviteter från ett mål genom att ta bort dem. Borttagna resultat och aktiviteter kan inte återställas.
* När du tar bort resultatet eller aktiviteten från ett mål påverkar förloppet för det borttagna resultatet eller aktiviteten det övergripande förloppet för målet.
* Du kan inte ta bort ett projekt från ett mål, men du kan koppla bort det från målet. När du kopplar från projektet från målet påverkas inte längre projektets förlopp i procent.

  Mer information om hur projekt påverkar målförloppet finns i [Lägga till projekt i mål i Adobe Workfront-mål](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

* Du kan inte ta bort ett resultat eller en aktivitet från ett mål, och du kan inte koppla från ett underordnat mål eller ett projekt, om det är den sista förloppsindikatorn för målet.
* Om ett projekt tas bort från projektområdet och det är den sista förloppsindikatorn för ett mål, blir målet inaktivt.

## Ta bort resultat och aktiviteter från mål

Du tar bort resultat och aktiviteter från ett mål genom att ta bort dem. Att ta bort resultat och aktiviteter från ett mål är identiskt.

<!--
How you delete results and activities differs depending on the environment you use.

### Delete results and activities in the Production environment


1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click **Results** to remove results or **Activities** to remove activities. 

1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the result or activity name, then click **Delete** > **Yes, delete**.

   ![Delete result](assets/delete-result-goal-details-350x108.png)

   The result or activity is deleted and cannot be recovered. The percent complete of the goal updates to exclude the deleted activity or result.

-->

1. Klicka på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **Mål**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
   Detta öppnar området Workfront-mål och mållistan visas som standard.

1. Klicka på namnet på ett mål som du vill ta bort resultat och aktiviteter från.

   Målsidan öppnas.

1. Klicka på **Förloppsindikatorer** i den vänstra panelen.

1. Markera ett resultat eller en aktivitet och klicka sedan på ikonen **Ta bort** ![Ta bort](assets/delete-icon.png) överst i listan.

1. Klicka på **Ta bort** för att bekräfta borttagningen. Resultatet eller aktiviteten tas bort och kan inte återställas. Procent färdigt av måluppdateringarna som ska exkludera den borttagna aktiviteten eller det borttagna resultatet.


## Ta bort projekt från mål

<!--
Dsconnecting projects from goals differs depending on the environment you use.

### Disconnect projects from goals in the Production environment


1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click the **right-pointing arrow** to the left of the Activities sections to expand it. 
1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the project name, then click **Disconnect**.

   ![Disconnect](assets/disconnect-project-goal-details-350x94.png)

   The project is disconnected from the goal. The percent complete of the goal updates to exclude the percent complete of the disconnected project.
-->


1. Klicka på ikonen **Huvudmeny** i det övre högra hörnet och klicka sedan på **Mål**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Detta öppnar området Workfront-mål och mållistan visas som standard.

1. Klicka på namnet på ett mål som du vill ta bort resultat och aktiviteter från.

   Målsidan öppnas.
1. Klicka på **Förloppsindikatorer** i den vänstra panelen.
1. Markera ett projekt och klicka sedan på ikonen **Koppla från** ![Koppla från](assets/disconnect-icon.png) högst upp i listan.
1. Bekräfta genom att klicka på **Koppla från**.

   Projektet är inte längre anslutet till målet. Procent färdigt av måluppdateringarna som ska exkludera det frånkopplade projektet.


---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Ta bort måljustering i Adobe Workfront-mål
description: Du kan ta bort justeringen mellan två mål om det inte längre är lämpligt att koppla ihop dem.
author: Alina
feature: Workfront Goals
exl-id: a6196356-ca11-4759-9cff-64850a60208e
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Ta bort måljustering i Adobe Workfront-mål

<!--Audited P&P only: 4/2025-->

Du kan ta bort justeringen mellan två mål om det inte längre är lämpligt att koppla ihop dem.

Mer information om hur du justerar mål finns i följande artiklar:

* [Justera mål genom att ansluta dem i Adobe Workfront-mål](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)
* [Justera mål genom att konvertera resultat och aktiviteter till mål](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md)

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
 <p>Begäran eller senare</p> </td>
 </tr>
  <tr>
 <td role="rowheader">Åtkomstnivå</td>
 <td> <p>Redigera åtkomst till mål</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Objektbehörigheter</td>
 <td>
  <p>Visa eller högre behörigheter för målet för att visa det</p>
  <p>Hantera behörigheter till målet för att redigera det</p>

</td>
 </tr>
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
 <p>Current license: Request or higher</p> </td>
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
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </td>
 </tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Förutsättningar

Du måste ha följande innan du kan börja:

* Ett överordnat mål som har minst ett underordnat mål kopplat till sig. Barnens mål är målets förloppsindikatorer.

## Att tänka på när du tar bort måljustering

Tänk på följande när du tar bort justeringen mellan två mål:

* Det överordnade målet måste ha ett annat associerat mål, en annan aktivitet eller ett annat resultat för att kunna förbli aktivt.
* Du kan inte ta bort ett justerat underordnat mål från ett överordnat mål om det är den enda förloppsindikatorn för det överordnade målet.
* Det underordnade målet blir ett fristående mål när du tar bort dess justering till det överordnade målet.

## Ta bort måljustering

<!--
Removing goal alignment differs depending on which environment you use.

### Remove goal alignment in the Production environment


1. Go to a child goal aligned to a parent goal. 
1. Click the goal name to open the **Goal Details** panel. 
1. Click the **gear icon** ![Gear icon](assets/gear-icon-settings.png) next to the parent goal, then click **Remove alignment**.

   ![Reove alignment](assets/edit-remove-alignment-350x88.png)

   The goal becomes a standalone goal and its progress no longer influences the progress of the original parent goal. 

1. (Optional) Click **Undo** in the lower-left corner of the screen if you want to revert this change and keep the goals aligned. 
1. (Optional) Add activities and results to either goals to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)
-->

1. Gå till området **Mål** i Workfront och klicka på namnet på ett mål för att öppna målets sida.
1. Klicka på **Förloppsindikatorer** i den vänstra panelen på målets sida för ett överordnat mål.

   ![Flytta om måljustering](assets/remove-goal-alignment-from-list-unshimmed.png)

1. I gruppen **Typ: Mål** väljer du ett mål och klickar sedan på ikonen **Koppla från** ![Koppla från ](assets/disconnect-goal-to-remove-alignment-icon-unshimmed.png) överst i listan.

   Frånkopplingsrutan visas.

1. Klicka på **Koppla från** om du vill koppla från det valda målet från det överordnade målet.

   Målet blir ett fristående mål och visas inte längre som en förloppsindikator för det ursprungliga målet. Förloppet för det bortkopplade målet påverkar inte längre förloppet för det ursprungliga målet.

   Ett meddelande om att åtgärden lyckades visas i det övre högra hörnet på sidan för att bekräfta att målet var frånkopplat.

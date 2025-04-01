---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Ta bort måljustering i Adobe Workfront-mål
description: Du kan ta bort justeringen mellan två mål om det inte längre är lämpligt att koppla ihop dem.
author: Alina
feature: Workfront Goals
exl-id: a6196356-ca11-4759-9cff-64850a60208e
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---

# Ta bort måljustering i Adobe Workfront-mål

<!--Audited P&P only: 4/2025-->

Du kan ta bort justeringen mellan två mål om det inte längre är lämpligt att koppla ihop dem.

Mer information om hur du justerar mål finns i följande artiklar:

* [Justera mål genom att ansluta dem i Adobe Workfront-mål](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)
* [Justera mål genom att konvertera resultat och aktiviteter till mål](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md)

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
 <p>Aktuell licens: Begär eller högre</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produkt*</td>
 <td>
   <p> Nytt produktkrav: Workfront</p>
   eller
   <p>Aktuellt produktkrav: Förutom en Workfront-licens måste du köpa en licens för Adobe Workfront Goals. </p> <p>Mer information finns i <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Krav för att använda Workfront-mål</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Åtkomstnivå</td>
 <td> <p>Redigera åtkomst till mål</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objektbehörigheter</td>
 <td>
  <p>Visa eller högre behörigheter för målet för att visa det</p>
  <p>Hantera behörigheter till målet för att redigera det</p>
  <p>Mer information om delningsmål finns i <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Dela ett mål i Workfront-mål</a>. </p>
  </td>
 </tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller området Mål på huvudmenyn. </p>  
</td>
  </tr>
</tbody>
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
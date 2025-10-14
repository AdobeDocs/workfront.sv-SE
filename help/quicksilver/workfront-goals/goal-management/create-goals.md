---
product-previous: workfront-goals
navigation-topic: goal-management
title: Skapa mål i Adobe Workfront-mål
description: Oavsett om du är VD, chef eller enskild medverkande kan du skapa mål i Adobe Workfront Target för att anpassa ditt arbete efter dina mål och de mål som skisserar organisationens strategi.
author: Alina
feature: Workfront Goals
exl-id: 14bf48b6-eb0c-4b00-a1a4-0d070ccc1392
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# Skapa mål i Adobe Workfront-mål

<!--Audited for P&P only: 4/2025-->

Oavsett om du är VD, chef eller enskild medverkande kan du skapa mål i Adobe Workfront Target för att anpassa ditt arbete efter dina mål och de mål som skisserar organisationens strategi.

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
  <p> Nytt produktkrav: Workfront</p>
 <p>eller</p>
  <p>Aktuellt produktkrav: Förutom en Workfront-licens måste du köpa en licens för Adobe Workfront Goals. </p> <p>Mer information finns i <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Krav för att använda Workfront-mål</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Åtkomstnivå</td>
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

+++

## Riktlinjer för att skapa mål

Innan du börjar med Workfront-mål rekommenderar vi att du läser om våra rekommendationer och riktlinjer för bästa praxis för att hantera mål effektivt. Mer information om riktlinjer för att skapa och hantera mål finns i [Översikt över Adobe Workfront-mål](../../workfront-goals/goal-management/wf-goals-overview.md).

## Skapa mål

I den här artikeln beskrivs hur du skapar ett strategiskt mål i Workfront-mål. Mer information om hur du skapar ett mål för ett affärsärende finns i [Skapa mål för affärsärende](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

Du kan skapa ett strategiskt mål på något av följande sätt:

* [Skapa ett mål från grunden](#create-a-goal-from-scratch)
* [Kopiera ett befintligt mål](#copy-an-existing-goal)
* [Konvertera ett resultat eller en aktivitet till ett mål](#convert-a-result-or-activity-to-a-goal)

### Skapa ett helt nytt mål {#create-a-goal-from-scratch}

<!--
Creating goals differs depending on what environment you use.

#### Create a goal from scratch in the Production environment 


1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) in the upper right corner, then click **Goals**.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -)

   The Goal List displays.

1. (Conditional) Click **Goal List**, **Graphs**, **Pulse**, or **Check-in** in the left pane, then click **Add Goal** in the upper-right corner of the page. The Add Goal box displays.

   ![Add goal box](assets/add-goal-box-350x235.png)

   >[!TIP]
   >
   >You can add a goal from any section in Workfront Goals. The process for creating a goal is identical regardless of the section you choose to add the goal from.

1. Start typing what you want to achieve in the **Goal** field. This is the name of the goal and a required field. 
1. Select a time period when the goal should be executed in the **Period** drop-down menu. This is a pre-filled field. The default is the current quarter.

   Select from the following predefined options:

   * The current year
   * The quarters of the current year
   * The next two years
   * The quarters of the next two years

   Or

   Click **Define custom dates** to select a custom time frame. 

1. (Conditional) Select a **Start date** and an **End date** for your goal, if you clicked **Define custom dates**.

   >[!TIP]
   >
   >* You can create a goal with dates in any time period, including up to 2 years in the past. 
   >* When defining custom dates, they are constrained by the initial date you selected. So if you select quarter and then custom dates, you can't go beyond that quarter.

1. (Optional) Click **Reset custom dates** to return to the predefined options.

   >[!TIP]
   >
   >We recommend that everyone in your organization selects the same timeframes for similar goals or goals that are aligned. This provides better alignment between goals and ensures that everyone's work supports your over-arching strategy.

1. (Optional) Click your name in the **Owner** field, if you want to indicate someone else as the owner of the goal. By default, you are the owner of goals you create. 
1. Start typing the name of a user, team, group, or the name of your organization in the **Owner** field, then select it when it displays in the list. You can have only one owner for a goal. 
1. (Optional) Enter a **Description** for the goal. This field is optional. 
1. Click **Save**.

   The status of the new goal is Draft.

   >[!IMPORTANT]
   >
   >You must associate a goal with a progress indicator to activate it and start working on it. 
   >
   >Do at least one of the following to be able to activate a goal: 
   >
   >* Add a Result
   >
   >  For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   >   
   >* Add an Activity
   >   
   >  For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 
   >   
   >* Align another goal to it
   >   
   >  For information about aligning goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

1. Click the **X** icon in the upper-right of the Goal Details panel to close it.

-->

1. Klicka på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **Mål**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Mållistan visas.
1. Klicka på **Nytt mål**.

   Rutan Nytt mål visas.

   ![Ny målruta](assets/new-goal-box-unshimmed.png)

1. Ange information i följande fält:
   * **Målnamn**: Ange ett namn för målet. Detta är ett obligatoriskt fält.
   * **Period**: Välj ett fördefinierat kvartal eller år i listrutan **Period**

     eller

     Välj alternativet **Aktivera anpassade datum** och välj sedan ett **Start** och **slutdatum** för målet.

     Föregående, innevarande och följande år och deras respektive kvartal listas som fördefinierade alternativ i listrutan Period.

     Målets period anger tidsramen när du förväntar dig att målet ska slutföras.

   * **Målägare**: Börja skriva namnet på en användare, ett team, en grupp eller din organisation för att ange vem som är ägare till målet. Som standard är du markerad som ägare av målet.
   * **Beskrivning**: Ange ytterligare information om målet.
1. Klicka på **Skapa mål**.

   Det nya målet listas i mållistan och har statusen **Utkast**.

   Du måste associera ett mål med en förloppsindikator för att kunna aktivera det och börja arbeta med det.

   Gör minst något av följande för att förbereda ett mål som ska aktiveras:
   * Lägg till ett resultat

     Mer information om hur du lägger till resultat finns i [Lägga till resultat i mål i Adobe Workfront &#x200B;](../results-and-activities/add-results-to-goals.md).
   * Lägg till en aktivitet

     Mer information om hur du lägger till aktiviteter finns i [Lägga till aktiviteter i mål i Adobe Workfront-mål](../results-and-activities/add-activities-to-goals.md).
   * Justera ett annat mål mot det

     Mer information om att justera mål finns i [Justera mål genom att koppla dem i Adobe Workfront-mål](../goal-alignment/align-goals-by-connecting-them.md).


### Kopiera ett befintligt mål {#copy-an-existing-goal}

Du kan skapa ett mål genom att kopiera en befintlig.

Mer information om kopieringsmål finns i [Kopiera mål i Adobe Workfront-mål](../../workfront-goals/goal-management/copy-goals.md).

### Konvertera ett resultat eller en aktivitet till ett mål {#convert-a-result-or-activity-to-a-goal}

Du kan skapa ett mål genom att konvertera resultatet eller aktiviteten för ett befintligt mål till ett mål. Det nya målet anpassas till det ursprungliga målet.

Mer information om hur du konverterar resultat och aktiviteter till mål finns i [Justera mål genom att konvertera resultat och aktiviteter till mål](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).


---
product-previous: workfront-goals
navigation-topic: goal-management
title: Skapa mål i Adobe Workfront-mål
description: Oavsett om du är VD, chef eller enskild medverkande kan du skapa mål i Adobe Workfront Target för att anpassa ditt arbete efter dina mål och de mål som skisserar organisationens strategi.
author: Alina
feature: Workfront Goals
exl-id: 14bf48b6-eb0c-4b00-a1a4-0d070ccc1392
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '687'
ht-degree: 0%

---

# Skapa mål i Adobe Workfront-mål

Oavsett om du är VD, chef eller enskild medverkande kan du skapa mål i Adobe Workfront Target för att anpassa ditt arbete efter dina mål och de mål som skisserar organisationens strategi.

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
   <td> <p>Redigera åtkomst till mål eller högre</p> <p><b>ANMÄRKNING</b><p>Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra din åtkomstnivå finns i:</p> 
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

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Du måste ha följande innan du kan börja:

* En layoutmall som innehåller området Mål på huvudmenyn.

## Riktlinjer för att skapa mål

Innan du börjar med Workfront-mål rekommenderar vi att du läser om våra rekommendationer och riktlinjer för bästa praxis för att hantera mål effektivt. Mer information om riktlinjer för att skapa och hantera mål finns i [Översikt över Adobe Workfront-mål](../../workfront-goals/goal-management/wf-goals-overview.md).

## Skapa mål

I den här artikeln beskrivs hur du skapar ett strategiskt mål i Workfront-mål. Mer information om hur du skapar ett mål för ett affärsärende finns i [Skapa mål för affärsärenden](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

Du kan skapa ett strategiskt mål på något av följande sätt:

* [Skapa ett helt nytt mål](#create-a-goal-from-scratch)
* [Kopiera ett befintligt mål](#copy-an-existing-goal)
* [Konvertera ett resultat eller en aktivitet till ett mål](#convert-a-result-or-activity-to-a-goal)

### Skapa ett helt nytt mål {#create-a-goal-from-scratch}

<!--
Creating goals differs depending on what environment you use.

#### Create a goal from scratch in the Production environment 


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper right corner, then click **Goals**.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -)

   The Goal List displays.

1. (Conditional) Click **Goal List**, **Graphs**, **Pulse**, or **Check-in** in the left pane, then click **Add Goal** in the upper-right corner of the page. The Add Goal box displays.

   ![](assets/add-goal-box-350x235.png)

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

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **Mål**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Mållistan visas.
1. Klicka **Nytt mål**.

   Rutan Nytt mål visas.

   ![](assets/new-goal-box-unshimmed.png)

1. Ange information i följande fält:
   * **Målnamn**: Ange ett namn för målet. Detta är ett obligatoriskt fält.
   * **Period**: Välj ett fördefinierat kvartal eller år från **Period** nedrullningsbart fält

      eller

      Välj **Aktivera anpassade datum** väljer du ett **Starta** och **Slutdatum** för målet.

      Föregående, innevarande och följande år och deras respektive kvartal listas som fördefinierade alternativ i listrutan Period.

      Målets period anger tidsramen när du förväntar dig att målet ska slutföras.

   * **Målägare**: Börja skriva namnet på en användare, ett team, en grupp eller din organisation för att ange vem som är ägare till målet. Som standard är du markerad som ägare av målet.
   * **Beskrivning**: Ange ytterligare information om målet.
1. Klicka **Skapa mål**.

   Det nya målet listas i listan Mål och har statusen **Utkast**.

   Du måste associera ett mål med en förloppsindikator för att kunna aktivera det och börja arbeta med det.

   Gör minst något av följande för att förbereda ett mål som ska aktiveras:
   * Lägg till ett resultat

      Mer information om hur du lägger till resultat finns i [Lägg till resultat i mål i Adobe Workfront](../results-and-activities/add-results-to-goals.md).
   * Lägg till en aktivitet

      Mer information om hur du lägger till aktiviteter finns i [Lägga till aktiviteter i mål i Adobe Workfront](../results-and-activities/add-activities-to-goals.md).
   * Justera ett annat mål mot det

      Mer information om hur du justerar mål finns i [Justera mål genom att koppla dem till Adobe Workfront mål](../goal-alignment/align-goals-by-connecting-them.md).


### Kopiera ett befintligt mål {#copy-an-existing-goal}

Du kan skapa ett mål genom att kopiera en befintlig.

Mer information om att kopiera mål finns i [Kopiera mål i Adobe Workfront-mål](../../workfront-goals/goal-management/copy-goals.md).

### Konvertera ett resultat eller en aktivitet till ett mål {#convert-a-result-or-activity-to-a-goal}

Du kan skapa ett mål genom att konvertera resultatet eller aktiviteten för ett befintligt mål till ett mål. Det nya målet anpassas till det ursprungliga målet.

Mer information om hur du konverterar resultat och aktiviteter till mål finns i [Justera mål genom att konvertera resultat och aktiviteter till mål](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).


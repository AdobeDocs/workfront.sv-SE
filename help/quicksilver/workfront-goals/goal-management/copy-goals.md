---
product-previous: workfront-goals
navigation-topic: goal-management
title: Kopiera mål i Adobe Workfront-mål
description: Du kan kopiera mål i Adobe Workfront-mål för att skapa ett mål. En del av den ursprungliga målinformationen överförs till det nya målet.
author: Alina
feature: Workfront Goals
exl-id: 690a6030-ee29-4e50-869f-cd014050b364
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 0%

---

# Kopiera mål i Adobe Workfront-mål

Du kan kopiera mål i Adobe Workfront-mål för att skapa ett mål. En del av den ursprungliga målinformationen överförs till det nya målet.

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
 <p> Nytt produktkrav, något av följande: </p>
<ul>
<li>A Select- eller Prime Adobe Workfront-plan och ytterligare licens för Adobe Workfront Goals.</li>
<li>En Ultimate Workfront-plan som innehåller Workfront-mål som standard. </li></ul>
 <p>eller</p>
 <p>Aktuellt produktkrav: En Workfront-plan och ytterligare licens för Adobe Workfront-mål. </p> <p>Mer information finns i <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Krav för att använda Workfront-mål</a>. </p> </td>
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

*Mer information finns på [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Att tänka på när du kopierar mål

Du måste ha tillgång till Redigera mål på åtkomstnivån innan du kan kopiera mål. Mer information om hur du beviljar åtkomst till mål finns i [Ge åtkomst till Adobe Workfront mål](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

Några av orsakerna till att du vill kopiera ett befintligt mål är:

* När du vill återskapa samma mål för nästa period vid slutet av en tidsperiod (kvartal eller år).
* När målet inte kan slutföras i slutet av en tidsperiod och du vill arbeta med det under en annan tidsperiod.
* När flera teammedlemmar har liknande mål och du kan behöva skapa ett för varje mål.

>[!TIP]
>
>Du kan kopiera ett mål med valfri status. Mer information om målstatus finns i [Översikt över målstatus i Adobe Workfront-mål](../../workfront-goals/goal-management/goal-status-overview.md).

Tänk på följande när du kopierar mål:

* All information om målet kopieras också till det nya målet.
* Du kan välja att kopiera resultatet av ett befintligt mål. Namnet på resultatet överförs till det nya målet, men det aktuella förloppet för resultaten på det befintliga målet kopieras inte till det nya målet. De kopierade resultaten tilldelas som standard till samma ägare.

  >[!NOTE]
  >
  >Om den ursprungliga ägaren togs bort eller inaktiverades från Workfront tilldelas det nya resultatet till den inloggade användaren.

* Du kan inte kopiera aktiviteter för ett mål när du kopierar målet.

## Kopiera mål

<!--
Copying goals differs depending on what environment you use. 

To copy goals in the Production environment:

1. Go to a goal and click it to open the Goal Details panel.

   For information about accessing an individual goal, see the "Access individual goals" section in [Access and open goals in Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md).

   This opens the Goal Details panel.

1. Click the **More icon** ![](assets/more-icon.png), then click **Copy**. 

1. Update any of the following information for the copied goal:

   | Field |Description  |
   |---|---|
   | New Goal |The name of the new goal. The default is the name of the original goal.  |
   | Period |The time period during which you want to achieve the goal. Select a time period from the drop-down menu or click **Define custom dates** to indicate a custom time period. By default, the Period is always the current quarter. |
   | Owner |The owner of the goal. It can be a user, team, group, or a company. The default is the owner of the original goal.  |
   | Description |Additional information about the goal.  |

1. (Conditional) Select **Copy results** if the original goal had results added to it and you want to copy them to the new goal. This duplicates the original results to the new goal. The results of the copied goal have the same owner, names and measured values as the results of the original goal.

   >[!TIP]
   >
   >* The progress of the original result does not transfer to the copied goal. 
   >* If the original owner was deleted or deactivated from Workfront, the new result is assigned to the logged in user.

1. Click **Save**.

   The copied goal is saved with a status of Draft and displays in the Goal Details panel.

   >[!IMPORTANT]
   >
   >If you have not copied the results from the original goal, you must first associate the new goal with a progress indicator before you can activate it and start working towards achieving it. 
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
   >
   > For information about activating a goal, see [Activate goals in Adobe Workfront Goals](../goal-management/activate-goals.md). 

1. Click the **X** icon in the upper-right of the Goal Details panel to close it.

   The copied goal displays in the following sections:

   * Goal List 
   * Check-in (after it is activated)
   * Goal Alignment section (after it is activated) 
   * Pulse
(!--drafted - this was important when we could not update the goal timeframe in the past but we can do that now - not needed
1. (Optional and conditional) If you have copied a goal that was not achieved in a previous time period to continue working on it in the following time period, do the following:

   1. Go to the original goal in the Goal List, Check-in page, or Pulse section and comment on the goal, to indicate that this goal was copied to another, more current goal. For information about commenting on a goal, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md).
   1. Close the original goal, to preserve the progress in its original time period. For information about closing goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   1. Update the the **Initial** value of the new Result to match the **End At** value of the previous result, so that your new goal progress will start calculating from the point you achieved in the previous period.
   
-->


1. Gå till ett mål och klicka på **Mer** meny ![](assets/more-icon.png)och sedan klicka **Kopiera mål**.

   ![](assets/copy-goal-box-unshimmed.png)

1. Uppdatera följande information för det kopierade målet:
   * **Målnamn**: Namnet på det nya målet. Standardnamnet för det kopierade målet är &quot;Kopia av &lt;original goal=&quot;&quot;>&quot;.
   * **Period**: Den tidsperiod under vilken du vill uppnå målet. Välj en tidsperiod i listrutan

     eller

     Välj **Aktivera anpassade datum** för att ange anpassade datum för målets **Starta** och **Slutdatum**. Inställningen Aktivera anpassade datum är inaktiverad som standard.

     >[!TIP]
     >
     >   Om du avmarkerar Aktivera anpassade datum återställs det ursprungliga målets tidsperiod.

      * **Målägare**: Ägaren till målet. Det kan vara användare, team, grupp eller företag. Standardvärdet är ägaren till det ursprungliga målet.
      * **Beskrivning**: Ytterligare information om målet.
      * **Kopiera resultat**: Välj det här alternativet om du vill överföra resultaten från det aktuella målet till det kopierade målet. Detta duplicerar de ursprungliga resultaten och kopplar dem till det kopierade målet. Resultatet av det kopierade målet har samma ägare, namn och uppmätta värden som det ursprungliga målets resultat.

        >[!NOTE]
        >
        >* Förloppet för det ursprungliga resultatet överförs inte till det kopierade målet.
        >* Om den ursprungliga ägaren togs bort eller inaktiverades från Workfront tilldelas det nya resultatet till den inloggade användaren.

1. Klicka **Kopiera mål**.

   Ett mål som liknar det ursprungliga skapas och har statusen Utkast.

   >[!NOTE]
   >
   >Om du inte har kopierat resultaten från det ursprungliga målet måste du först koppla det nya målet till en förloppsindikator innan du kan aktivera det och börja arbeta mot att uppnå det.
   >Mer information om hur du associerar mål med förloppsindikatorer finns i följande artiklar:
   >* [Lägga till resultat i mål i Adobe Workfront](../results-and-activities/add-results-to-goals.md)
   >* [Lägga till aktiviteter i mål i Adobe Workfront](../results-and-activities/add-activities-to-goals.md)
   >* [Justera mål genom att koppla dem till Adobe Workfront mål](../goal-alignment/align-goals-by-connecting-them.md)
   >
   >Mer information om hur du aktiverar mål finns i [Aktivera mål](../goal-management/activate-goals.md).


---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Redigera resultat och aktiviteter i Adobe Workfront-mål
description: När Adobe Workfront-administratören har gett dig rätt åtkomst till Adobe Workfront-mål kan du skapa och redigera mål, resultat och aktiviteter.
author: Alina
feature: Workfront Goals
exl-id: 922a05f9-2995-4401-a6d2-e5a331270fd3
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 0%

---

# Redigera resultat och aktiviteter i Adobe Workfront-mål

När Adobe Workfront-administratören har gett dig rätt åtkomst till Adobe Workfront-mål kan du skapa och redigera mål, resultat och aktiviteter.

Mer information om att skapa mål, resultat och aktiviteter finns i följande artiklar:

* [Skapa mål i Adobe Workfront-mål](../../workfront-goals/goal-management/create-goals.md)
* [Kom igång med resultat och aktiviteter i Adobe Workfront-mål](../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md)
* [Lägga till resultat i mål i Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Lägga till aktiviteter i mål i Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md)

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

*Mer information finns på [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Att tänka på när du redigerar resultat och aktiviteter

<!--
According to Vazgen, access levels will add more considerations.)
-->

* Du kan redigera resultat och aktiviteter som tillhör de mål som du har skapat eller mål som du har behörighet att hantera.
* Du kan inte redigera förloppet för projekt som är kopplade till mål som aktiviteter från Workfront-mål. Projektets förlopp uppdateras när aktiviteter i projektet slutförs. Du kan ta bort projekt från målet genom att koppla från dem. Mer information finns i avsnittet om att koppla från projekt i artikeln [Ta bort resultat, aktiviteter och projekt från mål i Adobe Workfront](../../workfront-goals/results-and-activities/remove-results-activities-from-goals.md).

  >[!NOTE]
  >
  >Om följande projektinformation uppdateras på projektnivå uppdaterar Workfront Goals den automatiskt på målnivå:
  >
  >   
  >   
  >   * Projektägare
  >   * Projektnamn
  >   * Projektprocent klart
  >   
  >   
  >Mer information om hur du kopplar projekt till mål finns i [Lägg till projekt i mål i Adobe Workfront](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

* Du kan ta bort resultat och aktiviteter från mål när de inte längre är relevanta för målförloppet. Borttagna resultat och aktiviteter kan inte återställas. Mer information om hur du tar bort resultat och aktiviteter finns i [Ta bort resultat, aktiviteter och projekt från mål i Adobe Workfront](../../workfront-goals/results-and-activities/remove-results-activities-from-goals.md).
* Du kan redigera resultat och aktiviteter som är kopplade till mål från vilken tidsperiod som helst, även tidigare.
* När du redigerar resultat och aktiviteter uppdateras deras inställningar inte, och deras förlopp uppdateras inte. Du måste uppdatera förloppet för resultat och aktiviteter. Mer information om hur du uppdaterar framsteg för mål, resultat och aktiviteter finns i [Uppdatera målstatus i Adobe Workfront-mål](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).

## Redigera resultat

<!--
Editing results differs depending on which environment you use.

### Edit results in the Production environment

1. Go to the goal for which you want to edit a result and click the goal name to open the **Goal Details** panel.
1. Click **Results**.
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result you want to edit.

   ![](assets/results-gear-icon-options-350x85.png)

1. Click **Edit** to edit the following information:

   | Field |Description|
   |---|---|
   | Name |The name of the result. |
   | Owner |The owner of result.  |
   | Value |How you measure the progress of the result. |
   | Initial |The original value of the result. |
   | Target |The desired value when the result is completed. |

1. Click **Save**.
-->


1. Klicka på **Huvudmeny** ![](assets/main-menu-icon.png)sedan **Mål**.
1. Öppna målsidan genom att klicka på namnet på ett mål i mållistan.
1. Klicka **Progress-indikatorer** till vänster.
1. Välj ett resultat i listan med förloppsindikatorer och klicka på **Redigera** icon ![](assets/edit-icon.png).

   Rutan Redigera resultat öppnas.

   ![](assets/edit-result-box-unshimmed.png)

1. Redigera följande information:
   * **Resultatnamn**: Namnet på resultatet. Använd ett beskrivande namn som visar vilket resultat du behöver uppnå för att slutföra målet.
   * **Resultatägare**: Ägaren till resultatet. Ägaren måste vara en aktiv Workfront-användare.
   * **Värdetyp**: Hur du mäter resultatets förlopp.
   * **Startvärde**: Resultatets ursprungliga värde.
   * **Målvärde**: Det önskade värdet när resultatet är klart.
Mer information om resultatfält finns i [Lägg till resultat i mål](../results-and-activities/add-results-to-goals.md).
1. Klicka **Spara**.

## Redigera aktiviteter

<!--
Editing activities differs depending on which environment you use.

### Edit activities in the Production environment

>[!TIP]
>
>You cannot edit the Activity Type after you saved an activity on a goal.

1. Go to the goal for which you want to edit an activity and click the goal name to open the **Goal Details** panel.
1. Click **Activities**.
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the activity you want to edit .

   ![](assets/activities-gear-icon-options-350x84.png)

1. Click **Edit** to edit the following information:

   | Field |Description |
   |---|---|
   | Name |The name of the activity. |
   | Owner |The owner of activity.  |

1. Click **Save**.
-->

1. Klicka på **Huvudmeny** ![](assets/main-menu-icon.png)sedan **Mål**.
1. Öppna målsidan genom att klicka på namnet på ett mål i mållistan.
1. Klicka **Progress-indikatorer** till vänster.
1. Välj en aktivitet i listan Förloppsindikatorer och klicka på **Redigera** icon ![](assets/edit-icon.png).

   Rutan Redigera aktivitet öppnas.

   ![](assets/edit-activity-box-unshimmed.png)

1. Redigera följande information:
   * **Aktivitetsnamn**: Namnet på aktiviteten. Använd ett beskrivande namn som visar vilken aktivitet du bör utföra för att ange att målet har slutförts.
   * **Aktivitetsägare:** Aktivitetens ägare. Ägaren måste vara en aktiv Workfront-användare.\
     Mer information om aktivitetsfält finns i [Lägg till aktiviteter i mål](../results-and-activities/add-activities-to-goals.md).
1. Klicka **Spara**.



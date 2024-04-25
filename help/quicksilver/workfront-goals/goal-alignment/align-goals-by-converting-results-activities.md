---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Justera mål genom att konvertera resultat och aktiviteter till mål
description: Du kan justera två mål manuellt eller konvertera resultaten och aktiviteterna för ett befintligt mål till ett annat mål. Det konverterade resultatet eller aktiviteten blir det underordnade målet för det ursprungliga målet. Mer information om hur du justerar två mål manuellt finns i Justera mål genom att koppla dem till Adobe Workfront-mål.
author: Alina
feature: Workfront Goals
exl-id: 48371389-952c-4732-b519-9774cd4d1b93
source-git-commit: 09e34ecdfeec531ebbaaba4fb8682496c53d86bf
workflow-type: tm+mt
source-wordcount: '642'
ht-degree: 0%

---

# Justera mål genom att konvertera resultat och aktiviteter till mål

Du kan justera två mål manuellt eller konvertera resultaten och aktiviteterna för ett befintligt mål till ett annat mål. Det konverterade resultatet eller aktiviteten blir det underordnade målet för det ursprungliga målet.
Mer information om hur du justerar två mål manuellt finns i [Justera mål genom att koppla dem till Adobe Workfront mål](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

## Åtkomstkrav


<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">Adobe Workfront</td>
 <td>
 <p>Alla</p>

</td>
 </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-licens*</td>
 <td>
 <p>Aktuell licens: Medarbetare eller högre</p>
 eller
 <p>Äldre licens: Begär eller högre</p> <p>Mer information finns i <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Översikt över Adobe Workfront-licenser</a>.</p> </td>
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

## Förutsättningar

Du måste ha följande innan du kan börja:

* Ett befintligt mål med befintliga resultat och aktiviteter.

  Mer information om hur du skapar mål finns i [Skapa mål i Adobe Workfront-mål](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>Ett mål kan ha upp till 1 000 förloppsindikatorer.

<!--drafted for goal redesign: At PRODUCTION: update the sentence above to remove Production/ Preview references-->

## Att tänka på när du konverterar resultat och aktiviteter till mål

Ibland kan ett resultat eller en aktivitet ha ett större omfång än förväntat och det skulle vara mer rimligt att de blir mål. Du kan konvertera resultat och aktiviteter för ett befintligt mål till ett nytt mål. Det här är en nedifrån och upp-metod för att anpassa målen.

Tänk på följande när du konverterar resultat och aktiviteter till mål:

* Det konverterade resultatet eller aktiviteten blir det underordnade målet för det ursprungliga målet, och de två målen justeras.
* Det nya målet blir en enda förloppsindikator för det ursprungliga målet, om det inte finns några ytterligare resultat eller aktiviteter i det ursprungliga målet. Du måste lägga till resultat och aktiviteter i det underordnade målet för att kunna spåra förloppet.
* Det går inte att ångra konverteringen av ett resultat eller en aktivitet till ett mål. När det konverterats kan det nya underordnade målet aldrig igen bli ett resultat eller en aktivitet för det överordnade målet.

## Konvertera ett resultat eller en aktivitet till ett mål

<!--
<span class="preview">Converting results and activities differs depending on what environment you use. </span>

### Convert a result or activity to a goal in the Production environment

1. Go to a goal that has a result or an activity that you want to convert to a goal.
1. Click the name of the goal to open the **Goal Details** panel.
1. Expand the **Results** or **Activities** right-pointing arrows to see a list of results or activities for the goal. 

1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result or activity name that you want to convert, then click **Convert into a Goal**.

   ![](assets/convert-to-goal-link-highlighted-350x191.png)

1. (Optional) Remove the name of the original activity or result owner from the **Goal Owner** field and replace it with another user, team, group, or your organization's name. By default, Workfront selects the owner of the result or the activity as the goal owner. 
1. Click **Convert**. The activity or result displays as an aligned goal in the Goal Details panel of the original goal and the original activity or result is removed from the original goal and transferred to the second goal. By default, the new goal has the same name as the original converted result or activity. 
1. (Optional) Click the name of the new goal to open the **Goal Details** panel and edit the name of the goal. For information about editing any information for an existing goal, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
-->

1. Gå till ett mål som har ett resultat eller en aktivitet som du vill konvertera till ett mål.
1. Klicka på **Progress-indikatorer** till vänster.
1. Välj ett resultat eller en aktivitet i listan med förloppsindikatorer och klicka sedan på **Konvertera till mål** icon ![](assets/convert-to-goal-icon-unshimmed.png) högst upp i förloppsindikatorlistan. Rutan Konvertera till mål öppnas.

   ![](assets/convert-to-goal-box-unshimmed.png)
1. Uppdatera följande information:
   * **Målnamn**: Som standard har det nya målet samma namn som det ursprungliga resultatet eller den ursprungliga aktiviteten.
   * **Period**: Som standard är det nya målets period det aktuella kvartalet. Du kan välja **Aktivera anpassade datum** inställning för att definiera en anpassad tidsperiod för det nya målet.
   * **Målägare**: Som standard är den nya målägaren ägare till det ursprungliga resultatet eller den ursprungliga aktiviteten.
   * **Beskrivning**: Lägg till mer information om det nya målet.
1. Klicka **Spara**

   Resultatet eller aktiviteten konverteras nu till ett underordnat mål för det ursprungliga målet. Det listas som ett mål i listan med förloppsindikatorer för det ursprungliga målet.




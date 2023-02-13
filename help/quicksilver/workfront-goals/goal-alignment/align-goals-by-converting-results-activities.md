---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Justera mål genom att konvertera resultat och aktiviteter till mål
description: Du kan justera två mål manuellt eller konvertera resultaten och aktiviteterna för ett befintligt mål till ett annat mål. Det konverterade resultatet eller aktiviteten blir det underordnade målet för det ursprungliga målet. Mer information om hur du justerar två mål manuellt finns i Justera mål genom att koppla dem till Adobe Workfront-mål.
author: Alina
feature: Workfront Goals
exl-id: 48371389-952c-4732-b519-9774cd4d1b93
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 0%

---

# Justera mål genom att konvertera resultat och aktiviteter till mål

Du kan justera två mål manuellt eller konvertera resultaten och aktiviteterna för ett befintligt mål till ett annat mål. Det konverterade resultatet eller aktiviteten blir det underordnade målet för det ursprungliga målet.
Mer information om hur du justerar två mål manuellt finns i [Justera mål genom att koppla dem till Adobe Workfront mål](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

## Åtkomstkrav


<!--drafted for P&P release: 

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

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Du måste ha följande innan du kan börja:

* En layoutmall som innehåller området Mål på huvudmenyn.
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
1. Klicka på **Förloppsindikatorer** i den vänstra panelen.
1. Välj ett resultat eller en aktivitet i listan med förloppsindikatorer och klicka sedan på **Konvertera till mål** icon ![](assets/convert-to-goal-icon-unshimmed.png) högst upp i förloppsindikatorlistan. Rutan Konvertera till mål öppnas.

   ![](assets/convert-to-goal-box-unshimmed.png)
1. Uppdatera följande information:
   * **Målnamn**: Som standard har det nya målet samma namn som det ursprungliga resultatet eller den ursprungliga aktiviteten.
   * **Period**: Som standard är det nya målets period aktuellt kvartal. Du kan välja **Aktivera anpassade datum** inställning för att definiera en anpassad tidsperiod för det nya målet.
   * **Målägare**: Som standard är den nya målägaren ägare till det ursprungliga resultatet eller den ursprungliga aktiviteten.
   * **Beskrivning**: Lägg till mer information om det nya målet.
1. Klicka **Spara**

   Resultatet eller aktiviteten konverteras nu till ett underordnat mål för det ursprungliga målet. Det listas som ett mål i listan med förloppsindikatorer för det ursprungliga målet.




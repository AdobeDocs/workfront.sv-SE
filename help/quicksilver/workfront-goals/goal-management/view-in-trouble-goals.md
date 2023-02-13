---
product-previous: workfront-goals
navigation-topic: goal-management
title: Granska problematiska mål i Adobe Workfront-mål
description: Det finns risk för att mål med statusvärdet"Progress of In" inte kan nås, och de representeras av en röd förloppsindikator i Adobe Workfront-målen. Du bör granska dina mål ofta och förstå varför framstegen släpar efter.
author: Alina
feature: Workfront Goals
exl-id: df2cdc12-9102-4759-9daa-1f8ae68f110b
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---

# Granska problematiska mål i Adobe Workfront-mål

<!--
<p>(NOTE: the status of goals in "red" used to be called At Risk. Now, it is "in trouble") </p>
-->

Mål med ett förlopp för In-problem riskerar att inte uppnås och representeras av en röd förloppsindikator i Adobe Workfront-målen. Du bör granska dina mål ofta och förstå varför framstegen släpar efter. Mer information om målförloppet finns i [Översikt över målets förlopp och villkor i Adobe Workfront-mål](../../workfront-goals/goal-management/calculate-goal-progress.md).

## Åtkomstkrav

<!--drafted for P&P release: replace the existing requirements with this:

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

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Du måste ha följande innan du kan börja:

* En layoutmall som innehåller området Mål på huvudmenyn.

## Recommendations för att förhindra att mål når en utveckling i In-Trouble

Innan målen når upp till en utveckling av I Problem kan du övervaka dem ofta och justera deras framsteg när de når en riskutveckling. Mål som riskerar att hamna i trubbel. Mer information om målförloppet finns i [Översikt över målets förlopp och villkor i Adobe Workfront-mål](../../workfront-goals/goal-management/calculate-goal-progress.md)

Innan dina mål når en utveckling i Problem rekommenderar vi följande:

* Granska mål som har villkoret Riskrisk som du ofta har tilldelats samt organisatoriska mål som har tilldelats era team, grupper eller din organisation och som kan påverkas av hur målen utvecklas. Riksdagens mål riskerar att hamna i trubbel. Riskmålen markeras med en gul förloppsindikator. Använd mållistan för att visa mål som tillhör dig, dina team, grupper eller din organisation.


## Granska problemmål i mållistan

Du kan se målen i alla delar av Workfront mål. Mer information om Workfront-mål finns i [Översikt över avsnitten om Adobe Workfront-mål](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

I den här artikeln beskrivs hur du granskar mål i mållistan.

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) > **Mål** i det övre högra hörnet.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Detta öppnar området Workfront-mål och mållistavsnittet visas som standard.

1. (Rekommenderas) Justera följande filter för mållistan för att granska riskmålen:

   * Klicka **Företag** sedan **Mina team** sedan **Mina grupper** sedan **Personligt** mål i den här ordningen för att visa mål som tillhör organisationen, era team, grupper och sedan era egna mål.

      >[!TIP]
      >
      >I Adobe Workfront Goals visar filtret Company de mål som din organisation har valts som ägare för.
      >
      >
      >Du kan inte söka efter företag som använder det här fältet. Endast den organisation som äger din Workfront-instans är markerad som standard.

   * För varje organisationsenhet som du väljer ovan klickar du på **Nytt filter** > **Förlopp** > **I problem** >**Använd.**
   * (Valfritt) Välj den tidsperiod för vilken du vill visa mål.

      Förloppsindikatorn visas i rött för varje mål i mållistan.

      Mer information om hur du filtrerar mål med hjälp av alla andra villkor i den högra panelen finns i [Filtrera information i Adobe Workfront mål](../../workfront-goals/goal-management/filter-information-wf-goals.md).

1. Håll pekaren över förloppsindikatorn för att se hur stor den faktiska förloppsprocenten är och vad det förväntade värdet är för den aktuella dagen.

   ![](assets/goal-progress-hover-over-detail-unshimmed.png)

1. (Valfritt) Använd filtren för att hitta mål som tillhör en viss ägare.

   Felfria mål för de valda användarna visas i mållistan.

1. Klicka på ett målnamn för att öppna målsidan och klicka sedan på **Förloppsindikatorer** i den vänstra panelen. Visa vilken förloppsindikator som gör att målet ligger bakom och uppdatera förloppet för indikatorn inline i **Faktiskt förlopp** -kolumnen i listan med förloppsindikatorer.

   Information om hur du uppdaterar resultat och aktiviteter finns i [Uppdatera målstatus i Adobe Workfront-mål](../goal-review-and-workfront-goals-sections/check-in-goals.md)

   ![](assets/actual-progress-editable-column-in-indicator-list-unshimmed.png)

   >[!NOTE]
   >
   >Du kan bara uppdatera resultat och aktiviteter i listan med förloppsindikatorer. Du måste uppdatera förloppsindikatorerna för underordnade mål genom att komma åt målen, och du måste uppdatera uppgifterna för de kopplade projekten för att uppdatera förloppet för projekten.



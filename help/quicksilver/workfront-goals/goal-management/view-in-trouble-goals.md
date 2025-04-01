---
product-previous: workfront-goals
navigation-topic: goal-management
title: Granska problem i Adobe Workfront-mål
description: Det finns risk för att mål med statusvärdet"Progress of In" inte kan nås, och de representeras av en röd förloppsindikator i Adobe Workfront-målen. Du bör granska dina mål ofta och förstå varför framstegen släpar efter.
author: Alina
feature: Workfront Goals
exl-id: df2cdc12-9102-4759-9daa-1f8ae68f110b
source-git-commit: 01e53bbc10573950d08f2df63fc742e6b9771e77
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# Granska problematiska mål i Adobe Workfront-mål

<!--Audited: 4/2025-->

<!--
<p>(NOTE: the status of goals in "red" used to be called At Risk. Now, it is "in trouble") </p>
-->

Mål med ett förlopp för In-problem riskerar att inte uppnås och representeras av en röd förloppsindikator i Adobe Workfront-målen. Du bör granska dina mål ofta och förstå varför framstegen släpar efter. Mer information om målförloppet finns i [Översikt över målförloppet och målvillkoret i Adobe Workfront-mål](../../workfront-goals/goal-management/calculate-goal-progress.md).

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
 <p>Aktuell licens: Begär eller högre</p> <p>Mer information finns i <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Översikt över Adobe Workfront-licenser</a>.</p> </td>
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
 <td> <p>Redigera åtkomst till mål</p></td>
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

## Rekommendationer för att förhindra att mål når en utveckling i In-PROBLEM

Innan målen når upp till en utveckling av I Problem kan du övervaka dem ofta och justera deras framsteg när de når en riskutveckling. Mål som riskerar att hamna i trubbel. Mer information om målförloppet finns i [Översikt över målförloppet och målvillkoret i Adobe Workfront-mål](../../workfront-goals/goal-management/calculate-goal-progress.md)

Innan dina mål når en utveckling i Problem rekommenderar vi följande:

* Granska mål som har villkoret Riskrisk som du ofta har tilldelats samt organisatoriska mål som har tilldelats era team, grupper eller din organisation och som kan påverkas av hur målen utvecklas. Riksdagens mål riskerar att bli problematiska. Riskmålen markeras med en gul förloppsindikator. Använd mållistan för att visa mål som tillhör dig, dina team, grupper eller din organisation.


## Granska problemmål i mållistan

Du kan se målen i alla delar av Workfront mål. Mer information om avsnitten om Workfront-mål finns i [Översikt över avsnitten om Adobe Workfront-mål](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

I den här artikeln beskrivs hur du granskar mål i mållistan.

1. Klicka på ikonen **Huvudmeny** ![Huvudmeny ](assets/main-menu-icon.png) > **Mål** i det övre högra hörnet.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Detta öppnar området Workfront-mål och mållisteavsnittet visas som standard.

1. (Rekommenderas) Justera följande filter för mållistan för att granska riskmålen:

   * Klicka på **Företag**, **Mina team**, **Mina grupper** och sedan på **Personliga** mål i den här ordningen för att visa mål som tillhör din organisation, dina team, grupper och sedan dina egna mål.

     >[!TIP]
     >
     >I Adobe Workfront Goals visar filtret Company de mål som din organisation har valts som ägare för.
     >
     >
     >Du kan inte söka efter företag som använder det här fältet. Som standard är det bara den organisation som äger din Workfront-instans som är vald.

   * Klicka på **Nytt filter** > **Förlopp** > **I problem** >**Använd.** för var och en av de organisationsenheter du väljer ovan.
   * (Valfritt) Välj den tidsperiod för vilken du vill visa mål.

     Förloppsindikatorn visas i rött för varje mål i mållistan.

     Mer information om hur du filtrerar mål med hjälp av alla andra villkor på den högra panelen finns i [Filtrera information i Adobe Workfront-mål](../../workfront-goals/goal-management/filter-information-wf-goals.md).

1. Håll pekaren över förloppsindikatorn för att se hur stor den faktiska förloppsprocenten är och vad det förväntade värdet är för den aktuella dagen.

   ![Allmän förloppshovringsinformation](assets/goal-progress-hover-over-detail-unshimmed.png)

1. (Valfritt) Använd filtren för att hitta mål som tillhör en viss ägare.

   Felfria mål för de valda användarna visas i mållistan.

1. Klicka på ett målnamn för att öppna målsidan och klicka sedan på **Förloppsindikatorer** i den vänstra panelen. Visa vilken förloppsindikator som gör att målet ligger bakom och uppdatera förloppet för indikatorn inline i kolumnen **Faktisk förlopp** i listan Förloppsindikatorer.

   Mer information om att uppdatera resultat och aktiviteter finns i [Uppdatera målförloppet i Adobe Workfront-mål](../goal-review-and-workfront-goals-sections/check-in-goals.md)

   ![Faktisk status](assets/actual-progress-editable-column-in-indicator-list-unshimmed.png)

   >[!NOTE]
   >
   >Du kan bara uppdatera resultat och aktiviteter i listan med förloppsindikatorer. Du måste uppdatera förloppsindikatorerna för barnens mål genom att komma åt målen och du måste uppdatera uppgifterna för de kopplade projekten för att uppdatera förloppet för projekten.



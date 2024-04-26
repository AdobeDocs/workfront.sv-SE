---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Granska diagram för att förstå målutvecklingstrender i Adobe Workfront-mål
description: Du kan visa den övergripande statusen för dina mål och deras utvecklingstrend i tid i avsnittet Diagram för Adobe Workfront-mål. Diagrammen i det här avsnittet bryter inte ned förloppet för varje mål utan ger dig i stället en helhetsbild av alla målens förloppsstatus samt deras förloppstrend under en angiven period.
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: 948cd81908df3174eb985d1c65533077d3ef5d49
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 0%

---

# Granska diagram för att förstå målutvecklingstrender i Adobe Workfront-mål

<!-- drafted mostly for P&P release-->

Du kan visa den övergripande statusen för dina mål och deras utvecklingstrend i tid i avsnittet Diagram för Adobe Workfront-mål. Diagrammen i det här avsnittet bryter inte ned förloppet för varje mål utan ger dig i stället en helhetsbild av alla målens förloppsstatus samt deras förloppstrend under en angiven period.

>[!IMPORTANT]
>
>Du kan se det totala antalet för dina mål i avsnittet Diagram för en vald tidsperiod. Workfront-mål tar dock endast hänsyn till mål med statusen Aktiv och Stängd vid beräkning av det övergripande målets förloppsstatus och procent färdigt.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra de åtgärder som beskrivs i den här artikeln:

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

## Typer av diagram i Workfront-mål

Följande diagram är tillgängliga i diagramavsnittet eller Workfront-mål:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Målhälsodiagrammet</td> 
   <td> <p>Ett mätardiagram som visar följande:</p> 
    <ul> 
     <li>Ett totalt antal mål för den valda tidsperioden. Mål med valfri status beaktas. </li> 
     <li>Förloppsstatus för mål med statusen Aktiv och Stängd.</li> 
    </ul> <p>Mer information om hur Workfront-mål beräknar förloppsstatus finns i <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Översikt över målets förlopp och villkor i Adobe Workfront-mål</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Målförloppsdiagram</td> 
   <td> <p>Ett linjediagram som visar uppdateringar av mål i steg om veckan under målets varaktighet. Följande visas i målförloppsdiagrammet:</p> 
    <ul> 
     <li>En genomsnittlig förväntad och faktisk procent slutförd av alla aktiva och stängda mål under den valda perioden. Förloppet för procent färdigt delas upp i veckovisa steg som markeras med noder. </li> 
     <li>Den totala procentandelen av framsteg för aktiva och stängda mål sedan föregående vecka. </li> 
    </ul> <p>Tips! Målförloppsdiagrammet kanske inte visar någon information när det görs uppdateringar för målen utanför den valda tidsperioden. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Granska målförloppet i diagram

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) > **Mål** längst upp till höger.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Detta öppnar området Workfront-mål.

1. Klicka **Diagram** till vänster.

   ![](assets/graphs-in-left-panel.png)

   Avsnittet Diagram visas.

   Som standard begränsas de mål som visas i avsnittet Diagram av följande kriterier:

   * De filter som används i området Diagram.
   * Mål som har statusen Aktiv och Utkast.

1. (Valfritt) Markera den typ av information som du vill visa genom att uppdatera filtren i det övre högra hörnet av diagramavsnittet.

   Mer information om filtreringsmål finns i [Filtrera information i Adobe Workfront-mål](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   >[!TIP]
   >
   >Om du har valt att visa mer än en tidsperiod visas både ett hälsodiagram (mätare) och ett förloppsdiagram (rad) för varje tidsperiod.

1. Granska informationen i tabellen nedan när du granskar målhälsodiagrammet.

   ![](assets/gauge-graph-wf-align-350x230.png)

   | Totalt antal mål | Siffran längst ned i diagrammet anger antalet mål i den valda perioden, i alla statusvärden som du har valt. |
   |---|---|
   | Genomsnitt procent klart | I överkanten av diagrammet anger det här talet den genomsnittliga procentandelen färdigt av aktiva och stängda mål under den valda tidsperioden. |
   | Mål och deras framsteg | Antalet mål för varje förloppsstatussegment, när du hovrar över segmenten i diagrammet. Endast mål med statusen Aktiv eller Stängd räknas i segmenten. |


1. Granska informationen i tabellen nedan när du granskar statusdiagrammet för mål.

   ![](assets/line-graph-wf-align-350x161.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Baslinjeförlopp</td> 
      <td>Den gröna sluttningslinjen anger det förväntade totala genomsnittet i procent slutfört av aktiva och stängda mål för den valda tidsperioden. Alla mål inom en period förväntas bli klara, så baslinjeförloppet är alltid 100 % vid periodens slut. </td> 
     </tr> 
     <tr> 
      <td>Faktiskt förlopp</td> 
      <td> <p>Den blå raden visar det faktiska totala procentvärdet för antalet slutförda och aktiva mål för den valda tidsperioden i veckointervall. Varje vecka under målets varaktighet markeras med en nod på raden. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Hovra en veckonod i målförloppsdiagrammet och granska följande:

   * **Veckodatum**: Månad, dag och år för den valda veckan.
   * **Förlopp**: Ett genomsnitt av den faktiska procentandelen färdigt av alla mål för den valda veckan.
   * **Baslinje**: Ett genomsnitt av den förväntade procentandelen färdigt av alla mål för den valda veckan.

1. (Valfritt) Klicka på **Förlopp** längst ned i förloppsdiagrammet för att ta bort den totala förloppslinjen

   eller

   Klicka **Baslinje** längst ned i förloppsdiagrammet för att ta bort den förväntade förloppet från diagrammet.

 

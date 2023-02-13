---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Granska diagram för att förstå målutvecklingstrender i Adobe Workfront-mål
description: Du kan visa den övergripande statusen för dina mål och deras utvecklingstrend i tid i avsnittet Diagram för Adobe Workfront-mål. Diagrammen i det här avsnittet bryter inte ned förloppet för varje mål utan ger dig i stället en helhetsbild av alla målens förloppsstatus samt deras förloppstrend under en angiven period.
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: 3989903687f2ea64ebd5ad754119ce1a9d70b9f3
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 0%

---

# Granska diagram för att förstå målutvecklingstrender i Adobe Workfront-mål

<!-- drafted mostly for P&P release-->

Du kan visa den övergripande statusen för dina mål och deras utvecklingstrend i tid i avsnittet Diagram för Adobe Workfront-mål. Diagrammen i det här avsnittet bryter inte ned förloppet för varje mål utan ger dig i stället en helhetsbild av alla målens förloppsstatus samt deras förloppstrend under en angiven period.

>[!IMPORTANT]
>
>Du kan se det totala antalet för dina mål i avsnittet Diagram för en vald tidsperiod. Workfront-mål tar dock endast hänsyn till mål med statusen Aktiv och Stängd vid beräkning av det övergripande målets förloppsstatus och procent färdigt.

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

Du måste ha följande åtkomst för att kunna utföra de åtgärder som beskrivs i den här artikeln:

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
   <td role="rowheader">Åtkomstnivå*</td> 
   <td> <p>Visa eller öka åtkomsten till mål</p> <p><b>ANMÄRKNING</b><p>Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra din åtkomstnivå finns i:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Bevilja åtkomst till Adobe Workfront-mål</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> 
    <div> 
     <p>Visa eller öka behörigheter för mål</p> 
     <p>Mer information om delningsmål finns i <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Dela ett mål i Workfront-mål</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Du måste ha följande innan du kan börja:

* En layoutmall som innehåller området Mål på huvudmenyn.

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
     <li>Ett totalt antal mål för den valda tidsperioden. Mål med valfri status tas med i beräkningen. </li> 
     <li>Förloppsstatus för mål med statusen Aktiv och Stängd.</li> 
    </ul> <p>Mer information om hur Workfront-mål beräknar förloppsstatus finns i <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Översikt över målets förlopp och villkor i Adobe Workfront-mål</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Målförloppsdiagram</td> 
   <td> <p>Ett linjediagram som visar uppdateringar av mål i steg om veckan under målets varaktighet. Följande visas i målförloppsdiagrammet:</p> 
    <ul> 
     <li>En genomsnittlig förväntad och faktisk procent slutförd av alla aktiva och stängda mål under den valda perioden. Förloppet för procent färdigt delas upp i veckovisa steg som markeras med noder. </li> 
     <li>Den totala genomsnittliga procentandel av förloppet för aktiva och stängda mål sedan föregående vecka. </li> 
    </ul> <p>Tips: Målförloppsdiagrammet kanske inte visar någon information när det görs uppdateringar av målen utanför den valda tidsperioden. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Granska målförloppet i diagram

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) > **Mål** i det övre högra hörnet.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Detta öppnar området Workfront-mål.

1. Klicka **Diagram** i den vänstra panelen.

   ![](assets/graphs-in-left-panel.png)

   Avsnittet Diagram visas.

   Som standard begränsas de mål som visas i avsnittet Diagram av följande kriterier:

   * De filter som används i området Diagram.
   * Mål som har statusen Aktiv och Utkast.

1. (Valfritt) Markera den typ av information som du vill visa genom att uppdatera filtren i det övre högra hörnet av diagramavsnittet.

   Mer information om filtreringsmål finns i [Filtrera information i Adobe Workfront mål](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   >[!TIP]
   Om du har valt att visa mer än en tidsperiod visas både ett hälsodiagram (mätare) och ett förloppsdiagram (rad) för varje tidsperiod.

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
      <td>Den gröna sluttningslinjen anger det förväntade totala procentvärdet för det aktiva och stängda målet för den valda tidsperioden. Alla mål inom en period förväntas bli klara, så baslinjeförloppet är alltid 100 % vid periodens slut. </td> 
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
   * **Baslinje**: Ett genomsnitt av den förväntade procentandelen slutfört av alla mål för den valda veckan.

1. (Valfritt) Klicka på **Förlopp** längst ned i förloppsdiagrammet för att ta bort den totala förloppslinjen

   eller

   Klicka **Baslinje** längst ned i förloppsdiagrammet för att ta bort den förväntade förloppet från diagrammet.

 

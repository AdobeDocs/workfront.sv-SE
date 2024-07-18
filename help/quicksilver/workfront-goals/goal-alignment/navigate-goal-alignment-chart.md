---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Navigera i avsnittet Måljustering i Adobe Workfront-mål
description: Använd delen Måljustering för att visa en helhetsbild av måljusteringen i hela organisationen i ett flödesschema. Justerade mål visas på kort som sammanlänkar i ett hierarkiskt träd.
author: Alina
feature: Workfront Goals
exl-id: e79ced31-4680-4af7-b083-3d615c747af8
source-git-commit: 09e34ecdfeec531ebbaaba4fb8682496c53d86bf
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 0%

---

# Navigera i avsnittet Måljustering i Adobe Workfront-mål

Använd delen Måljustering för att visa en helhetsbild av måljusteringen i hela organisationen i ett flödesschema. Justerade mål visas på kort som sammanlänkar i ett hierarkiskt träd.

Mer information om måljustering och hur du uppnår det finns i följande artiklar:

* [Översikt över måljustering i Adobe Workfront-mål](../../workfront-goals/goal-alignment/goal-alignment-overview.md)
* [Justera mål genom att koppla dem till Adobe Workfront mål](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)

## Åtkomstkrav

Du måste ha följande för att kunna utföra de aktiviteter som beskrivs i den här artikeln:

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
<p>Aktuell licens: Begär eller högre</p>  </td>
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

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Navigera i avsnittet Måljustering

1. Klicka på ikonen **Huvudmeny** ![Huvudmeny ](../goal-alignment/assets/dots-main-menu-icon.png) i skärmens övre högra hörn och klicka sedan på **Mål**.
   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-alignment/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. Klicka på **Måljustering** i den vänstra panelen.
1. Använd filtren i det övre högra hörnet av justeringsdiagrammet om du bara vill markera de mål som är viktiga för dig. Mer information om hur du använder filter i Workfront-mål finns i [Filtrera information i Adobe Workfront-mål](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   De mål som matchar dina filter visas i justeringsdiagrammet på kort.

   Följande information visas på ett målkort:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tidsperiodens datum </td> 
      <td> <p>Detta är den period för vilken målet är öppet. Målet måste vara uppnått vid periodens slutdatum. Workfront-mål beräknar förloppet för målet baserat på målperiodens längd och aktuellt datum.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progress-indikatorer</td> 
      <td>Antalet förloppsindikatorer för målet. Förloppsindikatorer kan vara anpassade till mål, resultat eller aktiviteter. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ägarens namn</td> 
      <td>Namnet på den användare, det team, den grupp eller den organisation som har angetts som målägare. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Målnamn</td> 
      <td>Målets namn. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Målförloppsindikator <span>och förlopp</span></td> 
      <td> <p>Målförloppet visar hur mycket av målet som för närvarande har uppnåtts. Detta är en automatisk beräkning av medelvärdet av förloppet för alla justerade mål, resultat och aktiviteter för målet baserat på den tid som gått sedan målets tidsperiod startades. Mer information om hur du beräknar förloppet för mål finns i <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Översikt över målförloppet och villkoret i Adobe Workfront-mål</a>. </p> 
       <div> 
        <p>Målets faktiska förlopp vid dagens datum. Följande förloppsvärden och färger visar hur sannolikt det är att målet uppnås i tid: </p> 
        <ul> 
         <li><span>På mål</span> (grön indikator): målet är i tid och kommer att uppnås i tid.</li> 
         <li> <span>Vid risk</span> (gul indikator): målet ligger efter och kanske inte uppnås i tid.</li> 
         <li> <span>I problem </span> (röd indikator): det finns risk för att målet inte kan uppnås i tid. </li> 
        </ul> 
       </div> </td> 
     </tr> <!--
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">Updated on date </td> 
       <td> <p>The date when the goal was last updated</p> <p>(NOTE: drafted because I think this was removed with the alignment chart redesign - 21.1) </p> </td> 
      </tr>
     --> 
     <tr> 
      <td role="rowheader">Status</td> 
      <td><span>Mål i alla statusvärden visas i avsnittet Måljustering.</span> </td> 
     </tr> 
    </tbody> 
   </table>

   Mål som är justerade mot andra mål visar antalet justerade mål under målkortet.

   ![](assets/alignment-chart-arrow-for-aligned-goals-highlighted-350x241.png)

1. Klicka på ikonen **nedåtriktad pil** under ett mål om du vill expandera och visa de underordnade målen ytterligare.

   ![](assets/alignment-chart-arrow-for-aligned-goals-highlighted-350x241.png)

   >[!TIP]
   >
   >Mål med underordnade mål justerade mot dem visar antalet justerade mål under deras respektive kort.

1. (Villkorligt) Om det aktuella filtret utesluter några av de mål som ingår i en justering visas ett varningsmeddelande som anger att inte alla mål visas.

   ![](assets/parent-goal-excluded-by-filter-alignment-section-350x230.png)

1. Klicka på **Visa dem** för att visa de mål som för närvarande är eliminerade av filtret.

   Observera följande ändringar i justeringsdiagrammet:

   * Kopplade mål som tidigare tagits bort av filtret visas nu i justeringsdiagrammet.
   * Filtret i det övre högra hörnet markeras med gult för att ange att det för närvarande inte används.

     ![](assets/reapply-filter-link-and-yellow-filter-highlight-350x120.png)

     En länk för återanvändning av filter visas till vänster om filternamnet.

1. (Valfritt) Klicka på **Använd om filter** om du vill återgå till det ursprungliga resultatet och visa målhierarkin.
1. (Valfritt) Håll muspekaren över förloppsindikatorn för att förstå var målförloppet ska vara för den aktuella dagen.

   ![](assets/progress-mouse-over-alignment-chart-350x163.png)

   Följande information visas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Från och med idag</td> 
      <td>Förloppsstatusen är alltid aktuell. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>Faktiskt</span> </td> 
      <td>Målets faktiska förlopp (i procent) vid dagens datum, beräknat genom att ta hänsyn till alla förloppsindikatorer för målet. Målförloppsindikatorer är anpassade till mål, aktiviteter och resultat. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Förväntat</td> 
      <td> <p>Förväntat förlopp (en procentandel) för målet vid dagens datum, förutsatt att du kommer att uppnå målet i tid.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på ett målkort för att öppna målsidan. Mer information om hur du redigerar befintliga mål finns i [Redigera mål i Adobe Workfront-mål](../../workfront-goals/goal-management/edit-goals.md). Mer information om hur du uppdaterar förloppet för mål finns i [Uppdatera målförloppet i Adobe Workfront-mål](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).

1. Klicka på uppåtpilen för målet på aktuell nivå för att gå tillbaka till föregående nivå i hierarkin i diagrammet.

   eller

   (Valfritt) Klicka på **Avsluta målhierarki** om du vill visa korten för alla mål som matchar det aktuella filtret, utan att visa deras anslutning till varandra.



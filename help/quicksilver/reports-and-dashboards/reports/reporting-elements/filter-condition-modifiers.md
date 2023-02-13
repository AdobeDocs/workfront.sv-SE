---
product-area: reporting
navigation-topic: reporting-elements
title: Filter- och villkorsmodifierare
description: Med filter- och villkorsmodifierarna kan du skapa filter och skapa villkor för formatering av rapportresultat.
author: Lisa
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '1556'
ht-degree: 0%

---

# Filter- och villkorsmodifierare

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit) </p>
-->

Med filter- och villkorsmodifierarna kan du skapa filter och skapa villkor för formatering av rapportresultat.

Mer information om hur du skapar filter finns i artikeln [Översikt över filter i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Mer information om hur du använder villkorsstyrd formatering i Vyer finns i artikeln [Använd villkorsstyrd formatering i vyer](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Filter- och villkorsmodifierare

En lista med inbyggda modifierare för tidsramar finns i artikeln [Filtrera rapporter efter tidsramar](../../../reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

Vissa modifierare är inbyggda och du kan välja dem från en nedrullningsbar meny i filtret eller villkorsstyrd formateringssats. Andra modifierare kan bara användas i textlägesfilter. Mer information om textläge finns i [Översikt över textläge](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Du kan använda följande villkorsmodifierare i filter och villkorsstyrda formateringssatser:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Inbyggd modifierare</strong> </p> </th> 
   <th> <p><strong>Textlägesmodifierare</strong> </p> </th> 
   <th> <p><strong>Beskrivning</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td> <p><strong>Är tom</strong> </p> </td> 
   <td> <p><strong>blank</strong> </p> </td> 
   <td> <p>Fältet finns för objektet men fältet har ännu inte fått något värde.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Är inte tom</strong> </p> </td> 
   <td> <p><strong>notblank</strong> </p> </td> 
   <td> <p>Fältet som du filtrerar efter finns och har fått ett värde.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>null</strong> </p> </td> 
   <td> <p>Fältet är antingen tomt eller finns inte. Du vill till exempel söka efter objekt utan ett överordnat uppgifts-ID. Det innebär att du bara vill se fristående uppgifter. Kvalificeraren för det överordnade uppgifts-ID:t skulle vara <strong>null</strong>eftersom en uppgift utan ID (i det här fallet det överordnade) inte finns. </p> <p>Den här modifieraren kan bara användas i textlägesfilter. Mer information om textläge i filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notnull</strong> </p> </td> 
   <td> <p>Fältet som du filtrerar efter finns och innehåller ett annat värde än null.</p> <p>Den här modifieraren kan bara användas i textlägesfilter. Mer information om textläge i filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Innehåller</strong> </p> </td> 
   <td> <p><strong>cicontains</strong> </p> </td> 
   <td> <p>(Skiftlägesokänslig) Detta är den skiftlägesokänsliga versionen av <strong>innehåller</strong>. Till exempel: cicontains inf hämtar alla värden som innehåller antingen Inf eller inf.</p> <p> <p>Obs! Adobe Workfront söker efter det exakta ord eller den fras du anger för varje filtersats. Om du t.ex. söker efter ett projekt som innehåller frasen"nytt projekt" i namnet, visas inga projekt som bara innehåller"nytt" eller"projekt", eller"nytt huvudprojekt" i namnet. Filtret hittar bara projekt med den exakta frasen"nytt projekt" i namnet.</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>(Skiftlägesokänslig) Det här alternativet är inte skiftlägeskänsligt för <strong>eq</strong>. Det returnerar bara en exakt matchning av det sökda värdet.</p> <p>Om du till exempel söker efter en uppgift med ett specifikt namn söker "task name cieq test" efter uppgifter där namnet är "Test", "TEST" eller "Test", men inte en uppgift med namnet "test 123".</p> <p>Den här modifieraren kan bara användas i textlägesfilter. Mer information om textläge i filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>ciin</strong> </p> </td> 
   <td> <p>(Skiftlägesokänslig) Detta är den skiftlägesokänsliga versionen av <strong>in</strong>.</p> <p>Den här modifieraren kan bara användas i textlägesfilter. Mer information om textläge i filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cilike</strong> </p> </td> 
   <td> <p>Det här är en skiftlägeskänslig version av <strong>gilla</strong>. Till exempel: "cilike %Current% %Dead%" returnerar alla anteckningar som innehåller "Current to Dead" eller "current to död".</p> <p>Den här modifieraren kan bara användas i textlägesfilter. Mer information om textläge i filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cinotin</strong> </p> </td> 
   <td> <p>(Skiftlägesokänslig) Detta är den skiftlägesokänsliga versionen av <strong>notin</strong>.</p> <p>Den här modifieraren kan bara användas i textlägesfilter. Mer information om hur du skapar filter i textläge finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>innehåller</strong> </p> </td> 
   <td> <p>(Skiftlägeskänsligt) Söker efter den angivna texten i en hel textsträng.</p> <p>Om du till exempel använder"contains Inf" hämtas allt med"Inf" i det, till exempel ordet"Infinity".</p> <p>Den här modifieraren kan bara användas i textlägesfilter.Mer information om textläge i filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Innehåller inte</strong> </p> </td> 
   <td> <p><strong>cinotcontains</strong> </p> </td> 
   <td> <p>(Skiftlägesokänslig) Den filtrerar efter objekt som saknar det angivna värdet.</p> <p>"innehåller till exempel inte inf" fångar något utan "Inf" eller "inf" i namnet.</p> <p>Obs! <span>Om fältet som du filtrerar efter har flera alternativ filtreras resultaten som innehåller både det alternativ som du anger, samt det alternativ som du anger och eventuella ytterligare alternativ.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>Finns inte</strong> </td> 
   <td><strong>ANTECKNINGAR</strong> </td> 
   <td> <p>Den här modifieraren används bara med komplexa filter i en EXISTS-programsats. Dessa filter refererar endast till följande objekt: </p> 
    <ul> 
     <li>Objekt som sträcker sig över flera nivåer i objekthierarkin </li> 
     <li>Objekt som saknas </li> 
    </ul> <p>Mer information om hur du skapar komplexa filter med EXISTS-programsatser finns i artikeln <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">Skapa komplexa textlägesfilter med EXISTS-satser</a>. Detta är den enda modifieraren som används i EXISTS-satser.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>Jämn</strong> </p> </td> 
   <td> <p><strong>in</strong> </p> </td> 
   <td> <p>(Skiftlägeskänsligt) Med den här modifieraren kan du skapa en kommaavgränsad lista med variabler som ska jämföras med ett enskilt attribut utvärderat i ett filter. Hela listan behandlas som en OR-sats och returnerar alla resultat som uppfyller villkoren för en eller flera av variablerna.</p> <p>Om du till exempel söker efter projekt och använder"i CUR, PLN, CPL" returneras alla projekt som har statusen Aktuell, ELLER Planering, ELLER Fullständig.</p> <p>Den inbyggda modifieraren <strong>Jämn</strong> motsvarar textlägesmodifieraren i <strong>in</strong>. Det innebär att du kan välja Lika med flera värden för fältet.</p> <p>Du kan t.ex. välja "Status är lika med aktuell, Planering, Död" i en projektrapport och du kan visa projekt i någon av dessa statusar.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>(Skiftlägeskänsligt) Detta returnerar endast en exakt matchning av det sökda värdet.</p> <p>Om du till exempel söker efter fullständiga projekt returnerar "eq CPL" alla projekt med fullständig status. "eq CPL, CUR" returnerar inget resultat eftersom ett projekt inte kan vara fullständigt och aktuellt samtidigt.</p> <p>Den här modifieraren kan bara användas i textlägesfilter. Mer information om hur du använder textläge för att skapa filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Större än</strong> </p> </td> 
   <td> <p><strong>gt</strong> </p> </td> 
   <td> <p>Detta söker efter alla resultat med ett värde som är större än det angivna värdet, exklusive det angivna värdet.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>gilla</strong> </p> </td> 
   <td> <p>(Skiftlägeskänsligt) Söker efter delar av en textsträng på liknande sätt som <strong>innehåller</strong>. Men <strong>gilla</strong> gör att du kan infoga jokertecken för att dela upp texten.</p> <p>Om du till exempel söker efter anteckningar och använder "som %Current% %Dead%" returneras alla anteckningar som innehåller frasen "Aktuell till aktuell". Den innehåller inga anteckningar som innehåller"Dead to Current". Varje värde söks igenom i den ordning som det listas. % representerar ett jokertecken som ersätter tecken eller textsegment.</p> <p>Den här modifieraren kan bara användas i textlägesfilter. Mer information om textläge i filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Mindre än</strong> </p> </td> 
   <td> <p><strong>lt</strong> </p> </td> 
   <td> <p>Detta söker efter alla resultat med ett värde som är mindre än det som anges, exklusive det angivna värdet.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Större än lika</strong> </p> </td> 
   <td> <p><strong>gte</strong> </p> </td> 
   <td> <p>Detta söker efter alla resultat med värden som är större än eller lika med det angivna värdet.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Mindre än lika med</strong> </p> </td> 
   <td> <p><strong>lte</strong> </p> </td> 
   <td> <p>Detta söker efter alla resultat med ett värde som är mindre än eller lika med det angivna värdet.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Mellan</strong> </p> </td> 
   <td> <p><strong>mellan</strong> </p> </td> 
   <td> <p>Tillhandahåller två obligatoriska fältvärden och söker efter alla resultat inom intervallet för båda fälten inklusive de angivna värdena.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notcontains</strong> </p> </td> 
   <td> <p>(Skiftlägeskänsligt) Den filtrerar efter objekt som saknar det angivna värdet.</p> <p>"notcontains inf" fångar till exempel allt med utan "inf", men visar värden som innehåller "Inf".</p> <p>Den här modifieraren kan bara användas i textlägesfilter. Mer information om textläge i filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notbetween</strong> </p> </td> 
   <td> <p>Det här är motsatsen till <strong>mellan</strong>. Det innehåller två obligatoriska värdefält och söker efter alla resultat utanför intervallet för båda fälten inklusive de angivna värdena.</p> <p>Den här modifieraren kan bara användas i textlägesfilter. Mer information om textläge i filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Inte lika med</strong> </p> </td> 
   <td> <p><strong>notin</strong> </p> </td> 
   <td> <p>(Skiftlägeskänsligt) Detta är motsatsen till <strong>in</strong>. Det returnerar bara resultat som inte finns i den angivna listan.</p> <p>Den här modifieraren kan bara användas i textlägesfilter. Mer information om textläge i filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p> <p>Obs! <span>Om fältet som du filtrerar efter har flera alternativ filtreras resultaten som innehåller både det alternativ som du anger, samt det alternativ som du anger och eventuella ytterligare alternativ.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p>(Skiftlägeskänsligt) Detta är motsatsen till <strong>eq</strong>. Det returnerar bara resultat som inte är en exakt matchning av det sökda värdet, och det matchar även värdets skiftläge.</p> <p>Till exempel: <b>ne</b> returnerar värden som inte är lika med "Aktuell", men som inte returnerar några värden som inte är lika med "aktuell". </p> <p>Den här modifieraren kan bara användas i textlägesfilter. Mer information om textläge i filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>cine</strong> </td> 
   <td> <p>(Skiftlägesokänslig) Det här alternativet är inte skiftlägeskänsligt för <strong>ne</strong> och det är motsatsen till <b>cieq</b> modifierare. Det returnerar bara resultat som inte är en exakt matchning av det sökda värdet, utan hänsyn tagen till värdets skiftläge.</p> <p>Till exempel: <b>cine</b> returnerar alla värden som inte är lika med "current" eller "Current". </p> <p>Den här modifieraren kan bara användas i textlägesfilter. Mer information om textläge i filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

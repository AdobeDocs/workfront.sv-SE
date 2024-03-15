---
product-area: reporting
navigation-topic: reporting-elements
title: Filter- och villkorsmodifierare
description: Med filter- och villkorsmodifierarna kan du skapa filter och skapa villkor för formatering av rapportresultat.
author: Nolan
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: d2268e50080ddbe306731d034d88fd29b712b86d
workflow-type: tm+mt
source-wordcount: '1516'
ht-degree: 0%

---

# Filter- och villkorsmodifierare

<!-- Audited: 1/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit) </p>
-->

Med filter- och villkorsmodifierarna kan du skapa filter och skapa villkor för formatering av rapportresultat.

Mer information om hur du skapar filter finns i artikeln [Översikt över filter](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Mer information om hur du använder villkorsstyrd formatering i Vyer finns i artikeln [Använd villkorsstyrd formatering i vyer](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Filter- och villkorsmodifierare

Vissa modifierare är inbyggda och du kan välja dem från en nedrullningsbar meny i filtret eller villkorsstyrd formateringssats. Andra modifierare kan bara användas i textlägesfilter.

Mer information om textläge finns i [Översikt över textläge](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

En lista med inbyggda modifierare för tidsramar finns i artikeln [Filtrera rapporter efter tidsramar](../../../reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

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
   <td> <p>Fältet finns för objektet men fältet har för närvarande inget värde.</p> </td> 
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
   <td> <p>Det här är <i>skiftlägesokänslig</i> version av <strong>innehåller</strong>. Till exempel: <code>cicontains inf</code> hämtar alla värden som innehåller antingen <code>Inf</code> eller <code>inf</code>.</p> <p> <p>Obs! Adobe Workfront söker efter det exakta ord eller den fras som du anger för varje filtersats. Om du till exempel söker efter ett projekt som innehåller frasen <code>new project</code> i namnet visar inte Workfront projekt som bara <code>new</code> eller bara <code>project</code>, eller <code>new main project</code> i namnet. Filtret hittar bara projekt med den exakta frasen <code>new project</code> i namnet.</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Innehåller inte</strong> </p> </td> 
   <td> <p><strong>cinotcontains</strong> </p> </td> 
   <td> <p>Det här är <i>skiftlägesokänslig</i> version av <strong>notcontains</strong>.</p><p>Den här modifieraren filtrerar efter objekt som saknar det angivna värdet.</p> <p>Till exempel: <code>does not contain inf</code> hämtar allt utan <code>Inf</code> eller <code>inf</code> i namnet.</p> <p>Obs! <span>Om fältet som du filtrerar efter har flera alternativ filtreras resultaten som innehåller både det alternativ som du anger, samt det alternativ som du anger och eventuella ytterligare alternativ.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>innehåller</strong> </p> </td> 
   <td> <p> Söker efter angiven <i>skiftlägeskänslig</i> text genom en hel textsträng.</p> <p>Använd till exempel <code>contains Inf</code> fångar allt med <code>Inf</code> i den, till exempel ordet <code>Infinity.</code></p> <p>Den här modifieraren kan bara användas i textlägesfilter.Mer information om textläge i filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p> </td> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notcontains</strong> </p> </td> 
   <td> <p>Den filtrerar efter objekt som saknar <i>skiftlägeskänslig</i> angivet värde.</p> <p>Till exempel: <code>notcontains inf</code> hämtar allt utan <code>inf</code>men visar värden som innehåller <code>Inf</code>.</p> <p>Den här modifieraren kan bara användas i textlägesfilter. Mer information om textläge i filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p> </td> 
  </tr> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>Det här är <i>skiftlägesokänslig</i> alternativ för <strong>eq</strong>. Det returnerar bara en exakt matchning av det sökda värdet.</p> <p>Om du t.ex. söker efter en uppgift med ett specifikt namn <code>task name cieq test</code> söker efter uppgifter där namnet är <code>Test</code>, <code>TEST</code>, eller <code>Test</code>, men ingen uppgift med namnet hittas <code>test 123.</code></p> <p>När du söker efter en status visas <strong>cieq</strong> modifierare stöds inte. Du bör använda skiftlägeskänslig modifierare <strong>eq</strong>, om du vill söka efter en status.</p> <p>Den här modifieraren kan bara användas i textlägesfilter. Mer information om textläge i filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p> </td>
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>cine</strong> </td> 
   <td> <p>Det här är <i>skiftlägesokänslig</i> alternativ för <strong>ne</strong>, och det är motsatsen till <b>cieq</b> modifierare. Det returnerar bara resultat som inte är en exakt matchning av det sökda värdet, utan hänsyn tagen till värdets skiftläge.</p> <p>Till exempel: <b>cine</b> returnerar alla värden som inte är lika med "current" eller "Current". </p> <p>Den här modifieraren kan bara användas i textlägesfilter. Mer information om textläge i filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p> </td> 
  </tr>   <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>Den här modifieraren returnerar bara en exakt, <i>skiftlägeskänslig</i> matchar det sökda värdet.</p> <p>Om du till exempel söker efter fullständiga projekt, <code>eq CPL</code> returnerar alla projekt med statusen Slutför. <code>eq CPL, CUR</code> returnerar inget resultat eftersom ett projekt inte kan vara fullständigt och aktuellt samtidigt.</p> <p>Den här modifieraren kan bara användas i textlägesfilter. Mer information om textläge i filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p>Det här är <i>skiftlägeskänslig</i> motsatt <strong>eq</strong>. Det returnerar bara resultat som inte är en exakt matchning av det sökda värdet, och det matchar även värdets skiftläge.</p> <p>Till exempel: <b>ne</b> returnerar värden som inte är lika med "Aktuell", men som inte returnerar några värden som inte är lika med "aktuell". </p> <p>Den här modifieraren kan bara användas i textlägesfilter. Mer information om textläge i filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>ciin</strong> </p> </td> 
   <td> <p> Det här är <i>skiftlägesokänslig</i> version av <strong>in</strong>.</p> <p>Den här modifieraren kan bara användas i textlägesfilter. Mer information om textläge i filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cinotin</strong> </p> </td> 
   <td> <p>Det här är <i>skiftlägesokänslig</i> version av <strong>notin</strong>.</p> <p>Den här modifieraren kan bara användas i textlägesfilter. Mer information om textläge i filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>Jämn</strong> </p> </td> 
   <td> <p><strong>in</strong> </p> </td> 
   <td> <p>Med den här modifieraren kan du skapa en kommaavgränsad lista med <i>skiftlägeskänslig</i> variabler som ska jämföras med ett enskilt attribut utvärderat i ett filter. Hela listan behandlas som en OR-sats och returnerar alla resultat som uppfyller villkoren för en eller flera av variablerna.</p> <p>Om du t.ex. söker efter projekt, använder <code>in CUR, PLN, CPL</code> returnerar alla projekt som har statusvärdet Aktuell, ELLER Planering, ELLER Fullständig.</p> <p>Inbyggd modifierare <strong>Jämn</strong> motsvarar textlägesmodifieraren i <strong>in</strong>. Det innebär att du kan välja Lika med flera värden för fältet.</p> <p>Du kan t.ex. välja "Status är lika med aktuell, Planering, Död" i en projektrapport och du kan visa projekt i någon av dessa statusar.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Inte lika med</strong> </p> </td> 
   <td> <p><strong>notin</strong> </p> </td> 
   <td> <p>Det här är <i>skiftlägeskänslig</i> motsatt <strong>in</strong>. Det returnerar bara resultat som inte finns i den angivna listan.</p> <p>Den här modifieraren kan bara användas i textlägesfilter. Mer information om textläge i filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p> <p>Obs! <span>Om fältet som du filtrerar efter har flera alternativ filtreras resultaten som innehåller både det alternativ som du anger, samt det alternativ som du anger och eventuella ytterligare alternativ.</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cilike</strong> </p> </td> 
   <td> <p>Det här är <i>skiftlägesokänslig</i> version av <strong>gilla</strong>. Till exempel: <code>cilike %Current% %Dead%</code> returnerar alla anteckningar som innehåller <code>Current to Dead</code> eller <code>current to dead</code>.</p> <p>Den här modifieraren kan bara användas i textlägesfilter. Mer information om textläge i filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>gilla</strong> </p> </td> 
   <td> <p>Den här modifieraren söker efter delar av en <i>skiftlägeskänslig</i> textsträng på liknande sätt som <strong>innehåller</strong>. Men <strong>gilla</strong> gör att du kan infoga jokertecken för att dela upp texten.</p> <p>Om du till exempel söker efter anteckningar, använda <code>like %Current% %Dead%</code> returnerar alla anteckningar som innehåller frasen"Aktuell till död". Den innehåller inga anteckningar som innehåller"Dead to Current". Varje värde söks igenom i den ordning som det listas. % representerar ett jokertecken som ersätter tecken eller textsegment.</p> <p>Den här modifieraren kan bara användas i textlägesfilter. Mer information om textläge i filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>Finns inte</strong> </td> 
   <td><strong>NOTEXISTER</strong> </td> 
   <td> <p>Den här modifieraren används bara med komplexa filter i en EXISTS-programsats. Dessa filter refererar endast till följande objekt: </p> 
    <ul> 
     <li>Objekt som sträcker sig över flera nivåer i objekthierarkin </li> 
     <li>Objekt som saknas </li> 
    </ul> <p>Mer information om hur du skapar komplexa filter med EXISTS-programsatser finns i artikeln <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">Skapa komplexa textlägesfilter med EXISTS-satser</a>. Detta är den enda modifieraren som används i EXISTS-satser.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Större än</strong> </p> </td> 
   <td> <p><strong>gt</strong> </p> </td> 
   <td> <p>Detta söker efter alla resultat med ett värde som är större än det angivna värdet, exklusive det angivna värdet.</p> </td> 
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
   <td> <p>Tillhandahåller två obligatoriska fältvärden och söker efter alla resultat inom intervallet för båda fälten, inklusive de angivna värdena.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notbetween</strong> </p> </td> 
   <td> <p>Det här är motsatsen till <strong>mellan</strong>. Det innehåller två obligatoriska värdefält och söker efter alla resultat utanför intervallet för båda fälten inklusive de angivna värdena.</p> <p>Den här modifieraren kan bara användas i textlägesfilter. Mer information om textläge i filter finns i <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p> </td> 
  </tr>

</tbody> 
</table>

---
product-area: reporting
navigation-topic: text-mode-reporting
title: Översikt över vanliga användningsområden för textläge
description: Översikt över vanliga användningsområden för textläge
author: Nolan
feature: Reports and Dashboards
exl-id: 81512837-1ec4-4dbc-ace4-bdf08fe667ce
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 0%

---

# Översikt över vanliga användningsområden för textläge

<!-- Audited: 1/2025 -->

<!--(NOTE: Alina: ***This is linked to Understanding Text Mode (article), and the TOC article for examples of various reporting elements)</p>-->

Du kan utöka rapportfunktionerna genom att använda textläge i rapporter och rapportelement. Du kan också använda en version av textläget för att skapa mer komplexa, beräknade anpassade fält. Mer information om textläge finns i [Översikt över textläge](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

I den här artikeln beskrivs bara några exempel på var du troligen skulle behöva använda textläget för att utöka funktionerna för rapporter och beräknade anpassade fält i Adobe Workfront. En mer omfattande lista med exempel finns i:

* [Egna exempel på vy, filter och gruppering: artikelindex](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
* [Beräknade anpassade data i rapporter](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md)

Mer information om hur du skapar rapporter i textläge, inklusive klasser, videoklipp och självstudiekurser, finns i avsnittet Lär dig på Adobe Experience League webbplats.

## Instanser där du kan använda textläge i listor och rapporter

Vi rekommenderar att du använder rapport- och listverktyget för att skapa vyer, filter och grupperingar. I vissa fall kan du dock använda textläge för att förbättra rapporter och listor.

Du kan använda textläget när du vill uppnå följande i Workfront:

* Skapa anpassade beräknade anpassade fält i ett anpassat formulär.\
  Mer information om beräknade anpassade fält finns i avsnittet [Använd textläge i beräknade anpassade fält](#use-text-mode-in-calculated-custom-fields) i den här artikeln.
* Förbättra filter, vyer och grupperingar utöver vad som är möjligt i Report Builder. Mer information om hur du använder textläge för filter, vyer och grupperingar finns i följande avsnitt i den här artikeln:

   * [Använd textläge i vyer](#use-text-mode-in-views)
   * [Använd textläge i filter](#use-text-mode-in-filters)
   * [Använd textläge i grupperingar](#use-text-mode-in-groupings)

* Skapa egna uppmaningar. Du kan bara skapa egna uppmaningar med textläge.

  Mer information om hur du skapar anpassade uppmaningar finns i [Lägga till en uppmaning i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

## Använd textläge i beräknade anpassade fält {#use-text-mode-in-calculated-custom-fields}

Du kan använda textläge för att lägga till ett beräknat anpassat fält i ett anpassat formulär.

Mer information om hur du lägger till ett beräknat anpassat fält i ett anpassat formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Mer information om hur du skapar ett beräknat anpassat fält i textläge finns i [Lägg till beräknade fält i ett formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Du kan t.ex. lägga till ett beräknat anpassat fält som visar en tids- och datumstämpel för den tidpunkt då ett objekt markerades som Pågår. Du kan använda den här beräkningen för andra statusvärden.

Mer information finns i [Exempel på beräknade anpassade fält: visa en statustidsstämpel i ett anpassat formulär](../../../reports-and-dashboards/reports/calc-cstm-data-reports/example-status-timestamp-in-calculated-field.md).

## Använd textläge i vyer {#use-text-mode-in-views}

Du kan använda textläge i vyer för att expandera fält och objekt som du kan visa i vyn.

Exempel på de vanligaste anledningarna att använda textläge i en vy finns i följande artiklar:

* [Visa: visningsobjekt som inte ingår i standardgränssnittet](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-objects-not-in-standard-interface.md)
* [Visa: visa resultatet av en beräkning mellan två fält i en kolumn](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-calculation-between-two-fields.md)
* [Visa: redigera bredden på en kolumn permanent](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md)
* [Visa: sammanfoga information från flera kolumner i en delad kolumn](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md)
* [Visa: ta bort länk till ett objekt i en kolumn](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-remove-link-to-object.md)
* [Referenssamlingar i en rapport](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)
* [Visa: dölj innehållet i en kolumn](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-hide-column-content.md)
* [Visa: visa en bild i stället för en sträng i en kolumn](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-image-in-view.md)
* [Visa: visa indrag för aktiviteter i en uppgiftslista](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-task-identations.md)
* [Visa: beräkna tid- och datumskillnader](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-calculate-time-and-date-differences.md)

## Använd textläge i filter {#use-text-mode-in-filters}

Du kan använda textläget när du skapar filter för att expandera fält och objekt som du kan filtrera efter.

Exempel på de vanligaste anledningarna att använda textläge i ett filter finns i följande artiklar:

* [Filter: skapa flera filterregler som refererar till samma fält (&quot;AND&quot;-satser)](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-refrence-the-same-field-multiple-times.md)
* [Filter: visa endast objekt med godkännandestatus](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-for-items-in-approval-status.md)
* [Filter: visa objekt efter status med samma namn när statusvärdena är kopplade till olika grupper](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-same-name-statuses-from-different-groups.md)
* [Filter: ta bort objekt i en lista genom att jämföra två fält](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-items-by-comparing-two-fields.md)
* Avsnittet [Exempel på textlägesfilter som sträcker sig över flera nivåer i objekthierarkin](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md#examples) i artikeln [Skapa komplexa textlägesfilter med EXISTS-satser](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md)
* Avsnittet [Skapa filter för komplexa textlägen för saknade objekt](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md#missing-object-filters) i artikeln [Skapa filter för komplexa textlägen med EXISTS-satser](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md)

## Använd textläge i grupperingar {#use-text-mode-in-groupings}

Du kan använda textläget när du skapar grupperingar för att utöka fält och objekt som du kan gruppera efter i listor och rapporter.

Exempel på de vanligaste anledningarna att använda textläge i en gruppering finns i följande artiklar:

* [Gruppering: Organisera listresultat med ett beräknat värde som är gemensamt för alla objekt i grupperingen](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-by-calculated-common-values.md)
* [Gruppering: lägg till en fjärde gruppering i en lista](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-add-fourth-grouping.md)
* [Gruppering: redigera visningsnamnet i en gruppering](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-rename-grouping.md)
* [Gruppering: ange om resultatet av en gruppering ska komprimeras eller expanderas i textläge](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-collapsed-or-expanded-results.md)

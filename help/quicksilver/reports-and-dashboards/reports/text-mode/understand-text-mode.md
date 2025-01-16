---
product-area: reporting
navigation-topic: text-mode-reporting
title: Översikt över textläge
description: Du kan skapa en rapport eller en lista i Adobe Workfront med hjälp av standardgränssnittet eller textlägesgränssnittet när du skapar elementen som utgör rapporten eller listan.
author: Nolan
feature: Reports and Dashboards
exl-id: 8be8cbd0-da1b-4e90-a52e-dc352f646d18
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 0%

---

# Översikt över textläge

<!-- Audited: 1/2025 -->

<!--(NOTE: Linked to the UI (for the areas mentioned in the comments below and the new NWE filters as well))-->

<!--(NOTE: Alina: ***Linked to other articles. Do not move, rename or change url.Linked to the product, in the report builder, when using a field that is not recognized in standard mode.)-->

<!--(NOTE: This will be linked to the Ninja feature about adding a filter to the User typeahead field (which originally is open only for text mode filters). Update the Context Sensitive sheet at release time)-->

Du kan skapa en rapport eller en lista i Adobe Workfront med hjälp av standardgränssnittet eller textlägesgränssnittet när du skapar elementen som utgör rapporten eller listan.

Med standardgränssnittet kan du referera till fält och deras attribut som är tillgängliga i Workfront-gränssnittet.

I textläge kan du referera till fält och attribut som kanske inte är tillgängliga i standardläge, men som är tillgängliga i Workfront-databasen.

Mer information om hur du skapar rapporter i textläge, inklusive klasser, videoklipp och självstudiekurser, finns i avsnittet Lär dig på Adobe Experience League webbplats.

## Att tänka på innan du använder textläge

>[!TIP]
>
>Du kan också utöka funktionerna för beräknade anpassade fält genom att använda en version av textläget för anpassade fält. Syntaxen och reglerna för att skapa ett beräknat anpassat fält skiljer sig från dem du använder i rapporter och listor. Mer information om hur du lägger till ett beräknat anpassat fält finns i [Lägg till beräknade fält i ett formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

* Innan du börjar använda textläge i dina rapporter rekommenderar vi att du går igenom våra lektioner för avancerad rapportering för att få en bättre förståelse för vårt textläge.
* Vi rekommenderar att du använder standardläget för att säkerställa att de rapporter du skapar förblir intakta när Workfront uppdateras. I textläget kan du skapa mer komplexa vyer, filter och grupperingar, men det är också mer komplicerat att underhålla och garanteras inte när Workfront uppdateras.
* Vi rekommenderar att du alltid försöker att skapa alla rapportelement i standardgränssnittet och växlar till textlägesbyggaren endast för få justeringar.

  >[!TIP]
  >
  >Med standardverktyget får du viktiga byggstenar och mönster för kod som du sedan kan använda när du ändrar koden i textläge.

* Det finns en uppsättning regler och en unik syntax som du måste använda för att kunna skapa rapporter och listor i textläge. Kontrollera att du känner till Workfront syntax för textläge innan du börjar.

  Mer information om syntax och regler för användning av textläge finns i [Syntaxöversikt i textläge](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

* När du har anpassat ett rapportelement i textläge kanske du inte kan växla tillbaka till standardläge (i en vy) eller så kan koden för det element du skapade tas bort (i filter och grupperingar). Detta beror på att inte alla fält som stöds i textläge stöds i standardläge.

## Gränssnitt för standardläge

Gränssnittet Standardläge visar fält som mappar de programelement som du vill visa i en rapport eller lista. Standardlägesgränssnittet är en uppsättning listrutor där du kan välja de fält som du vill visa i rapporter eller listor.

Mer information om standardlägesgränssnittet och hur du skapar en rapport eller en lista finns i:

* [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
* [Rapportelement: filter, vyer och grupperingar](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)

## Textlägesgränssnitt

I textläget kan du skapa mer komplexa vyer, filter, grupperingar och uppmaningar genom att låta dig använda fält som inte är tillgängliga i standardlägesgränssnittet. I Workfront-textläge är en samling kodade satser som anger vilka objekt som ska visas i en rapport eller lista.

En fullständig lista över alla våra rapportbara fält finns i [API-utforskaren](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>Alla fält som är tillgängliga via API är inte tillgängliga via textlägesgränssnittet. Om du använder rätt fält i textlägeskoden och inte visar de resultat du förväntar dig, kan det hända att fältet bara kan rapporteras via API:t.

## Få åtkomst till rapportelement och redigera textläge {#access-reporting-elements-and-edit-text-mode}

Att få åtkomst till textlägesgränssnittet är detsamma för vyer, grupperingar och filter när du får åtkomst till dem från en rapport eller lista.

Mer information om hur du använder textläge i vyer, filter och grupperingar finns i:

* [Redigera en vy i textläge](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
* [Redigera ett filter i textläge](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
* [Redigera en gruppering i textläge](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

Anpassade uppmaningar kan bara redigeras i textläge. Du kan bara komma åt uppmaningar från en rapport.

Mer information om hur du får åtkomst till textlägesgränssnittet för anpassade uppmaningar finns i [Lägga till en uppmaning i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

## Vanliga skäl att använda textläge {#common-reasons-to-use-text-mode}

Förutom att skapa anpassade uppmaningar som bara kan konfigureras i textläge rekommenderar vi att du använder rapportverktyget för att skapa vyer, filter och grupperingar. I vissa fall kan du dock använda textläge för att förbättra rapporter och listor.

Mer information om vanliga användningsområden för textläge finns i [Översikt över vanliga användningsområden för textläge](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

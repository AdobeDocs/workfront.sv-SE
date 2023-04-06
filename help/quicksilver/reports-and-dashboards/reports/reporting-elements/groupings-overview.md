---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Översikt över grupperingar i Adobe Workfront
description: Du kan lägga till grupperingar för att hantera layouten för informationen i rapporter och listor.
author: Nolan
feature: Reports and Dashboards
exl-id: d050372e-c4a0-4c49-b220-5b35334ab8d0
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 0%

---

# Översikt över grupperingar i Adobe Workfront

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This article was supposed to be replaced by "Groupings overview", but decided to keep this here because this is linked in too many places. "Create groupings" and "Edit existing groupings" have been added also (with videos) to replace portions of the old content here.) </p>
-->

Du kan lägga till grupperingar för att hantera layouten för informationen i rapporter och listor.

Du kan lägga till grupperingar i rapporter på följande sätt:

* Du kan skapa grupperingar genom att redigera befintliga grupperingar.

   Mer information om hur du anpassar en befintlig gruppering finns i [Redigera befintliga grupperingar](../../../reports-and-dashboards/reports/reporting-elements/edit-existing-groupings.md).

* Du kan skapa grupperingar från grunden.

   Mer information om hur du skapar en gruppering från grunden finns i [Skapa grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

Som standard visas grupperingar i en grå eller blå markering i rapporten eller listan. Resultatet av rapporten eller listan visas under den enskilda grupperingen, utan någon högdager.

Du kan lägga till upp till tre grupperingar i en rapport. Du kan ordna information med upp till fyra grupperingar genom att skapa en matrisrapport. Mer information om matrisrapporter finns i [Skapa en matrisrapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

I en standardgrupperingsrapport är den första grupperingen en mörkare färg, den andra och den tredje grupperingen ljusare. Du kan inte anpassa färgen på högdagern för din gruppering eller teckensnittet för grupperingsnamnet. Siffran inom parentes efter grupperingens namn representerar antalet resultat under den grupperingen. Om rapporten sträcker sig över flera sidor måste du se till att den visas *Alla* resultaten i rapporten eller listan för att få en korrekt uppskattning av resultaten för varje gruppering.

![Exempelgruppering](assets/grouping-example-blue.png)

Tänk på följande när du arbetar med grupperingar:

* Du kan anpassa informationen i befintliga grupperingar. Alla användare som kan visa grupperingarna kan också se dina ändringar.
* Din Workfront-administratör måste ge dig åtkomst till Redigera filter, Vyer och Grupperingar för att kunna skapa grupperingar.

   Information om hur du beviljar åtkomst till filter, vyer och grupperingar finns i [Bevilja åtkomst till filter, vyer och grupperingar](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Din behörighetsnivå för en gruppering avgör hur en gruppering sparas. Om du skapade grupperingen från början kan du spara ändringarna, annars uppmanas du att spara en version av grupperingen. Om du gör ändringar i en gruppering som du har delat med andra påverkas även dessa.
* Du kan bara anpassa en gruppering som delats med dig om den användare som delade den gav dig behörigheten Hantera. Mer information om hur du delar en gruppering finns i [Dela ett filter, en vy eller en gruppering](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
* Du kan inte redigera en infogad gruppering.
* Du kan inte gruppera efter anpassade fält som har flera val (till exempel kryssrutor) eller efter fält som kan ha flera värden (till exempel Resurshanteraren).

## Ytterligare information om grupperingar

Du kan hantera rapportinformation ytterligare när du använder grupperingar genom att samla värdena i varje kolumn på grupperingsraden samt sortera informationen efter fältet i grupperingen. Du kan också ta bort en gruppering när den inte längre behövs.

* [Sammanställa värden i grupperingar](#aggregate-values-in-groupings)
* [Sortera efter gruppering](#sort-by-a-grouping)
* [Ta bort en gruppering](#remove-a-grouping)

### Sammanställa värden i grupperingar {#aggregate-values-in-groupings}

Du kan sammanställa de data som visas i rapporten på grupperingsraden genom att sammanfatta värdena i varje kolumn i rapporten. Mer information om hur du sammanfattar kolumndata i en gruppering finns i [Översikt över vyer i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

>[!NOTE]
>
>Följande undantag gäller för överordnade objekt (till exempel överordnade uppgifter) när du samlar värden för följande fält i grupperingar:
>
>* Alla sifferfält och valutafält utom Faktiska timmar (till exempel Planerad/Faktisk arbetskostnad, Planerad/Faktisk utgiftskostnad, Planerad/Faktisk kostnad, Planerad timmar) samlar endast värdena för de underordnade aktiviteterna och fristående aktiviteter. De sammanställer inte värdena för de överordnade uppgifterna eller de överordnade överordnade uppgifterna.
>* Faktiska timmar sammanställer värdena för huvuduppgiften och de fristående uppgifterna. de sammanställer inte siffrorna för överordnade och underordnade uppgifters överordnade uppgifter.
>* Anpassade datafält för tal- och valutavärden samlar alla uppgifter: föräldrar, barn, föräldrar till föräldrar och fristående uppgifter.


### Sortera efter gruppering {#sort-by-a-grouping}

Det går inte att sortera grupperingar. Vyer kan sorteras. Om du vill sortera en lista efter det värde som hämtas i grupperingen måste du ta med det värdet i någon av vykolumnerna och tillämpa sorteringen i vyn. På så sätt sorteras listan efter värdet i grupperingen indirekt (sorteras efter värdet i vyn som också fångas i grupperingen). Mer information om hur du skapar vyer och sorterar efter värden i vyer finns i [Översikt över vyer i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### Ta bort en gruppering {#remove-a-grouping}

Hur du tar bort en gruppering beror på om du först skapade grupperingen eller om grupperingen delades med dig. Du kan inte ta bort en standardgruppering.

* **Om du har skapat grupperingen och du tar bort den** tas grupperingen bort från Workfront. Grupperingen är inte längre tillgänglig för användare som du tidigare delat den med.
* **Om grupperingen delades med dig och du tar bort den**, tas grupperingen bara bort åt dig. Den användare som ursprungligen skapade den och alla andra användare som den har delats med har fortfarande åtkomst till grupperingen.

Mer information om hur du tar bort en gruppering finns i artikeln [Ta bort filter, vyer och grupperingar](../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).

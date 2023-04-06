---
product-area: reporting
navigation-topic: reporting-elements
title: '''Rapporteringselement: filter, vyer och grupperingar'
description: De huvudelement som varje lista och rapport måste ha i Workfront är ett filter, en vy och en gruppering. Varje element innehåller olika information i alla rapporter.
author: Nolan
feature: Reports and Dashboards
exl-id: 5697905e-42c0-403b-85d4-798a1a3a2e7f
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 0%

---

# Rapportelement: filter, vyer och grupperingar

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>AL: Add information here about all the different kinds of FVGs: in reports, in lists, beta, etc // OR: this article should be a high-level overview of reporting elements. Then, each type of element should have:</p>
<p>- overview for Filters</p>
<p>- create a filter</p>
<p>- share a filter</p>
<p>ALL in Reporting elements but the Shared ones should be linked to Basics> Sharing; some of the articles in the Basics> Navigation> Use lists might beed to link here as well</p>
</div>
-->

Det finns flera element som gör det möjligt att skapa en lista eller rapport i Adobe Workfront. De huvudelement som varje lista och rapport måste ha är ett filter, en vy och en gruppering. Varje element innehåller olika information i alla rapporter.

## Överväganden om rapportelement

Tänk på följande när du arbetar med filter, vyer och grupperingar:

* Rapporteringselement fungerar som byggstenar för rapportering. De definierar utseendet på en rapport eller en lista samt informationen i rapporten eller listan.
* Rapporter i Workfront är specifika för ett objekt. Du måste definiera huvudobjektet för en rapport innan du kan skapa rapporten. Därför är alla rapportelement objektspecifika.
* Din Workfront-administratör måste ge dig åtkomst till filter, vyer och grupperingar på din åtkomstnivå för att kunna visa eller redigera dem i listor och rapporter.

   Information om hur du beviljar åtkomst till filter, vyer och grupperingar finns i [Bevilja åtkomst till filter, vyer och grupperingar](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Din Workfront-administratör måste ge dig åtkomst till rapporter, instrumentpaneler och kalendrar på din åtkomstnivå för att kunna visa eller redigera rapporter.

   Information om hur du beviljar åtkomst till rapporter, kontrollpaneler och kalendrar finns i [Ge åtkomst till rapporter, instrumentpaneler och kalendrar](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Om du väljer ett filter, en vy eller en gruppering i en rapport eller lista behåller Workfront markeringen för objektets listor även efter att du har loggat ut eller stängt webbläsaren. Om du t.ex. väljer en viss vy för en uppgiftsrapport visas valet för andra uppgiftslistor, t.ex. listan med uppgifter i ett projekt.

## Filter

Filtret styr de resultat som visas i en rapport och begränsar vanligtvis resultatet från allmän till specifik. Det fungerar som en utsikt som bara hämtar den information du behöver och återför den informationen till din rapport.

Om du till exempel bara vill se uppgifter som tilldelats den inloggade användaren, kan du skapa ett filter med namnet &quot;Mina uppgifter&quot;, definiera villkoren som måste uppfyllas för filtret och köra rapporten så att endast uppgifter som tilldelats den inloggade användaren visas.

Vissa filterattribut är:

* Workfront tillhandahåller ett antal filter för olika objekt som standard.
* Du kan anpassa filter som du äger eller hanterar.

   Mer information om filter finns i artikeln [Översikt över filter i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

![Filterikon](assets/projects-list-with-filter-drop-down-highlighted-nwe.png)

## Vyer

Genom att definiera vyn för en rapport definierar du vilken information du vill ta med i rapporten. Precis som för alla rapportelement baseras vyerna på en objekttyp.\
En vy för en uppgiftsrapport kan t.ex. visa Förfallodatum, innehålla ekonomisk information som Kostnad eller användas för att visa information om tilldelningar och leveransdatum. Vyer kan användas för att ge olika detaljer om data i rapporten.

Vissa attribut för vyer är:

* Du kan använda en Workfront-standardvy eller skapa en egen.
* Du kan använda ytterligare vyer från listrutan Visa när du har kört en rapport.
* Ytterligare vyer ersätter tillfälligt den vy som definierats när rapporten skapas. Standardvyn visas dock nästa gång du återgår till rapporten.

   Mer information om vyer finns i artikeln [Översikt över vyer i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Grupperingar

En gruppering styr hur du organiserar data, vilket gör det lättare att läsa och förstå. Grupperingar skapar vågräta fält i en rapport som visar resultat som listas tillsammans med gemensamma attribut. Du definierar villkoren för hur du vill gruppera resultaten av rapporten när du skapar grupperingen.

Om du till exempel grupperar en lista med uppgifter som omfattar flera projekt efter deras projektnamn, ordnas alla respektive uppgifter som tillhör ett enskilt projekt under det namnet.

Vissa attribut för grupperingar är:

* Grupperingar är ett obligatoriskt rapportelement om du senare vill lägga till ett diagram i rapporten.
* Grupperingar visar ett sammanställningsvärde i resultatet. &#x200B;
* Grupperingar bestämmer axeln i diagram.
* Grupperingar bestämmer rubrikidentifieringen i matrisrapporter.\
   Mer information om matrisrapporter finns i artikeln [Skapa en matrisrapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

* Grupperingar hjälper till att skapa fliken Sammanfattning för en rapport, med rapportens aggregerade värden.
* I Workfront finns ett antal grupperingar för olika objekt som standard.
* Du kan anpassa grupperingar som du äger eller hanterar.

   Mer information om grupperingar finns i [Översikt över grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## Andra rapporteringselement

Förutom filter, vyer och grupperingar kan du även lägga till följande element i en rapport:

* **Fråga**: Ett öppet filter som kan anpassas och tillämpas på olika sätt varje gång du kör en rapport.\
   Mer information om uppmaningar finns i artikeln [Lägga till en fråga i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* **Diagram**: Du kan förbättra dina rapporter genom att lägga till ett diagram och visa informationen på ett visuellt sätt.\
   Mer information om diagram i rapporter finns i artikeln [Lägga till ett diagram i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

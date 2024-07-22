---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Översikt över planerade och beräknade datum
description: Det finns flera typer av datum som visar tidslinjen för uppgifter mellan när de kan starta och när de kan slutföras.
author: Alina
feature: Work Management
exl-id: 7cc68fc4-5f79-4ce6-a404-737ea8959ec3
source-git-commit: 811d8076a0b344e863b25aa253a0fb1c102f0435
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# Översikt över planerade och beräknade datum

<!--Audited: 07/2024-->

Det finns flera typer av datum som visar tidslinjen för uppgifter mellan när de kan starta och när de kan slutföras. Nedan följer några datum som visar tidslinjen för uppgifter:

* Planerade startdatum och planerade slutförandedatum
* Planerade startdatum och planerade slutförandedatum
* Beräknad starttid och beräknad förfallotid
* Faktiska start- och slutförandedatum

I den här artikeln beskrivs skillnaderna mellan beräknade och planerade datum för projekt.

När aktiviteten skapas för första gången bör datumen för planerad, projicerad och beräknad matcha. Det finns vissa undantag.

Mer information om projekt-, uppgifts- och utgivningsdatum i Adobe Workfront finns i [Översikt över projekt-, uppgifts- och utgivningsdatum i Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/definitions-pti-dates.md).

## Översikt över planerade datum

Planerade datum är de datum som projektägaren definierar som start- och slutdatum för aktiviteterna. Du eller projektägaren kan ändra planerade datum för en uppgift manuellt.

## Översikt över faktiska datum

När en uppgift skapas för första gången har den inga faktiska datum eftersom den inte har startats eller slutförts än.

## Översikt över planerade och beräknade datum

Under ett projekts livslängd ligger de beräknade och beräknade datumen mer i linje med projektets verklighet, eftersom de tar hänsyn till vad som kan påverka början och slutet av en uppgift. Detta gör att de ändras från planerade datum.

Tänk på följande när du arbetar med Planerade och beräknade datum för uppgifter:

* Du kan inte ändra varken beräknade eller planerade datum för uppgifter manuellt. Båda beräknas av Adobe Workfront.
* När du skapar en uppgift bör datumen för Projicerat och Uppskattat vara identiska och de bör visa de faktiska tidpunkterna när uppgifterna kan börja eller sluta.\
  Vissa uppdateringar som du gör för uppgifter påverkar värdena för Planerade och Uppskattade datum direkt.

  Om användaren till exempel startar eller slutför en uppgift, visar aktiviteten Faktiska start- och slutförandedatum som påverkar aktivitetens beräknade och beräknade datum. Om en tilldelad för aktiviteten ändrar implementeringsdatumet påverkar det här datumet även aktivitetens planerade datum.

## Skillnad mellan planerade och beräknade datum

Skillnaden mellan beräknade och beräknade datum är:

* Planerade datum påverkas av att en användare gör följande uppdateringar för uppgiften:

   * Lägg till ett begränsningsdatum genom att lägga till en fast aktivitetsbegränsning
   * Lägg till ett implementeringsdatum

* Beräknade datum tar endast hänsyn till det verkliga förloppet för en aktivitet under en viss tidpunkt.

**Exempel:** Om vi har en aktivitet som har ett planerat startdatum den 20 september och ett planerat slutförandedatum den 24 september och som måste avslutas den måste avslutas den 24 september. Den här aktiviteten har en varaktighet på 4 dagar.

Det beräknade slutförandedatumet beräknas utifrån det aktuella förloppet för arbetet i uppgiften. Om det är den 23 september idag och uppgiften inte har startat ännu är det beräknade slutförandedatumet den 27 september (det ska vara slutfört efter 4 dagar, förutsatt att arbetet har startats idag).

Om aktiviteten har slutförts till 50 % idag är det beräknade slutförandedatumet den 25 september (det ska vara slutfört efter 2 dagar, vilket är halva tiden för uppgiften).


### Förstå när planerade datum uppdateras för aktiviteter {#understand-when-projected-dates-update-on-tasks}

De beräknade datumen kan antingen matcha andra aktivitetsdatum eller så är de en beräkning som görs av Workfront och som tar hänsyn till aktivitetens verkliga förlopp.

I följande lista visas flera scenarier när de beräknade datumen för uppgifter ändras under ett projekts livslängd beroende på vad som händer i det verkliga livet för aktiviteten:

* När en uppgift har markerats som slutförd:

  `Projected Dates = Estimated Dates = Actual Dates`

* När en uppgift har ett faktiskt startdatum:

  `Projected Start Date = Estimated Start Date = Actual Start Date`

* När en aktivitet inte har ett faktiskt startdatum, men det finns ett obligatoriskt villkor för det planerade startdatumet (måste börja den) som kommer i framtiden:

  `Projected Start Date = Constraint Date`

  Mer information om begränsningsdatum finns i [Ordlista för Adobe Workfront-terminologi](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* När en aktivitet inte har ett faktiskt startdatum och aktiviteten inte har ett tvingat villkorsdatum:

  `Projected Start Date = the next available date in the future that falls within working schedule`

* När den som tilldelats uppdaterar implementeringsdatumet:

  `Projected Completion Date = Commit Date`

  Mer information om implementeringsdatum finns i [Genomför datumöversikt](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

* När aktiviteten inte har ett uppdaterat implementeringsdatum och aktiviteten har en tvingad begränsning (Måste slutföras) för det planerade slutförandedatumet som infaller i framtiden:

  `Projected Completion Date = Constraint Date`

* När en aktivitet inte har ett uppdaterat implementeringsdatum, ett framtvingat villkorsdatum i framtiden eller har ett tidigare begränsningsdatum:

  `Projected Completion Date = system calculation for the Completion Date based on the current progress and the work left to be done`

### Förstå när beräknade datum uppdateras för uppgifter {#understand-when-the-estimated-dates-update-on-tasks}

Jämfört med de scenarier som beskrivs ovan för Planerade datum återspeglar de beräknade datumen alltid Workfront verkliga analys av när aktiviteten kommer att starta eller slutföras, oavsett begränsnings- eller implementeringsdatum.

## Vad påverkar tidslinjen för en uppgift

Nedan följer några exempel på vad som kan påverka den verkliga tidslinjen för en uppgift:

* Uppgiftsförlopp i relation till planerade datum och till aktuell dag
* Procent färdigt för uppgiften hittills
* Föregående relation
* Föregående förlopp
* Användartilldelning

  >[!NOTE]
  >
  >Användartilldelning kan påverka det beräknade slutförandedatumet för en aktivitet om det påverkar hastigheten med vilken uppgiften kan slutföras. Om till exempel varaktighetstypen för aktiviteten är Anstruken kan du slutföra uppgiften tidigare genom att lägga till tilldelningar. Därför ändras det beräknade slutförandedatumet.

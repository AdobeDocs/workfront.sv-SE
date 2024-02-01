---
title: Översikt över avsnittet Historik
description: Du kan granska ändringar som gjorts i posten och som spelats in av systemet på den högra panelen i en post i Adobe Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---


# Översikt över avsnittet Historik

{{maestro-important-intro}}

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Maestro records" should be there-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

Du kan samarbeta med poster i Adobe Maestro genom att lägga till kommentarer eller svar på den högra panelen i en post. I det här området kan du även visa andra ändringar som har gjorts i posten och som har spelats in av systemet.

I den högra panelen för en post visas följande avsnitt:

* **Kommentar**: Visar kommentarer och svar som användare lägger till i poster. Mer information om hur du hanterar kommentarer i Maestro-poster finns i [Hantera postkommentarer](/help/quicksilver/maestro/records/manage-record-comments.md).
* **Historik**: Visar ändringar som användarna gör i postfälten.

## Leta reda på historikavsnittet för en post

{{step1-to-maestro}}

Den senast öppnade arbetsytan öppnas som standard.

1. Välj en tabellvy på menyn **Visa** listruta.
1. Klicka på namnet på en post i tabellvyn.

   Posten **Information** sidan öppnas. Kommentarsområdet öppnas som standard i den högra panelen.
1. Klicka på **Visa historik** icon ![](assets/show-history-icon.png). Alla ändringar som görs i postens fält visas på den högra panelen, med början från den senaste.
1. (Valfritt) Klicka på **Dölj historik** icon ![](assets/hide-history-icon.png) för att stänga den högra panelen.

## Överväganden om historikavsnittet

Du kan granska ändringarna som gjorts för postfält i historikavsnittet på den högra panelen för en driftspost eller taxonomis informationssida.

![](assets/history-area-in-comments.png)

* Följande information registreras i historikavsnittet:

   * Alla fältändringar

   * Det gamla och de nya värdena i fälten när värdena ändras. De gamla värdena visas i genomstrykningsformat.

   * Det fullständiga namnet på användaren som gjorde ändringen

   * En datum- och tidsstämpel som anger när ändringen inträffade.

* Fält av följande typer visar alltid det gamla värdet (i genomstrykningsformat) och det nya värdet:

   * Text
   * Stycke
   * Valuta
   * Datum
   * Nummer
   * Procent
   * Enkelval

* Fält av följande typer visar det gamla värdet i genomstrykningsformat endast om minst ett av de flera värdena har tagits bort:

   * Flera val
   * Länkade postfält
   * Folk

  Om ändringen bara har lagt till värden i fältet visas inte det gamla värdet och bara det nya fältvärdet visas.

* Fält av typen Kryssruta visar aldrig det gamla värdet i genomstrykningsformat. Om fältet redigeras visas bara det aktuella läget när ändringen gjordes.

  Mer information om Maestro-fält finns i [Skapa fält](/help/quicksilver/maestro/fields/create-fields.md).

* Ändringar i fält av följande typer visas inte i avsnittet Historik:

   * Länkade (sökning) fält
   * Formel
   * Skapad av
   * Skapad den
   * Senast ändrad av
   * Senast ändrat den

* Om ett fält tas bort från systemet finns uppdateringarna som gjorts i det fältet kvar i historikavsnittet. Det finns inget som tyder på att fältet har tagits bort i historikdelen av en post.
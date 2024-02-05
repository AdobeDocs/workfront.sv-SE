---
title: Översikt över posttyper och taxonomier
description: Posttyper är byggstenarna i en Maestro-arbetsyta.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: 5681b540bceddaae85116b632e968d94761eec0d
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Översikt över posttyper och taxonomier

{{maestro-important-intro}}

Till skillnad från Workfront, där objekttyperna är fördefinierade, kan du skapa egna objekttyper i Adobe Maestro. I Workfront har till exempel objekttyperna Program, Portfolio, Projekt, Uppgift eller Utgåva redan skapats.

Maestro-objekttyper kallas&quot;posttyper&quot;. Posttyper är byggstenarna i en Maestro-arbetsyta. Mer information om arbetsytor finns i [Skapa arbetsytor](../architecture/create-workspaces.md).

## Översikt över posttyp

I Maestro kan du skapa anpassade posttyper som passar din organisations behov.

* Följande typer är Maestro-posttyper:

   * [Driftposttyp](#operational-record-type): En posttyp som representerar strategiska planer, initiativ eller planerat arbete. Exempel: Campaign, Activity, Tactic, Opportunity kan vara operativa posttyper.
   * [Taxonomi](#taxonomy): Posttyper som samlar in attribut om en operativ posttyp. Region, Adress, Audience kan till exempel vara taxonomier.

* När du skapar en posttyp kan bara du och de du ger behörighet att komma åt arbetsytan visa posttypen.
* Du måste skapa en arbetsyta innan du kan skapa posttyper för arbetsytan.
* Du kan ha en kombinerad summa på 1 000 driftsposttyper och taxonomier på en arbetsyta. Detta inkluderar posttyper eller taxonomier som du skapar från grunden eller som du importerar från andra system.

### Driftposttyp{#operational-record-type}

En operativ posttyp är en Maestro-posttyp som representerar arbetsrelaterade objekt.

![](assets/operational-record-type-blank.png)

Mer information om posttyper, inklusive hur du skapar dem, finns i [Skapa posttyper](../architecture/create-record-types.md).

### Taxonomi{#taxonomy}

En taxonomi är en posttyp som samlar in attribut om en operativ posttyp.

![](assets/taxonomy-record-type-blank.png)

Mer information om posttyper för taxonomi finns i [Skapa en taxonomi](../architecture/create-a-taxonomy.md).

Även om det är samma sak att skapa taxonomier som att skapa operativa posttyper, skiljer Maestro konceptuellt mellan en operativ posttyp och en taxonomiposttyp. Syftet med taxonomier är att förbättra den operativa registertypen. Taxonomier bör inte representera arbetsobjekt direkt.  <!--this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.-->

<!--mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc -->

Till exempel kan Audience, Region eller Address vara posttyper av taxonomintyp.

Mer information finns i [Skapa en taxonomi](../architecture/create-a-taxonomy.md).

## Likheter och skillnader mellan den operativa posttypen och taxonomier

I följande tabell visas några likheter och skillnader mellan de operativa posttyperna och taxonomierna:

| Posttyp och -egenskap | Driftposttyp | Posttyp för taxonomi |
|-------------------------------------------------------------|:-----------------------:|:--------------------:|
| De ingår i en arbetsyta | ✓ | ✓ |
| Du kan skapa dem automatiskt från en arbetsytemall | ✓ | ✓ |
| Du kan skapa dem manuellt, från början | ✓ | ✓ |
| Du kan skapa dem genom att kopiera och klistra in information från en extern fil eller lista | ✓ | ✓ |
| Du kan skapa genom att importera en Excel- eller CSV-fil | ✓ |                     |
| Du kan skapa skrivskyddade posttyper genom att ansluta till objekttyper från andra program | ✓ |                     |
| De representerar arbetsrelaterade objekt | ✓ |                      |
| De representerar attribut om arbetsrelaterade objekt |                         | ✓ |
| Du kan skapa från början | ✓ | ✓ |
| Du kan skapa genom att importera en Excel- eller CSV-fil | ✓ |                      |
| Du kan ansluta posttypen till ett objekt från ett annat program | ✓ |                      |
| Du kan ansluta till andra Maestro-posttyper | ✓ |                    |
| Du kan visa deras associerade poster i en tabellvy | ✓ | ✓ |
| Du kan visa deras associerade poster i en tidslinjevy | ✓ | ✓ |

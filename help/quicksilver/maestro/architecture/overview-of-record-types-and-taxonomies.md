---
title: Översikt över posttyper
description: Posttyper är byggstenarna i en Adobe Workfront Planning-arbetsyta.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: 49335ec86057e4985477034558a271bf4efcab5e
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Översikt över posttyper

{{planning-important-intro}}

Till skillnad från Workfront där objekttyperna är fördefinierade kan du skapa egna objekttyper i Adobe Workfront Planning. I Workfront har till exempel objekttyperna Program, Portfolio, Projekt, Uppgift eller Utgåva redan skapats.

Workfront Planning-objekttyper kallas&quot;posttyper&quot; och du kan skapa och anpassa alla. Posttyper är byggstenarna i en Workfront Planning-arbetsyta. Mer information om arbetsytor finns i [Skapa arbetsytor](../architecture/create-workspaces.md).

## Översikt över posttyp

I Workfront Planning kan du skapa anpassade posttyper som passar din organisations behov.

* När du skapar en arbetsyta från en mall skapas posttyper i följande avsnitt på arbetsytan:

   * [Operativa posttyper](#operational-record-type): En posttyp som representerar strategiska planer, initiativ eller planerat arbete. Exempel: Campaign, Activity, Tactic, Opportunity kan vara operativa posttyper.
   * [Taxonomier](#taxonomy): Posttyper som samlar in attribut om en operativ posttyp. Region, Adress, Audience kan till exempel vara taxonomier.

* När du skapar en posttyp på en arbetsyta som du har skapat från grunden kan du placera posttypen i vilket avsnitt som helst som du skapar på arbetsytan.
* När du skapar en posttyp kan bara du och de du ger behörighet att komma åt arbetsytan visa posttypen.
* Du måste skapa en arbetsyta innan du kan skapa posttyper för arbetsytan.
* Du kan ha totalt 1 000 posttyper på en arbetsyta, oavsett hur många avsnitt arbetsytan har. Detta inkluderar posttyper som du skapar från grunden eller som skapas när du använder en mall.


<!--

### Operational Record Type{#operational-record-type}

An operational record type is a Maestro record type that represents work-related objects.  

(***********insert screen shot**************)
For more information about operational record types including how to create them, see [Create record types](../architecture/create-record-types.md). 

### Taxonomy{#taxonomy}

A taxonomy is a record type that captures attributes about an operational record type. 

(**********add screen shot**********)

For more information about taxonomy record types, see [Create a taxonomy](../architecture/create-a-taxonomy.md). 

Although creating taxonomies is identical to creating operational record types, Maestro distinguishes conceptually between an operational record type and a taxonomy record type. The purpose of taxonomies is to enhance operational record types. Taxonomies should not directly represent work objects.  (***********this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.***********) 

(********mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc*************)

For example, Audience, Region, or Address can be taxonomy-type record types.  

For more information, see [Create a taxonomy](../architecture/create-a-taxonomy.md). 

## Similarities and differences between operational record types and taxonomies

The following table illustrates some of the similarities and differences between operational record types and taxonomies: 

| Record type and characteristic                              | Operational Record Type | Taxonomy Record Type |
|-------------------------------------------------------------|:-----------------------:|:--------------------:|
| They are part of a workspace                                |            ✓            |           ✓          |
| You can create them automatically, from a workspace template                    |            ✓            |           ✓          |
| You can create them manually, from scratch                    |            ✓            |           ✓          |
| You can create them by copying and pasting information from an external file or list                   |            ✓            |           ✓          |
| You can create by importing an Excel or CSV file                    |            ✓            |                     |
| You can create read-only record types by connecting to object types from other applications                    |            ✓            |                     |
| They represent work-related objects                         |            ✓            |                      |
| They represent attributes about work-related objects        |                         |           ✓          |
| You can create from scratch                                 |            ✓            |           ✓          |
| You can create by importing an Excel or CSV file            |            ✓            |                      |
| You can connect the record type to an object from another application|            ✓            |                      |
| You can connect to other Maestro record types               |            ✓            |                    |
| You can view their associated records in a table view       |            ✓            |           ✓          |
| You can view their associated records in a timeline view    |            ✓            |           ✓          |

-->
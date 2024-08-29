---
title: Översikt över posttyper
description: Posttyper är byggstenarna i en Adobe Workfront Planning-arbetsyta.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: 425c3d3afb892ac83a10bbd36efb4c7d9712c4dc
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---


# Översikt över posttyper

{{planning-important-intro}}

Till skillnad från Workfront där objekttyperna är fördefinierade kan du skapa egna objekttyper i Adobe Workfront Planning. I Workfront har till exempel objekttyperna Program, Portfolio, Projekt, Uppgift eller Utgåva redan skapats.

Workfront Planning-objekttyper kallas&quot;posttyper&quot; och finns bara när användare skapar dem. Posttyper är byggstenarna i en Workfront Planning-arbetsyta. Mer information om arbetsytor finns i [Skapa arbetsytor](/help/quicksilver/planning/architecture/create-workspaces.md).

## Översikt över posttyp

I Workfront Planning kan du skapa anpassade posttyper som passar din organisations behov.

Mer information om hur du skapar posttyper finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

* När du skapar en arbetsyta från en mall skapas posttyper i följande avsnitt på arbetsytan:

   * **Driftsposttyper**: Posttyper som representerar strategiska planer, initiativ eller planerade arbeten. Exempel: Campaign, Activity, Tactic, Opportunity är operativa posttyper.
   * **Taxonomier**: Posttyper som samlar in attribut om en operativ posttyp. Till exempel är Region, Adress och Audience taxonomier.

* När du skapar en posttyp på en arbetsyta som du har skapat från grunden kan du placera posttypen i vilket avsnitt som helst som du skapar på arbetsytan.
* När du skapar en posttyp kan bara du och de du ger behörighet att komma åt arbetsytan visa posttypen.
* Du måste skapa en arbetsyta innan du kan skapa posttyper för arbetsytan.
* Information om begränsningar för hur många posttyper du kan ha på en arbetsyta eller i en Workfront-instans finns i [Översikt över begränsningar för Adobe Workfront Planning-objekt](/help/quicksilver/planning/general/limitations-overview.md).


<!--

### Operational Record Type{#operational-record-type}

An operational record type is a Wrorkfront Planning record type that represents work-related objects.  

(***********insert screen shot**************)
For more information about operational record types including how to create them, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md). 

### Taxonomy{#taxonomy}

A taxonomy is a record type that captures attributes about an operational record type. 

(**********add screen shot**********)

Although creating taxonomies is identical to creating operational record types, Workfront Planning distinguishes conceptually between an operational record type and a taxonomy record type. The purpose of taxonomies is to enhance operational record types. Taxonomies should not directly represent work objects.  (***********this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.***********) 

(********mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc*************)

For example, Audience, Region, or Address can be taxonomy-type record types.  

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
| You can connect to other record types               |            ✓            |                    |
| You can view their associated records in a table view       |            ✓            |           ✓          |
| You can view their associated records in a timeline view    |            ✓            |           ✓          |

-->
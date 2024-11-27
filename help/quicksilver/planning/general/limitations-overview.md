---
title: Översikt över begränsningar för Adobe Workfront Planning-objekt
description: Adobe Workfront Planning har gränser för hur många objekt du kan skapa i din instans. Objektbegränsningar finns för att förbättra produktprestanda och förbättra din upplevelse av Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 2a640cd5-f4a8-4ff3-81b6-32f85f6e4535
source-git-commit: d962d60294295dd1f3771d1f0b737c9d1f03dfef
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 1%

---

<!--check the workfront.com/plans article linked below to see if there is content in there about Planning - after August 28, 2024-->

# Översikt över begränsningar för Adobe Workfront Planning-objekt

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}


Adobe Workfront Planning har gränser för hur många objekt du kan skapa i din instans. Objektbegränsningar finns för att förbättra produktprestanda och förbättra din upplevelse av Workfront Planning.

I följande tabell visas gränserna för hur många objekt du kan skapa i Workfront Planning. Begränsningarna kan komma att ändras när vi går vidare till nästa utvecklingsfas.

| Adobe Workfront Planning-objekt | Gräns |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| Antal arbetsytor för en Workfront-instans | obegränsat* |
| Antal avsnitt för en arbetsyta | 50 |
| Antal posttyper för en arbetsyta | 1 000 (inkluderar posttyper från alla avsnitt och de som skapas när en arbetsytemall används) |
| Antal poster för en posttyp | 25 000 |
| Antal poster för en arbetsyta | 25 000 för kunder med Planning <br> 500 000 för kunder med Planning Plus |
| Antal poster för en instans av Workfront Planning | 500 000 för kunder med Planning-planen <br>2 miljoner för kunder med Planning Plus |
| Antal fält för en posttyp eller taxonomi | 500 |
| Antal tecken för ett textfält med en rad | 1 000 tecken |
| Antal tecken för ett styckefält | 10 000 tecken |
| Antal styckefält för en posttyp | 20 styckefält |
| Storlek på fil som du kan klistra in i en posttypstabell | 1 MB |
| Storlek på fil som du kan importera via API för en posttypstabell | 1,5 MB |
| Frekvensen med vilken API-begäranden kan göras | 200 begäranden per minut |
| Antal vyer som en användare kan skapa för en posttyp | 100 |
| Storlek på Excel-fil som du kan importera för att skapa posttyper | 5 MB |
| <span class="preview">Antal rader som du kan importera i en CSV- eller Excel-fil för att skapa posttyper</span> | 10 000 |
| <span class="preview">Antal kolumner som du kan importera i en CSV- eller Excel-fil för att skapa posttyper</span> | 500 |

*Vi rekommenderar att du inte har för många arbetsytor eftersom de kan bli svåra att hantera och arbetsflödena kan vara för fragmenterade.

Information om priser och paketering för Workfront Planning finns i [Adobe Workfront priser och paketering](https://business.adobe.com/products/workfront/pricing.html).

<!--
****************KEEP THIS COMMENTED OUT:

**This functionality has been temporarily removed and it will be available at a later date.**********************
-->


<!--OLD limitations (before GA:)

|       Adobe Workfront Planning  object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   1,000                                                                                                         |
|     Number of sections for one workspace                                      |   50                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes record types from all sections and those that are created when using a workspace template)  |
|     Number of records for one record type                                               |   50,000                                                                                                        |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a text field                                                               |   1,000 characters                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     The rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Number of views one user can create for one record type | 100 |

-->
<!--| Size of CSV of Excel file you can import* | 5MB |-->

<!--[!IMPORTANT]
>
>*This functionality has been temporarily removed and it will be available at a later date.-->

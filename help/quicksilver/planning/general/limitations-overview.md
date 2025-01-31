---
title: Översikt över begränsningar för Adobe Workfront Planning-objekt
description: Adobe Workfront Planning har gränser för hur många objekt du kan skapa i din instans. Objektbegränsningar finns för att förbättra produktprestanda och förbättra din upplevelse av Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 2a640cd5-f4a8-4ff3-81b6-32f85f6e4535
source-git-commit: 7c1bd52c6d1878b556bc92849b5d65fd0e89f51b
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 1%

---


# Översikt över begränsningar för Adobe Workfront Planning-objekt

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

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
| Antal rader som du kan importera i en CSV- eller Excel-fil för att skapa posttyper | 10 000 |
| Antal kolumner som du kan importera i en CSV- eller Excel-fil för att skapa posttyper | 500 |

*Vi rekommenderar att du inte har för många arbetsytor eftersom de kan bli svåra att hantera och arbetsflödena kan vara för fragmenterade.

Kontakta din kontoansvarige om du vill ha information om priser och paketering för Workfront Planning.

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

---
title: Översikt över begränsningar för Adobe Workfront Planning-objekt
description: Adobe Workfront Planning har gränser för hur många objekt du kan skapa i din instans. Objektbegränsningar finns för att förbättra produktprestanda och förbättra din upplevelse av Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: f252140e4fec01c7bb8092804532d79954cef618
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Översikt över begränsningar för Adobe Workfront Planning-objekt

Adobe Workfront Planning har gränser för hur många objekt du kan skapa i din instans. Objektbegränsningar finns för att förbättra produktprestanda och förbättra din upplevelse av Workfront Planning.

I följande tabell visas gränserna för hur många objekt du kan skapa i Workfront Planning. Begränsningarna kan komma att ändras när vi går vidare till nästa utvecklingsfas.

| Adobe Workfront Planning-objekt | Gräns |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| Antal arbetsytor för en Workfront-instans | 1 000 |
| Antal avsnitt för en arbetsyta | 50 |
| Antal posttyper för en arbetsyta | 1 000 (inkluderar posttyper från alla avsnitt och de som skapas när en arbetsytemall används) |
| Antal poster för en posttyp | 50 000 |
| Antal fält för en posttyp eller taxonomi | 500 |
| Antal tecken för ett textfält | 1 000 tecken |
| Storlek på fil som du kan klistra in i en posttypstabell | 1 MB |
| Storlek på fil som du kan importera via API för en posttypstabell | 1,5 MB |
| Frekvensen med vilken API-begäranden kan göras | 200 begäranden per minut |
| Storlek på Excel-fil som du kan importera* | 5 MB |
| Antal vyer som en användare kan skapa för en posttyp | 100 |

<!--add to the table above: Maximum number of views created by one use 100 -->

>[!IMPORTANT]
>
>*Den här funktionen har inaktiverats tillfälligt och kommer att finnas tillgänglig vid ett senare tillfälle.

<!--At GA, replace the table above with this:

|       Adobe Workfront Planning  object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   unlimited*                                                                                                        |
|     Number of sections for one workspace                                      |   50                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes record types from all sections and those that are created when using a workspace template)  |
|     Number of records for one record type                                               |   25,000                                                                                                        |
|     Number of records for one workspace                                               |   25,000 for customers with the Planning plan <br> 500,000 for customers with the Planning Plus  plan                                                                                                         |
|     Number of total records for one instance of Workfront Planning type                                               |   500,000 for customers with the Planning plan <br>2 million for customers with the Planning Plus plan                                                                                                        |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a text field                                                               |   1,000 characters                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     The rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Size of CSV of Excel file you can import** | 5MB |
| Number of views one user can create for one record type | 100 |

*We recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.
**This functionality has been temporarily disabled and it will be available at a later date.
-->
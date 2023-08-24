---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Flytta objekt från en miljö till en annan
description: Funktionen för miljömarknadsföring är avsedd att göra det möjligt att flytta konfigurationsrelaterade objekt från en miljö till en annan. Det stöder inte möjligheten att flytta transaktionsobjekt (med begränsade undantag).
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
source-git-commit: 5d3c8e3626dabf88394bd6b3c2dd48e6168b56c4
workflow-type: tm+mt
source-wordcount: '2317'
ht-degree: 0%

---

# Flytta objekt från ett objekt [!DNL Workfront] miljö till annan

<!-- 
TO DO

Overview of value
Check for any code changes
Fix {}
Add to tocs
-->

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] plan</td> 
   <td> <p>Enterprise, Prime eller Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] licens</p> </td> 
   <td> <p>[!UICONTROL Plan] </p> <p>Du måste vara en [!DNL Workfront] administratör. För information om [!DNL Workfront] administratörer, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Objektbehörigheter</p> </td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Supportpaket</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL Preferred], eller [!UICONTROL Enterprise]</p> <p>Standardsupportpaketet har inte tillgång till den anpassade uppdateringssandlådan, men det har tillgång till förhandsvisningens sandlåda.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Förutsättningar

Slutpunkten Skapa kampanjpaket förutsätter att du redan har konfigurerat källmiljön. Detta API-anrop kräver att du skapar en objektmappning av [!DNL Workfront] objCodes och objekt-GUID. Kartans specifika struktur beskrivs nedan.

## Objekt som stöds för miljöbefordran

Funktionen för miljömarknadsföring är avsedd att göra det möjligt att flytta konfigurationsrelaterade objekt från en miljö till en annan. Det stöder inte möjligheten att flytta transaktionsobjekt (med begränsade undantag).

* [Arbetsobjekt](#work-objects)
* [Rapporteringsobjekt](#reporting-objects)
* [Anpassade dataobjekt](#custom-data-objects)
* [Organisationsobjekt](#organization-objects)
* [Andra konfigurationsobjekt](#other-configuration-objects)


### Arbetsobjekt

| Upphöjt objekt | Inkluderade flyttbara underobjekt |
| --- | --- |
| Projekt (PROJ) | Projekt<br>Uppgift<br>Tilldelning<br>Föregående<br>Företag<br>Åsidosätt hastighet<br>Grupp<br>Roll<br>Team<br>Godkännandeprocess<br>Godkännandesökväg<br>Godkännandesteg<br>Steggodkännare<br>Schema<br>Ledig arbetsdag<br>Ködefinition<br>Köämnesgrupp<br>Köämne<br>Cirkulationsregel<br>Sökväg för milstolpe<br>Milstolpe<br>Timtyp<br>Resurspool<br>Kategori<br>Kategoriparameter<br>Parameter<br>Parametergrupp<br>Parameteralternativ<br>Kategorivisningslogik |
| Mall (TMPL) | Mall<br>Malluppgift<br>Mallaktivitetstilldelning<br>Föregångare för mallaktivitet<br>Företag<br>Åsidosätt hastighet<br>Grupp<br>Roll<br>Team<br>Godkännandeprocess<br>Godkännandesökväg<br>Godkännandesteg<br>Steggodkännare<br>Schema<br>Ledig arbetsdag<br>Ködefinition<br>Köämnesgrupp<br>Köämne<br>Cirkulationsregel<br>Sökväg för milstolpe<br>Milstolpe<br>Timtyp<br>Resurspool<br>Kategori<br>Kategoriparameter<br>Parameter<br>Parametergrupp<br>Parameteralternativ<br>Kategorivisningslogik |

### Rapporteringsobjekt

| Upphöjt objekt | Inkluderade flyttbara underobjekt |
| --- | --- |
| Layoutmall (UITMPL) | Layoutmall<br>Kontrollpanel<br>Kalender<br>Kalenderavsnitt<br>Extern sida<br>Rapport<br>Filter<br>Gruppering<br>Visa<br>Parameter |
| Kontrollpanel (PTLTAB) | Kontrollpanel<br>Kalender<br>Kalenderavsnitt<br>Extern sida<br>Rapport<br>Filter<br>Gruppering<br>Visa<br>Parameter |
| Kalender (KALEND) | Kalender<br>Kalenderavsnitt |
| Extern sida (EXTSEC) | Extern sida |
| Rapport (PTLSEC) | Rapport<br>Filter<br>Gruppering<br>Visa<br>Parameter |
| Filter (UIFT) | Filter<br>Parameter |
| Gruppering (UIGB) | Gruppering<br>Parameter |
| Visa (UIVW) | Visa<br>Parameter |

### Anpassade dataobjekt

| Upphöjt objekt | Inkluderade flyttbara underobjekt |
| --- | --- |
| Kategori (CTGY) | Kategori<br>Kategoriparameter<br>Parameter<br>Parametergrupp<br>Parameteralternativ<br>Kategorivisningslogik<br>Grupp |
| Parameter (PARAM) | Parameter<br>Parameteralternativ |
| Parametergrupp (PGRP) | Parametergrupp |

### Organisationsobjekt

| Upphöjt objekt | Inkluderade flyttbara underobjekt |
| --- | --- |
| Grupp (GRUPP) | Grupp <br>Undergrupper (upp till 5 nivåer)<br>Kategori<br>Kategoriparameter<br>Parameter<br>Parametergrupp<br>Parameteralternativ<br>Kategorivisningslogik |
| Roll (ROLE) | Roll |
| Team (TEAM) | Team<br>Grupp |
| Företag (CMPY) | Företag<br>Åsidosätt hastighet<br>Kategori<br>Kategoriparameter<br>Parameter<br>Parametergrupp<br>Parameter <br>Kategorivisningslogik<br>Grupp |
| Portfolio (PORT) | Portfolio<br>Program<br>Grupp<br>Kategori<br>Kategoriparameter<br>Parameter<br>Parametergrupp<br>Parameteralternativ<br>Kategorivisningslogik |
| Program (PRGM) | Program<br>Portfolio<br>Grupp<br>Kategori<br>Kategoriparameter<br>Parameter<br>Parametergrupp<br>Parameteralternativ<br>Kategorivisningslogik |

### Andra konfigurationsobjekt

| Upphöjt objekt | Inkluderade flyttbara underobjekt |
| --- | --- |
| Godkännandeprocess (ARVPRC) | Godkännandeprocess<br>Godkännandesökväg<br>Godkännandesteg<br>Steggodkännare<br>Roll<br>Team<br>Grupp |
| Schema (SCHED) | Schema<br>Ledig arbetsdag<br>Grupp |
| Sökväg för milstolpe (MPATH) | Sökväg för milstolpe<br>Milstolpe |
| Tidrapportprofil (TSPRO) | Tidrapportprofil<br>Timtyp |
| Timtyp (HOURT) | Timtyp |
| Utgiftstyp (EXPTYP) | Utgiftstyp |
| Risktyp (risktyp) | Risktyp |
| Resurspool (RSPL) | Resurspool |

## Autentisering

API:t autentiserar varje begäran för att säkerställa att klienten har åtkomst att visa eller ändra ett begärt objekt.

Autentisering utförs genom att ett sessions-ID eller en API-nyckel skickas, som kan ges på något av följande sätt:

### Autentisering av begärandehuvud

Den autentiseringsmetod som rekommenderas är att skicka ett begärandehuvud med namnet SessionID som innehåller sessionstoken. Fördelen med att vara säker mot [CSRF (Cross-site Request Forgery)](http://en.wikipedia.org/wiki/Cross-site_request_forgery) och inte störa URI:n för cachelagring.

Följande är ett exempel på en begäranderubrik:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

## API-slutpunkter

* [Skapa ett paket](#create-a-package)
* [Hämta en lista med paket](#get-a-list-of-packages)
* [Hämta ett paket med ID](#get-a-package-by-id)
* [Hämta ett pakets konfigurationsdefinition](#get-a-packages-configuration-definition)
* [Ersätt paketinformation och definition](#replace-package-details-and-definition)
* [Uppdatera specifika egenskaper för ett paket](#update-specific-properties-of-a-package)
* [Ta bort ett paket](#delete-a-package)
* [Utför en förkörning](#execute-a-pre-run)
* [Kör en installation](#execute-an-installation)
* [Hämta en lista över installationer för ett specifikt paket](#get-a-list-of-installations-for-a-specific-package)
* [Hämta installationsinformation för en installation](#get-the-installation-details-for-an-installation)

### Skapa ett paket

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

Det här anropet kör en flerstegsprocess.

I det första steget skapas ett tomt kampanjpaket med statusen&quot;ASSEMBLING&quot;.

I det andra steget används `objectCollections` arrayen finns i POSTENS brödtext för att sammanställa de begärda posterna från Workfront. Det här steget kan ta flera minuter, beroende på hur många poster som har begärts och din Workfront-konfiguration. I slutet av processen uppdateras det tomma erbjudandepaketet med `packageEntities` och statusen anges automatiskt till &quot;UTKAST&quot;.


>[!NOTE]
>
>Notera strukturen för `objectCollections`  array.
>
>Varje objekt i arrayen innehåller en `objCode` som motsvarar objektkoden som finns dokumenterad i Workfront API Explorer.
>
>Varje objekt innehåller också `entities` samling. Detta förväntar sig `ID` och `name` nycklar som ska finnas.
>
>För listan över tillåtna objektkoder som ska begäras i `objectCollections` finns i [Objekt som stöds för miljöbefordran](#supported-objects-for-environment-promotion) i den här artikeln.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### Sidhuvuden

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Brödtext

```json
{
    "packageName": "Agency Onboarding - 2023-06-06",
    "description": "This promotion package contains configuration to support the agency onboarding processes...",
    "source": "https://{domain}.{environment}.workfront.com",
    "objectCollections": [
        {
            "objCode": "PROJ",
            "entities": [
                {
                    "ID": "6419b8b9001151ee258921a4f7597ba1",
                    "name": "Agency Request"
                }
            ]
        },
        {
            "objCode": "TMPL",
            "entities": [
                {
                    "ID": "6419b8b9001151ee258921a4f7597bb2",
                    "name": "New Agency Onboarding"
                },
                {
                    "ID": "6419b8b9001151ee258921a4f7597bc3",
                    "name": "New Agency Offboarding"
                }
            ]
        },
        {
            "objCode": "PTLTAB",
            "entities": [
                {
                    "ID": "645e6435000b4aaebe4776f4a42ed5ad",
                    "name": "Agency Performance and Readiness"
                }
            ]
        }
    ]
}
```

#### Svar

```json
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "ASSEMBLING",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d"
}
```

### Hämta en lista med paket

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages</code></td> 
  </tr> 
  </tbody> 
</table>

Det här samtalet returnerar en ofiltrerad lista över kampanjpaket som tillhör kunden.

Svaret inkluderar alla paket som skapats från någon av kundens sandlåda, förhandsgranskning eller produktionsinstanser av Workfront.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### Sidhuvuden

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
}
```

#### Brödtext

_Tom_

#### Svar

```
200
```

```json
{
    "data": [
        {
            "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
            "name": "Agency Onboarding - 2023-06-06",
            "description": "This promotion package contains configuration to support the agency onboarding processes...",
            "status": "ASSEMBLING",
            "version": 1,
            "installationCounts": {},
            "createdAt": "2023-06-06T17:29:21.600Z",
            "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
            "publishedAt": null,
            "customerId": "61aa9d090005fa42152c1cb66659f38d"
        },
        {...}
    ]
}
```

### Hämta ett paket med ID

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Detta samtal returnerar information om ett begärt kampanjpaket.

Begäran kan göras i vilken miljö som helst, oavsett kampanjpaketets ursprungliga källa.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### Sidhuvuden

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
}
```

#### Brödtext

_Tom_

#### Svar

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "DRAFT",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "displayEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "null"
                   - or -
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### Hämta ett pakets konfigurationsdefinition

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages/{id}/definition</code></td> 
  </tr> 
  </tbody> 
</table>

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/definition
```

#### Sidhuvuden

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
}
```

#### Brödtext

_Tom_

#### Svar

```
200
```

```json
{
    "packageEntities": {
        "GROUP": [
           {
               "id": "52aa9d0e0005fcee8f212835bdaa2691",
               "name": "Default Group",
               "businessLeaderID": "...",
               "categoryID": "...",
               "defaultInterface": 1,
               "description": "...",
               "extRefID": null,
               "isActive": true,
               "isGroupPublic": true,
               "isPublic": true,
               "parentID": null,
               "rootID": null,
               "rootName": null,
               "uiTemplateID": null
           }
        ],
        "ROLE": [
           {...}
        ],
        ...
    }
}
```

### Ersätt paketinformation och definition

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>PUT /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Det här samtalet ersätter allt innehåll i erbjudandepaketet.

Alla redigerbara fält måste anges för begäran.

De redigerbara attributen är:

1. name (sträng)
1. description (string)
1. källa (sträng med URL-validering)
1. status (sträng med värdevalidering)
1. version (heltal)
1. packageEntities (collection)

Statusalternativen är:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>SAMMANSÄTTNING</td> 
   <td><p>Den här statusen tilldelas automatiskt medan objekt monteras.</p><p>Den här statusen kan inte anges direkt av en kund.</p></td> 
  </tr> 
  <tr> 
   <td>UTKAST</td> 
   <td><p>Denna status tilldelas när en sammansättningsprocess avslutas eller när ett tomt kampanjpaket skapas.</p><p>Det är möjligt för en kund att flytta kampanjpaketet tillbaka till den här statusen.</p><p>I den här statusen kan erbjudandepaketet inte installeras i någon miljö.</p></td> 
  </tr> 
  <tr> 
   <td>TESTNING</td> 
   <td><p>Den här statusen tillåter att ett kampanjpaket installeras i alla sandlådor av typerna Förhandsgranska eller Anpassad uppdatering. I den här statusen kan paketet inte installeras i Production.</p></td> 
  </tr> 
  <tr> 
   <td>AKTIV</td> 
   <td><p>Denna status tillåter att ett kampanjpaket installeras i alla miljöer, inklusive Production.</p><p>När en paketstatus är inställd på AKTIV <code>publishedAt</code> datumet anges automatiskt till den aktuella tidsstämpeln för begäran.</p></td> 
  </tr> 
  <tr> 
   <td>INAKTIVERAT</td> 
   <td><p>Den här statusen används för att dölja tidigare använda erbjudandepaket som inte kommer att installeras i någon miljö i framtiden.</p><p>När ett paket har den här statusen kan det inte installeras i någon miljö.</p><p>När paketstatusen är INAKTIVERAD visas <code>retiredAt</code> datumet anges automatiskt till den aktuella tidsstämpeln för begäran.</p><p>Vi rekommenderar att du använder den här statusen framför<code>DELETE /package</code> slutpunkten eftersom den kan hämtas och installationshistoriken sparas för alla distributioner som görs med det här paketet.</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING_FAILED</td> 
   <td><p>Kampanjpaketet får automatiskt denna status om ASSEMBLING-fasen misslyckas.</p><p>Om du vill returnera paketet till ASSEMBLING-steget måste du starta extraheringsprocessen igen.</p></td> 
  </tr> 
  </tbody> 
</table>

#### URL

```
PUT https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### Sidhuvuden

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Brödtext

```json
{
    "packageName": "Agency Onboarding - 2023-06-06",
    "description": "This promotion package contains configuration to support the agency onboarding processes... with a description change",
    "source": "https://{domain}.{environment}.workfront.com",
    "status": "TESTING",
    "version": 1,
    "metadata": {
        "displayOrder": ["GROUP","ROLE","TMPL","PROJ","PTLTAB"],
        "historyOrder": ["GROUP","ROLE","TMPL","TTSK","PROJ","PTLTAB"], 
        "installOrder": ["GROUP","ROLE","TMPL","TTSK","TPRED","TASSGN","PROJ","QUED","RRUL","QUET","UIFT","UIGB","UIVW","PTLTAB"], 
        "summaryOrder": ["GROUP","ROLE","TMPL"], 
        "shapeVersion": 2
    },
    "packageEntities": {
        "GROUP": [
           {
               "id": "52aa9d0e0005fcee8f212835bdaa2691",
               "name": "Default Group",
               "businessLeaderID": "...",
               "categoryID": "...",
               "defaultInterface": 1,
               "description": "...",
               "extRefID": null,
               "isActive": true,
               "isGroupPublic": true,
               "isPublic": true,
               "parentID": null,
               "rootID": null,
               "rootName": null,
               "uiTemplateID": null
           }
        ],
        "ROLE": [
           {...}
        ],
        ...
    }
}
```

#### Svar

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "TESTING",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "displayEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### Uppdatera specifika egenskaper för ett paket

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>PATCH /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Det här samtalet uppdaterar allt innehåll i erbjudandepaketet som finns i PATCH.

De redigerbara attributen är:

1. name (sträng)
1. description (string)
1. källa (sträng med URL-validering)
1. status (sträng med värdevalidering)
1. version (heltal)
1. packageEntities (collection)

   eller

   objectCollections (array)

Tillhandahåller `packageEntities` uppdaterar erbjudandepaketet med den angivna konfigurationsdefinitionen.

Tillhandahåller `objectCollections` kommer att initiera en återextrahering från `source` miljö som är associerad med erbjudandepaketet. The `source` fältet måste anges när `objectCollections` anges.

#### URL

```
PATCH https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```


#### Sidhuvuden

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Brödtext

```json
{
    "status": "ACTIVE"
}
```

#### Svar

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "ACTIVE",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": "2023-06-06T19:39:01.600Z",
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "displayEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### Ta bort ett paket

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>DELETE /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Det här anropet tar bort kampanjposten. Den här åtgärden är oåterkallelig.

>[!NOTE]
>
>I stället för att ta bort ett kampanjpaket rekommenderar vi att du ändrar paketets status till INAKTIVERAT. Detta gör att paketet kan hämtas och att installationshistoriken för var det distribuerades sparas.

#### URL

```
DELETE https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### Sidhuvuden

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
}
```

#### Brödtext

_Tom_

#### Svar

```
200
```

```
Deleted
```

### Utför en förkörning

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST  {customer-domain}/environment-promotion/api/v1/packages/{id}/prepare-installation</code></td> 
  </tr> 
  </tbody> 
</table>

Det här anropet utför en jämförelse mellan paketdefinitionen och målmiljön som identifieras i URL:en.

Resultatet är ett JSON-organ som identifierar om ett erbjudande-objekt hittas eller inte i målmiljön.

För varje erbjudande, något av följande `actions`  ställs in:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>SKAPA</td> 
   <td><p>När en motsvarande post inte kan hittas i målmiljön, ställs åtgärden in på CREATE.</p><p>När den här åtgärden anges i <code>translationmap</code> som tillhandahålls <code>/install</code> slutpunkten skapas posten av installationstjänsten.</p></td> 
  </tr> 
  <tr> 
   <td>ANVÄNDNING</td> 
   <td><p>När en motsvarande post hittas i målmiljön ställs åtgärden in på USEEXISTING och en <code>targetId</code> hämtas också i <code>translationmap</code>.</p><p>När den här åtgärden anges i <code>translationmap</code> som tillhandahålls <code>/install</code> slutpunkten kommer installationstjänsten inte att skapa posten. Det använder dock <code>targetId</code> som ingår i mappningsposten för andra objekt som kan ha en referens till den här posten.</p><p>En standardgrupp kan till exempel hittas i målmiljön som ett paket distribueras till. Det går inte att ha två standardgruppposter, så installationstjänsten använder GUID för den befintliga gruppen i andra objektskapande åtgärder som innehåller en referens till standardgruppen, till exempel ett projekt, ett formulär eller någon annan enhet som är relaterad till den här gruppen.</p><p><b>Obs!</b> <ul><li><p>När åtgärden USEEXISTING tilldelas ändras inte den befintliga posten i målmiljön. </p><p>Om beskrivningen för standardgruppen till exempel har ändrats i sandlådan där paketet skapades och beskrivningsvärdet är ett annat i målmiljön, ändras inte värdet efter en installation med det här <code>translationmap</code>.</li></ul></td> 
  </tr> 
  <tr> 
   <td>IGNORE</td> 
   <td><p>Den här åtgärden ställs inte in automatiskt.</p><p>Den ger möjlighet att manuellt åsidosätta en tilldelad CREATE- eller USEEXISTING-åtgärd innan den körs <code>/install</code> ring.</p><p><b>Anteckningar: </b><ul><li><p>Om en post som ursprungligen var inställd på CREATE är inställd på IGNORE, bör alla underordnade poster också vara inställda på IGNORE.</p><p>Om en mallpost till exempel har mappats med en CREATE-åtgärd och användaren vill utesluta den från distributionen, kan de ange att mallens åtgärd ska vara IGNORE.</p><p>Om den installerande användaren inte anger IGNORE för malluppgifter, malluppgiftstilldelningar, föregående malluppgifter, ködefinition, köämnen, routningsregler osv. resulterar distributionen i ett misslyckat installationsförsök.</p></li><li><p>Om en post som ursprungligen var inställd på USEEXISTING är inställd på IGNORE kan det uppstå vissa negativa effekter under installationen.</p><p>Om en grupppost till exempel har mappats med åtgärden USEEXISTING och användaren som installerar ändrar åtgärden till IGNORE, för objekt som kräver en grupp (t.ex. ett projekt kan inte finnas utan en grupp tilldelad), tilldelas systemstandardgruppen till det projektet.</p></li><li><p>Om en post som ursprungligen var inställd på USEEXISTING är inställd på CREATE kan det uppstå vissa negativa effekter under installationsprocessen eftersom många Workfront-enheter har unika namnbegränsningar.</p><p>Om till exempel en post av typen "Standardgrupp" mappades med åtgärden USEEXISTING, och den installerande användaren ändrar åtgärden till CREATE eftersom det redan finns en "Standardgrupp", kommer installationsförsöket inte att kunna slutföra alla steg. Gruppnamn måste vara unika.</p><p>Vissa entiteter har ingen unik namnbegränsning. Om du gör den här ändringen för dessa objekt får du två poster med samma namn. Mallar, projekt, vyer, filter, grupperingar, rapporter och kontrollpaneler kräver till exempel inga unika namnbegränsningar. Det är bäst att ha unika namn för de här posterna, men de används inte.</p></li></ul></p></td> 
  </tr> 
  </tbody> 
</table>

Det finns för närvarande inget stöd för UPDATE `action` i den här tjänstens alfafunktioner. Alternativet att tillåta en UPPDATERING `action` är något vi undersöker.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/translationmap
```

#### Sidhuvuden

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Brödtext

```json
{}
```

#### Svar

```
200
```

```json
{}
```

### Kör en installation

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /install</code></td> 
  </tr> 
  </tbody> 
</table>

Det här anropet initierar ett installationsförsök för ett kampanjpaket till målmiljön som identifieras i POSTENS URL.

#### Alternativ

Om en `translationmap` finns inte med i POSTENS brödtext, startar processen automatiskt `/translationmap` ring. The `translationmap` som returneras kommer att användas som det är, utan möjlighet att granska eller justera den.

Om en `translationmap` finns i POSTENS brödtext, kommer mappningen att användas i installationsprocessen. Detta ger en installerande användare möjlighet att granska och göra nödvändiga justeringar innan installationsförsöket utförs.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/install
```

#### Sidhuvuden

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Brödtext

```json
{
}
```

#### Svar

```
200
```


```json
{}
```

### Hämta en lista över installationer för ett specifikt paket

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
</code></td> 
  </tr> 
  </tbody> 
</table>

Resultatet är installationshändelser från alla miljöer som paketet har distribuerats till. De är inte begränsade till de anläggningar för miljön genom vilka begäran görs. På så sätt kan du identifiera vilka miljöer som har tagit emot det här paketet.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
```

#### Sidhuvuden

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
}
```

#### Brödtext

_Tom_

#### Svar

```
200
```

```json
[
    {
        "id": "2892b936-e09e-455a-935f-e1462ab9753c",
        "environmentPromotionPackageId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
        "environmentPromotionPackageVersion": 1,
        "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
        "customerId": "54286d78b064451096752b99bf968481",
        "status": "COMPLETED",
        "environment": "https://{domain}.{environment}.workfront.com",
        "registeredAt": "2021-03-16T02:21:31.908Z",
        "updatedAt": null,
        "translationMap": {
            "ROLE": {
                "5f6d114f006883209828ddd9088e63b3": {
                    "name": "DAM Curator",
                    "action": "USEEXISTING",
                    "isValid": true,
                    "targetId": "600f4bed00028a718599f29575840053"
                },
                "ad535a9ebe647361e053a7656a0a1575": {
                    "name": "Copywriter",
                    "action": "USEEXISTING",
                    "isValid": true,
                    "targetId": "600f162700001ca051081c06667b14a4"
                },
                ...
            },
            "TMPL": {
                "5f9b317c00b3db5af69abcd1ed5f82aa": {
                    "name": "Digital Asset Production (Integrated)",
                    "action": "CREATE",
                    "isValid": true,
                    "targetId": "6054cda40000d5af63dc811d9c2b3a07"
                },
                ...
            },
            ...
        }
    },
    {...}
]
```

### Hämta installationsinformation för en installation

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /installations/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Det här samtalet returnerar det sista `translationMap` som har producerats av installationstjänsten för en specifik installation.

Varje post anger vad som föreskrivs `action` och om åtgärden lyckades eller inte.

För poster med en CREATE `action` den `targetId` fältet ställs in med värdet för den nyligen skapade posten i målsystemet. Dessutom kan du `installationStatus` fältet ställs in på INSTALLED.

För poster med USEEXISTING `action` den `targetId` -fältet ställs också in och `installationStatus` kommer att ställas in på REGISTRERAD. Detta innebär att mappningsprocessen var slutförd och att installationstjänsten bekräftar att den har utvärderat posten och att det inte finns något att agera på.

Om posten har en CREATE `action` men posten inte kan skapas, `installationStatus` ställs in på FAILED och orsaken till felet anges också.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}
```

#### Sidhuvuden

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
}
```

#### Brödtext

_Tom_

#### Svar

```
200
```

```json
{
    "id": "2892b936-e09e-455a-935f-e1462ab9753c",
    "environmentPromotionPackageId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
    "environmentPromotionPackageVersion": 1,
    "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
    "customerId": "54286d78b064451096752b99bf968481",
    "status": "COMPLETED",
    "environment": "https://{domain}.{environment}.workfront.com",
    "registeredAt": "2021-03-16T02:21:31.908Z",
    "updatedAt": null,
    "translationMap": {
        "ROLE": {
            "5f6d114f006883209828ddd9088e63b3": {
                "name": "DAM Curator",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "600f4bed00028a718599f29575840053"
            },
            ...
        },
        "TMPL": {
            "5f9b317c00b3db5af69abcd1ed5f82aa": {
                "name": "Digital Asset Production (Integrated)",
                "action": "CREATE",
                "isValid": true,
                "targetId": "6054cda40000d5af63dc811d9c2b3a07"
            },
            ...
        },
        ...
    }
}
```



<!--table templates

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

<table style="table-layout:fixed"> 
 <col> 
 <tbody> 
  <tr> 
   <td><b></b></td> 
  </tr> 
  <tr> 
   <td><pre></pre></td> 
  </tr> 
  </tbody> 
</table>
-->
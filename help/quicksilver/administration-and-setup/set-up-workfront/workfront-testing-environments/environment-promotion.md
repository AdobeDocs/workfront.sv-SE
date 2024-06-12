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
recommendations: noDisplay, noCatalog
exl-id: dd3c29df-4583-463a-b27a-bbfc4dda8184
source-git-commit: d249751b78e9d40fe7a351db14cbf0f3b7c79889
workflow-type: tm+mt
source-wordcount: '2103'
ht-degree: 0%

---

# Flytta objekt mellan [!DNL Workfront] miljöer som använder [!DNL Workfront] API för miljöerbjudande

Med funktionen för miljöfrämjande åtgärder kan du flytta konfigurationsrelaterade objekt från en miljö till en annan. Du kan flytta dessa objekt med Workfront API enligt beskrivningen i den här artikeln.

Instruktioner om hur du flyttar objekt mellan miljöer med Workfront finns i:

* [Skapa eller redigera ett miljöerbjudande](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
* [Installera ett miljöerbjudande](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)


## Åtkomstkrav

Du måste ha följande:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan</strong>
   </td>
   <td> Organisationen måste följa den nya prismodellen och ha en Prime- eller Ultimate-plan.
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenser</strong>
   </td>
   <td> [!UICONTROL Standard]
   </td>
  </tr>
   <tr>
   <td>Konfigurationer på åtkomstnivå
   </td>
   <td>Du måste vara en [!DNL Workfront] administratör.
   </td>
  </tr>
</table>

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Förutsättningar

Slutpunkten Skapa kampanjpaket förutsätter att du redan har konfigurerat källmiljön. Detta API-anrop kräver att du skapar en objektmappning av [!DNL Workfront] objCodes och objekt-GUID. Kartans specifika struktur beskrivs nedan.

## Objekt som stöds för miljöbefordran

Funktionen för miljömarknadsföring är avsedd att göra det möjligt att flytta konfigurationsrelaterade objekt från en miljö till en annan. Det stöder inte möjligheten att flytta transaktionsobjekt (med begränsade undantag).

En lista över befordrbara objekt och deras tillhörande befordrbara underobjekt finns i [Objekt som stöds för miljöbefordran](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion) i artikeln [Översikt över rörliga objekt mellan Workfront-miljöer](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).

## Autentisering

API:t autentiserar varje begäran för att säkerställa att klienten har åtkomst att visa eller ändra ett begärt objekt.

Autentisering utförs genom att ett sessions-ID eller en API-nyckel skickas, som kan ges med följande metod:

### Autentisering av begärandehuvud

Den autentiseringsmetod som rekommenderas är att skicka ett begärandehuvud med namnet SessionID som innehåller sessionstoken. Fördelen med att vara säker mot [CSRF (Cross-site Request Forgery)](https://en.wikipedia.org/wiki/Cross-site_request_forgery) och inte störa URI:n för cachelagring.

Följande är ett exempel på en begäranderubrik:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

## API-slutpunkter

* [Skapa ett paket](#create-a-package)
* [Hämta en lista med paket](#get-a-list-of-packages)
* [Hämta ett paket med ID](#get-a-package-by-id)
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
>Varje objekt innehåller också `entities` samling. Detta förväntar sig `ID` fält. Den kan också acceptera ett valfritt `name` för att göra det enklare att veta vad `ID` representerar.
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
    "Content-Type": "application/json"
}
```

eller

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Brödtext

```json
{
    "name": "Agency Onboarding - 2023-06-06",
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
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "ASSEMBLING",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d"
    }
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
    "apikey": "**********"
}
```

eller

```json
{
    "sessionID": "*****************"
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
            "createdAt": "2023-06-06T17:29:21.600Z",
            "deletedAt": null
},
        {...}
    ]
}
```

&lt;!—Check on &quot;status&quot; above—was added?—>

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
    "apikey": "**********"
}
```

eller

```json
{
    "sessionID": "*****************"
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
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "DRAFT",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "packageEntities": {
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
1. status (sträng med värdevalidering)

En detaljerad beskrivning av tillgängliga statusar finns på [Status för miljöbefordran](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) i artikeln [Översikt över rörliga objekt mellan Workfront-miljöer](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).


#### URL

```
PATCH https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```


#### Sidhuvuden

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

eller

```json
{
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
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "ACTIVE",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "publishedAt": "2023-06-06T19:39:01.600Z",
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "packageEntities": {
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
    "apikey": "**********"
}
```

eller

```json
{
    "sessionID": "*****************"
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

>[!IMPORTANT]
>
>Innan du kan köra en installation måste du köra den här förkörningen. Du kommer att använda det ID som genereras från det här anropet när du kör installationen.

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
   <td>ÖVERSKRIVNING</td> 
   <td><p>Den här åtgärden ställs inte in automatiskt.</p><p>Den här åtgärden ger möjlighet att uppdatera ett objekt som finns i målmiljön. Den ger möjlighet att manuellt åsidosätta en tilldelad CREATE- eller USEEXISTING-åtgärd innan den körs <code>/install</code> ring.<ul><li>En användare kan uppdatera ett objekt i testmiljön och sedan använda åtgärden VERWRITING för att uppdatera objektet i målmiljön.</p></li><li><p>Om användaren installerar ett erbjudandepaket från början och sedan ett nytt (eller uppdaterat) paket i framtiden innehåller ändringar av objekt i det ursprungliga paketet, kan användaren använda OVERWRITING för att ersätta (åsidosätta) tidigare installerade objekt. </p><p>Mer information om överskrivning finns i avsnittet [Skriva över](#overwriting) i den här artikeln.</li><ul></td> 
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
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/:id/prepare-installation
```

#### Sidhuvuden

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

eller

```json
{
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
{
    "environmentPromotionPackageId": "45f2ae94-76c0-4b13-8f3b-f688de83043d",
    "environmentPromotionPackageVersion": 1,
    "id": "c0bc79bd-c9c1-4b5b-b118-b1241392de0e",
    "userId": "5ba38da500b752fd66439d4f6a9999a1",
    "customerId": "5ba38d9d00b74f0c7a38b1b487fc9710",
    "status": "PREPARING",
    "environment": "mmi.my.workfront.com",
    "registeredAt": "2023-10-19T20:00:16.697Z",
    "updatedAt": "2023-10-19T20:00:16.701Z",
    "translationMap": {
        "CTGY": {
            "62d9c9a0000013aeeefe7242a0a5fdb2": {
                "name": "Example Document Form",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c9a0000013aeeefe7242a0a5fdb2"
            }
        },
        "PGRP": {
            "62d1eee4001c6618e6b9f9a588ba1598": {
                "name": "Asset Detail",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee4001c6618e6b9f9a588ba1598"
            }
        },
        "GROUP": {
            "5ba38da500b752b0f46d13186030b7ad": {
                "name": "Default Group",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "5ba38da500b752b0f46d13186030b7ad"
            }
        },
        "PARAM": {
            "62d1eee400f8578895166ee91a83f97a": {
                "name": "Asset Type",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee400f8578895166ee91a83f97a"
            },
            "62d1eee50001407c713514a8970b58e4": {
                "name": "Keywords",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee50001407c713514a8970b58e4"
            },
            "62d1eee5000333ac3981ea4f3df6d88e": {
                "name": "Permitted Uses",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee5000333ac3981ea4f3df6d88e"
            },
            "62d1eee5000b188e9ec8039a097fc7ab": {
                "name": "File Format",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee5000b188e9ec8039a097fc7ab"
            },
            "62d1eee500100c159fd5f838ce560507": {
                "name": "CTA",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee500100c159fd5f838ce560507"
            },
            "62d9c988001c1f23954dbb9d646335b5": {
                "name": "Other CTA",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c988001c1f23954dbb9d646335b5"
            },
            "62d9c9880070f546cf4c798ea6c3eaa4": {
                "name": "Other Audience",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c9880070f546cf4c798ea6c3eaa4"
            },
            "62d9c990006258baf1b40f2569c3eab7": {
                "name": "Target Audience",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c990006258baf1b40f2569c3eab7"
            }
        }
    }
}
```

>[!NOTE]
>
>Det ID som du måste köra installationen är `id` fält. I det här exemplet `id` fältet är tredje uppifrån och har ett värde som börjar med `c0bc79bd`.

### Kör en installation

>[!IMPORTANT]
>
>Innan du kan köra en installation måste du köra en förkörning. Du använder det ID som genereras från förkörningen när du kör installationen.
>
>Om några ändringar har gjorts i målmiljön (miljön som paketet distribueras till) efter att förkörningen har körts rekommenderar vi att du kör förkörningen igen. Om du inte kör förkörningen igen kanske inte körningen är korrekt eller så kan installationen misslyckas.
>
>Instruktioner om hur du kör en förkörning finns i [Utför en förkörning](#execute-a-pre-run).

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /install</code></td> 
  </tr> 
  </tbody> 
</table>

Det här anropet initierar ett installationsförsök för ett kampanjpaket till målmiljön som identifieras i POSTENS URL.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}/install
```

#### Sidhuvuden

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

eller

```json
{
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
202
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
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
```

#### Sidhuvuden

```json
{
    "apikey": "**********"
}
```

eller

```json
{
    "sessionID": "*****************"
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
        "status": "INSTALLED",
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
    "apikey": "**********"
}
```

eller

```json
{
    "sessionID": "*****************"
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
    "status": "INSTALLED",
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

## Skriv över

Detta är en trestegsprocess.

1. Skapa en översättningskarta (motsvarar fasen&quot;förbereda installation&quot;)
1. Redigera den genererade översättningskartan och ange `action` och `targetId` fält för objekt som de vill skriva över. Åtgärden bör vara `OVERWRITING`och `targetId` ska vara uuid för objektet som ska skrivas över
1. Kör installationen.

* [Steg 1 - Skapa en översättningskarta](#step-1---create-a-translation-map)
* [Steg 2 - Ändra översättningskartan](#step-2---modify-the-translation-map)
* [Steg 3 - Installera](#step-3---install)

### **Steg 1 - Skapa en översättningskarta**

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/translation-map
```

#### Brödtext

Ingen

#### Svar

En översättningskarta, med en `202 - OK` status

```json
{
    {objcode}: {
        {object uuid}: {
            "targetId": {uuid of object in destination},
            "action": {installation action},
            "name": {name of the object},
            "isValid": true
        },
        {...more objects}
    },
    {...more objcodes}
}
```


#### Exempel

```json
{
    "UIVW": {
        "109f611680bb3a2b0c0a8c1f5ec63f6d": {
            "targetId": "6643a26b0001401ff797ccb318f97aa6",
            "action": "CREATE",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIGB": {
        "edb4c6c127d38910e4860eb25569a5cc": {
            "targetId": "6643a26b000178fb5cc27b74cc1e87ec",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIFT": {
        "f97b662e229fd09ee595d8d359ec88bd": {
            "targetId": "6643a26b00015cdd6727b76d6fda1d1d",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "PTLSEC": {
        "4bb80aa88a96420296a7f47bf866f162": {
            "targetId": "4bb80aa88a96420296a7f47bf866f162",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "EXTSEC": {
        "65f8637900015e4dceb6fe079bd5409d": {
            "targetId": "65f8637900015e4dceb6fe079bd5409d",
            "action": "USEEXISTING",
            "name": "Asnyc List",
            "isValid": true
        }
    },
    "PTLTAB": {
        "65f8638a00016422a83ddc3508852d0f": {
            "targetId": "65f8638a00016422a83ddc3508852d0f",
            "action": "CREATEWITHALTNAME",
            "name": "Cool 2.0 The Best",
            "isValid": true
        }
    }
}
```

### Steg 2 - Ändra översättningskartan

Det finns ingen slutpunkt för det här steget.

1. I översättningskartan returneras [Steg 1 - Skapa en översättningskarta](#step-1---create-a-translation-map)kontrollerar du listan med objekt som ska installeras.
1. Uppdatera åtgärdsfältet för varje objekt till önskad installationsåtgärd.
1. Validera `targetId` på varje objekt. Om set-åtgärden är `USEEXISTING` eller `OVERWRITING`, `targetId` ska anges till UUID för målobjektet i målmiljön. För andra åtgärder ska targetId vara en tom sträng.

   >[!NOTE]
   >
   >The `targetId` fylls redan i om en kollision upptäcktes.

### **Steg 3 - Installera**

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/install
```

#### Brödtext

Detta är ett objekt med ett enda fält `translationMap`som ska vara lika med den ändrade översättningskartan från [Steg 2 - Ändra översättningskartan](#step-2---modify-the-translation-map).

```json
{
    "translationMap": {
        {objcode}: {
            {object uuid}: {
                "targetId": {uuid of object in destination},
                "action": {installation action},
                "name": {name of the object},
                "isValid": true
            },
            {...more objects}
        },
        {...more objcodes}
    }
}
```


#### Exempel

```json
{
    "translationMap": {
    "UIVW": {
        "109f611680bb3a2b0c0a8c1f5ec63f6d": {
            "targetId": "6643a26b0001401ff797ccb318f97aa6",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIGB": {
        "edb4c6c127d38910e4860eb25569a5cc": {
            "targetId": "6643a26b000178fb5cc27b74cc1e87ec",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIFT": {
        "f97b662e229fd09ee595d8d359ec88bd": {
            "targetId": "6643a26b00015cdd6727b76d6fda1d1d",
            "action": "OVERWRITING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "PTLSEC": {
        "4bb80aa88a96420296a7f47bf866f162": {
            "targetId": "4bb80aa88a96420296a7f47bf866f162",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "EXTSEC": {
        "65f8637900015e4dceb6fe079bd5409d": {
            "targetId": "65f8637900015e4dceb6fe079bd5409d",
            "action": "USEEXISTING",
            "name": "Asnyc List",
            "isValid": true
        }
    },
    "PTLTAB": {
        "65f8638a00016422a83ddc3508852d0f": {
            "targetId": "65f8638a00016422a83ddc3508852d0f",
            "action": "CREATEWITHALTNAME",
            "name": "Cool 2.0 The Best",
            "isValid": true
        }
    }
}
}
```

#### Svar

Svaret innehåller `{uuid of the created installation}` och `202 - ACCEPTED` status.

Exempel: `b6aa0af8-3520-4b25-aca3-86793dff44a6`

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

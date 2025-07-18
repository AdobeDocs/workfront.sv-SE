---
title: Grunderna i Adobe Workfront Planning API
description: Målet för Adobe Workfront Planning API är att förenkla byggintegreringen med Planning genom att införa en REST-full arkitektur som fungerar över HTTP. I det här dokumentet förutsätts att du känner till REST- och JSON-svar och beskriver den metod som används i Planning API.
author: Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: afb58d04-fa75-4eb7-9c19-2a8c1748fbc2
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 0%

---


# Grunderna i Adobe Workfront Planning API

{{planning-important-intro}}

Målet för Adobe Workfront Planning API är att förenkla byggintegreringen med Planning genom att införa en REST-full arkitektur som fungerar över HTTP. I det här dokumentet förutsätts att du känner till REST- och JSON-svar och beskriver den metod som används i Planning API.

Tack vare Workfront Planning-schemat är det lättare att förstå de databasrelationer som kan användas för att hämta data från Workfront Planning för integrering.

Du kan anropa planerings-API:t från ett externt sökfält i ett anpassat Workfront-formulär.

Mer information om externa sökfält finns i [Exempel på ett externt sökfält i ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

>[!NOTE]
>
>Användare måste läggas till i Adobe Admin Console för att vara tillgängliga i API-anrop. Det går inte att komma åt användare som bara har Workfront via Adobe Planning API.
>
>Mer information finns i [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).


## URL för Workfront Planning API

<!--For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).-->

### Operationer

Objekten ändras genom att en HTTP-begäran skickas till deras unika URI. Den åtgärd som ska utföras anges av HTTP-metoden.

HTTP-standardmetoderna motsvarar följande åtgärder:

* **GET** - Hämtar ett objekt efter ID, söker efter alla objekt efter en fråga
* **POST** - Infogar ett nytt objekt
* **PUT** - Redigerar ett befintligt objekt
* **DELETE** - Tar bort ett objekt

Mer information och exempel på de olika åtgärderna finns i [dokumentationen för Workfront Planning API-utvecklare](https://developer.adobe.com/wf-planning/).

### Fälttyper och sökmodifieringar som används med dem

Du kan använda modifierare och filter med fält för att styra vilka data som returneras i resultatet.

<!--For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).-->

#### Använda sökmodifierare

Workfront Planning stöder följande sökmodifierare:

<table>
    <tr>
        <td><b>Modifierare</b></td>
        <td><b>Exempel</b></td>
        <td><b>Beskrivning</b></td>
        <td><b>Möjliga värden</b></td>
    </tr>
    <tr>
        <td>$contains </td>
        <td><code>"fieldId": { "$contains": "product" } </code> </td>
        <td>Returnerar poster vars fältvärde innehåller filtret  </td>
        <td>"Ny produktlansering"  </td>
    </tr>
    <tr>
        <td>$doesNotContain</td>
        <td><code>"fieldId": { "$doesNotContain": "product" } </code> </td>
        <td>Returnerar poster där fältvärdet inte innehåller filtret  </td>
        <td>"New Launch"  </td>
    </tr>
    <tr>
        <td>$is </td>
        <td><ul><li><code>"fieldId" : { "$is": "new product launch" } </code></li><li><code>"fieldId" : { "new product launch" } </code></li><ul> </td>
        <td>Returnerar poster vars fältvärde exakt matchar filtret  </td>
        <td>"Ny produktlansering"  </td>
    </tr>
    <tr>
        <td>$isNot </td>
        <td><code>"fieldId": { "$isNot": "product" } </code> </td>
        <td>Returnerar poster vars fältvärde inte matchar filtret exakt  </td>
        <td>"Ny produktlansering"  </td>
    </tr>
    <tr>
        <td>$isEmpty </td>
        <td><ul><li><code>"fieldId": "$isEmpty" </code></li><li><code>"fieldId": { "$isEmpty": null } </code></li><ul> </td>
        <td>Returnerar poster vars fältvärde inte är tomt  </td>
        <td><ul><li>"" </li><li>null </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotEmpty </td>
        <td><ul><li><code>"fieldId": "$isNotEmpty"  </code></li><li><code>"fieldId": { "$isNotEmpty": null } </code></li><ul> </td>
        <td>Returnerar poster vars fältvärde inte är tomt  </td>
        <td>"Ny produktlansering"  </td>
    </tr>
    <tr>
        <td>$greaterThan </td>
        <td><code>"fieldId": { "$greaterThan": 10 } </code> </td>
        <td>Returnerar poster vars fältvärde är större än filtret  </td>
        <td><ul><li>20</li><li>25</li><ul> </td>
    </tr>
    <tr>
        <td>$greaterThanOrEqual </td>
        <td><code>"fieldId": { "$greaterThanOrEqual": 10 } </code> </td>
        <td>Returnerar poster vars fältvärde är större än eller lika med filtret  </td>
        <td><ul><li>10</li><li>20</li><li>25</li> </ul></td>
    </tr>
    <tr>
        <td>$lessThan </td>
        <td><code>"fieldId": { "$lessThan": 10 } </code> </td>
        <td>Returnerar poster vars fältvärde är mindre än filtret  </td>
        <td><ul><li>5</li><li>9</li></td></ul> 
    </tr>
    <tr>
        <td>$lessThanOrEqual </td>
        <td><code>"fieldId": { "$lessThanOrEqual": 10 } </code> </td>
        <td>Returnerar poster vars fältvärde är mindre än eller lika med filtret </td>
        <td><ul><li>5</li><li>9</li><ul><li>10</li> </td>
    </tr>
    <tr>
        <td>$isAfter </td>
        <td><code>"fieldId": { "$isAfter": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Returnerar poster vars fältvärde är efter filtret  </td>
        <td>"2024-05-15T20:00:00.000Z"  </td>
    </tr>
    <tr>
        <td>$isBefore </td>
        <td><code>"fieldId": { "$isBefore": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Returnerar poster vars fältvärde är före filtret </td>
        <td>"2024-05-12T20:00:00.000Z" </td>
    </tr>
    <tr>
        <td>$isBetween </td>
        <td><code>"fieldId": { "$isBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Returnerar poster vars fältvärde är mellan filtret  </td>
        <td><ul><li>"2024-05-12T20:00:00.000Z" </li><li>"2024-05-14T20:00:00.000Z" </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotBetween </td>
        <td><code>"fieldId": { "$isNotBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Returnerar poster vars fältvärde inte är mellan filtret  </td>
        <td><ul><li>"2024-05-09T20:00:00.000Z"  </li><li>"2024-05-17T20:00:00.000Z"  </li><ul>  </td>
    </tr>
    <tr>
        <td>$isAnyOf </td>
        <td><code>"fieldId": { "$isAnyOf": ["active", "completed"] } </code> </td>
        <td>Returnerar poster vars fältvärde är något av filtret  </td>
        <td><ul><li>"active" </li><li>"avslutad" </li><ul> </td>
    </tr>
    <tr>
        <td>$isNoneOf </td>
        <td><code>"fieldId": { "$isNoneOf": ["active", "completed"] } </code> </td>
        <td>Returnerar poster vars fältvärde inte är något av filtret </td>
        <td><ul><li>"avslutad"  </li><li>"fixed"  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAnyOf </td>
        <td><code>"fieldId": { "$hasAnyOf": ["active", "completed"] } </code> </td>
        <td>Returnerar poster vars fältvärde har något av filtren  </td>
        <td><ul><li>["active", "fixed"]  </li><li>["fixed", "completed", "completed"]  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAllOf </td>
        <td><code>"fieldId": { "$hasAllOf": ["active", "completed"] } </code> </td>
        <td>Returnerar poster vars fältvärde innehåller hela filtret  </td>
        <td><ul><li>["active", "completed"]   </li><li>["active", "completed", "completed"]   </li><ul> </td>
    </tr>
    <tr>
        <td>$hasNoneOf </td>
        <td><code>"fieldId": { "$hasNoneOf": ["active", "completed"] } </code> </td>
        <td>Returnerar poster vars fältvärde inte har något filter </td>
        <td>["fixed", "completed"]  </td>
    </tr>
    <tr>
        <td>$isexact </td>
        <td><code>"fieldId": { "$isExactly": ["active", "completed"] } </code> </td>
        <td>Returnerar poster vars fältvärde är exakt lika med filtret  </td>
        <td>["active", "completed"]  </td>
    </tr>
</table>

#### Fälttyper

Nedan finns en lista över de fälttyper som stöds och vilka sökmodifierare som kan användas för var och en av dessa fälttyper

| Fälttyp | Sökmodifierare som stöds |
|---|---|
| text | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| lång text | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| tal | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| procent | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| valuta | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| datum | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| enkelval | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| markera flera | $hasAnyOf, $hasAllOf, $isExakt, $hasNoneOf, $isEmpty, $isNotEmpty |
| boolesk | $is |
| användare | $hasAnyOf, $hasAllOf, $isExakt, $hasNoneOf, $isEmpty, $isNotEmpty |
| formel | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| url | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| skapad av | $is, $isNot, $isAnyOf, $isNoneOf |
| created-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween |
| uppdaterad | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| uppdaterad-kl | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| referens | $hasAnyOf, $hasAllOf, $isExakt, $hasNoneOf, $isEmpty, $isNotEmpty |
| sökning | Beroende på det länkade fältet |

### Använda programsatserna &quot;And&quot; och &quot;Or&quot;

I API-anropet kan du ha filter som baseras på flera kriterier som kombineras med $and&quot; och&quot;$or&quot;.

```
{
  "recordTypeId": "recordTypeId",
  "offset": "integer",
  "limit": "integer",
  "filters": [
    {
      "$or": [
        {
          "launch_date": {
            "$isBetween": [
              "2024-03-31T20:00:00.000Z",
              "2024-04-01T20:00:00.000Z"
            ]
          }
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-03-31T20:00:00.000Z",
                  "2024-04-01T20:00:00.000Z"
                ]
              }
            },
            {
              "status": "active"
            }
          ]
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-04-15T00:00:00.000Z",
                  "2024-04-16T00:00:00.000Z"
                ]
              }
            },
            {
              "status": "planned"
            }
          ]
        }
      ]
    }
  ]
}
```

### Använda fältförfrågningsparametern

Du kan använda fältparametern request för att ange en kommaavgränsad lista med specifika fält som ska returneras. Dessa fältnamn är skiftlägeskänsliga.

Till exempel begäran

`/v1/records/search?attributes=data,createdBy`

```
{
    "records": [
        {
            "id": "Rc6527ecb35df57c441d92ba00",
            "createdBy": "61a9cc0500002f9fdaa7a6f824f557e1",
            "createdAt": null,
            "updatedBy": null,
            "updatedAt": null,
            "customerId": null,
            "imsOrgId": null,
            "recordTypeId": null,
            "data": {
                "F666c0b58b6fee61a2ea6ea81": [
                    {
                        "externalId": null,
                        "id": "Rc665728ff95730b58bc757b13",
                        "value": null
                    },
..
```

returnerar ett svar som liknar följande:


```
{ 
    "priority": 2, 
    "name": "first task", 
    "ID": "4c7c08fa0000002ff924e298ee148df4", 
    "plannedStartDate": "2010-08-30T09:00:00:000-0600" 
} 
```

### Sortera frågeresultat i API

Du kan sortera resultatet efter vilket fält som helst om du lägger till följande i ditt API-anrop:


`/v1/records/search`

Begärandetext:

```
{
    "recordTypeId": "Rt6527ecb25df57c441d92b9fa",
    "filters": [],
    "sorting": [
        {
            "fieldId": "F6527ecb25df57c441d92b9fc",
            "direction": "asc"
        },
        {
            "fieldId": "F658afcbd4a0273c67c346fd5",
            "direction": "desc"
        }
    ],
    "limit": 500,
    "offset": 0,
    "rowOrderViewId": "V6527ecb75df57c441d92ba03",
    "groupingFieldIds": []
}
```

### Frågebegränsningar och sidnumrerade svar

Som standard returnerar Planning API-begäranden 500 resultat från början av listan. Om du vill åsidosätta standardbegränsningen för antal resultat kan du använda parametern `limit` i dina begäranden och ange ett annat tal, upp till 2 000 resultat.

Vi rekommenderar att du använder sidnumrerade svar för stora datauppsättningar genom att lägga till parametern `offset` i dina förfrågningar. Med sidnumrerade svar kan du ange platsen för det första resultatet som ska returneras.

Om du till exempel vill returnera resultatet 2001-4000 kan du använda följande begäran. I det här exemplet returneras 2000 poster som har aktiv status, från och med resultatet 2001:

`POST /v1/records/search `



Begärandetext:

```
{ 
    "recordTypeId": "recordTypeId", 
    "offset": "2001", 
    "limit": "2000", 
    "filters": [ 
        { "status": "active" } 
    ] 
} 
```

Använd en sorteringsparameter för att försäkra dig om att resultatet är rätt sidnumrerat. Detta gör att resultaten kan returneras i samma ordning, så att sidnumreringen inte upprepas eller hoppar över resultat.

Mer information om sortering finns i [Sortera frågeresultat i API:t](#sorting-query-results-in-the-api) i den här artikeln.

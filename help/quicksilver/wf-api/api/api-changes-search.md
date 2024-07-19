---
filename: api-changes-search
content-type: api
keywords: objekt,status,sökning,bästa,praxis,svar
navigation-topic: api-navigation-topic
title: "Core API changes: Status search responses"
description: Förändringar i hur Workfront lagrar statusobjekt.
feature: Workfront API
role: Developer
exl-id: 322f1525-d1d5-4845-a590-e34eb94ccdc2
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 0%

---

# Centrala API-ändringar: statussöksvar

Det har gjorts ändringar i hur statusobjekt lagras i Workfront. De här ändringarna påverkar inte hur statussökningar utförs, men påverkar svaret som returneras av API-begäranden som innehåller en sökning efter statusobjekt genom att returnera en ofullständig lista med gruppstatus.

## God praxis

För att på ett tillförlitligt sätt hämta den fullständiga listan över status som är tillgängliga för en grupp, anses följande begäranden vara bästa praxis.

>[!NOTE]
>
>Dessa begärandestrukturer rekommenderas för alla användare oavsett om statussökningen har ändrats i klustret eller inte.

För projektgruppsstatus:

>**Exempel:**

```
/attask/api/<VERSION>/CSTEM/projectGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

För aktivitetsgruppstatus:

>**Exempel:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

För Ärendegruppsstatus:

>**Exempel:**

```
/attask/api/<VERSION>/CSTEM/opTaskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Alla dessa tre slutpunkter accepterar parametern **includeHidden=true** för att hämta de dolda statusvärdena för projekt/aktivitet/problem i en viss grupp. När du utformar dina statussökfrågor efter dessa metodexempel ser du till att all gruppstatusinformation inkluderas i varje svar.

Här är ett exempel på en statussökfråga som görs till en uppgiftsgrupp som innehåller en låst status på systemnivå **Custom_1** och en olåst status **Custom_2**:

>**Exempel:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d286d000004fc8f53942de697a868
```

Om du använder det här formatet ser du till att ditt svar innehåller följande:

```
{
    "data": [
        {
            "color": "1C68FF",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "New",
            "objCode": "CSTEM",
            "value": "NEW"
        },
        {
            "color": "39FF39",
            "equatesWith": "INP",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "In Progress",
            "objCode": "CSTEM",
            "value": "INP"
        },
        {
            "color": "FF3939",
            "equatesWith": "CPL",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Complete",
            "objCode": "CSTEM",
            "value": "CPL"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_1",
            "objCode": "CSTEM",
            "value": "JET"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_2",
            "objCode": "CSTEM",
            "value": "OGC"
        }
    ]
}
```

## Förstå ändringar som gjorts i den äldre statussökfrågan

I det äldre systemet kopierar en statussökfråga alla systemstatusar som är tillgängliga för alla grupper som ingår i en fråga. Det gamla svaret skulle sedan inkludera alla systemstatusar och gruppnivåstatusar som är tillgängliga för varje grupp i frågan.

Den här frågan (som inte följer aktuella rekommenderade metoder):

>**Exempel:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

Skulle få följande svar under det äldre systemet, som inkluderar alla objektstatusar:

```
{
    "data": [
        {
            "color": "1C68FF",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "New",
            "objCode": "CSTEM",
            "value": "NEW"
        },
        {
            "color": "39FF39",
            "equatesWith": "INP",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "In Progress",
            "objCode": "CSTEM",
            "value": "INP"
        },
        {
            "color": "FF3939",
            "equatesWith": "CPL",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Complete",
            "objCode": "CSTEM",
            "value": "CPL"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_1",
            "objCode": "CSTEM",
            "value": "JET"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_2",
            "objCode": "CSTEM",
            "value": "OGC"
        }
    ]
}
```

Efter de uppdateringar som gjorts av hur statusvärden lagras och används, kopieras inte statusvärdena för grupper och ärvs av varje grupp på systemnivå. Detta resulterar i att söknings-API-frågan bara läser de statusar som är direkt kopplade till en viss grupp, så svaret innehåller status som är låst i systemet och olåst, men bara för de grupper som skapades efter att statusen i fråga lades till.

Om de uppdaterade metoderna för bästa praxis inte används för att söka efter status efter att det äldre systemet har uppdaterats, returneras en ofullständig lista över gruppstatus i svaret.

Här är ett exempel på vad den här föråldrade begärandestrukturen returnerar efter att det äldre systemet har uppdaterats:

>**Exempel:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

Observera att detta svar endast omfattar gruppspecifika statusar och utelämnar de statusvärden som deklarerats på systemnivå:

```
{
  "data": [
    {
      "color": "8BC34A",
      "equatesWith": "NEW",
      "groupID": "602d286d000004fc8f53942de697a868",
      "label": "Custom_2",
      "objCode": "CSTEM",
      "value": "MMI"
    }
  ]
}
```

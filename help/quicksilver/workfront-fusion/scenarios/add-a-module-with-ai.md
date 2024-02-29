---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Generera en modul med AI
description: Du kan ange en textfråga för att skapa en HTTP-modul som är konfigurerad för frågan.
author: Becky
feature: Workfront Fusion
source-git-commit: 8f6216938b2fe946f6acd02c45c2072476b0c47b
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Generera en modul med AI

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>Eftersom den här funktionen fortfarande är i ett tidigt utvecklingsskede är den endast tillgänglig för användare inom Workfront.

Du kan använda AI för att ange en textprompt som beskriver vad du behöver en modul för att göra. Fusion genererar sedan en HTTP-modul som ansluter till rätt slutpunkt för det önskade API:t.

Precis som för allt som genereras från AI rekommenderar vi att du dubbelkontrollerar och testar den genererade modulen för att se till att den fungerar som den ska.

## AI-modulprogram som stöds för närvarande

Fusion AI kan för närvarande generera moduler som ansluter till följande program:

* Adobe Maestro
* Adobe Analytics
* Adobe PDF Services
* Adobe Marketo
* Adobe Frame.io
* Dropbox
* NetSuite
* Google Calendar
* Atlassian Jira
* GitLab
* Spotify
* Bitbucket
* OpenAI
* Slack

## Generera en modul

1. Lägg till en modul och markera **Generera med AI** i listan över program.

   eller

   Högerklicka på ett tomt område i scenarioredigeraren och välj sedan **Generera med AI**.
1. Skriv en textruta i rutan.

   Tips om uppmaningar finns på [Tips för att skapa textmeddelanden](#tips-for-creating-text-prompts) i den här artikeln.
1. Lägg till API-token för programmet i modulen.
1. Kontrollera att modulen verkar vara konfigurerad för rätt program och åtgärd.
1. (Villkorligt) Om modulen inte är kopplad till ditt scenario drar du den på plats.

Vi rekommenderar att du testar modulen för att kontrollera att den genererade modulen fungerar som den ska.

## Tips för att skapa textmeddelanden

Textmeddelanden ska innehålla minst följande information:

* Programmet som du ansluter till
* Den åtgärd som du vill utföra

>[!INFO]
>
>**Exempel**:
>
>* `Retrieve a list of my calendars from Google Calendar`
>
>   Detta inkluderar programmet `Google Calendar` och åtgärden `Retrieve a list of my calendars`.
>
>* `Retrieve popular songs from Spotify`
>
>   Detta inkluderar programmet `Spotify` och åtgärden `Retrieve popular songs`.

Tänk på följande när du skapar textmeddelanden:

* Eftersom varje Fusion-modul utför en enda åtgärd bör en specifik åtgärd beskrivas i textprompten.
* Använd direkt, enkelt språk.
* Kontrollera och testa modulen. Om den inte fungerar som förväntat kan du förfina uppmaningen och försöka igen.




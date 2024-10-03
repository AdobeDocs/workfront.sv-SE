---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Generera ett scenariosegment med AI
description: Du kan ange en textfråga för att skapa en HTTP-modul som är konfigurerad för frågan.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 899641a0-a104-4be9-b423-34a32e985b53
source-git-commit: 5de5b96bc74ce9b819acfa7b5f16652509ccade1
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Generera ett scenariosegment med AI

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>Eftersom den här funktionen är i Beta är den bara tillgänglig för vissa Workfront-användare.

Du kan använda AI för att ange en textprompt som beskriver vad du behöver en del av ditt scenario för att göra. Fusion genererar sedan moduler som utför dessa åtgärder, som du kan använda i ditt scenario.

Precis som för allt som genereras från AI rekommenderar vi att du kontrollerar och testar de genererade modulerna för att se till att de fungerar som de ska.

## AI-modulprogram som stöds för närvarande

Fusion AI kan för närvarande generera moduler som ansluter till följande program:

* Adobe Firefly
* Azure OpenAI
* Microsoft Graph
* Adobe Workfront Planning
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

## Generera moduler

1. Börja lägga till en modul och välj **Generera med AI** i listan över program.

   eller

   Klicka på ikonen Generera med AI ![Generera med AI](assets/generate-with-ai-icon-beta.png) längst ned på sidan för scenarieredigering.

   AI-assistentpanelen öppnas.
1. Skriv en textruta i rutan.

   Tips om uppmaningar finns i [Tips om hur du skapar textmeddelanden](#tips-for-creating-text-prompts) i den här artikeln.

   AI Assistant genererar modulen eller moduluppsättningen.
1. (Villkorligt) Lägg till API-token för programmet i modulerna om det behövs.
1. Kontrollera modulerna för att se till att de är konfigurerade för rätt program och åtgärd.
1. (Villkorligt) Om det genererade scenarioavsnittet inte är kopplat till ditt scenario drar du det till rätt plats.

Vi rekommenderar att du testar modulerna för att kontrollera att de fungerar som de ska.

## Tips för att skapa textmeddelanden

Textmeddelanden ska innehålla minst följande information:

* Programmet som du ansluter till
* Den eller de åtgärder som du vill utföra

>[!IMPORTANT]
>
>Du kan generera mer än en modul i taget, men du kan bara generera moduler för ett program i taget.

>[!INFO]
>
>**Exempel**:
>
>* `Delete the records 'xyz-123', 'xyz-456', 'xyz-789' from Adobe Workfront Planning`
>Detta inkluderar programmet `Workfront Planning` och åtgärden `delete records`. Denna uppmaning skapar tre moduler, en för varje post som ska tas bort.
>* `Change campaign summary of the record 'xyz-123' from Adobe Workfront Planning`
>Detta inkluderar programmet `Workfront Planning` och åtgärden `change campaign summary`.
>* `Get all field details in the record type with ID 'test-record' from Adobe Workfront Planning`
>Detta inkluderar programmet `Workfront Planning` och åtgärden `get field details`.
>
>Följande exempel är INTE korrekt:
>
>* `Generate an image in Adobe Firefly and upload it to Dropbox`
>
>    Det här exemplet är felaktigt eftersom det innehåller mer än ett program

Tänk på följande när du skapar textmeddelanden:

* Använd direkt, enkelt språk.
* Kontrollera och testa dina moduler. Om den inte fungerar som förväntat kan du förfina uppmaningen och försöka igen.

---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion - översikt
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: 13d6230d-51f6-4f68-8697-30f8ce6c8599
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# Översikt över scenariot [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [Scenarioöversikt](https://experienceleague.adobe.com/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/scenario-overview.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] kräver en [!DNL Adobe Workfront Fusion]-licens utöver en [!DNL Adobe Workfront license].

>[!IMPORTANT]
>
>[!DNL Workfront Fusion]-scenarier får inte blandas ihop med [!DNL Workfront Scenario Planner]-scenarier. Mer information om [!DNL Workfront Scenario Planner]-scenarier finns i [Översikt [!DNL Scenario Planner] över](../../scenario-planner/scenario-planner-overview.md).

Rollen för [!DNL Adobe Workfront Fusion] är att automatisera dina processer så att du kan koncentrera dig på nya uppgifter i stället för att upprepa samma uppgifter om och om igen. Det fungerar genom att länka åtgärder inom och mellan program och tjänster för att skapa ett scenario som överför och omvandlar data automatiskt. Scenariot du skapar letar efter data i en app eller tjänst och bearbetar data för att ge det resultat du vill ha.

Ett scenario består av en serie moduler som anger hur data ska omvandlas i en app eller överföras mellan program och webbtjänster.

## Översikt över scenarioelement

Ett scenario består av olika element. Om du förstår terminologin för dessa element blir det enklare att använda dokumentationen.

### Scenario

Ett **scenario** är en användarskapad serie med automatiska steg som skapats för att flytta och ändra data. Termen scenario avser hela gruppen med anslutna steg.

![Scenario](assets/entire-scenario-scenario.png)

### Utlösare

Ett scenario börjar med en **utlösare**. Utlösaren söker efter nya och uppdaterade data och startar scenariot när vissa villkor som har konfigurerats i modulen tillämpas. Utlösare kan konfigureras för att starta ett scenario enligt ett schema (avsökning) eller när dataändringar sker (direkt).

![Utlösare](assets/scenario-trigger.png)

### Modul

Utlösaren följs av ett antal **moduler**. En modul representerar ett steg i ett scenario som utför en viss åtgärd. Moduler är konfigurerade och sammankopplade för att skapa scenarier.

![Modul](assets/scenario-module.png)

### Flöde

Ett scenario kan delas upp i **vägar**. En väg är en del av scenariot som kan användas eller inte för ett givet datapaket. Rutorna konfigureras med hjälp av en routermodul och filter.

![Routning](assets/scenario-route.png)

### Scenariosegment

Ett scenariesegment är ett avsnitt i ett scenario som består av en serie sammanhängande moduler som alla ansluter till samma program. Scenariosegment representerar ofta ett kort arbetsflöde i programmet.

![Scenariosegment](assets/scenario-segment.png)

### Koppling

En koppling är en uppsättning moduler för ett visst program. Workfront Fusion har kopplingar till många vanliga arbetsapplikationer, som Workfront, Salesforce och Jira, samt generiska anslutningar som kan användas för alla webbtjänster.

![Anslutningar](assets/scenario-connectors.png)



## Exempel: Automatiserar processer i [!DNL Adobe Workfront]

>[!NOTE]
>
>Den här funktionen är tillgänglig för följande licenser:
>
>* [!UICONTROL [!DNL Workfront Fusion] for Work Automation]
>* [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]

Med [!DNL Workfront Fusion] kan du automatisera enkla eller komplexa arbetsflöden inom [!DNL Workfront], vilket sparar tid och säkerställer att processen utförs på ett konsekvent sätt.

I det här exemplet utlöses scenariot när ett angivet fält ändras i en aktivitet eller ett problem i [!DNL Workfront]. När scenariot aktiveras hämtas information i det relaterade projektet och en skräddarsydd uppdatering skapas för en person som tilldelats en specifik roll i projektet.

![](assets/fusion-template-example-350x102.png)

## Exempel: Ansluta [!DNL Workfront] till en annan app eller webbtjänst

>[!NOTE]
>
>Den här funktionen är tillgänglig för följande licens:
>
>* [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]
>

[!DNL Workfront Fusion] kan även ansluta till andra program och webbtjänster. Du kan komma åt, importera, ändra och exportera data från andra program och integrera dem med Workfront eller med varandra. Många program har dedikerade [!DNL Workfront Fusion]-anslutningar. Om det inte finns någon dedikerad anslutning för programmet som du vill komma åt kan du använda [!UICONTROL HTTP]- eller [!UICONTROL SOAP]-modulerna för [!DNL Workfront Fusion] för att ansluta till programmet via dess API.

I det här exemplet utlöses scenariot när en användare läggs till i ett [!DNL Excel]-kalkylblad. Scenariot kontrollerar om användaren är i [!DNL Workfront]. Om så inte är fallet skapas användaren i [!DNL Workfront] och användar-ID:t för Workfront läggs tillbaka i kalkylbladet.

![](assets/fusion-integration-example--350x171.png)

En lista över dedikerade anslutningar finns i [Program och deras moduler](../../workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

>[!IMPORTANT]
>
>[!DNL Adobe Workfront Fusion] kan ansluta till nästan alla webbtjänster. Om appen du vill arbeta med inte har någon dedikerad [!DNL Workfront Fusion]-anslutning kan du använda följande moduler för att ansluta direkt till webbtjänsten:
>
>* [[!UICONTROL HTTP] moduler](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)
>* [[!UICONTROL SOAP] modul](../../workfront-fusion/apps-and-their-modules/soap-module.md)
>* [[!UICONTROL JSON] moduler](../../workfront-fusion/apps-and-their-modules/json-modules.md)
>

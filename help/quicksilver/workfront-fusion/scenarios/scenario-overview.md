---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion - översikt
description: Adobe Workfront Fusion kräver en Adobe Workfront Fusion-licens förutom en Adobe Workfront-licens.
author: Becky
feature: Workfront Fusion
exl-id: 13d6230d-51f6-4f68-8697-30f8ce6c8599
source-git-commit: 27158301e491d4ff45ce7987a81f841fb4525b2a
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Översikt över scenariot [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] kräver en [!DNL Adobe Workfront Fusion]-licens utöver en [!DNL Adobe Workfront license].

>[!IMPORTANT]
>
>[!DNL Workfront Fusion]-scenarier får inte blandas ihop med [!DNL Workfront Scenario Planner]-scenarier. Mer information om [!DNL Workfront Scenario Planner]-scenarier finns i [Översikt [!DNL Scenario Planner] över](../../scenario-planner/scenario-planner-overview.md).

Rollen för [!DNL Adobe Workfront Fusion] är att automatisera dina processer så att du kan koncentrera dig på nya uppgifter i stället för att upprepa samma uppgifter om och om igen. Det fungerar genom att länka åtgärder inom och mellan program och tjänster för att skapa ett scenario som överför och omvandlar data automatiskt. Scenariot du skapar letar efter data i en app eller tjänst och bearbetar data för att ge det resultat du vill ha.

Ett scenario består av en serie moduler som anger hur data ska omvandlas i en app eller överföras mellan program och webbtjänster.

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

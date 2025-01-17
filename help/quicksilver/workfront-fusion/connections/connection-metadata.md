---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-2-0
title: Anslutningsmetadata i Adobe Workfront Fusion
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: af260c63-3385-4d5c-abc2-d5c23175be40
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Anslutningsmetadata i Adobe Workfront Fusion

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [Anslutningsmetadata](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/connections/connection-metadata.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] kräver en [!DNL Adobe Workfront Fusion]-licens utöver en [!DNL Adobe Workfront]-licens.

Alla anslutningar är inte desamma. Att förstå skillnaderna mellan anslutningar är mycket viktigt för att man ska veta vilken affärsmiljö de lever i. Fusion använder metadata för att identifiera viktiga attribut i en anslutning.

Du kan ange anslutningsmetadata när du skapar en ny anslutning. Attributen finns i samma dialogruta som används för att konfigurera en anslutning:

![Anslutningsmetadata](assets/connection-metadata-setup.png)

Fusion-användare kan visa och redigera anslutningar från området Anslutningar.

![Anslutningsmetadata i området Anslutningar](assets/connections-area-metadata.png)

## Miljötyp

Fusion-anslutningar kan användas både i produktionssystem och icke-produktionssystem. Att veta skillnaden är mycket viktigt för att skydda produktionsmiljöer. Observera att miljötypen, liksom andra anslutningsmetadata, endast används i informationssyfte. Användarna ansvarar fortfarande för att ställa in attributet korrekt.

## Autentiseringstyp

Fusion-anslutningar kan användas för både tjänstkonton och personliga konton. Tjänstkonton används för autentisering när ett scenario automatiseras som Fusion. Personkonton är autentisering baserat på en viss person. Vilken autentiseringstyp som används beror på scenariots krav. Personkonton bör användas för automatiska användaråtgärder. Om till exempel ett Fusion-scenario automatiserar godkännande av en viss person, ska autentiseringstypen vara för den personen. I annat fall fungerar Fusion som Fusion och typen ska vara&quot;Tjänstkonto&quot;.

Observera att typen, liksom andra anslutningsmetadata, endast används i informationssyfte. Användarna ansvarar fortfarande för att ställa in attributet manuellt.

Mer information om autentiseringstyper finns i [Autentisering](https://developer.adobe.com/developer-console/docs/guides/authentication/) i Adobe autentiseringsguide.

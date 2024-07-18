---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-2-0
title: Anslutningsmetadata i Adobe Workfront Fusion
description: Adobe Workfront Fusion kräver en Adobe Workfront Fusion-licens förutom en Adobe Workfront-licens.
author: Becky
feature: Workfront Fusion
exl-id: af260c63-3385-4d5c-abc2-d5c23175be40
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# Anslutningsmetadata i Adobe Workfront Fusion

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

---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: '''Workfront Fusion-lanseringsaktivitet: Vecka 17 maj 2021"'
description: Den här sidan beskriver alla förbättringar som gjorts i Adobe Workfront Fusion den 17 maj 2021.
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: 930c335e-2c88-41af-983f-82be790c1a4b
hidefromtoc: true
source-git-commit: e6995cd57c4210725d49379df5bcd7e93ce4b02a
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# Versionsaktivitet för Workfront Fusion: 17 maj 2021

Den här sidan beskriver alla förbättringar som gjorts i Adobe Workfront Fusion den 17 maj 2021.

En lista med alla senaste ändringar finns på [Versionsaktivitet för Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

En lista med de senaste felkorrigeringarna i Workfront Fusion finns i [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) och sök efter uppdateringar som heter Workfront Fusion Maintenance Update.

## Kopiera moduler i Workfront Fusion-scenarier

För att göra dina Workfront Fusion-scenarier enklare att arbeta med har vi gjort det möjligt att kopiera och klistra in moduler. Nu kan du kopiera en modul eller en grupp moduler och klistra in dem i samma eller ett annat scenario. När du kopierar moduler bevaras fältvärdena i den modulen.

Mer information finns i [Kopiera moduler eller scenarier i Adobe Workfront Fusion](../../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

## Markera flera moduler i ett Workfront Fusion-scenario

När du redigerar ett scenario kan du nu markera flera moduler i taget. Du kan sedan utföra gruppåtgärder på de valda modulerna.

* Kopiera
* Flytta
* Ta bort

När du kopierar och flyttar moduler behålls modulvärdena och alla linjer som ansluter modulerna.

Mer information om redigeringsscenarier finns i [Skapa ett scenario i Adobe Workfront Fusion](../../../workfront-fusion/scenarios/create-a-scenario.md).

## Modulerna bevarar nu information som inte har sparats

För att göra det enklare att skapa scenarier har vi gjort det möjligt för moduler att bevara fältvärden när de inte är i fokus. När du klickar bort från en modul utan att spara den och sedan återgår till den, visas de värden som du har angett tidigare i fälten. När modulen stängs visas en indikator på att det finns osparade fält.

## Azure AD Connector hanterar nu nya och uppdaterade poster separat

Nya poster och uppdateringar av befintliga poster hanteras nu av separata moduler.

* Du kan använda utlösarmodulen Bevakade poster för att bevaka nya poster. Den här modulen söker inte längre efter uppdaterade poster.
* Om du vill hämta uppdaterade poster kan du använda den nya modulen Sök användare/grupper (delta). Den här modulen returnerar nya, uppdaterade och borttagna poster.

Mer information finns i [Azure Active Directory-moduler](../../../workfront-fusion/apps-and-their-modules/azure-ad-modules.md).

---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: "Workfront Fusion-lansering: 3 maj 2021"
description: Den här sidan beskriver alla förbättringar som gjorts i Adobe Workfront Fusion den 3 maj 2021.
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: af3312c5-3416-4c03-8528-6a2c0240110e
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Versionsaktivitet för Workfront Fusion: 3 maj 2021

Den här sidan beskriver alla förbättringar som gjorts i Adobe Workfront Fusion den 3 maj 2021.

En lista med alla senaste ändringar finns på [Versionsaktivitet för Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

En lista med de senaste felkorrigeringarna i Workfront Fusion finns i [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) och sök efter uppdateringar som heter Workfront Fusion Maintenance Update.

## Salesforce-kopplingen kan nu söka med SOQL

Salesforce > Sök efter poster-modulen har nu möjlighet att söka med hjälp av SOQL (Salesforce Object Query Language). Du kan också söka med de tidigare tillgängliga alternativen (SOSL och enkla sökningar).

Mer information finns i [Salesforce-moduler](../../../workfront-fusion/apps-and-their-modules/salesforce-modules.md).

## Ny anslutningstyp i Azure DevOps-anslutaren kräver färre omfång

För att förbättra säkerheten har vi lagt till en ny anslutningstyp i Workfront Fusion Azure DevOps Connector. När du nu skapar en anslutning i en Azure DevOps-modul kan du välja mellan två typer av anslutningar:

* Azure DevOps

  Den nya anslutningstypen begränsar omfattningen till de som specifikt behövs av Workfront Fusion.

* Azure DevOps (begär alla scope)

  Det här är den äldre anslutningstypen, som begär alla scope som är tillgängliga i en anslutning till Azure DevOps.

Vi rekommenderar att du använder anslutningstypen Azure DevOps i alla nya scenarier där Azure DevOps används. Vi rekommenderar även att du ändrar några Azure DevOps-moduler i dina befintliga scenarier så att de använder den nya anslutningstypen. Den gamla anslutningstypen för Azure DevOps (Begär alla omfattningar) kommer att bli inaktuell inom den närmaste framtiden.

Mer information finns i [Azure DevOps-moduler](../../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md).

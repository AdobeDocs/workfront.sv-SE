---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: '''Workfront Fusion-lanseringsaktivitet: Vecka 3 maj 2021"'
description: Den här sidan beskriver alla förbättringar som gjorts i Adobe Workfront Fusion den 3 maj 2021.
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: af3312c5-3416-4c03-8528-6a2c0240110e
hidefromtoc: true
source-git-commit: 9c2321794c5ba773bfda1d6e9dfda6b8de1a1449
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# Versionsaktivitet för Workfront Fusion: 3 maj 2021

Den här sidan beskriver alla förbättringar som gjorts i Adobe Workfront Fusion den 3 maj 2021.

En lista med alla senaste ändringar finns på [Versionsaktivitet för Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

En lista med de senaste felkorrigeringarna i Workfront Fusion finns i [Workfront Maintenance Updates](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) och sök efter uppdateringar som heter Workfront Fusion Maintenance Update.

## Salesforce-kopplingen kan nu söka med SOQL

Salesforce > Sök efter poster-modulen har nu möjlighet att söka med hjälp av SOQL (Salesforce Object Query Language). Du kan också söka med de tidigare tillgängliga alternativen (SOSL och enkla sökningar).

Mer information finns i [Salesforce-moduler](../../../workfront-fusion/apps-and-their-modules/salesforce-modules.md).

## Ny anslutningstyp i Azure DevOps-anslutaren kräver färre omfång

För att förbättra säkerheten har vi lagt till en ny anslutningstyp i Workfront Fusion Azure DevOps Connector. När du nu skapar en anslutning i en Azure DevOps-modul kan du välja mellan två typer av anslutningar:

* Azure DevOps

   Den nya anslutningstypen begränsar omfattningen till de som specifikt behövs av Workfront Fusion.

* Azure DevOps (begär alla scope)

   Det här är den äldre anslutningstypen, som begär alla scope som är tillgängliga i en anslutning till Azure DevOps.

Vi rekommenderar att du använder anslutningstypen Azure DevOps i alla nya scenarier där Azure DevOps används. Vi rekommenderar även att du ändrar några Azure DevOps-moduler i dina befintliga scenarier så att de använder den nya anslutningstypen. Den gamla anslutningstypen Azure DevOps (Request all scopes) kommer inom kort att bli inaktuell.

Mer information finns i [Azure DevOps-moduler](../../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md).

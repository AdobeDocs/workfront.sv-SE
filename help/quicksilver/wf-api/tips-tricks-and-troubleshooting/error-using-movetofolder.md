---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Åtgärden moveToFolder för dokumentet fungerar inte
description: När åtgärden moveToFolder används returneras ett 422-fel.
author: Becky
feature: Workfront API
role: Developer
exl-id: 811efabc-e101-4de5-a800-a1447654dc3e
source-git-commit: 53edc378e000e5b36fe0ce5750b8917fb13cfde1
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---

# Åtgärden moveToFolder för dokumentet fungerar inte

## Problem

När åtgärden `moveToFolder` för Document-objektet används returneras ett 422-fel.

eller

Om du använder den här åtgärden via Adobe Authenticator-modulen i Workfront Fusion flyttas inte dokumentet, men det finns ingen indikation på felet. Felet är detsamma, men det visas inte i Adobe Authenticator-modulen.

## Lösning

En möjlig orsak till ett 422-fel för den här åtgärden är att åtgärden försöker flytta ett dokument i en länkad mapp till en annan länkad mapp.

Kontrollera att dokumentet som du vill flytta inte redan finns i en länkad mapp.

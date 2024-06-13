---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Åtgärden moveToFolder för dokumentet fungerar inte
description: När åtgärden moveToFolder används returneras ett 422-fel.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 86c0517443537ec5af640036c290b3a495825fdc
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---


# Åtgärden moveToFolder för dokumentet fungerar inte

## Problem

När du använder dokumentobjektets `moveToFolder` returneras ett 422-fel.

eller

Om du använder den här åtgärden via Adobe Authenticator-modulen i Workfront Fusion flyttas inte dokumentet, men det finns ingen indikation på felet. Felet är detsamma, men det visas inte i Adobe Authenticator-modulen.

## Lösning

En möjlig orsak till ett 422-fel för den här åtgärden är att åtgärden försöker flytta ett dokument i en länkad mapp till en annan länkad mapp.

Kontrollera att dokumentet som du vill flytta inte redan finns i en länkad mapp.

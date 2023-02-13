---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Länkade mappar stöds inte för DOCU-objekt
description: Länkade mappar stöds inte för DOCU-objekt
author: Becky
feature: Workfront API
source-git-commit: 9bdc433158e471729bd27d701947d6ae41aa06e7
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---


# API:t för att lägga till en länkad mapp stöds inte

Det går inte att lägga till en länkad mapp i mapparrayen för ett Document-objekt (DOCU) med API:t. Begäran kommer att slutföras, men dokumentet kan tas bort från systemet av vissa externa leverantörer. Detta beror på att det externa systemet kommer att användas som den sista källan till sanning. Om dokumentet tas bort från den externa providern anses därför dokumentet inte längre finnas. Alla dokument som inte hittas i den länkade (externa) mappen kan tas bort automatiskt från [!DNL Workfront] utan möjlighet att återhämta dem.

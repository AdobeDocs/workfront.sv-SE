---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Länkade mappar stöds inte för DOCU-objekt
description: Länkade mappar stöds inte för DOCU-objekt
author: Becky
feature: Workfront API
role: Developer
exl-id: 33b5a998-f3e1-42a2-852e-fb862d770d50
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---

# API:t för att lägga till en länkad mapp stöds inte

Det går inte att lägga till en länkad mapp i mapparrayen för ett Document-objekt (DOCU) med API:t. Begäran kommer att slutföras, men dokumentet kan tas bort från systemet av vissa externa leverantörer. Detta beror på att det externa systemet kommer att användas som den sista källan till sanning. Om dokumentet tas bort från den externa providern anses därför dokumentet inte längre finnas. Alla dokument som inte hittas i den länkade (externa) mappen kan tas bort automatiskt från [!DNL Workfront] utan möjlighet att återhämta dem.

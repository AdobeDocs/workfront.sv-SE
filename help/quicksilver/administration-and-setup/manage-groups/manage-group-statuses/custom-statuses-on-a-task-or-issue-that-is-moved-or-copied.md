---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Anpassade statusvärden för en aktivitet eller ett problem som har flyttats eller kopierats
description: När du flyttar eller kopierar en uppgift eller ett problem till ett annat projekt kan vissa statusvärden för aktiviteten eller problemet uppdateras så att de matchar statusvärdena som används av målprojektgruppen.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4bd9b89d-9c66-4af7-97bf-f9518ad55d7c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# Anpassade statusvärden för en aktivitet eller ett problem som har flyttats eller kopierats

När du flyttar eller kopierar en uppgift eller ett problem till ett annat projekt kan vissa statusvärden för aktiviteten eller problemet uppdateras så att de matchar statusvärdena som används av målprojektgruppen. Detta beror på om det finns statusar med samma nyckel i gruppen:

* Om en status för aktiviteten eller utgåvan har samma nyckel som en status som används av målprojektgruppen, förblir statusen för aktiviteten eller utgåvan densamma.

   Om etiketten för de här två statusvärdena inte matchar, ärver aktivitetens eller frågans status etiketten för statusen som används av målprojektets grupp.

* Om en status i uppgiften eller utgåvan inte har samma nyckel som motsvarande status i målprojektgruppen, ändras statusen i aktiviteten eller utgåvan till motsvarande standardstatus i målprojektgruppen.

Mer information om statusnycklar finns i [Skapa eller redigera en gruppstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

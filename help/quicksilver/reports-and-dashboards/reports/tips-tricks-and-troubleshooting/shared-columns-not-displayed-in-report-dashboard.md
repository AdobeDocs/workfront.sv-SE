---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Data från delade kolumner visas inte i instrumentpanelsrapporter
description: Data från delade kolumner visas inte när rapporten placeras i en layout med flera kolumner, men den visas i en enda kolumnlayout. Radbrytningar åsidosätts också.
author: Nolan
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---

# Data från delade kolumner visas inte i instrumentpanelsrapporter

## Problem

Data från delade kolumner visas inte när rapporten placeras i en layout med flera kolumner, men den visas i en enda kolumnlayout. Radbrytningar åsidosätts också.

## Orsak

Endast kolumner markerade som

```
shortview=true
```

ingår i rapportens kontrollpanelsvy när den vänstra/högra delningen eller vänster/mitten/höger delningsuppsättningen har gjorts i kontrollpanelslayouten.

## Lösning

Öppna den vy som används i rapporten och öppna textläget. (Mer information finns i [Redigera en vy i textläge](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md).) Märk alla kolumner i rapporten, inklusive kolumnerna som används i en delad/sammanfogad kolumn, med

```
shortview=true
```

. Rapportkolumnerna visas sedan korrekt på kontrollpanelen.

---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-tasks
title: Den planerade varaktigheten matchar inte den planerade varaktigheten
description: '"Du får följande felmeddelande: "Den planerade varaktigheten för en aktivitet/ett ärende har gått till 0 och matchar inte den planerade varaktigheten."'
author: Alina
feature: Work Management
exl-id: ef135d44-3138-457d-b54a-3f1102ce3116
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# Den planerade varaktigheten matchar inte den planerade varaktigheten

## Problem

Du får följande felmeddelande: &quot;Den planerade varaktigheten för en aktivitet/ett problem har gått till 0 och matchar inte den planerade varaktigheten.&quot;

## Orsak

Detta inträffar när det planerade startdatumet matchar det planerade slutförandedatumet.

## Lösning

Det finns många faktorer som kan göra att datumen för Projected Start och Completion matchar. Detta problem är till stor del knutet till tidsfördelningen för uppgiften eller frågan.

I de flesta fall, beroende på varaktighetstyp och aktivitetsbegränsning för aktiviteten, bör allokeringen utöka det planerade slutförandedatumet betydligt mer än förväntat. I vissa fall, baserat på hur varaktighetstypen och aktivitetsbegränsningen är konfigurerade, är det möjligt att den i stället är noll.

Här är de bästa sätten att i de fallen kontrollera med länkar till tillhörande artiklar:

* Planerat slutförandedatum: [Översikt över planerat slutförandedatum för projekt, uppgifter och ärenden](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)
* Aktivitetsbegränsning: [Översikt över uppgiftsbegränsning](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)
* Typ av varaktighet: [Översikt över aktivitetsvaraktighet och varaktighetstyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)

Om den planerade typen av slutförandedatum, aktivitetsbegränsning eller Varaktighet fungerar som väntat kontaktar du supporten för mer ingående felsökning.

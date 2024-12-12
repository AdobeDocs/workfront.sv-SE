---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Beräkna planerad arbetskostnad
description: När du planerar arbetet med dina projekt beräknar Adobe Workfront den planerade arbetskostnaden för rollerna och användarna som är tilldelade arbetet baserat på deras värden för Kostnad per timme.
author: Lisa
feature: Work Management
exl-id: af053e9a-09dc-4b4d-8ed4-f681ed611a59
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# Beräkna planerad arbetskostnad

När du planerar arbetet med dina projekt beräknar Adobe Workfront den planerade arbetskostnaden för rollerna och användarna som är tilldelade arbetet baserat på deras värden för Kostnad per timme.

Planerad arbetskostnad för ett projekt är en beräkning mellan kostnaden som är associerad med jobbrollerna eller användarna som är tilldelade att slutföra arbetet i projektet och det antal timmar som planeras (Planerade timmar) som kan ta varje roll eller användare för att slutföra arbetet.

## Översikt över planerad arbetskostnad

Den **planerade arbetskostnaden** för ett projekt beräknas genom att alla planerade arbetskostnader läggs till för alla aktiviteter i projektet.

>[!TIP]
>
>Det finns ingen planerad arbetskostnad kopplad till problem eller själva projektet.

Workfront beräknar den planerade arbetskostnaden för ett projekt med följande formel:

```
Project Planned Labor Cost= SUM(Tasks Planned Labor Cost)
```

Den planerade arbetskostnaden för aktiviteten beräknas utifrån följande:

* Antalet resurser för aktiviteten och deras individuella tilldelning till aktiviteten
* Aktivitetens kostnadstyp.

Den planerade arbetskostnaden för aktiviteten beräknas med följande formel:

```
Task Planned Cost = Planned Hours x User or Job Role Cost Per Hour
```

Mer information om hur Workfront beräknar planerad arbetskostnad för uppgifter, beroende på aktivitetstilldelningar och kostnadstyp, finns i avsnittet Ändra kostnadstyper för enskilda uppgifter i artikeln [Spåra kostnader](../../../manage-work/projects/project-finances/track-costs.md).

## Hitta den planerade arbetskostnaden

Du hittar Planerad arbetskostnad för ett projekt i följande områden i Workfront:

* En projektrapport
* En lista med projekt
* En baslinjerapport där du kan spåra den över tid
* Via API:t

Mer information om hur du skapar rapporter och använder Workfront API finns i följande artiklar:

* [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
* [Grunderna i API](../../../wf-api/general/api-basics.md)

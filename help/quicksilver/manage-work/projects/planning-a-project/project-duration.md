---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Översikt över projektvaraktighet
description: Adobe Workfront beräknar varaktigheten för ett projekt genom att ta hänsyn till startdatumet för den tidigaste aktiviteten och till slutförandedatumet för den senaste aktiviteten och räknar antalet dagar mellan de två datumen.
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Översikt över projektvaraktighet

Adobe Workfront beräknar varaktigheten för ett projekt genom att ta hänsyn till startdatumet för den tidigaste aktiviteten och till slutförandedatumet för den senaste aktiviteten och räknar antalet dagar mellan de två datumen.

## Projektets längd

Projektets längd beräknas enligt följande formel:

```
Project Duration = Completion Date of the latest task - Start Date of the earliest task
```

>[!NOTE]
>
>Varaktigheten för problem i projektet påverkar inte projektets längd.

Projektets längd är antalet dagar mellan de två aktivitetsdatumen baserat på schemat som är associerat med projektet eller de användare som är tilldelade till aktiviteterna. Mer information om vilket schema Workfront använder för att beräkna varaktighet finns i [Översikt över scheman](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).

## Typ av projektvaraktighet

Det finns två typer av projektvaraktighet och formlerna som Workfront använder för att beräkna dem:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Check these formulas? Should they be divided by the hours per day?!) </p>
-->

* **Planerad varaktighet**:

  ```
  Project Planned Duration = Planned Completion Date of the latest task - Planned Start Date of the earliest task / Typical hour per day
  ```

* **Verklig varaktighet**:

  ```
  Project Actual Duration = Actual Completion Date of the latest task - Actual Start Date of the earliest task / Typical hour per day
  ```

## Leta reda på projektvaraktighet

Du hittar alternativen Projektplanerad och Faktisk varaktighet i följande områden i Workfront:

* . Under Projektinformation i avsnittet Översikt.

  Mer information om underfliken Översikt för ett projekt finns i artikeln [Hantera information i projektöversiktsområdet](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* I en projektrapport genom att inkludera fälten Varaktighet eller Verklig varaktighet i rapporten.

  Mer information om hur du skapar rapporter finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

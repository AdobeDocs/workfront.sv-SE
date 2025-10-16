---
content-type: overview
navigation-topic: use-the-gantt-chart
title: Kom igång med diagrammet [!UICONTROL Gantt]
description: Gantt-scheman i Adobe Workfront ger en visuell representation av tidslinjen för en lista över uppgifter eller projekt.
author: Alina
feature: Work Management
exl-id: 96c4e254-ebbe-41d8-a178-7a79ac0abbbd
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---

# Kom igång med [!UICONTROL Gantt Chart]

<!-- Audited: 08/2025 -->

Gantt-scheman i Adobe Workfront ger en visuell representation av tidslinjen för en lista över uppgifter eller projekt.

I [!DNL Adobe Workfront] finns det två [!UICONTROL Gantt Charts] med liknande funktionalitet:

* **Uppgiftslistan[!UICONTROL Gantt Chart]**: visar information om aktiviteter och deras tidslinje på projektnivå. En liknande [!UICONTROL Gantt Chart] visar information om malluppgifter på mallnivå.
* **Projektlistan[!UICONTROL Gantt Chart]**: visar information om projekt och deras tidslinje.

Även om de ser ut och känns lika har de olika funktionalitet.

## Överväganden om Gantt-schemat

* Du kan redigera information i följande [!UICONTROL Gantt Chart]:
   * En uppgiftslista
* Du kan inte redigera information i följande [!UICONTROL Gantt Charts]:
   * En malluppgiftslista
   * En projektlista
* Det finns inget [!UICONTROL Gantt Chart]-alternativ för en lista med mallar.
* Du kan konfigurera vilken information som ska visas både i uppgiftslistan [!UICONTROL Gantt Chart] och i projektlistan [!UICONTROL Gantt Chart].
* Du kan inte konfigurera färgerna eller teckensnitten som [!UICONTROL Gantt chart]-informationen visas i.
* När information uppdateras från aktiviteter återspeglas den automatiskt i både aktivitetslistan [!UICONTROL Gantt Chart] och projektlistan [!UICONTROL Gantt Chart].
* När information uppdateras från malluppgifter återspeglas den automatiskt i malluppgiftslistan [!UICONTROL Gantt Chart].

## Åtkomst till [!UICONTROL Gantt Chart]

Diagrammen [!UICONTROL Gantt] i [!DNL Workfront] ger en visuell representation av en lista med uppgifter eller projekt.

Du kan visa uppgiftslistan [!UICONTROL Gantt Chart] direkt från uppgiftslistan i ett projekt eller från en uppgiftsrapport.

Du kan visa projektlistan [!UICONTROL Gantt Chart] i en projektlista eller en projektrapport.

### Uppgiftslista [!UICONTROL Gantt Chart] {#task-list-gantt-chart}

<!--The task list [!UICONTROL Gantt Chart] is accessible in the following areas:

* In a Project

   * [!UICONTROL Tasks] section
   * [!UICONTROL Subtasks] section of a task

* In a [!UICONTROL Template]

* In a [!UICONTROL Task] report-->

Så här kommer du åt uppgiftslistan [!UICONTROL Gantt Chart] för ett projekt eller en mall:

1. Gå till något av följande:

   * Ett projekt och klicka sedan på [!UICONTROL **Åtgärder**] i den vänstra panelen.
   * En mall och klicka sedan på [!UICONTROL **Malluppgifter**] i den vänstra panelen
   * En aktivitet eller malluppgift och klicka sedan på [!UICONTROL **Underaktiviteter**] i den vänstra panelen.
   * En uppgiftsrapport

1. Klicka på ikonen [!UICONTROL **Gantt**] ![Gantt](assets/gantt-icon-nwe.png) högst upp i uppgiftslistan.

   ![Gantt för uppgiftslista](assets/task-list-gantt.png)

   Uppgiftslistan [!UICONTROL Gantt Chart] öppnas till höger om uppgiftslistan.

1. Om du vill konfigurera vilken information du vill visa i aktivitetsdiagrammet [!UICONTROL Gantt] klickar du på ikonen [!UICONTROL **Inställningar**] och aktiverar sedan något av följande alternativ:

   * [!UICONTROL Actual Dates]
   * [!UICONTROL Assignments]
   * [!UICONTROL Baseline]
   * [!UICONTROL Commit Date]
   * [!UICONTROL % Complete]
   * [!UICONTROL Critical Path]
   * [!UICONTROL Milestone Diamonds]
   * [!UICONTROL Milestone Lines]
   * [!UICONTROL Predecessors]
   * [!UICONTROL Progress Status]
   * [!UICONTROL Projected Dates]

1. Börja redigera uppgifterna enligt följande artiklar:

   * [Konfigurera hur information visas i Gantt-schemat](../use-the-gantt-chart/configure-info-on-gantt-chart.md)
   * [Uppdatera information i Gantt-schema för uppgiftslista](../use-the-gantt-chart/update-info-task-list-gantt.md)

### Projektlista [!UICONTROL Gantt Chart] {#project-list-gantt-chart}

<!--The project list [!UICONTROL Gantt Chart] is accessible in the following areas:

* In the [!UICONTROL Projects] area
* In the [!UICONTROL Projects] section of a [!UICONTROL Portfolio]
* In the [!UICONTROL Projects] section of a [!UICONTROL Program]
* In a [!UICONTROL Project] report-->

Så här kommer du åt projektlistan [!UICONTROL Gantt Chart]:

1. Gå till något av följande:

   * Området [!UICONTROL **Projekt**]
   * Avsnittet [!UICONTROL **Projekt**] i en [!UICONTROL Portfolio]
   * Avsnittet [!UICONTROL **Projekt**] i en [!UICONTROL Program]
   * En [!UICONTROL **Project**]-rapport

1. Klicka på ikonen [!UICONTROL **Gantt**] längst upp i projektlistan.

   ![Projektlista - Gantt](assets/project-list-gantt.png)

   Projektlistan [!UICONTROL Gantt Chart] öppnas.

1. Om du vill konfigurera vilken information du vill visa i projektet [!UICONTROL Gantt] klickar du på ikonen [!UICONTROL **Inställningar**] och aktiverar sedan något av följande alternativ:

   * [!UICONTROL Actual Dates]
   * [!UICONTROL % Complete]
   * [!UICONTROL Milestone Diamonds]
   * [!UICONTROL Milestone Lines]
   * [!UICONTROL Predecessors]
   * [!UICONTROL Progress Status]
   * [!UICONTROL Projected Dates]

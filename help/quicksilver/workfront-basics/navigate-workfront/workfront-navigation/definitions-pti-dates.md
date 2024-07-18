---
content-type: reference
navigation-topic: workfront-navigation
title: Översikt över projekt-, uppgifts- och utfärdandedatum i  [!DNL Workfront]
description: Den här artikeln innehåller definitioner för de vanligaste datumen som är associerade med projekt, uppgifter och utgåvor i  [!DNL Adobe Workfront].
feature: Get Started with Workfront
author: Alina
exl-id: 3808200f-a573-4c39-8965-b254f69c893c
source-git-commit: 040dd446ff2b347dabf8a139feb17fd1a7d50e4e
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 0%

---

# Översikt över projekt-, uppgifts- och utfärdandedatum i [!DNL Workfront]

<!-- Audited: 05/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider expanding on this article with ALL dates for PTIs - Hand off dates, Approval Dates, etc) </p>
-->

Den här artikeln innehåller definitioner för de vanligaste datumen som är associerade med projekt, uppgifter och utgåvor i [!DNL Adobe Workfront]. Bilderna här är exempel på var datumen visas i Workfront och de är inte fullständiga. Det finns andra områden som visar datumen. Alla datum visas också i projekt, uppgifter och utgivningsrapporter och listor.

Mer information om rapporter och listor finns i följande artiklar:

* [Kom igång med listor i  [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)
* [Kom igång med rapporter](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)

Mer information om projekt-, aktivitets- och problemfält finns i [Ordlista för  [!DNL Adobe Workfront] terminologi](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## [!UICONTROL Planned Start Date]

[!UICONTROL Planned Start Date] är det datum då ett projekt, en aktivitet eller ett problem planeras starta.

Beroende på [!UICONTROL Task Constraint] kanske du inte kan redigera [!UICONTROL Planned Start Date] för en aktivitet. Beroende på [!UICONTROL Schedule Mode] för projektet kanske du inte kan redigera [!UICONTROL Planned Start Date] för ett projekt.

Mer information finns i [Översikt över projektet [!UICONTROL Planned Start Date]](../../../manage-work/projects/planning-a-project/project-planned-start-date.md).

![](assets/planned-start-date-on-edit-task-highlighted-nwe.png)

![](assets/planned-start-date-in-task-list-highlighted-nwe-350x167.png)

## [!UICONTROL Planned Completion Date]

Datumet [!UICONTROL Planned Completion Date] eller [!UICONTROL Due On] är det datum då ett projekt, en aktivitet eller ett ärende planeras att slutföras.

Beroende på [!UICONTROL Task Constraint] kanske du inte kan redigera [!UICONTROL Planned Completion Date] för en aktivitet. Beroende på [!UICONTROL Schedule Mode] för projektet kanske du inte kan redigera [!UICONTROL Planned Completion Date] för ett projekt.

[!UICONTROL Planned Completion Date] visas som förfallodatum i vissa områden i [!DNL Workfront].

Mer information finns i följande artiklar:

* [Översikt över uppgiften [!UICONTROL Planned Completion Date]](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [Ange projektet [!UICONTROL Planned Completion Date]](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [Översikt över utgåvan [!UICONTROL Planned Completion Date]](../../../manage-work/issues/issue-information/issue-planned-completion-date.md)

![](assets/project-header-planned-completion-date-highlighted-nwe-350x34.png)

![](assets/planned-completion-date-in-task-list-highlighted-nwe-350x183.png)

## [!UICONTROL Entry Date]

[!UICONTROL Entry Date] är det datum då ett projekt, en uppgift eller ett problem skapades i Workfront.

[!UICONTROL Entry Date] påverkar inte tidslinjen för projekt, aktiviteter eller problem, men det är viktigt för spårnings- och rapportsyften. [!DNL Workfront] genererar automatiskt [!UICONTROL Entry Date] när objektet skapas och du kan inte redigera det manuellt.

![](assets/entry-date-in-task-details-highlighted-nwe.png)

## [!UICONTROL Actual Start Date]

[!UICONTROL Actual Start Date] är det datum då en användare faktiskt börjar arbeta med ett projekt, en uppgift eller ett problem. [!UICONTROL Actual Start Date] är tom när projektet, aktiviteten eller utgåvan skapas.

Du kan ange manuellt när arbetet påbörjades med en uppgift eller ett problem, eller så fylls [!UICONTROL Actual Start Date] automatiskt i när uppgifts- eller utgivningsstatusen ändras från [!UICONTROL New] till [!UICONTROL In Progress] eller [!UICONTROL Complete]. [!UICONTROL Actual Start Date] för ett projekt sammanfaller med datumet då den första aktiviteten i projektet startar.

>[!TIP]
>
>[!UICONTROL Actual Start Date] kanske inte matchar en [!UICONTROL Planned Start Date] för ett projekt, en aktivitet eller ett problem eftersom användaren kan börja arbeta senare eller tidigare än det planerade datumet.

Mer information finns i [Översikt över projektet [!UICONTROL Actual Start Date]](../../../manage-work/projects/planning-a-project/project-actual-start-date.md).

>[!NOTE]
>
>[!UICONTROL Must Start On]-aktiviteten eller begränsningarna Fasta datum påverkar [!UICONTROL Planned Start Date] för en aktivitet, inte [!UICONTROL Actual Start Date]. Detta uppdaterar [!UICONTROL Planned Start Date] till ett datum som du anger. [!UICONTROL Actual Start Date] uppdateras oberoende av [!UICONTROL Planned Start Date], vilket beskrivs ovan.

![](assets/actual-start-date-on-edit-task-highlighted-nwe-350x251.png)

![](assets/actual-start-date-on-task-details-highlighted-nwe-350x191.png)

## [!UICONTROL Actual Completion Date]

[!UICONTROL Actual Completion Date] är det datum som en användare faktiskt slutför ett projekt, en uppgift eller ett problem. [!UICONTROL Actual Completion Date] är tom när projektet, aktiviteten eller utgåvan skapas.

Du kan ange manuellt när arbetet har slutförts för en uppgift eller ett problem, eller så fylls [!UICONTROL Actual Completion Date] automatiskt i när något av följande inträffar:

* Projektet, aktiviteten eller utgivningsstatusen ändras till [!UICONTROL Complete], [!UICONTROL Closed] eller [!UICONTROL Resolved].
* Aktivitets- eller projektprocenten slutförd är 100 %.

[!UICONTROL Actual Completion Date] för ett projekt sammanfaller med datumet när du slutförde den senaste aktiviteten i projektet.

>[!TIP]
>
>[!UICONTROL Actual Completion Date] kanske inte matchar [!UICONTROL Planned Completion Date].

Mer information finns i [Översikt över projektet [!UICONTROL Actual Completion Date]](../../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

![](assets/actual-completion-date-task-details-highlighted-nwe-350x189.png)

## [!UICONTROL Commit Date]

[!UICONTROL Commit Date] är det datum då en användare som har tilldelats en aktivitet eller ett problem bekräftar att uppgiften eller problemet ska slutföras. Detta skiljer sig från [!UICONTROL Planned Completion Date], eftersom det är en mer realistisk uppskattning av det slutförandedatum som bara anges av den användare som ansvarar för arbetet. Mer information finns i [[!UICONTROL Commit Date] - översikt](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

>[!NOTE]
>
>Om du ändrar [!UICONTROL Commit Date] påverkas [!UICONTROL Projected Completion Date] men inte [!UICONTROL Planned Completion Date] för en aktivitet eller ett problem. Projektledaren kan använda de ändringar som en tilldelad gör på [!UICONTROL Commit Date] för att uppdatera [!UICONTROL Planned Completion Date] för en aktivitet eller ett problem.

## [!UICONTROL Projected Start Date]

[!UICONTROL Projected Start Date] är ett realtidsdatum när projektet, aktiviteten eller utgåvan börjar och tar hänsyn till alla förseningar. Detta är ett mer korrekt startdatum för projektet, aktiviteten eller utgåvan än [!UICONTROL Planned Start Date]. [!UICONTROL Planned Start Date] tar inte hänsyn till fördröjningar eller tidigare datum.

När du först planerar ett projekt är [!UICONTROL Planned Start Date] och [!UICONTROL Projected Start Date] för aktiviteterna och projektet identiska. Eftersom förseningar kan inträffa eller uppgifter kan slutföras tidigare kan [!UICONTROL Projected Start Date] skilja sig från [!UICONTROL Planned Start Date].

För en aktivitet kan en [!UICONTROL Projected Start Date] också skilja sig från dess [!UICONTROL Planned Start Date] när en av dess föregångare körs bakom schemat.

>[!TIP]
>
>Du kan bara visa [!UICONTROL Projected Start Date] för ett problem i en lista eller rapport.

Mer information finns i [Översikt över projektet [!UICONTROL Projected Start Date]](../../../manage-work/projects/planning-a-project/project-projected-start-date.md).

![](assets/projected-start-date-in-task-details-highlighted-nwe-350x188.png)

## [!UICONTROL Projected Completion Date]

[!UICONTROL Projected Completion Date] är en beräknad realtidsindikator för när projektet, aktiviteten eller utgåvan ska slutföras. När projektet, aktiviteten eller utgåvan har markerats som Slutförd ändras [!UICONTROL Projected Completion Date] till datumet för [!UICONTROL Actual Completion Date].

Om allt blir jämnt och som planerat ska [!UICONTROL Projected Completion date] matcha [!UICONTROL Planned Completion Date]. I annat fall kan [!UICONTROL Projected Completion Date] skilja sig från [!UICONTROL Planned Completion Date] på grund av fördröjningarna för föregående aktiviteter.

Mer information finns i [Översikt över [!UICONTROL Projected Completion Date] för projekt, uppgifter och problem](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

![](assets/projected-completion-date-in-task-details-highlighted-nwe-350x187.png)

## [!UICONTROL Hour Entry Date]

När du loggar tid för projekt, uppgifter och utleveranser för att ange hur mycket faktisk tid (i timmar) du tillbringar med att arbeta med projektet, aktiviteten eller utleveransen, blir den tid du loggar [!UICONTROL Actual Hours] för projektet, aktiviteten eller utgåvan.

Datumet som du loggar tiden för är fältet [!UICONTROL Hour Entry Date] på timposten. I vissa timlistor och rapporter visas Timinmatningsdatum som datum.

>[!TIP]
>
>[!UICONTROL Hour Entry Date] skiljer sig från [!UICONTROL Entry Date] på så sätt att det inte är det datum då timloggen skapades, utan det datum som du vill att timmarna ska associeras med.

Du kan logga och visa tiden i följande områden i Workfront:

* Logga och visa tiden i avsnittet [!UICONTROL project], [!UICONTROL task] eller [!UICONTROL issue Updates] eller i avsnittet [!UICONTROL Hours]. När du loggar in i avsnittet [!UICONTROL Hours] kan du manuellt ange timanmälningsdatum och användaren som timmarna tillhör.

  ![](assets/log-time-box-task-hours-section-nwe-350x500.png)

  Mer information finns i [Loggtid](../../../timesheets/create-and-manage-timesheets/log-time.md).

  >[!TIP]
  >
  >Vi rekommenderar att du loggar in på arbetsuppgifter och problem i stället för överordnade uppgifter eller projekt. Den tid som är inloggad på arbetsuppgifterna sammanställs till de överordnade aktiviteterna och projektet som [!UICONTROL Actual Hours] för de överordnade aktiviteterna och projektet. Tidsloggade problem sammanställs till projektet som [!UICONTROL Actual Hours] för projektet.

* Logga tid i uppdateringsflödet för en uppgift eller ett problem.

  ![](assets/log-time-in-update-stream-task-nwe-350x185.png)

* Visa [!UICONTROL Hour Entry Dates] i timrapporter och listor.

  ![](assets/hour-entry-date-in-view-nwe-350x173.png)

---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Översikt över läget Uppgiftsspårning
description: Du kan justera inställningen för spårningsläge för en uppgift när du skapar eller redigerar en uppgift för att styra hur och när statusindikatorerna för en uppgift visas. I Adobe Workfront visas statusflaggor när du konfigurerar vissa inställningar för att spåra förloppet för uppgifter.
author: Alina
feature: Work Management
exl-id: 397b5593-ac01-40cf-b683-fcf671a53d26
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# Översikt över läget Uppgiftsspårning

Du kan justera inställningen för spårningsläge för en uppgift när du skapar eller redigerar en uppgift för att styra hur och när statusindikatorerna för en uppgift visas. I Adobe Workfront visas statusflaggor när du konfigurerar vissa inställningar för att spåra förloppet för uppgifter.

Mer information om aktiviteternas förloppsstatus finns i [Översikt över status för åtgärdsförlopp](../../../manage-work/tasks/task-information/task-progress-status.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set Tracking Mode for tasks</h2>
<p>(NOTE: drafted, because we created a new article and linked it below. Left this article as a "Overview" article only.) </p>
<p>To set the tracking mode:</p>
<ol>
<li value="1">Go to the task you want to set the tracking mode for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png">next to the name of the task, then click&nbsp;<strong>Edit</strong>.</p> <p>The Edit Task dialog box opens. </p> </li>
<li value="3"> <p>In the&nbsp;<strong>Settings</strong> section, use the&nbsp;<strong>Tracking Mode</strong> drop-down menu to select the Tracking Mode for the task.</p> <p>For more information about the tracking mode options, see the <a href="#tracking-mode-options" class="MCXref xref" xrefformat="{para}">Tracking Mode options</a> section in this article. </p> </li>
<li value="4">Click&nbsp;<strong>Save Changes.</strong></li>
</ol>
</div>
-->

## Alternativ för spårningsläge {#tracking-mode-options}

Som aktivitetsägare eller projektledare kan du välja hur Workfront ska ange förloppsstatus för varje uppgift. Mer information om hur du anger spårningsläge för dina uppgifter finns i [Ange spårningsläge för uppgifter](../../../manage-work/tasks/task-information/set-tracking-mode-for-tasks.md).

Du kan välja mellan följande alternativ:

* [Användaren måste uppdatera](#user-must-update)
* [Anta i tid](#assume-on-time)
* [Ignorera sena varningar](#ignore-late-warnings)
* [Komplettera automatiskt](#auto-complete)
* [Föregående](#predecessor)

### Användaren måste uppdatera {#user-must-update}

När det här alternativet är markerat använder Workfront uppgiftens loggade procentvärde för slutfört och faktiska timmar för att fastställa uppgiftens förloppsstatus. Det här är standardalternativet.

### Anta i tid {#assume-on-time}

Workfront antar att en uppgift kommer att slutföras i tid oavsett aktuell slutförandestatus. Om så inte är fallet antar Workfront automatiskt ett planerat slutförandedatum som infaller nästa arbetsdag. Du måste fortfarande ange när uppgiften har slutförts. Använd det här alternativet när användare inte regelbundet uppdaterar sina uppgifter.

### Ignorera sena varningar {#ignore-late-warnings}

En uppgifts förloppsstatus är I tid tills den blir sen. Om du t.ex. schemalägger en aktivitet att ta 10 dagar och den dag den ska slutföras, visar Workfront ett Procent färdigt som är 60 %, uppdaterar det beräknade slutförandedatumet genom att lägga till fyra dagar och aktivitetens förloppsstatus blir SENT.

### Komplettera automatiskt {#auto-complete}

Workfront antar att uppgifterna kommer att slutföras enligt schemat och markerar dem som slutförda på förfallodatum eller planerat slutförandedatum. Till dess använder Workfront loggade procentvärden för slutförande och faktiska timmar för att fastställa förloppsstatusen. Oberoende av förloppsstatus före schemalagt slutförandedatum markerar Workfront ändå uppgiften som slutförd.

Följande undantag finns:

* Om aktiviteten har ofullständiga föregångare slutförs den inte automatiskt förrän alla dess föregångare har slutförts.
* Om aktiviteten har begränsningen Fast datum slutförs alltid aktiviteten på det planerade slutförandedatumet, oavsett om dess föregångare har slutförts eller inte.

>[!IMPORTANT]
>
>Om du väljer att låta uppgifter slutföras automatiskt markeras aktiviteten som slutförd när projekttiden beräknas om. Om projektets uppdateringstyp är inställd på Automatisk eller Automatisk och vid ändring, beräknas projekttidslinjen dagligen. Mer information om tidslinjeomberäkningar för projekt finns i [Beräkna om projekttidslinjer](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).
>
>Tiden för det faktiska slutförandedatumet är midnatt på dagen när tidslinjen beräknas automatiskt. Den tid som används för att generera den här tidsstämpeln är datorns Tid&amp;zon som definieras av Workfront-administratören under Kundinformation i installationsprogrammet. Mer information om hur du ställer in datorns tidszon finns i [Konfigurera grundläggande information för ditt system](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Föregående {#predecessor}

Workfront uppskattar det beräknade slutförandedatumet för en aktivitet enligt dess föregående relation. En uppgifts förloppsstatus bestäms utifrån den här uppskattningen. Aktivitet B har till exempel Varaktighet 1 Dag och är schemalagd att slutföras två dagar efter föregående aktivitet, Aktivitet A, som bör ta fem dagar. En användare uppdaterar sedan aktivitet B till 50 % färdigt, men föregående aktivitet, Aktivitet A, har inte startats ännu. Workfront ändrar beroende uppgift B för slutförande sex dagar efter startdatumet för föregående uppgift, vilket ger 5 dagar för uppgift A och 1 dag för uppgift B.

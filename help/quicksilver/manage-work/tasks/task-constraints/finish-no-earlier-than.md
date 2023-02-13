---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Översikt över aktivitetsbegränsning: Avsluta inte tidigare än'
description: Avsluta tidigast (FNET) är en aktivitetsbegränsning som schemalägger en aktivitet att slutföras efter det datum du anger.
author: Alina
feature: Work Management
exl-id: b1dbf5c9-34b6-4c25-b582-ce9454501e03
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Översikt över uppgiftsbegränsning: Avsluta tidigast

Avsluta tidigast (FNET) är en aktivitetsbegränsning som schemalägger en aktivitet att slutföras efter det datum du anger.

## Översikt över villkoret Slutför inte tidigare än

Tänk på följande när du använder begränsningen Slutför inte tidigare än (FNET) för en uppgift:

* Du bör använda den här begränsningen när projektet schemaläggs från slutförandedatum. I det här fallet kan du ange en mjuk begränsning för aktiviteten innan du tvingar andra beroende aktiviteter att visa Vid risk.
* När du använder FNET på ett schemalagt projekt **Från startdatum**, schemalägger villkoret aktiviteten på samma sätt som om villkoret var så snart som möjligt.
* När du flyttar eller kopierar en aktivitet med en FNET-begränsning till ett annat projekt kan villkoret för aktiviteten eller datumen i projektet ändras beroende på vilka villkorsdatumen är och vilka datum projektet börjar och slutförs. Följande scenarier finns:

   * När målprojektet är schemalagt från start:

      * När villkorsdatumet för aktiviteten är tidigare än projektets planerade startdatum, ändras aktivitetsbegränsningen till Så snart som möjligt.
      * När begränsningsdatumet för aktiviteten är senare än projektets Planerat slutförandedatum ändras projektets planerade slutförandedatum så att det matchar slutvillkorsdatumet för aktiviteten.
   * När målprojektet är schemalagt från slutförande:

      * När begränsningsdatumet för aktiviteten är senare än Project Completion Date ändras aktivitetsbegränsningen till As Late As Possible.
      * När villkorsdatumet för aktiviteten är tidigare än det planerade startdatumet för projektet ändras projektets planerade startdatum så att det matchar startvillkorsdatumet för aktiviteten.
   * Oavsett schemat för projektet, när villkorsdatumet för aktiviteten ligger inom projektets start- och slutförandedatum, finns det inga ändringar i aktivitetsbegränsningen eller projektdatumen.

   Mer information om hur du flyttar uppgifter finns i [Flytta uppgifter](../../../manage-work/tasks/manage-tasks/move-tasks.md). Mer information om att kopiera uppgifter finns i [Kopiera och duplicera uppgifter](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

   Mer information om hur du uppdaterar aktivitetsbegränsningen för en uppgift finns i [Uppdatera uppgiftsbegränsningen för en uppgift](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Finish No Earlier Than constraint</h2>
<p>(NOTE: replaced with new article linked above)&nbsp;</p>
<p>To update the Task Constraint to Finish No Earlier Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>Finish No Earlier Than</strong>.</p> <p> <img src="assets/fnet-350x267.png" alt="FNET.png" style="width: 350;height: 267;"> </p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete no earlier than this date. </p> </li>
<li value="6">Click <strong>Save Changes.</strong> </li>
</ol>
</div>
-->

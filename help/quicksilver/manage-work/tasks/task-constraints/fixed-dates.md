---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Översikt över begränsning av aktivitet: fasta datum'
description: Du kan använda aktivitetsbegränsningen Fasta datum när du vill ange ett exakt startdatum och slutdatum för dina uppgifter. Mer information om uppgiftsbegränsningar finns i Översikt över uppgiftsbegränsning.
author: Alina
feature: Work Management
exl-id: 084f54a6-e757-405c-b388-5d5f61608e71
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Översikt över uppgiftsbegränsning: Fasta datum

Du kan använda aktivitetsbegränsningen Fasta datum när du vill ange ett exakt startdatum och slutdatum för dina uppgifter. Mer information om uppgiftsbegränsningar finns i [Översikt över uppgiftsbegränsning](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

## Översikt över begränsningen Fasta datum

Tänk på följande när du använder villkoret Fasta datum:

* När du väljer aktivitetsbegränsningen Fasta datum (FIXT) måste du ange aktivitetens Planerade startdatum och Planerat slutförandedatum. I det här fallet ignoreras aktivitetens föregående relation.
* Fältet Varaktighet för aktiviteten kan inte redigeras när du använder FIXT-begränsningen. Varaktighet beräknas som skillnaden mellan aktivitetens planerade startdatum och planerade slutförandedatum.
* Om aktivitetens varaktighetstyp är Ansträngningsstyrd påverkar antalet tilldelningar för aktiviteten även aktivitetens varaktighet.
* När du flyttar eller kopierar en uppgift med en FIXT-begränsning till ett annat projekt kan villkoret för aktiviteten eller datumen i projektet ändras beroende på vilka villkorsdatumen är och vilka datum projektet börjar och slutförs. Följande scenarier finns:

   * När målprojektet är schemalagt från start:

      * När ett villkorsdatum för aktiviteten är tidigare än projektets startdatum ändras villkoret till Så snart som möjligt.
      * När ett eller båda villkorsdatumen för aktiviteten är senare än projektets planerade slutförandedatum, ändras projektets planerade slutförandedatum så att det matchar slutvillkorsdatumet för aktiviteten.

   * När målprojektet är schemalagt från slutförande:

      * När ett villkorsdatum för aktiviteten är senare än Project Completion Date, ändras aktivitetsbegränsningen till As Late As Possible.
      * När ett eller båda villkorsdatumen för aktiviteten är tidigare än projektets planerade startdatum ändras projektets planerade startdatum så att det matchar startvillkorsdatumet för aktiviteten.

   * Oavsett schemat för projektet, när villkorsdatumen för aktiviteten ligger inom projektets start- och slutförandedatum, finns det inga ändringar i aktivitetsbegränsningen eller projektdatumen.

  Mer information om att flytta uppgifter finns i [Flytta uppgifter](../../../manage-work/tasks/manage-tasks/move-tasks.md). Mer information om att kopiera uppgifter finns i [Kopiera och duplicera uppgifter](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Mer information om hur du uppdaterar aktivitetsbegränsningen för en aktivitet finns i [Uppdatera aktivitetsbegränsningen för en aktivitet](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Fixed Dates Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Finish No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Fixed Dates</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>The task must start on this date. </p> </li>
<li value="6"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete on this date. </p> </li>
<li value="7">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

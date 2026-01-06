---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Översikt över begränsning av aktivitet: Måste starta på'
description: Använd åtgärdsbegränsningen Måste starta på (MSO) om du vill schemalägga en aktivitet att starta exakt på ett visst datum.
author: Alina
feature: Work Management
exl-id: 09062d46-2b80-4758-946e-d6dec0f7a7c0
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Översikt över aktivitetsbegränsning: Måste starta på

Använd åtgärdsbegränsningen Måste starta på (MSO) om du vill schemalägga en aktivitet att starta exakt på ett visst datum.

Begränsningen Måste starta den schemalägger en aktivitet att starta exakt vid den tidpunkt och det datum som du anger i fältet **Planerat startdatum**.

>[!TIP]
>
>Om du uppdaterar en uppgifts planerade startdatum manuellt ändras aktivitetens begränsning till Måste starta den.

## Översikt över måste starta vid aktivitetsbegränsning

Tänk på följande när du schemalägger en aktivitet med en must Start On-begränsning:

* Föregående relationer tvingar inte den här aktiviteten att schemalägga om. Workfront ignorerar i stort sett alla föregående relationer för aktiviteten med den här begränsningen.
* Aktiviteten visar **Vid risk** om föregående aktiviteter börjar köras bakom eller sent.

* När du flyttar eller kopierar en uppgift med en MSO-begränsning till ett annat projekt kan begränsningen för aktiviteten eller datumen i projektet ändras beroende på vilka villkorsdatumen är och vilka datum projektet börjar och slutförs. Följande scenarier finns:

   * När målprojektet är schemalagt från start:

      * När villkorsdatumet för aktiviteten är tidigare än projektets planerade startdatum, ändras aktivitetsbegränsningen till Så snart som möjligt.
      * När begränsningsdatumet för aktiviteten är senare än projektets Planerat slutförandedatum ändras projektets planerade slutförandedatum så att det matchar slutvillkorsdatumet för aktiviteten.

      * När målprojektet är schemalagt från slutförande:

         * När begränsningsdatumet för aktiviteten är senare än Project Completion Date, ändras aktivitetsbegränsningen till As Late As Possible.
         * När villkorsdatumet för aktiviteten är tidigare än det planerade startdatumet för projektet ändras projektets planerade startdatum så att det matchar startvillkorsdatumet för aktiviteten.

      * Oavsett schemat för projektet, när villkorsdatumet för aktiviteten ligger inom projektets start- och slutförandedatum, finns det inga ändringar i aktivitetsbegränsningen eller projektdatumen.

  Mer information om att flytta uppgifter finns i [Flytta uppgifter](../../../manage-work/tasks/manage-tasks/move-tasks.md). Mer information om att kopiera uppgifter finns i [Kopiera och duplicera uppgifter](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Mer information om hur du uppdaterar aktivitetsbegränsningen för en aktivitet finns i [Uppdatera aktivitetsbegränsningen för en aktivitet](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Must Start On Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Must Start On:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Must Start On</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>The task must start by this date, and no later than this date.</p> </li>
<li value="6">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

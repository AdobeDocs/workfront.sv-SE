---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Aktivitetsbegränsningsöversikt: Måste avslutas den'
description: Du kan använda uppgiftsbegränsningen Måste vara klar (MFO) för att schemalägga att en uppgift avslutas ett visst datum.
author: Alina
feature: Work Management
exl-id: 9e546a0f-7f7a-4f1c-9d9d-aa3cea377fdf
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Översikt över aktivitetsbegränsning: Måste avslutas

Du kan använda uppgiftsbegränsningen Måste vara klar (MFO) för att schemalägga att en uppgift avslutas ett visst datum.

Begränsningen Måste avslutas den schemalägger en aktivitet att avslutas exakt vid den tidpunkt och det datum som du anger i fältet **Planerat slutförandedatum**.

>[!TIP]
>
>Om du uppdaterar en uppgifts planerade slutförandedatum manuellt ändras aktivitetens begränsning till Måste avslutas den.

## Översikt över Måste avslutas vid aktivitetsbegränsning

Tänk på följande när du schemalägger en aktivitet med villkoret Måste sluta den:

* Föregående relationer tvingar inte aktiviteten att schemaläggas om. Adobe Workfront ignorerar i stort sett föregående relationer.
* Aktiviteten visas som **Vid risk** om föregående aktiviteter börjar köras efter eller är sena.

* När du flyttar eller kopierar en uppgift med en MFO-begränsning till ett annat projekt kan begränsningen för aktiviteten eller datumen i projektet ändras beroende på vilka villkorsdatumen är och vilka datum projektet börjar och slutförs. Följande scenarier finns:

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
<h2>Use the Must Finish On Task Constraint</h2>
<p>To update the Task Constraint to Must Finish On:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Must Finish On</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete by this date, and no later than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Översikt över aktivitetsbegränsning: Starta inte senare än'
description: Starta tidigast (SNLT) är en aktivitetsbegränsning som schemalägger en aktivitet att starta före det datum du anger.
author: Alina
feature: Work Management
exl-id: 86139ce6-c6b1-4ac4-a5cb-fd4aa899a025
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# Översikt över uppgiftsbegränsning: Starta inte senare än

Starta tidigast (SNLT) är en aktivitetsbegränsning som schemalägger en aktivitet att starta före det datum du anger.

Tänk på följande när du arbetar med SNLT-begränsningen:

* Du bör använda begränsningen Starta senast när projektet är schemalagt från fullständigt datum. I det här fallet kan du ange en mjuk begränsning för en aktivitet innan den tvingar andra beroende uppgifter att visas som Risksumma.
* Starta tidigast är standardbegränsningen om ett projekt använder schemaläggningsläget Schemalägg från slutförandedatum och system- eller gruppstandardvärdet för startdatumet för en aktivitet är Idag. Mer information om var du ska ange standardbegränsning för en ny uppgift finns i [Konfigurera inställningar för uppgifter och problem i hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* När du använder SNLT-begränsningen med ett Schedule From Start Date-projekt schemalägger Adobe Workfront aktiviteten på samma sätt som en Så snart som möjligt-åtgärd.
* När du flyttar eller kopierar en uppgift med en SNLT-begränsning till ett annat projekt kan villkoret för aktiviteten eller datumen i projektet ändras beroende på vilka villkorsdatumen är och vilka datum projektet börjar och slutförs. Följande scenarier finns:

   * När målprojektet är schemalagt från start:

      * När villkorsdatumet för aktiviteten är tidigare än projektets planerade startdatum, ändras aktivitetsbegränsningen till Så snart som möjligt.
      * När begränsningsdatumet för aktiviteten är senare än projektets Planerat slutförandedatum ändras projektets planerade slutförandedatum så att det matchar slutvillkorsdatumet för aktiviteten.

      * När målprojektet är schemalagt från slutförande:

         * När begränsningsdatumet för aktiviteten är senare än Project Completion Date ändras aktivitetsbegränsningen till As Late As Possible.
         * När villkorsdatumet för aktiviteten är tidigare än det planerade startdatumet för projektet ändras projektets planerade startdatum så att det matchar startvillkorsdatumet för aktiviteten.
      * Oavsett schemat för projektet, när villkorsdatumet för aktiviteten ligger inom projektets start- och slutförandedatum, finns det inga ändringar i aktivitetsbegränsningen eller projektdatumen.

   Mer information om hur du flyttar uppgifter finns i [Flytta uppgifter](../../../manage-work/tasks/manage-tasks/move-tasks.md).

   Mer information om att kopiera uppgifter finns i [Kopiera och duplicera uppgifter](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Mer information om hur du uppdaterar aktivitetsbegränsningen för en uppgift finns i [Uppdatera uppgiftsbegränsningen för en uppgift](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Start No Later Than Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Start No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Start No Later Than</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>This is the date by which the task must start, and not later than this date.</p> </li>
<li value="6">Click <strong>Save Changes</strong>.<br></li>
</ol>
</div>
-->

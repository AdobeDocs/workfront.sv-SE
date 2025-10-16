---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Översikt över aktivitetsbegränsning: Start tidigast'
description: Använd åtgärdsbegränsningen Starta tidigast (SNET) om du vill schemalägga en aktivitet som ska starta efter det datum du anger.
author: Alina
feature: Work Management
exl-id: 857859fb-87ee-4397-b292-239ed9dc8281
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Översikt över aktivitetsbegränsning: Starta tidigast

Använd åtgärdsbegränsningen Starta tidigast (SNET) om du vill schemalägga en aktivitet som ska starta efter det datum du anger.

## Översikt över startdatum tidigast än aktivitetsbegränsning

Tänk på följande när du använder villkoret Start Nej tidigare än Aktivitetsbegränsning:

* Du bör använda begränsningen Starta tidigast när projektet är schemalagt från startdatum. I det här fallet kan du ange en mjuk begränsning för en aktivitet innan den tvingar andra beroende uppgifter att visas som Risksumma.
* Start No Earlier Than är standardbegränsningen om ett projekt är schemalagt från startdatum och om systemets eller gruppens standardstartdatum för en ny aktivitet är inställt på Today. Mer information om hur du konfigurerar standardinställningar för uppgifter finns i [Konfigurera uppgifter och inställningar för problem i hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Om du schemalägger projektet Från startdatum och systemets standardstartdatum för en ny uppgift anges till Baserat på projektplanerat datum, är standardbegränsningen för en ny uppgift Så snart som möjligt.
* Om du schemalägger projektet Från slutförandedatum och systemets standardstartdatum för en ny uppgift är inställt på I, schemaläggs aktiviteten som om den vore en så sen som möjligt-uppgift med villkoret Start No Tidigare Than.
* När du flyttar eller kopierar en uppgift med en SNET-begränsning till ett annat projekt, kan begränsningarna för aktiviteten eller datumen i projektet ändras beroende på vilka villkorsdatumen är och vilka datum projektet börjar och slutförs. Följande scenarier finns:

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
<h2>Use the Start No Earlier Than Task Constraint</h2>
<p>(NOTE:&nbsp;replaced with new article linked above)&nbsp;</p>
<p>To update the Task Constraint to Start No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Start No Earlier Than</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>This is the date by which the task must start, and not earlier than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

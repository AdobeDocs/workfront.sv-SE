---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Översikt över begränsning av aktivitet: så snart som möjligt'
description: Så snart som möjligt är en aktivitetsbegränsning som placerar starttiden för aktiviteten så nära början som möjligt av projektet.
author: Alina
feature: Work Management
exl-id: 9cb232fe-bc74-4433-afac-88be69514c88
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Översikt över uppgiftsbegränsning: Så snart som möjligt

Så snart som möjligt är en aktivitetsbegränsning som placerar starttiden för aktiviteten så nära början som möjligt av projektet.

## Att tänka på när du använder villkoret Så snart som möjligt

* Så snart som möjligt är standardbegränsningen om ett projekt använder schemaläggningsläget Schemalägg från startdatum och om systemets standardstartdatum för en ny aktivitet anges till Baserat på projektets planerade datum.

* Om ett projekt använder schemaläggningsläget Schemalägg från startdatum och om systemets eller gruppens standardstartdatum för en ny uppgift är inställt på I, är standardaktivitetsbegränsningen Start No Earlier Than.

  Mer information om var du ska ange standardbegränsning för en ny uppgift finns i [Konfigurera systemomfattande uppgifter och inställningar för problem](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Mer information om hur du uppdaterar aktivitetsbegränsningen för en aktivitet finns i [Uppdatera aktivitetsbegränsningen för en aktivitet](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Soon As Possible: </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>As Soon As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## Skillnaden mellan tidigaste tillgängliga tid och så snart som möjligt

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"]) </p>
-->

Begränsningen Tidigaste tillgängliga tid skiljer sig från villkoret Så snart som möjligt när alla följande villkor är uppfyllda:

* Projektet är schemalagt från slutförande.
* Aktiviteter i projektet har en föregående relation.
* Föregående aktivitet har en flexibel aktivitetsbegränsning.

I den här situationen:

* **Tidigaste tillgängliga tid:** Om du använder den tidigaste tillgängliga tidsbegränsningen för efterföljande aktivitet prioriteras föregående åtgärds flexibla begränsning.

  Anta t.ex. att Aktivitet A är en föregångare till Aktivitet B. Aktivitet B har tidsbegränsningen Tidigast tillgänglig och Aktivitet A har villkoret SENT som möjligt. I sådana fall är uppgiften schemalagd så nära att projektet har slutförts som möjligt.

* **Så snart som möjligt:** I det här scenariot ger begränsningen Så snart som möjligt för efterföljande aktivitet prioriteten för efterföljande aktivitet.

  Anta till exempel att Aktivitet A är en föregångare till Aktivitet B. Aktivitet B har begränsningen Så snart som möjligt och Aktivitet A har begränsningen Så sent som möjligt. I så fall är aktiviteten schemalagd så nära början som möjligt av projektet.

---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Aktivitetsbegränsning - översikt: Så sent som möjligt'
description: ALAP (Late As Possible) är en Adobe Workfront-aktivitetsbegränsning som gör att slutföringstiden för uppgiften ligger så nära projektets slut som möjligt.
author: Alina
feature: Work Management
exl-id: 475427d0-020b-4851-a614-c9931659e07d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%

---

# Översikt över aktivitetsbegränsning: Så sent som möjligt

ALAP (Late As Possible) är en Adobe Workfront-aktivitetsbegränsning som gör att slutföringstiden för uppgiften ligger så nära projektets slut som möjligt.

Om du använder den här begränsningen kan föregående eller beroende aktiviteter schemaläggas om.

Mer information om föregående relationer finns i [Använda föregående aktiviteter](../../../manage-work/tasks/use-prdcssrs/use-task-predecessors.md).

Så sent som möjligt är standardbegränsningen om ett projekt använder schemaläggningsläget Schemalägg från slutförandedatum och system- eller gruppstandardvärdet för startdatumet för en aktivitet baseras på projektplanerat datum.

Mer information om var du ska ange standardbegränsning för en ny uppgift finns i [Konfigurera systemomfattande uppgifter och inställningar för problem](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Mer information om hur du uppdaterar aktivitetsbegränsningen för en aktivitet finns i [Uppdatera aktivitetsbegränsningen för en aktivitet](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the As Late As Possible Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Late As Possible:&nbsp;</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click&nbsp;<strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the&nbsp;<strong>Overview</strong>&nbsp;section, expand the&nbsp;<strong>Task Constraint</strong>&nbsp;drop-down menu.</p> </li>
<li value="4"> <p>Select&nbsp;<strong>As Late As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>.&nbsp;</li>
</ol>
</div>
-->

## Skillnaden mellan den senaste tillgängliga tiden och så sen som möjligt

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;[! This section is duplicated in "Latest Available Time"] - inserted a snippet for both articles (Alina)) </p>
-->

Begränsningen Senaste tillgängliga tid skiljer sig från begränsningen som Sate As Possible när följande kriterier finns:

* Projektet är schemalagt från startdatum
* Aktiviteter i projektet har en föregående relation
* Efterföljande aktivitet har en flexibel uppgiftsbegränsning

I den här situationen:

* **Senaste tillgängliga tid:** Om du använder den senaste tillgängliga tidsbegränsningen för föregående aktivitet prioriteras den efterföljande aktivitetens flexibla begränsning.

  **Exempel:** Till exempel är Aktivitet A en föregångare till Aktivitet B. Aktivitet A har den senaste tillgängliga tidsbegränsningen och aktivitet B har begränsningen Per så snart som möjligt. I så fall är uppgift A schemalagd så nära projektets början som möjligt.

  ![](assets/latest-available-time-task-constraint-in-task-list-350x116.png)

* **Så här sent som möjligt:** I det här scenariot prioriterar föregående aktivitet med begränsningen Så sent som möjligt för föregående aktivitet.

  **Exempel:** Till exempel är Aktivitet A en föregångare till Aktivitet B. Aktivitet A har begränsningen Så sent som möjligt och aktivitet B har begränsningen Så snart som möjligt. I så fall är uppgift A schemalagd så nära projektets slut som möjligt.

  ![](assets/as-late-as-possible-task-constraint-in-task-list-350x104.png)

 

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: this content was here before but it was wrong - according to this issue in Hub, per Dev, the correct functionality is in the snippet above: https://hub.workfront.com/task/6193c6910004bce9de07cda7757f3ce8/updates?email-source=subscribedCommunication) </p>
<p>The Latest&nbsp;Available Time constraint differs from the As Late&nbsp;As Possible constraint when the following criteria exist:</p>
<ul>
<li> The project is scheduled From Completion </li>
<li> Tasks in the project have a predecessor relationship </li>
<li> The predecessor task has a flexible task constraint </li>
</ul>
<p> In this situation: </p>
<ul>
<li> <p><strong>Latest Available Time:</strong> Using the Latest&nbsp;Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest&nbsp;Available Time constraint and Task A has the As Soon&nbsp;As Possible constraint. In this situation, the task is scheduled as close&nbsp;to the start&nbsp;of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late&nbsp;As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late&nbsp;As Possible&nbsp;constraint and Task A has the As Soon&nbsp;As Possible constraint. In this situation, the task is scheduled as close to the end&nbsp;of the project as possible.</p> </li>
</ul>
</div>
-->

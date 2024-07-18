---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Översikt över aktivitetsbegränsning: Tidigast tillgänglig tid'
description: Tidigaste tillgängliga tid är en aktivitetsbegränsning som schemalägger att en uppgift påbörjas så snart som möjligt efter att ha övervägt eventuella föregående relationer.
author: Alina
feature: Work Management
exl-id: 9c01e4bd-c6ca-4540-a0f1-ecdd44df84e0
source-git-commit: 18f26f976a47af003817f2f82f8550bdfbc0ab90
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# Översikt över uppgiftsbegränsning: Tidigast tillgänglig tid

Tidigaste tillgängliga tid är en aktivitetsbegränsning som schemalägger att en uppgift påbörjas så snart som möjligt efter att ha övervägt eventuella föregående relationer.

Mer information om hur du uppdaterar aktivitetsbegränsningen för en aktivitet finns i [Uppdatera aktivitetsbegränsningen för en aktivitet](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above) </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To update the Task Constraint to Earliest Available Time:</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Go to a task whose constraint you want to modify. </li>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Edit Task</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Select <strong>Earliest Available Time</strong>.</p>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save Changes</strong>.</li>
   -->

## Skillnaden mellan tidigaste tillgängliga tid och så snart som möjligt

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])</p>
-->

Begränsningen Tidigaste tillgängliga tid skiljer sig från villkoret Så snart som möjligt när alla följande villkor är uppfyllda:

* Projektet är schemalagt från slutförande
* Aktiviteter i projektet har en föregående relation
* Föregående aktivitet har en flexibel aktivitetsbegränsning

I den här situationen:

* **Tidigaste tillgängliga tid:** Om du använder den tidigaste tillgängliga tidsbegränsningen för efterföljande aktivitet prioriteras föregående åtgärds flexibla begränsning.

  **EXEMPEL**

  Aktivitet A är en föregångare till aktivitet B. Aktivitet B har den tidigaste tillgängliga tidsbegränsningen och aktivitet A har begränsningen Så sent som möjligt. I sådana fall är uppdrag B schemalagt så nära att projektet har slutförts som möjligt.

  ![Tidigaste tillgängliga tidsbegränsning när aktiviteten har datum nära projektets slutförandedatum](assets/earliest-available-constraint-dates-closer-to-project-completion-350x137.png)

* **Så snart som möjligt:** I det här scenariot ger begränsningen Så snart som möjligt för efterföljande aktivitet prioriteten för efterföljande aktivitet.

  **EXEMPEL**

  Aktivitet A är en föregångare till Aktivitet B. Aktivitet B har begränsningen Så snart som möjligt och Aktivitet A har begränsningen Så sent som möjligt. I så fall är uppgift B schemalagd så nära projektets början som möjligt.

  ![Som möjligt så snart som möjligt när aktiviteten har datum nära projektets startdatum](assets/as-soon-as-possible-dates-closer-to-project-start-350x126.png)

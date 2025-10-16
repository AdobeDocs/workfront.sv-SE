---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Översikt över aktivitetens ursprungliga varaktighet och ursprungliga planerade timmar
description: Som en del av planeringen av ett projekt bör du fastställa värdena för Planerade timmar och Varaktighet (eller Planerad varaktighet) för varje aktivitet i projektet.
author: Alina
feature: Work Management
exl-id: 96d77d9f-3d5f-457e-a4ad-10edc371a991
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# Översikt över aktivitetens ursprungliga varaktighet och ursprungliga planerade timmar

Som en del av planeringen av ett projekt bör du fastställa värdena för Planerade timmar och Varaktighet (eller Planerad varaktighet) för varje aktivitet i projektet.

Mer information om planerade timmar för uppgifter finns i [Översikt över planerade timmar](../../../manage-work/tasks/task-information/planned-hours.md).

Mer information om aktivitetens varaktighet finns i [Översikt över aktivitetens varaktighet och varaktighetstyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Du kan se dessa värden på fliken Uppgiftsinformation eller när du redigerar en uppgift.

Om du skapar en vy för en uppgiftslista eller en aktivitetsrapport kan du även se fälten Original Planned Hours och Original Duration för aktiviteterna.

## Ursprungliga planerade timmar

De ursprungliga planerade timmarna för en aktivitet representerar antalet planerade timmar som en aktivitet ursprungligen hade innan den blev en överordnad aktivitet. När en aktivitet blir en överordnad aktivitet, sammanställs de underordnade aktiviteternas planerade timmar till den överordnade uppgiften för att ange den överordnade uppgiftens planerade timmar.

När du visar fältet Ursprungligt antal planerade timmar i en aktivitetsrapport eller lista kan du se det ursprungliga antalet planerade timmar innan aktiviteten ärver antalet planerade timmar för dess underordnade.

>[!NOTE]
>
>När du skapar en uppgift är antalet ursprungliga planerade timmar noll. Om aktiviteten blir en överordnad uppgift fylls värdet för det här fältet i med antalet planerade timmar för aktiviteten innan den ändrades till en överordnad. Det här värdet finns kvar i det här fältet även när aktiviteten återgår till att vara en fristående uppgift.

## Ursprunglig varaktighet

Ursprunglig varaktighet för en aktivitet är den varaktighet en aktivitet hade innan den blev en överordnad aktivitet, i minuter. När en aktivitet blir överordnad, kommer varaktigheten mellan det planerade startdatumet för den tidigaste underordnade och det planerade slutförandedatumet för den senaste underordnade aktiviteten att räknas upp till den överordnade aktiviteten och bli varaktigheten för den överordnade aktiviteten. Detta ersätter varaktigheten för den ursprungliga aktiviteten.

När du visar fältet Ursprunglig varaktighet i en aktivitetsrapport eller -lista kan du se det ursprungliga antalet dagar för aktivitetens varaktighet innan den ärver varaktigheten för dess underordnade.

>[!NOTE]
>
>När du skapar en uppgift är den ursprungliga varaktigheten noll. Om aktiviteten blir en överordnad uppgift fylls värdet för det här fältet i med varaktigheten för aktiviteten innan den ändrades till en överordnad. Det här värdet finns kvar i det här fältet även när aktiviteten återgår till att vara en fristående uppgift. Det här värdet visas på några minuter.

## Exempel

Om två uppgifter till exempel är fristående är deras ursprungliga varaktighet och ursprungliga planerade timmar noll.

![original_planning_hours_and_duration_without_parent.png](assets/original-planned-hours-and-duration-without-parent-350x38.png)

När den första aktiviteten blir överordnad den andra aktiviteten fylls fälten Ursprunglig varaktighet och Ursprunglig planerad timme i med värdena för Varaktighet och Planerad timme för aktiviteten innan den blev överordnad. Ursprunglig varaktighet visas i minuter. Längden och de planerade timmarna för barnet blir den överordnade personens varaktighet och planerade timmar.

![original_and_planning_hours_with_a_parent_task.png](assets/original-and-planned-hours-with-a-parent-task-350x38.png)

När den överordnade blir en fristående uppgift igen återställs varaktigheten och den planerade timmen till de ursprungliga värdena, medan den ursprungliga varaktigheten och de ursprungliga planerade timmarna förblir ifyllda. De återgår inte till noll.

![original_duration_and_planning_hours_after_reversal_of_a_parent.png](assets/original-duration-and-planned-hours-after-reversal-of-a-parent-350x39.png)

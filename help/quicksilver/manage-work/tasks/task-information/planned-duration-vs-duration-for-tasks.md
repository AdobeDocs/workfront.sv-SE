---
content-type: reference
product-area: projects
navigation-topic: task-information
title: Skillnad mellan planerad varaktighet och varaktighet för uppgifter
description: Varaktighet är tiden mellan planerad start och planerad slutförandedatum för en arbetsuppgift. Aktiviteter har en varaktighet och en planerad varaktighet i Adobe Workfront, beroende på aktivitetens varaktighetstyp.
author: Alina
feature: Work Management
exl-id: 183a3334-b4af-4f45-8e72-9e82ff3862a0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Skillnad mellan planerad varaktighet och varaktighet för uppgifter

Varaktighet är tiden mellan planerad start och planerad slutförandedatum för en arbetsuppgift. Aktiviteter har en varaktighet och en planerad varaktighet i Adobe Workfront, beroende på aktivitetens varaktighetstyp.

Problem och projekt kan inte associeras med en varaktighetstyp och har bara en Varaktighet.

## Aktivitetsvaraktighet

För uppgifter visas vanligtvis samma värde för Varaktighet och Planerad varaktighet: Tidslängden mellan det planerade startdatumet och det planerade slutförandedatumet för en aktivitet.

När varaktighetstypen för aktiviteten är Ansträngningsstyrd minskar den planerade varaktigheten när du lägger till resurser till aktiviteten.

**Exempel:** Om en aktivitet med varaktighetstypen styrd av insats har en varaktighet på 3 dagar och du tilldelar en resurs med ett heltidsschema till aktiviteten, är den planerade varaktigheten också 3 dagar.

Om du tilldelar tre resurser med ett heltidsschema till samma uppgift stannar varaktigheten 3 dagar, men den planerade varaktigheten blir 1 dag. Den planerade varaktigheten ändrar också datum för planerad start och planerad slutförande för aktiviteten, så att den återspeglar den nya planerade varaktigheten. Därför påverkas även tidslinjen i projektet.
Du kan använda den aktivitetsstyrda varaktighetstypen när du tilldelar en uppgift till flera resurser. Detta minskar tiden det tar för uppgiften att slutföras.

Mer information om aktivitetsstyrd varaktighetstyp finns i [Översikt över varaktighetstyp: Ansträngningsstyrd](../../../manage-work/tasks/taskdurtn/effort-driven.md).

## Problem och projektvaraktighet

Problem och projekt har bara ett varaktighetsvärde, vilket är skillnaden mellan det planerade startdatumet och det planerade slutförandedatumet för utgåvan respektive projektet.

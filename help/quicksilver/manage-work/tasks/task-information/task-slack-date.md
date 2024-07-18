---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Aktivitet, Slack - översikt
description: Uppgifter kan ibland börja och slutföras sent utan att det påverkar projektets slutförandedatum.
author: Alina
feature: Work Management
exl-id: ccdaa27d-e212-45dc-afca-08539f2b4001
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# Aktivitet, Slack - översikt

Uppgifter kan ibland börja och slutföras sent utan att det påverkar projektets slutförandedatum.

I Slack-datumet visas det exakta datumet när en åtgärd definitivt kan påverka projektets slutförandedatum.

## Slack - översikt

Slack-datumet skiljer sig från det planerade slutförandedatumet eftersom föregående relationer och aktivitetsbegränsningar ökar svarstiden.

Tänk på följande scenarier, beroende på om en åtgärd är den kritiska sökvägen för ett projekt eller inte:

* För uppgifter som finns på projektets kritiska sökväg eller som har efterföljande aktiviteter på den kritiska sökvägen, matchar Slack-datumet uppgiftens beräknade slutförandedatum såvida inte aktivitetens förloppsstatus redan är sen eller ligger bakom.

  Mer information om den kritiska sökvägen finns i [Översikt över projektets kritiska sökväg](../../../manage-work/tasks/manage-tasks/critical-path.md).

  Mer information om aktiviteternas förloppsstatus finns i [Översikt över status för aktivitetsstatus](../../../manage-work/tasks/task-information/task-progress-status.md).

* För uppgifter som inte finns på den kritiska sökvägen ökar den korta tiden tiden den tid som aktiviteten schemaläggs. För dessa uppgifter ligger Slack-datumet kvar i framtiden tills uppgifterna blir så sena att de börjar påverka projektets slutförandedatum.

## Leta reda på Slack för en uppgift

Om du vill visa Slack datum för en uppgift kan du lägga till fältet Slack datum i en uppgiftsvy eller rapport.

Mer information om hur du skapar en rapport finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

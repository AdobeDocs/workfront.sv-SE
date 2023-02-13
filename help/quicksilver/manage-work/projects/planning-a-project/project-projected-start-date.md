---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Översikt över projektets planerade startdatum
description: Det planerade startdatumet är ett realtidsdatum som anger när projektet ska starta baserat på det planerade startdatumet för den första aktiviteten i projektet.
author: Alina
feature: Work Management
exl-id: 6277e6cf-0a73-4ba8-a3fd-c0da473dc5d4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Översikt över projektets planerade startdatum

## Översikt över det planerade startdatumet för projekt och aktiviteter

Det planerade startdatumet är ett realtidsdatum som anger när projektet ska starta baserat på det planerade startdatumet för den första aktiviteten i projektet. 

När du först planerar ett projekt är det planerade startdatumet och det planerade startdatumet för aktiviteterna och projektet identiska. Eftersom förseningar kan inträffa eller uppgifter kan slutföras tidigare kan det planerade startdatumet skilja sig från det planerade startdatumet. 

Ändringar i det planerade startdatumet för den första aktiviteten i projektet utlöser ändringar i projektets planerade startdatum. 

## Ändra det planerade startdatumet för en aktivitet

Det planerade startdatumet för ett projekt eller en uppgift är en beräkning som gjorts av Adobe Workfront och kan inte ändras manuellt. 

Följande händelser kan utlösa en ändring i det planerade startdatumet för en aktivitet:

* När du börjar arbeta med en uppgift blir aktivitetens faktiska startdatum dess planerade startdatum.
* Om det planerade startdatumet för en aktivitet godkänns, flyttas det planerade startdatumet in i framtiden, vilket anger det senaste datumet som aktiviteten kan starta.\
   Workfront tar hänsyn till antalet planerade timmar för aktiviteten, liksom schemat för projektet eller för användaren som är tilldelad uppgiften vid beräkning av det tidigaste tillgängliga datumet för aktivitetens start. 
* Föregående aktiviteter som körs bakom påverkar det planerade startdatumet för de beroende aktiviteterna. Det planerade startdatumet för de beroende aktiviteterna flyttas enligt beroendetypen för föregående relation och enligt prognosdatumen för föregående aktiviteter. 

Om någon av dessa uppgifter är den första aktiviteten i ett projekt ändras projektets planerade startdatum så att det matchar det planerade startdatumet för den här aktiviteten. 

## Leta rätt på det planerade startdatumet för ett projekt eller en uppgift

Du kan hitta det planerade startdatumet för ett projekt eller en uppgift i följande områden i Workfront:

* Du kan lägga till den i ett projekt eller i en uppgiftsrapport eller vy.

   Mer information om hur du skapar en rapport finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* I avsnittet Projektinformation för ett projekt eller i avsnittet Uppgiftsinformation för en uppgift.

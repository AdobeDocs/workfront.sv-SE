---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: Översikt över uppgiftsbegränsning
description: Uppgiftsbegränsningar avgör när en uppgift ska starta och avslutas i ett projekt.
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# Översikt över uppgiftsbegränsning

Uppgiftsbegränsningar avgör när en uppgift ska starta och avslutas i ett projekt.

## Översikt över uppgiftsbegränsningar

När du bygger din projektplan fattar du beslut om i vilken ordning och inom vilken tidsram dina uppgifter ska utföras i projektet. Uppgifter kan fungera oberoende av aktivitetssekvenser, men de kan påverka projekttidslinjen. Med aktivitetsbegränsningar kan en projektledare planera när vissa uppgifter kan starta eller slutföras i ett projekt.

Beroende på vilken begränsning du använder kan du behöva ange ett planerat startdatum, ett planerat slutförandedatum eller båda för aktiviteten.

Begränsningstyper som kräver definierade datum påverkar föregående relationer.

>[!TIP]
>
>Du bör använda en begränsningstyp som inte kräver specifika datum om du använder föregående relationer mellan uppgifter.

I följande tabell visas varje begränsning och dess förkortning. Förkortningar används i uppgiftslistor och när du skapar importfiler med Snabbstart. Klicka på den länkade titeln för varje uppgiftsbegränsning om du vill ha mer information om den typen av begränsning.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Begränsningsnamn</strong> </p> </th> 
   <th> <p><strong>Förkortning</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref">Översikt över uppgiftsbegränsning: Så snart som möjligt</a> </p> </td> 
   <td scope="col"> <p>ASAP</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">Översikt över uppgiftsbegränsning: Så sent som möjligt </a> </p> </td> 
   <td scope="col"> <p>ALAP</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">Översikt över uppgiftsbegränsning: Tidigaste tillgängliga tid</a> </p> </td> 
   <td scope="col"> <p>ÄT</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">Översikt över uppgiftsbegränsning: Senaste tillgängliga tid</a> </p> </td> 
   <td scope="col"> <p>LAT</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">Översikt över uppgiftsbegränsning: Starta tidigast</a> </p> </td> 
   <td scope="col"> <p>SNET</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">Översikt över uppgiftsbegränsning: Starta inte senare än</a> </p> </td> 
   <td scope="col"> <p>SNLT</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">Översikt över uppgiftsbegränsning: Avsluta tidigast</a> </p> </td> 
   <td scope="col"> <p>FNET</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">Översikt över uppgiftsbegränsning: Avsluta senast</a> </p> </td> 
   <td scope="col"> <p>FNLT</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">Översikt över uppgiftsbegränsning: Måste börja på</a> </p> </td> 
   <td scope="col"> <p>MSO</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">Översikt över uppgiftsbegränsning: Måste avslutas</a> </p> </td> 
   <td scope="col"> <p>MFO</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">Översikt över uppgiftsbegränsning: Fasta datum</a> </p> </td> 
   <td> <p>FEM</p> </td> 
  </tr> 
 </tbody> 
</table>

## Översikt över standardbegränsningar

När du skapar nya uppgifter väljs en uppgiftsbegränsning automatiskt av Workfront.

Workfront använder två variabler för att bestämma vilken uppgiftsbegränsning som är vald som standard för en ny uppgift:

* The **Projektschema från** -fält i projektet.

   Mer information om fältet Projektschema från finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

* The **Startdatum** inställningarna konfigurerade av din Workfront- eller gruppadministratör i **Uppgifter och problem** område på **Inställningar**.

   Mer information om inställningar för uppgifter och problem finns i avsnittet Nya aktivitetsstandarder i [Konfigurera inställningar för uppgifter och problem i hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

I följande tabell visas standardåtgärdsbegränsningen när du väljer olika variabler för ditt projekt och dina nya uppgifter:

| Projektschema från | Startdatum för uppgift | Standard för aktivitetsbegränsning |
|---|---|---|
| Startdatum | Baserat på planerat projektdatum | Så snart som möjligt |
| Startdatum | Idag | Starta tidigast |
| Slutförandedatum | Baserat på planerat projektdatum | Så sent som möjligt |
| Slutförandedatum | Idag | Starta inte senare än |

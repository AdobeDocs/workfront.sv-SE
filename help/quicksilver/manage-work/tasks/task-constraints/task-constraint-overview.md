---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: Översikt över begränsning av aktivitet
description: Uppgiftsbegränsningar avgör när en uppgift ska starta och avslutas i ett projekt.
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 0%

---

# Översikt över uppgiftsbegränsning

<!-- Audited: 12/2023 -->

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
 <col>
 <thead> 
  <tr> 
   <th> <p><strong>Begränsningsnamn</strong> </p> </th> 
   <th> <p><strong>Förkortning</strong> </p> </th> 
   <th> <p><strong>Beskrivning</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref">Översikt över aktivitetsbegränsning: Så snart som möjligt</a> </p> </td> 
   <td scope="col"> <p>ASAP</p> </td>
   <td scope="col"> <p>Placerar starttiden för aktiviteten så nära början som möjligt.</p> 
   <p>Det är standardvillkoret om schemaläge från startdatum används i projektet och om systemets standardstartdatum för en ny uppgift anges till Baserat på projektplanerat datum. </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">Översikt över aktivitetsbegränsning: Så sent som möjligt </a> </p> </td> 
   <td scope="col"> <p>ALAP</p> </td> 
   <td scope="col"> <p>Placerar sluttiden för aktiviteten så nära projektets slut som möjligt.</p> 
   <p>Det här är standardbegränsningen när projektschemaläge är från slutförandedatum och systemets eller gruppens standardvärde för startdatumet för en uppgift är Baserat på projektets planerade datum. </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">Översikt över aktivitetsbegränsning: Tidigast tillgänglig tid</a> </p> </td> 
   <td scope="col"> <p>ÄT</p> </td> 
 <td scope="col"> <p>Schemalägger en aktivitet att börja så snart som möjligt efter att eventuella föregående relationer har beaktats.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">Översikt över aktivitetsbegränsning: Senaste tillgängliga tid</a> </p> </td> 
   <td scope="col"> <p>LAT</p> </td> 
   <td scope="col"> <p>Schemalägger en uppgift att börja senast tillgängliga efter att ha övervägt relationer mellan föregående och efterföljande i projektet.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">Översikt över aktivitetsbegränsning: Starta tidigast </a> </p> </td> 
   <td scope="col"> <p>SNET</p> </td> 
   <td scope="col"> <p>Schemalägger en aktivitet att starta efter det datum du anger.</p> 
   <p>Detta är standardvillkoret om projektets schemaläge är från startdatum och om systemets eller gruppens standardstartdatum för en ny uppgift är inställt på Idag.   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">Översikt över aktivitetsbegränsning: Starta inte senare än </a> </p> </td> 
   <td scope="col"> <p>SNLT</p> </td> 
   <td scope="col"> <p>Schemalägger en uppgift att starta före det datum du anger.</p> 
   <p>Det här är standardbegränsningen om projektschemaläge är från Slutförandedatum och om systemet eller gruppen som standard för Startdatum för en uppgift är inställd på I dag. 
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">Översikt över aktivitetsbegränsning: Slutför inte tidigare än </a> </p> </td> 
   <td scope="col"> <p>FNET</p> </td>
   <td scope="col"> <p>Schemalägger en aktivitet som ska slutföras efter det datum du anger.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">Översikt över aktivitetsbegränsning: Slutför inte senare än </a> </p> </td> 
   <td scope="col"> <p>FNLT</p> </td> 
   <td scope="col"> <p>Schemalägger en aktivitet som ska slutföras före det datum du anger.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">Översikt över aktivitetsbegränsning: Måste starta den</a> </p> </td> 
   <td scope="col"> <p>MSO</p> </td> 
   <td scope="col"> <p>Schemalägger en aktivitet att starta exakt på ett visst datum.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">Översikt över aktivitetsbegränsning: Måste avslutas </a> </p> </td> 
   <td scope="col"> <p>MFO</p> </td> 
   <td scope="col"> <p>Schemalägger en aktivitet som ska avslutas ett visst datum.</p> </td>
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">Översikt över aktivitetsbegränsning: Fasta datum</a> </p> </td> 
   <td> <p>FEM</p> </td> 
   <td> <p>Schemalägger en aktivitet att starta och sluta vid specifika datum.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Översikt över standardbegränsningar

När du skapar nya uppgifter väljs en uppgiftsbegränsning automatiskt av Workfront.

I Workfront används två variabler för att bestämma vilken uppgiftsbegränsning som är vald som standard för en ny uppgift:

* Fältet **Projektschema från** i projektet.

  Mer information om fältet Projektschema från finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

* Inställningen **Startdatum** som konfigureras av Workfront- eller gruppadministratören i området **Åtgärder och problem** i **installationsprogrammet**.

  Mer information om inställningar för uppgifter och problem finns i avsnittet [Nya standardinställningar för aktiviteter](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#new-task-defaults) i [Konfigurera systemomfattande inställningar för uppgifter och problem](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

I följande tabell visas standardåtgärdsbegränsningen när du väljer olika variabler för ditt projekt och dina nya uppgifter:

| Projektschema från | Startdatum för uppgift | Standard för aktivitetsbegränsning |
|---|---|---|
| Startdatum | Baserat på planerat projektdatum | Så snart som möjligt |
| Startdatum | Idag | Starta tidigast |
| Slutförandedatum | Baserat på planerat projektdatum | Så sent som möjligt |
| Slutförandedatum | Idag | Starta senast |

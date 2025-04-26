---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Översikt över fördröjningstyper
description: Lag är den tid som måste förflyta efter slutförandet av en framtvingad föregångare tills den beroende aktiviteten kan börja (Positive Lag), eller den tid som en beroende aktivitet kan starta innan den föregående startar (Negative Lag).
author: Alina
feature: Work Management
exl-id: 9b3cac9a-1b8d-4697-b5d4-a2d669c790a9
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1462'
ht-degree: 0%

---

# Översikt över fördröjningstyper

<!-- Audited: 01/2024 -->

Lag är den tid som måste förflyta efter det planerade slutförandet av en föregångare tills den beroende aktiviteten kan börja (Positive Lag), eller den tid som en beroende aktivitet kan starta innan den föregående startar (Negative Lag).

De planerade, planerade och beräknade datumen för efterföljande uppgifter beräknas med hänsyn till de föregående aktiviteternas fördröjning samt datum för planerade, planerade och beräknade start (slutförande).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planera </p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till uppgifter och projekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för aktiviteterna och projektet</p> </td> 
  </tr> 
 </tbody> 
</table>

*Mer information om informationen i den här tabellen finns i [Åtkomstkraven i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lag Types {#lag-types}

Ett exempel på en uppgift som skulle kräva en fördröjning kan vara att såga träd i lumber. Om det nyskurna träet måste torka under en tid innan det kan skäras upp, så blir det en fördröjning mellan att skära träden och såga upp dem i lummer.

I följande tabell visas Lag Types och hur du anger hur lång tid varje typ av tagg ska ha:

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>Värde</strong> </p> </td> 
   <td> <p><strong>Beskrivning</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Dagar (d eller de)</p> </td> 
   <td> <p>Fördröjningen mellan två uppgifter som är kopplade till beroendet mäts i arbetsdagar. Det här är standardtypen för fördröjning. </p> <p>Om det till exempel finns ett samband mellan avslutsstart med en 2-dagarsfördröjning och föregående aktivitet slutar på fredag, startar den beroende aktiviteten på onsdag. Helgdagarna räknas inte som en del av fördröjningen. </p> <p>Obs! Den maximala fördröjningsgränsen för dagar är 366.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Kalenderdagar (c eller ce)</p> </td> 
   <td> <p>Fördröjningen mellan två uppgifter mäts i kalenderdagar, inklusive helger och helger. </p> <p>Obs! Även om den här fördröjningstypen räknar lediga dagar som en del av fördröjningen, kan en beroende uppgift aldrig starta på en ledig dag. Om den här fördröjningstypen gör att den beroende aktiviteten startar på en ledig dag, schemaläggs det planerade startdatumet för den beroende aktiviteten till följande arbetsdag. </p> <p>Om det till exempel finns ett samband med avslutsstart med en 2-kalenderdagars fördröjning och föregående aktivitet slutar på torsdag, börjar den beroende aktiviteten på måndag i stället för söndag. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Procent (p eller pe)</p> </td> 
   <td> <p>Fördröjningen uttrycks som en procentandel av den beräknade tiden för att slutföra föregående aktivitet. </p> <p>Om det till exempel finns ett samband mellan avslutad start med 20 % fördröjning av en 10-dagars föregående aktivitet, beräknas hur många dagar som motsvarar 20 % av föregående uppgifts varaktighet och som fördröjning används. I så fall är det två dagar efter att uppgiften har slutförts. </p>

<p><b>ANMÄRKNING</b></p> Den maximala fördröjningsgränsen för procent är 2 000 %.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Veckodag (vi eller vi) </p> </td> 
   <td> <p>Fördröjningen mellan två uppgifter mäts genom att ange veckodagarna för veckan som innehåller det planerade slutförandedatumet för föregående aktivitet.</p> <p>För den här typen av Lag associeras varje veckodag med ett tal:</p> 
    <ul> 
     <li>söndag=1</li> 
     <li>Måndag=2</li> 
     <li>Tisdag=3</li> 
     <li>Onsdag=4</li> 
     <li>Torsdag=5</li> 
     <li>Fredag=6</li> 
     <li>Lördag=7</li> 
    </ul> <p>Om du vill ange att det planerade startdatumet för efterföljande ska infalla på en tisdag i den aktuella veckan, och tisdagen är före det planerade avslutsdatumet för föregående, ska du skriva följande formel för den efterföljande personen: </p> <p><code style="font-style: normal;">4fs-3w</code> </p>

<p><b>ANMÄRKNING</b></p>

Om det beräknade startdatumet för den efterföljande uppgiften är en viss tisdag och den dagen passerat för den aktuella veckan, är det planerade startdatumet för den efterföljande uppgiften samma dag (tisdag) i nästa vecka, om tillgängligt. </p> <p>Om du vill ange att fördröjningen ska infalla på en lördag i den aktuella veckan, och lördagen är efter det planerade slutförandedatumet för föregående, ska du skriva följande formel till den efterföljare du vill använda:</p> <p><code>4fs+7w</code> </p> <p>Om lördag är en ledig dag väljs nästa tillgängliga dag efter lördag (för att ange positiv fördröjning) som planerat startdatum för efterföljande dag. </p>

<p>Detta gäller inte schemaundantag. Om ett datum också är ett schemaundantag och startdatumet för efterföljande beräknas till den dagen, försöker systemet hitta det närmaste tillgängliga datumet som är den veckodag som anges i föregående uttryck.</p>

<p>Om till exempel startdatumet beräknas till en viss tisdag och den dagen är ett schemaundantag och föregående datum är positivt, väljer den följande tisdagen (om det även är en arbetsdag) som startdatum för efterföljande. Om fördröjningen är negativ väljer systemet föregående tisdag som startdatum.</p>

<p>Om du vill ange föregående eller kommande veckor kan du lägga till ett tal framför dagens nummer för lagtypen. </p> <p>Om du till exempel vill ange måndagen för 10 veckor sedan kan du använda den här koden för att ange föregående för din efterträdare:</p> <p><code>4fs-102w</code> </p> <p>10 betyder 10 veckor sedan och 2 är numret som tilldelats till måndag. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Veckodag icke-noll (k eller ke)</p> </td> 
   <td> <p>Fördröjningen mellan två uppgifter mäts identiskt med veckodag, förutom om föregående tid slutar på samma veckodag som anges. Fördröjningstiden beräknas sedan till intilliggande vecka (+/-). </p> <p>I det här fallet kan fördröjningen aldrig vara 0.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Negativ fördröjning

Du kan använda ett negativt värde, Lag, för att ange om aktiviteten behöver eller kan börja innan föregående aktivitet avslutas.

Tänk på följande regler när du använder negativ fördröjning:

* Med Negativ fördröjning kan inte start-/slutdatum för en aktivitet framtvingas före eller efter projektets planerade start-/slutdatum. Dessa datum anges i fältet Schemalägg från i projektet.

  I det här fallet bör du tänka på följande:

   * Schemalägg projektet från slutförandedatum.
   * Den sista aktiviteten i projektet ska använda alternativet Måste avslutas vid aktivitetsbegränsning. Vi rekommenderar att aktiviteten ges en tillräckligt lång varaktighet för att alla uppgifter i projektet ska kunna beaktas. De återstående uppgifterna fungerar bra med villkoret Så snart som möjligt.

* Ett felmeddelande kan visas om du använder en relation med en slutbehandlare med uppgifter.

  I det här fallet bör du tänka på följande:

   * Ange en relation mellan aktiviteter som föregås av Slutför/Slutför.
   * Varaktigheten för den efterföljande uppgiften bör vara lika med eller större än det planerade antalet fördröjningsdagar mellan uppgifterna.

## Ange typ av fördröjning och fördröjning för uppgifter

Du kan ange fördröjningstyper för uppgifter när du definierar deras föregångarrelationer.

### Ange typ av fördröjning i avsnittet Föregående aktiviteter i en uppgift {#indicate-lag-types-in-the-predecessors-section-of-a-task}

1. Gå till en uppgift som du vill definiera föregångaren och taggtypen för.
1. Klicka på **Föregående** i den vänstra panelen. Du kan behöva klicka på **Visa fler** och sedan på **Föregående**.
1. Klicka på **Lägg till föregående**.
1. (Valfritt) Om du vill lägga till en föregångare för flera projekt ersätter du namnet **Överordnat projekt** med ett annat projekt.
1. Börja skriva namnet på föregående aktivitet och markera den när den visas i listan.
1. Välj **Beroendetyp**.

   Mer information om föregående beroendetyper finns i [Översikt över aktivitetsberoendetyper](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Ange ett **Lag**-värde med ett numeriskt värde. Du kan ange negativa tal om du vill ange en negativ fördröjning.
1. Välj bland följande alternativ för att identifiera vilken typ av fördröjning du vill ange för föregående användare:

   * **Dagar**
   * **Kalenderdagar**
   * **Procent**
   * **Veckodag**
   * **Veckodag (inte noll)**

     Mer information om dessa Lag-typer och hur de beräknas finns i avsnittet [Lag Types](#lag-types) i den här artikeln.

1. Klicka på **Spara**.

### Ange typ av fördröjning i en uppgiftslista  {#indicate-lag-types-in-a-task-list}

1. Gå till en uppgiftslista och välj vyn **Standard**.

1. Klicka i kolumnen **Föregående** som motsvarar aktiviteten som du vill ange en föregångare och en fördröjning för.
1. Ange följande utan blanksteg:

   * numret på den uppgift som du vill ange som föregående för den valda uppgiften
   * förkortningen för den beroendetyp som du vill ange mellan aktiviteterna

     Mer information om förkortningarna för Beroendetyper finns i [Översikt över aktivitetsberoendetyper](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * antingen en **+** för positiv fördröjning eller en **-** för negativ fördröjning

   * mängden fördröjning
   * förkortningen för den Lag-typ som du vill använda

     Mer information om förkortningarna för Lag Types finns i avsnittet [Lag Types](#lag-types) i den här artikeln.

   Om du till exempel vill ange att en aktivitet har en föregångare och en positiv fördröjning på 2 dagar, anger du `1fs+2d` i kolumnen Föregående.

1. Tryck på Retur på tangentbordet för att spara ändringarna i uppgiften.

---
product-area: templates
navigation-topic: templates-navigation-topic
title: Översikt över start- och slutförandedagar i en mall
description: Du kan använda projektmallar för att hämta in de flesta repeterbara processer, information och inställningar som är kopplade till projekten i organisationen. Projekt har specifika start- och slutförandedatum, men mallar har allmänna start- och slutförandedagar som en indikation på var dessa datum hamnar i projektet, baserat på den övergripande tidslinjen för projektet.
author: Alina
feature: Work Management
exl-id: caa0e7b1-37c3-4973-92ce-cc93df4e4186
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---

# Översikt över start- och slutförandedagar i en mall

Du kan använda projektmallar för att hämta in de flesta repeterbara processer, information och inställningar som är kopplade till projekten i organisationen. Projekt har specifika start- och slutförandedatum, men mallar har allmänna start- och slutförandedagar som en indikation på var dessa datum hamnar i projektet, baserat på den övergripande tidslinjen för projektet.

**Exempel:** Om ett projekts startdatum är 1 april och du vill att en aktivitet ska starta 3 april (två dagar efter att projektet har startats), ska motsvarande aktivitet i mallen som skapar projektet starta på dag 2 i mallen, där mallens första dag räknas som dag 0.

## Startdag

Tänk på följande när du arbetar med mallar och malluppgifter:

* Som standard har mallarna startdagen 0 och malluppgifterna och mallen har startdagen 0. Startdagen för malluppgifterna kan ändras, men detta ändrar inte mallens startdag.
* Startdagen för en malluppgift representerar det antal arbetsdagar som Workfront lägger till i aktivitetens planerade startdatum när ett projekt skapas från mallen. Du kan t.ex. ha en mall med bara en uppgift och startdagen för malluppgiften är 4. Mallens startdag är fortfarande 0. När du skapar ett projekt från den här mallen, där projektets schemaläge är startdatum och det planerade startdatumet för projektet är 1 november 2019, lägger den nyligen skapade aktiviteten till fyra dagar till det här datumet och ställer in värdet för det planerade startdatumet till 5 november 2019.

Nedan följer några åtgärder som kan ändra startdagen för malluppgifterna:

* Uppdatera varaktigheten för föregående malluppgifter
* Uppdatera aktivitetsbegränsningar

  När du använder datumbaserade aktivitetsbegränsningar kan du uppdatera startdagen för malluppgifterna manuellt. Några exempel på datumbaserade aktivitetsbegränsningar är fasta datum, startdatum inte tidigare än, startdatum inte senare än, måste börja på.

* Uppdatera föregående malluppgift

## Slutförandedagen

Mallens slutförandedag är den dag då den sista malluppgiften slutförs. Som standard visar alla malluppgifter och mallen en avslutningsdag på 1, eftersom Workfront antar att alla malluppgifter har en varaktighet på 1 dag. Slutförandedagen för malluppgifterna kan ändras och detta ändrar även mallens slutförandedag. Mallens slutförandedag blir det planerade slutförandedatumet för det framtida projektet och slutförandedagarna för malluppgifterna blir de planerade slutförandedatumen för de framtida projektaktiviteterna.

Nedan följer några åtgärder som kan ändra slutförandedagen för malluppgifterna:

* Uppdatera varaktigheten för malluppgifterna
* Uppdatera aktivitetsbegränsningar

  När du använder datumbaserade aktivitetsbegränsningar kan du uppdatera malluppgifternas slutförandedag manuellt. Några exempel på datumbaserade aktivitetsbegränsningar är Fasta datum, Avsluta tidigast, Slutför inte senare än, Måste sluta den.

* Uppdatera föregående malluppgift

## Arbeta med mallar som schemalagts från slutförande

Du kan schemalägga en mall från Slutförandedagen. Mer information finns i [Redigera projektmallar](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Tänk på följande när du arbetar med mallar som schemalagts från slutförandedatum:

* Om du ändrar startdagen anges aktivitetsbegränsningen till Måste starta den.
* Om du ändrar slutförandedagen anges aktivitetsbegränsningen till Måste sluta den.
* När mallen schemaläggs från Slutförandedagen beräknas aktivitetsbegränsningsdagen från Slutförandedagen.

  **Exempel:** Mallens varaktighet är 285 dagar och du har en malluppgift med en varaktighet på 60 dagar. Om du ställer in aktivitetsbegränsningen på Måste börja den och begränsningsdagen på 120 får du startdagen på 165 (285 - 120) och slutförandedagen på 225 (165 + 60). När du redigerar startdagen tolkas den alltså som en begränsningsdag.

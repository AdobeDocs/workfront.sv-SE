---
title: Adobe Maestro-lansering
description: Använd maestro för att skapa egna objekt, fält och arbetsytor.
hidefromtoc: true
hide: true
source-git-commit: 1dffebd5075dc353f28402c79d0c87aff2c12cfa
workflow-type: tm+mt
source-wordcount: '1458'
ht-degree: 0%

---


# Adobe Maestro-lansering

>[!IMPORTANT]
>
>För närvarande ingår Adobe Maestro i ett betaprogram som är öppet för ett begränsat antal kunder.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.
>
>Mer information finns i [Adobe Maestro - översikt](../maestro/maestro-overview.md).

I den här artikeln listas de funktioner som har släppts efter lanseringen av betaprogrammet som avslutades av Maestro den 22 maj 2023.

De släppta funktionerna listas i den ordning de släpps, med den senaste först. Kunder som deltar i det nedstängda betaprogrammet från Maestro har tillgång till alla funktioner i sina förhandsgransknings- och produktionsmiljöer.

>[!IMPORTANT]
>
>Dokumentationen som beskrivs i avsnitten nedan kommer att vara tillgänglig en tid efter att funktionerna släppts till Produktion.

I det här avsnittet beskrivs de funktioner och korrigeringar som har släppts efter lanseringen av Maestro-betaprogrammet, som avslutades den 22 maj 2023.

Funktionerna släpps varje vecka och visas i den ordning de släpps, med den senaste först. Kunder som deltar i det nedstängda betaprogrammet från Maestro har tillgång till alla funktioner i sina förhandsgransknings- och produktionsmiljöer.

## Vecka 18 september 2023

### Ordna om rader

Förhandsgranskning och produktion: 20 september 2023

Du kan nu ändra ordningen på en eller flera rader (eller poster) i tabellvyn på en posttypsida.

## Vecka 4 september 2023

### Koppla ihop Maestro-poster med Workfront företag och grupper

Förhandsgranskning och produktion: 5 september 2023

Nu kan du koppla en Maestro-post till Workfront-företag och -grupper. Du måste först skapa en anslutning mellan en Maestro-posttyp och Workfront-företagen och gruppera objekttyper. Sedan kan du koppla en enda Maestro-post av den valda posttypen till enskilda Workfront-företag och -grupper.

Tänk på följande:

* Du måste skapa en anslutning mellan posttyperna Maestro och objekttyperna Workfront Company och Group för varje arbetsyta.

* Du kan inte ansluta taxonomiposttyper med Workfront objekttyper.

* Du kan koppla flera Maestro-poster till samma Workfront-företag eller -grupp, och flera företag eller grupper till samma Maestro-post.

* Du kan inte redigera företag eller grupper i Maestro. Alla företags- eller gruppändringar som gjorts i Workfront visas i Maestro när du granskar de länkade posterna i Maestro.

  Mer information finns i följande artiklar:

   * [Koppla posttyper](../maestro/architecture-and-fields/connect-record-types.md)
   * [Koppla poster](../maestro/records/connect-records.md)

### URL-stöd för enkelradiga textfält

Förhandsgranskning och produktion: 7 september 2023

För bättre synlighet när du arbetar med länkar i tabellvyn har vi lagt till stöd för URL-adresser i enkelradiga textfält. När du använder URL:er till andra webbplatser eller externa enheter när du uppdaterar ett textfält med en rad identifieras de nu som länkar och du kan klicka på dem från tabellen. Före den här förbättringen visas länkar som text.

## Vecka 28 augusti 2023

### Fältsynlighetsmeny för verktygsfältet Tabellvy

Förhandsgranskning och produktion: 31 augusti 2023

Om du vill visa rätt information för en viss postuppsättning, särskilt om du tänker dela vyn med andra som måste se vissa men inte alla fält av en posttyp, kan du nu välja vilka fält (eller kolumner) som ska visas och vilka som ska döljas i tabellvyn.

Du kan dölja eller visa enskilda fält från varje rubrik i fältkolumnerna, eller hantera alla fält av posttyp från en inställning i verktygsfältet för tabellvyn.

Mer information finns i [Hantera tabellvyn](../maestro/views/manage-the-table-view.md).

## Vecka 21 augusti 2023

### Koppla ihop Maestro-poster med program och portfolior

Förhandsgranskning och produktion: 24 augusti 2023

Nu kan du koppla samman en Maestro-post med Workfront program och portfolior. Du måste skapa en anslutning mellan en Maestro-posttyp och ett program eller en portfölj som skapar ett anslutet fält. Sedan kan du koppla alla Maestro-poster från alla andra posttyper inom samma arbetsyta till specifika program och portföljer som skapar en skrivskyddad posttyp för Workfront eller Workfront Portfolio i samma arbetsyta. Tänk på följande:

* Posttyper för Workfront-anslutning är unika för varje arbetsyta.
* Du kan koppla flera Maestro-poster till samma Workfront-program eller portfölj, samt flera program och portföljer till samma Maestro-post.
* Du kan inte redigera program och portföljer i Maestro. Alla program- och portföljändringar som görs i Workfront visas i Maestro när de länkade posterna granskas.

### Ny sorteringsfunktion för tabellvyn

Förhandsgranskning och produktion: 24 augusti 2023

Nu kan du sortera poster i tabellvyn på en posttypssida.
Följande funktioner är nu tillgängliga:

* Sortera på tabellnivå, där du kan sortera efter flera fält samtidigt.
* Sortera efter kolumn- eller fältnivå, där du kan sortera efter ett enskilt fält i taget.

### Förbättringar av tidslinjevyn: nytt utseende och känsla för grupperingar och växeln för vyn Kompakt/Standard

Förhandsgranskning och produktion: 24 augusti 2023

Vi har infört följande förbättringar av tidslinjevyn:

* Du kan nu visa tidslinjevyn i följande lägen:

   * Standard: Visar poster på separata rader.
   * Kompakt: Visa de poster vars datum inte överlappar på samma rad.

* Vi har ändrat utseendet på grupperingsraderna i tidslinjevyn så att de visas ovanför tidslinjen för de poster de innehåller. Före den här förbättringen visas grupperingslinjerna över hela tidslinjen.

## Vecka 14 augusti 2023

### Ändra ordning på kolumner i tabellvyn

Nu kan du ändra ordning på kolumner i tabellvyn i maestro. Tänk på följande när du ändrar ordning på kolumner:

* Fältet Namn är alltid det första fältet i tabellvyn för en posttypsida

* Du kan inte flytta namnfältet till en annan position

* Fältet Namn är fryst och ingår inte i den vågräta rullningen.

### Vågrät rullning för tidslinjevyn

Du kan nu rulla vågrätt i tidslinjevyn för en posttyp.

## 7 augusti 2023

### Importera posttyper från en Excel-fil

Förhandsgranska och producera: 10 augusti 2023

Nu kan du importera en Excel-fil för att skapa posttyper på en arbetsyta. Tabellerna i filen blir posttyper och kolumnerna i filen blir deras respektive fält.

### Förbättrad upplevelse vid anslutning av posttyper och projekt

Förhandsgranska och producera: 10 augusti 2023

Vi har förbättrat ditt sätt att koppla posttyper, inklusive att ansluta till Workfront-projekt. Som en del av den här förbättringen gjorde vi följande ändringar när vi lade till ett fält för en posttyp från tabellvyn:

* Fältet Relationstyp har tagits bort från fliken Nytt fält.

* Lägg till fliken Ny anslutning där du kan välja den post eller objekttyp som du vill ansluta till direkt, vilket eliminerar behovet av ett fält av relationstyp.

## Vecka 10 juli 2023

### Uppdatera utseendet för en posttyp

Förhandsgranskning och produktion: 13 juli 2023

Nu kan du välja en anpassad ikon för en posttyp och en anpassad färg för posttypsikonen.

### Ny fälttyp för kryssruta

Förhandsgranskning och produktion: 13 juli 2023

Nu kan du lägga till en fälttyp för kryssruta i Maestro-posttyper. Du kan använda ett fält av typen Kryssruta för att lägga till en kryssruta till en post. Du kan använda det här fältet för att ange ett specifikt attribut eller en specifik status för den aktuella posten. Du kan till exempel använda den som en flagga för att spåra slutförande, godkännande eller andra binära attribut för varje post.

## Vecka 26 juni 2023

### Snabbaktivering av snabbmenyn i en tabell

Förhandsgranskning och produktion: 28 juni 2023

Vi har aktiverat möjligheten att aktivera snabbmenyn genom att högerklicka var som helst i en postrad, när du visar posterna i tabellvyn eller en posttyp. Nu kan du snabbt visa, ta bort eller kopiera en länk till postens informationssida när du öppnar snabbmenyn från valfri plats i tabellvyn för en posttyp. Före den här förbättringen var snabbmenyn bara tillgänglig från menyn Mer i kolumnen Namn på en post.

## Vecka 19 juni 2023

### Postfältnamn är unika

Vi har infört ett krav nu på att fältnamnen för en Maestro-posttyp ska ha unika namn. Fält som tillhör olika posttyper behöver inte ha unika namn.

## Vecka 5 juni 2023

### Koppla ihop Maestro-poster med Workfront-projekt

Förhandsgranskning och produktion: 5 juni 2023

Nu kan du koppla en Maestro-post till Workfront-projekt. Du måste skapa en koppling till en Maestro-posttyp för att upprätta anslutningen mellan Maestro-poster och Workfront-projekt. Sedan kan du koppla alla Maestro-poster från alla andra posttyper till kopplingsposten med hjälp av fältet Relation. Tänk på följande:

* Du måste ha en anslutningsposttyp för Workfront för varje arbetsyta.
* Du kan koppla flera Maestro-poster till samma Workfront-projekt och flera projekt till samma Maestro-post.
* Du kan inte redigera projekt i Maestro. Alla projektändringar som görs i Workfront visas i maestro när du granskar de länkade posterna.

## Vecka 29 maj 2023

### Tvådatumskrav för att skapa en tidslinjevy

Förhandsgranskning och produktion: 31 maj 2023

Du måste ha minst två datumfält associerade med en posttyp för att kunna skapa en tidslinjevy.
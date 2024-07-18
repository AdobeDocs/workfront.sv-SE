---
title: Aktivitetsarkiv för lansering av Adobe Workfront Planning för 2023
description: Adobe Workfront Planning-funktionerna är för närvarande tillgängliga för vissa Workfront-kunder. Läs den här artikeln ofta och lär dig mer om de funktioner som nyligen släppts för planeringsfunktionerna.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 52e8ce6dd5146d72f698583b531b3db6bc5dbf25
workflow-type: tm+mt
source-wordcount: '2988'
ht-degree: 0%

---


# Aktivitetsarkiv för lansering av Adobe Workfront Planning för 2023

<!--this article is linked to the WF Planning landing page - do not change URL or move it; send the team a new URL after we add the redirects for this page-->

>[!IMPORTANT]
>
>Informationen i den här artikeln handlar om Adobe Workfront Planning, ett nytt erbjudande från Adobe Workfront.
>
>Workfront Planning är för närvarande i ett tidigt skede som är öppet för ett begränsat antal kunder.
>
>Du måste vara kund hos Workfront för att kunna använda dessa funktioner.
>
>Din kontorepresentant kommer att informera dig om du är en del av det här steget.
>
>Mer information finns i [Översikt över Adobe Workfront-planering](/help/quicksilver/planning/general/planning-overview.md).
>

I den här artikeln listas de funktioner som har släppts efter lanseringen av Adobe Workfront Planning Program, den 22 maj 2023 för 2023.

Mer information om de funktioner som släpptes under 2024 finns i [Adobe Workfront Planering - aktuell versionsaktivitet](/help/quicksilver/planning/general/release-activity.md).

De släppta funktionerna listas i den ordning de släpps, med den senaste först. Kunder som deltar i Workfront Planning Program har tillgång till alla funktioner i produktionsmiljön.

Mellan maj 2023 och december 2023 släpptes alla funktioner i den här artikeln till både förhandsgransknings- och produktionsmiljön.

Workfront Planning har tillfälligt tagits bort från förhandsgransknings- och sandlådemiljöerna sedan januari 2024. Alla funktioner som beskrivs i de här artiklarna är för närvarande tillgängliga i Produktion.

## Vecka 25 december 2023

### Söka i tidslinjevyn

Förhandsgranska och produktion: 27 december 2023

Nu kan du söka efter ett nyckelord för att snabbt hitta en post i tidslinjevyn. Du kan använda nyckelord och specialtecken från alla fält som visas på skärmen för att hitta en post. Mer information finns i [Hantera tidslinjevyn](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Vecka 18 december 2023

### Lägga till kommentarer på poster från postens sida

Preview and Production for all customers: 18 december 2023

>[!NOTE]
>
>Följande funktioner kommer att vara tillgängliga i Production i januari 2024:
>
>* Sök efter kommentarer
>
>* Kopiera och klistra in bilder
>
>* Dra och släppa bilder
>
>Mer information finns i [Översikt över utgåvan för första kvartalet 2024](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).

Nu kan du samarbeta med andra om enskilda poster genom att lägga till kommentarer eller svara andra samtidigt som du visar en posts sida.

Kommentarsupplevelsen för planeringsfunktionsposter matchar den nya kommentarsfunktionen för Workfront-objekt.

Mer information finns i [Hantera postkommentarer](/help/quicksilver/planning/records/manage-record-comments.md).

### Workfront Planning Connector for Adobe Workfront Fusion

Produktion: 21 december 2023

>[!IMPORTANT]
>
>Man måste köpa Adobe Workfront Fusion för att kunna bygga anslutningar med Adobe Workfront Planning.
>
>Mer information finns i [Adobe Workfront Fusion - översikt](/help/quicksilver/workfront-fusion/get-started/workfront-fusion-overview.md).

Nu kan du använda Adobe Workfront Fusion för att ansluta till planeringsfunktionerna. Med den nya Fusion-anslutningen kan du

* Skapa, läsa, uppdatera och ta bort poster

* Hämta en lista med poster efter posttyp

* Ta bort eller hämta en lista med posttyper

* Sök poster

* Anropa ett API

* Utlösa ett scenario när en ändring görs i planeringsfunktionerna

Mer information finns i [Planeringsmoduler för Adobe Workfront](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-planning-modules.md).

## Vecka 11 december 2023

### Uppdatera det primära fältet i en tabellvy för en posttyp

Förhandsgranska och produktion: 14 december 2023

Du kan nu välja det fält som du vill visa i den första kolumnen i en tabellvy. Det här fältet kallas nu primärt fält.

Före den här förbättringen visas namnfältet för en post alltid i den första kolumnen i tabellvyn och det kan inte placeras på en annan plats.

Observera följande med den här förbättringen:

* Kolumnen eller fältet Namn är som standard fortfarande den första kolumnen i en tabell.

* Du kan välja vilket fält som helst av följande typer som primärt fält och ersätta fältet Namn i den första kolumnen:

   * Enkelradig text

   * Nummer

   * Formel

* Det primära fältet i en tabellvy fryses alltid och kan inte flyttas om du inte anger ett annat fält som primärt fält.

* Du kan ändra det primära fältet från en icke-primär kolumnrubrik.

* Alla tabellvyer av en posttyp har samma primära fält som du väljer.

Mer information finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md).

### Koppla samman planeringsfunktionsposter med Adobe Experience Manager Assets

Förhandsversion: 14 december 2023

Produktionsrelease: 21 december 2023

>[!IMPORTANT]
>
>Din organisations instans av Workfront måste vara registrerad på Adobe Business Platform eller Adobe Admin Console för att Adobe Workfront Planning capabilities-poster ska kunna anslutas till Adobe Experience Manager Assets.
>
>Om du har frågor om hur du kommer igång med Adobe Admin Console kan du läsa [Adobe Unified Experience FAQ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

Nu kan du upprätta en anslutning mellan posttyperna för Adobe Workfront Planning-funktioner och Adobe Experience Manager Assets.

När du har upprättat anslutningen är följande funktioner tillgängliga med den här uppdateringen:

* Du kan länka resurser och mappar i Experience Manager till en planeringsfunktionspost från en viss databas i Experience Manager Assets som de har tillgång till. Du kan koppla resursfält till planeringsfunktionsfält i den här processen.

* Planeringsfunktionens användare kan visa namnet på de anslutna resurserna samt värdena för de anslutna fälten i planeringsfunktionerna.

<!--removed per PM, for now: 
* An Experience Manager Assets record type is automatically created in Planning after you establish the connection. Connected assets are visible in the table and timeline views of this new record type.  
-->

* Du kan klicka på resursnamnet i tabellvyn för planeringsfunktionsposten från det anslutna postfältet och visa ett popup-fönster med miniatyrbilden av resursen och flera nyckelfält. I popup-fönstret kan du navigera till resursvisningsprogrammet i Experience Manager och visa all information om det.

Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).

## Vecka 4 december 2023

### Kopiera och klistra in information från ett fält till ett annat i planeringstabellvyn för persontyper och länkade postfält

Förhandsgranska och produktion: 5 december 2023

Nu kan du kopiera och klistra in information från ett fält till ett annat fält av samma typ i en posttypstabellvy. Den här funktionen stöds nu för följande typer av fält:

* Folk
* Länkade postfält

Tänk på följande:

* Kopiering och inklistring av fältvärden från ett fält till ett annat stöds för fält som visar flera värden.

* Du kan inte kopiera information från en annan källa, förutom ett planeringsfunktionsfält av samma typ som det fält som du klistrar in informationen i.

* Du kan inte kopiera och klistra in fältvärden för fält som visas i området Detaljer för en post.

Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

Mer information om länkade fält finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).

## Vecka 27 november 2023

### Kopiera och klistra in information från ett fält till ett annat i tabellvyn för planeringsfunktioner

Förhandsgranska och produktion: 28 november 2023

Du kan nu kopiera och klistra in information från ett fält till ett annat fält av samma typ i en posttyptabellvy för planeringsfunktioner.

Tänk på följande:

* Du kan inte kopiera information från en annan källa, förutom ett planeringsfunktionsfält av samma typ som det fält som du klistrar in informationen i.

* Du kan inte kopiera och klistra in fältvärden för fält som visas i området Detaljer för en post.

* Du kan inte kopiera och klistra in fältvärden för följande fälttyper:

   * Folk

   * Systemfält

   * Länkade fält som har skapats som ett resultat av att poster kopplas

Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

## Vecka 6 november 2023

### Gruppering för registervyn

Förhandsgranska och produktion: 7 november 2023

Nu kan du gruppera poster i tabellvyn för en posttypsida. Du kan gruppera efter tre unika fält i planeringsfunktionsgränssnittet <!--checking into this for now: and by four fields when using the API-->.

Mer information finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md).

## Vecka 30 oktober 2023

### Nya fälttyper för användar- och datumfält för att fånga vem som skapade eller senast ändrade en post eller på vilket datum

Förhandsgranska och produktion: 30 oktober 2023

Vi har introducerat följande fälttyper för Adobe Workfront Planning-funktionsposter:

* Skapad av

* Skapad den

* Senast ändrad av

* Senast ändrat den

Fältvärdena för de fält som skapas från dessa fälttyper är skrivskyddade och fångar namnet på användaren som skapade eller senast ändrade en post, eller datumet då posten skapades eller ändrades senast.

Mer information finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

### Navigera till Workfront-objekt från en post för planeringsfunktioner

Förhandsgranskning och produktion: 31 oktober 2023

Nu kan du öppna Workfront objektsidor från följande områden i Workfront Planning:

* Skrivskyddad vy för Workfront-objektspostregister

* Den skrivskyddade postsidan för Workfront-objekt

Mer information finns i [Anslut poster](/help/quicksilver/planning/records/connect-records.md).

### Förbättrad navigering i tabellvyn

Förhandsgranska och produktion: 2 november 2023

Navigeringen i tabellvyn för en posttypssida har förbättrats.

Nedan följer några av förbättringarna:

* Använd tabbtangenten på tangentbordet för att navigera i tabellens kolumner och rader

* Lägg till en ny post från valfri kolumnposition. Före den här förbättringen kunde du bara lägga till en post från den första kolumnen.

* Använd tangentbordskombinationen Skift + Retur för att lägga till en ny post (eller rad) i tabellen.

Mer information finns i [Anslut poster](/help/quicksilver/planning/records/connect-records.md).

## Vecka 16 oktober 2023

### Ny personfältstyp

Förhandsgranska och produktion: 16 oktober 2023

Nu kan du lägga till ett persontypsfält i posttyper för planeringsfunktioner. Du kan använda fält av typen Personer för att associera befintliga användare med en post. Mer information finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

### RTF-format för styckefält

Förhandsgranska och produktion: 16 oktober 2023

Vi har lagt till kontroller för Rich Text-format för stycketextfält. Du kan formatera styckefälten med RTF antingen i tabellvyn av en posttyp eller på postsidan. Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).


### Spela in och gruppera färgkodning för tidslinjevyn

Förhandsgranska och produktion: 19 oktober 2023

Nu kan du färgkoda postfälten och grupperingarna i tidslinjevyn.

Följande är alternativ för de färger som du kan välja att visa för poststaplar och grupperingar i tidslinjevyn:

* Grupperingar kan matcha följande färger:

   * Grå (standard)

   * Färgen på fältet som du grupperar efter

* Staplar kan matcha följande färger:

   * Posttypens färg

   * Färgen på ett fält som du väljer

   * Färgen på grupperingen

   * Ingen färg (standard)

När du matchar färger till ett visst fält kan du bara markera fält med färgkodade alternativ.

Mer information finns i [Hantera tidslinjevyn](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Vecka 9 oktober 2023

### Sök i tabellvy

Förhandsgranskning och produktion: 9 oktober 2023

Nu kan du söka efter ett nyckelord för att snabbt hitta en post i tabellvyn. Du kan använda nyckelord och specialtecken från alla fält som visas på skärmen för att hitta en post. Mer information finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md).

## Vecka 18 september 2023

### Ordna om rader

Förhandsgranska och produktion: 20 september 2023

Du kan nu ändra ordningen på en eller flera rader (eller poster) i tabellvyn på en posttypsida. Mer information finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md).

## Vecka 4 september 2023

### Koppla samman planeringsfunktionsposter med Workfront företag och grupper

Förhandsgranskning och produktion: 5 september 2023

Nu kan du koppla en post för planeringsfunktioner till Workfront-företag och -grupper. Du måste först skapa en anslutning mellan en posttyp för planeringsfunktioner och Workfront-företagen och gruppera objekttyper. Sedan kan du koppla en enda post för planeringsfunktioner av den valda posttypen till enskilda Workfront-företag och -grupper.

Tänk på följande:

* Du måste skapa en anslutning mellan posttyper för planeringsfunktioner och objekttyperna Workfront Company och Group för varje Workspace.

* Du kan inte ansluta taxonomiposttyper med Workfront objekttyper.

* Du kan koppla flera poster för planeringsfunktioner till samma Workfront-företag eller -grupp och flera företag eller grupper till samma post för planeringsfunktioner.

* Du kan inte redigera företag eller grupper i planeringsfunktionerna. Alla företags- eller gruppändringar som görs i Workfront visas i planeringsfunktionerna när du granskar länkade poster för planeringsfunktioner.

  Mer information finns i följande artiklar:

   * [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [Koppla poster](/help/quicksilver/planning/records/connect-records.md)

### URL-stöd för enkelradiga textfält

Förhandsgranska och produktion: 7 september 2023

För bättre synlighet när du arbetar med länkar i tabellvyn har vi lagt till stöd för URL-adresser i enkelradiga textfält. När du använder URL:er till andra webbplatser eller externa enheter när du uppdaterar ett textfält med en rad identifieras de nu som länkar och du kan klicka på dem från tabellen. Före den här förbättringen visas länkar som text.

## Vecka 28 augusti 2023

### Fältsynlighetsmeny för verktygsfältet Tabellvy

Förhandsgranskning och produktion: 31 augusti 2023

Om du vill visa rätt information för en viss postuppsättning, särskilt om du tänker dela vyn med andra som måste se vissa men inte alla fält av en posttyp, kan du nu välja vilka fält (eller kolumner) som ska visas och vilka som ska döljas i tabellvyn.

Du kan dölja eller visa enskilda fält från varje rubrik i fältkolumnerna, eller hantera alla fält av posttyp från en inställning i verktygsfältet för tabellvyn.

Mer information finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md).

## Vecka 21 augusti 2023

### Koppla samman Adobe Workfront Planning-funktionsposter med program och portfolior

Förhandsgranska och produktion: 24 augusti 2023

Nu kan du koppla samman en post för planeringsfunktioner med Workfront program och portföljer. Du måste skapa en anslutning mellan posttypen för planeringsfunktioner och ett program eller en portfölj som skapar ett anslutet fält. Sedan kan du koppla alla planeringsfunktionsposter från alla andra posttyper inom samma arbetsyta till specifika program och portföljer som skapar en skrivskyddad posttyp för Workfront eller Workfront Portfolio i samma arbetsyta. Tänk på följande:

* Posttyper för Workfront-anslutning är unika för varje arbetsyta.
* Du kan koppla ihop flera poster för planeringsfunktioner till samma Workfront-program eller portfölj, samt flera program och portföljer till samma post för planeringsfunktioner.
* Du kan inte redigera program och portföljer i planeringsfunktionerna. Alla program- och portföljändringar som görs i Workfront visas i planeringsfunktionerna när de länkade posterna granskas.

### Ny sorteringsfunktion för tabellvyn

Förhandsgranska och produktion: 24 augusti 2023

Nu kan du sortera poster i tabellvyn på en posttypssida.
Följande funktioner är nu tillgängliga:

* Sortera på tabellnivå, där du kan sortera efter flera fält samtidigt.
* Sortera efter kolumn- eller fältnivå, där du kan sortera efter ett enskilt fält i taget.

### Förbättringar av tidslinjevyn: nytt utseende och känsla för grupperingar och växeln för vyn Kompakt/Standard

Förhandsgranska och produktion: 24 augusti 2023

Vi har infört följande förbättringar av tidslinjevyn:

* Du kan nu visa tidslinjevyn i följande lägen:

   * Standard: Visar poster på separata rader.
   * Kompakt: Visa de poster vars datum inte överlappar på samma rad.

* Vi har ändrat utseendet på grupperingsraderna i tidslinjevyn så att de visas ovanför tidslinjen för de poster de innehåller. Före den här förbättringen visas grupperingslinjerna över hela tidslinjen.

## Vecka 14 augusti 2023

### Ändra ordning på kolumner i tabellvyn

Nu kan du ändra ordning på kolumner i tabellvyn. Tänk på följande när du ändrar ordning på kolumner:

* Fältet Namn är alltid det första fältet i tabellvyn för en posttypsida

* Du kan inte flytta namnfältet till en annan position

* Fältet Namn är fryst och ingår inte i den vågräta rullningen

### Vågrät rullning för tidslinjevyn

Du kan nu rulla vågrätt i tidslinjevyn för en posttyp.

## 7 augusti 2023

### Importera posttyper från en Excel-fil

Förhandsgranska och produktion: 10 augusti 2023

Nu kan du importera en Excel-fil för att skapa posttyper på en arbetsyta. Tabellerna i filen blir posttyper och kolumnerna i filen blir deras respektive fält.

### Förbättrad upplevelse vid anslutning av posttyper och projekt

Förhandsgranska och produktion: 10 augusti 2023

Vi har förbättrat ditt sätt att koppla posttyper, inklusive att ansluta till Workfront-projekt. Som en del av den här förbättringen gjorde vi följande ändringar när vi lade till ett fält för en posttyp från tabellvyn:

* Fältet Relationstyp har tagits bort från fliken Nytt fält.

* Lägg till fliken Ny anslutning där du kan välja den post eller objekttyp som du vill ansluta till direkt, vilket eliminerar behovet av ett fält av relationstyp.

## Vecka 10 juli 2023

### Uppdatera utseendet för en posttyp

Förhandsgranska och produktion: 13 juli 2023

Nu kan du välja en anpassad ikon för en posttyp och en anpassad färg för posttypsikonen.

### Ny fälttyp för kryssruta

Förhandsgranska och produktion: 13 juli 2023

Nu kan du lägga till en fälttyp för kryssruta i posttyper för planeringsfunktioner. Du kan använda ett fält av typen Kryssruta för att lägga till en kryssruta till en post. Du kan använda det här fältet för att ange ett specifikt attribut eller en specifik status för den aktuella posten. Du kan till exempel använda den som en flagga för att spåra slutförande, godkännande eller andra binära attribut för varje post.

## Vecka 26 juni 2023

### Snabbaktivering av snabbmenyn i en tabell

Förhandsgranskning och produktion: 28 juni 2023

Vi har aktiverat möjligheten att aktivera snabbmenyn genom att högerklicka var som helst i en postrad, när du visar posterna i tabellvyn eller en posttyp. Nu kan du snabbt visa, ta bort eller kopiera en länk till postens sida när du öppnar snabbmenyn från valfri plats i tabellvyn för en posttyp. Före den här förbättringen var snabbmenyn bara tillgänglig från menyn Mer i kolumnen Namn på en post.

## Vecka 19 juni 2023

### Postfältnamn är unika

Vi har infört ett krav nu på att fältnamnen för en posttyp för planeringsförmåga ska ha unika namn. Fält som tillhör olika posttyper behöver inte ha unika namn.

## Vecka 5 juni 2023

### Koppla samman Adobe Workfront Planning-funktionsposter med Workfront-projekt

Förhandsgranskning och produktion: 5 juni 2023

Nu kan du koppla samman en post för planeringsfunktioner med Workfront-projekt. Du måste skapa en posttyp för anslutningsplaneringsfunktioner för att upprätta en koppling mellan planeringsfunktionsposterna och Workfront-projekt. Sedan kan du koppla alla planeringsfunktionsposter från alla andra posttyper till kopplingsposten med hjälp av fältet Relation. Tänk på följande:

* Du måste ha en kopplingsposttyp för Workfront för varje Workspace.
* Du kan koppla flera planeringsfunktionsposter till samma Workfront-projekt och flera projekt till samma planeringsfunktionspost.
* Du kan inte redigera projekt i planeringsfunktioner. Alla projektändringar som görs i Workfront visas i planeringsfunktionerna när du granskar de länkade posterna.

## Vecka 29 maj 2023

### Tvådatumskrav för att skapa en tidslinjevy

Förhandsgranska och produktion: 31 maj 2023

Du måste ha minst två datumfält associerade med en posttyp för att kunna skapa en tidslinjevy.
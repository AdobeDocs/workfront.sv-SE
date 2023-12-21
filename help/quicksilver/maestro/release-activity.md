---
title: Adobe Maestro-lansering
description: Adobe Maestro är för närvarande tillgängligt för utvalda Workfront-kunder. Läs den här artikeln ofta och lär dig mer om de funktioner som nyligen släppts för Adobe Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 53911aa3-74fd-4747-9008-f86a521ffba6
source-git-commit: 5d8e189f01a52b2d1b605b497ed17737fb0a0924
workflow-type: tm+mt
source-wordcount: '2890'
ht-degree: 0%

---

# Adobe Maestro-lansering

>[!IMPORTANT]
>
>Informationen i den här artikeln handlar om Adobe Maestro, ett nytt erbjudande från Adobe Workfront.
>
>För närvarande ingår Adobe Maestro i ett betaprogram som är öppet för ett begränsat antal kunder. Du måste vara Workfront-kund för att kunna använda Maestro-funktionerna.
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

<!--
## Week of November 27, 2023

### Maestro permissions for users and groups

Production: November 28, 2023

>[!IMPORTANT]
>
>This functionality is not yet available in Preview.

You can now share a workspace with users and groups. You can set their permissions to different levels, depending on what information they need to view or edit in a Maestro workspace. After you share permissions to a workspace, users have permissions to the record types, records, and fields in that space.

The following are the permissions levels for Maestro workspaces:  

* None: Users cannot access any workspaces in Maestro, even if the Maestro area is shared with them through a layout template. 

* View: Users can view workspaces that are shared with them. They can also view record types, and records from the shared workspace. 

* Contribute: Users can create, edit, or delete records in the workspace that is shared with them.  They cannot create or edit record types or workspaces ones shared with them.  

* Manage: Users can create, edit, and delete record types, records, and fields in workspaces that are shared with them. They cannot create workspaces.  

Only Workfront administrators can create, edit, or delete workspaces and all information associated with them.  

For more information, see [Grant access to Adobe Maestro](../maestro/access/grant-access.md) and [Overview of sharing permissions in Adobe Maestro](../maestro/access/sharing-permissions-overview.md). -->

## Vecka 18 december 2024

### Lägga till kommentarer på poster från detaljsidan

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
>Mer information finns i [Första utgåvan, kvartal 2024, översikt](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).

Nu kan du samarbeta med andra om enskilda poster genom att lägga till kommentarer eller svara andra samtidigt som du visar en post på detaljsidan.

Kommentarsupplevelsen för Maestro-poster matchar den nya kommentarsfunktionen för Workfront-objekt.

Mer information finns i [Hantera postkommentarer](/help/quicksilver/maestro/records/manage-record-comments.md).

### Macromedia-kontakt (beta) för Adobe Workfront Fusion

Produktion: 21 december 2023

>[!IMPORTANT]
>
>Din organisation måste köpa Adobe Workfront Fusion för att kunna skapa anslutningar med Maestro.
>
>Mer information finns i [Adobe Workfront Fusion - översikt](/help/quicksilver/workfront-fusion/get-started/workfront-fusion-overview.md).

Nu kan du använda Adobe Workfront Fusion för att ansluta till Maestro. Med den nya anslutningen till Adobe Maestro Fusion kan du

* Skapa, läsa, uppdatera och ta bort poster

* Hämta en lista med poster efter posttyp

* Ta bort eller hämta en lista med posttyper

* Sök poster

* Anropa ett API

* Utlösa ett scenario när en ändring görs i Maestro

Mer information finns i [Adobe Maestro-moduler](/help/quicksilver/workfront-fusion/apps-and-their-modules/maestro-modules.md).

## Vecka 11 december 2023

### Uppdatera det primära fältet i en tabellvy för en posttyp

Förhandsgranska och produktion: 14 december 2023

Du kan nu välja det fält som du vill visa i den första kolumnen i en Maestro-tabellvy. Det här fältet kallas nu primärt fält.

Före den här förbättringen visas namnfältet för en post alltid i den första kolumnen i tabellvyn och det kan inte placeras på en annan plats.

Observera följande med den här förbättringen:

* Kolumnen eller fältet Namn är som standard fortfarande den första kolumnen i en tabell.

* Du kan välja vilket fält som helst av följande typer som primärt fält och ersätta fältet Namn i den första kolumnen:

   * Enkelradig text

   * Nummer

   * Formel

     >[!NOTE]
     >
     >Formeltypsfält kommer att frisläppas vid ett senare datum.

* Det primära fältet i en tabellvy fryses alltid och kan inte flyttas om du inte anger ett annat fält som primärt fält.

* Du kan ändra det primära fältet från en icke-primär kolumnrubrik.

* Alla tabellvyer av en posttyp har samma primära fält som du väljer.

Mer information finns i [Hantera tabellvy](/help/quicksilver/maestro/views/manage-the-table-view.md).


### Koppla ihop Maestro-poster med Adobe Experience Manager Assets

Förhandsversion: 14 december 2023

Produktionsrelease: 21 december 2023

>[!IMPORTANT]
>
>Din organisations instans av Workfront måste vara registrerad på Adobe Business Platform eller Adobe Admin Console för att kunna ansluta Maestro-poster till Adobe Experience Manager Assets.
>
>Om du har frågor om hur du kommer igång med Adobe Admin Console kan du läsa [Adobe - frågor och svar om enhetliga upplevelser](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).


Nu kan du upprätta en anslutning mellan posttyperna Maestro och Adobe Experience Manager Assets.

När du har upprättat anslutningen är följande funktioner tillgängliga med den här uppdateringen:

* Du kan länka resurser och mappar i Experience Manager till en Maestro-post från en viss databas i Experience Manager Assets som de har tillgång till. Du kan koppla resursfält till Maestro-fält i den här processen.

* Maestro-användare kan visa namnet på de anslutna resurserna samt värdena för de anslutna fälten i Maestro

<!--removed per PM, for now: 
* An Experience Manager Assets record type is automatically created in Maestro after you establish the connection. Connected assets are visible in the Maestro table and timeline views of this new record type.  
-->

* Du kan klicka på resursnamnet i tabellvyn för Maestro-posten från det anslutna postfältet och visa ett popup-fönster med miniatyrbilden för resursen och flera nyckelfält. I popup-fönstret kan du navigera till resursvisningsprogrammet i Experience Manager och visa all information om det.

Mer information finns i [Koppla posttyper](/help/quicksilver/maestro/architecture/connect-record-types.md).

## Vecka 4 december 2023

### Kopiera och klistra in information från ett fält till ett annat i Maestro-tabellvyn för fält av typen Folk och länkade poster

Förhandsgranska och produktion: 5 december 2023

Nu kan du kopiera och klistra in information från ett fält till ett annat fält av samma typ i en tabellvy av typen Maestro. Den här funktionen stöds nu för följande typer av fält:

* Folk
* Länkade postfält

Tänk på följande:

* Kopiering och inklistring av fältvärden från ett fält till ett annat stöds för fält som visar flera värden.

* Du kan inte kopiera information från en annan källa, förutom ett Maestro-fält av samma typ som det fält som du klistrar in informationen i.

* Du kan inte kopiera och klistra in fältvärden för fält som visas i området Detaljer för en post.

Mer information finns i [Redigera poster](../maestro/records/edit-records.md).

Mer information om länkade fält finns i [Koppla posttyper](../maestro/architecture/connect-record-types.md).

## Vecka 27 november 2023

### Kopiera och klistra in information från ett fält till ett annat i Maestro-tabellvyn

Förhandsgranska och produktion: 28 november 2023

Nu kan du kopiera och klistra in information från ett fält till ett annat fält av samma typ i en tabellvy av typen Maestro.

Tänk på följande:

* Du kan inte kopiera information från en annan källa, förutom ett Maestro-fält av samma typ som det fält som du klistrar in informationen i.

* Du kan inte kopiera och klistra in fältvärden för fält som visas i området Detaljer för en post.

* Du kan inte kopiera och klistra in fältvärden för följande fälttyper:

   * Folk

   * Systemfält

   * Länkade fält som har skapats som ett resultat av att poster kopplas

Mer information finns i [Redigera poster](../maestro/records/edit-records.md).

## Vecka 6 november 2023

### Gruppering för registervyn

Förhandsgranska och produktion: 7 november 2023

Nu kan du gruppera poster i tabellvyn för en posttypsida. Du kan gruppera efter tre unika fält i Maestro-gränssnittet <!--checking into this for now: and by four fields when using the API-->.

Mer information finns i [Hantera tabellvyn](../maestro/views/manage-the-table-view.md).

## Vecka 30 oktober 2023

### Nya fälttyper för användar- och datumfält för att fånga vem som skapade eller senast ändrade en post eller på vilket datum

Förhandsgranska och produktion: 30 oktober 2023

Vi har introducerat följande fälttyper för Maestro-poster:

* Skapad av

* Skapad den

* Senast ändrad av

* Senast ändrat den

Fältvärdena för de fält som skapas från dessa fälttyper är skrivskyddade och fångar namnet på användaren som skapade eller senast ändrade en post, eller datumet då posten skapades eller ändrades senast.

Mer information finns i [Skapa fält](../maestro/fields/create-fields.md).

### Navigera till Workfront-objekt från en Maestro-post

Förhandsgranskning och produktion: 31 oktober 2023

Nu kan du öppna Workfront objektsidor från följande områden i Maestro:

* Skrivskyddad vy för Workfront-objektspostregister

* Workfront-objektets skrivskyddade postinformationssida

Mer information finns i [Koppla poster](../maestro/records/connect-records.md).

### Förbättrad navigering i tabellvyn

Förhandsgranska och produktion: 2 november 2023

Navigeringen i tabellvyn för en posttypssida har förbättrats.

Nedan följer några av förbättringarna:

* Använd tabbtangenten på tangentbordet för att navigera i tabellens kolumner och rader

* Lägg till en ny post från valfri kolumnposition. Före den här förbättringen kunde du bara lägga till en post från den första kolumnen.

* Använd tangentbordskombinationen Skift + Retur för att lägga till en ny post (eller rad) i tabellen.

Mer information finns i [Skapa poster](../maestro/records/connect-records.md).

## Vecka 16 oktober 2023

### Ny personfältstyp

Förhandsgranska och produktion: 16 oktober 2023

Nu kan du lägga till ett fält av typen Personer i Maestro-posttyper. Du kan använda fält av typen Personer för att associera befintliga användare med en post. Mer information finns i [Skapa fält](../maestro/fields/create-fields.md).

### RTF-format för styckefält

Förhandsgranska och produktion: 16 oktober 2023

Vi har lagt till kontroller för Rich Text-format för stycketextfält. Du kan formatera styckefält med RTF-text antingen i tabellvyn för en posttyp eller på detaljsidan för en post. Mer information finns i [Redigera poster](../maestro/records/edit-records.md).


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

Mer information finns i [Hantera tidslinjevyn](../maestro/views/manage-the-timeline-view.md).

## Vecka 9 oktober 2023

### Sök i tabellvy

Förhandsgranskning och produktion: 9 oktober 2023

Nu kan du söka efter ett nyckelord för att snabbt hitta en post i tabellvyn. Du kan använda nyckelord och specialtecken i alla fält som visas på skärmen för att hitta en post. Mer information finns i [Hantera tabellvyn](../maestro/views/manage-the-table-view.md).

## Vecka 18 september 2023

### Ordna om rader

Förhandsgranska och produktion: 20 september 2023

Du kan nu ändra ordningen på en eller flera rader (eller poster) i tabellvyn på en posttypsida. Mer information finns i [Hantera tabellvyn](../maestro/views/manage-the-table-view.md).

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

   * [Koppla posttyper](../maestro/architecture/connect-record-types.md)
   * [Koppla poster](../maestro/records/connect-records.md)

### URL-stöd för enkelradiga textfält

Förhandsgranska och produktion: 7 september 2023

För bättre synlighet när du arbetar med länkar i tabellvyn har vi lagt till stöd för URL-adresser i enkelradiga textfält. När du använder URL:er till andra webbplatser eller externa enheter när du uppdaterar ett textfält med en rad identifieras de nu som länkar och du kan klicka på dem från tabellen. Före den här förbättringen visas länkar som text.

## Vecka 28 augusti 2023

### Fältsynlighetsmeny för verktygsfältet Tabellvy

Förhandsgranskning och produktion: 31 augusti 2023

Om du vill visa rätt information för en viss postuppsättning, särskilt om du tänker dela vyn med andra som måste se vissa men inte alla fält av en posttyp, kan du nu välja vilka fält (eller kolumner) som ska visas och vilka som ska döljas i tabellvyn.

Du kan dölja eller visa enskilda fält från varje rubrik i fältkolumnerna, eller hantera alla fält av posttyp från en inställning i verktygsfältet för tabellvyn.

Mer information finns i [Hantera tabellvyn](../maestro/views/manage-the-table-view.md).

## Vecka 21 augusti 2023

### Koppla ihop Maestro-poster med program och portfolior

Förhandsgranska och produktion: 24 augusti 2023

Nu kan du koppla samman en Maestro-post med Workfront program och portfolior. Du måste skapa en anslutning mellan en Maestro-posttyp och ett program eller en portfölj som skapar ett anslutet fält. Sedan kan du koppla alla Maestro-poster från alla andra posttyper inom samma arbetsyta till specifika program och portföljer som skapar en skrivskyddad posttyp för Workfront eller Workfront Portfolio i samma arbetsyta. Tänk på följande:

* Posttyper för Workfront-anslutning är unika för varje arbetsyta.
* Du kan koppla flera Maestro-poster till samma Workfront-program eller portfölj, samt flera program och portföljer till samma Maestro-post.
* Du kan inte redigera program och portföljer i Maestro. Alla program- och portföljändringar som görs i Workfront visas i Maestro när de länkade posterna granskas.

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

Nu kan du ändra ordning på kolumner i tabellvyn i maestro. Tänk på följande när du ändrar ordning på kolumner:

* Fältet Namn är alltid det första fältet i tabellvyn för en posttypsida

* Du kan inte flytta namnfältet till en annan position

* Fältet Namn är fryst och ingår inte i den vågräta rullningen.

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

Förhandsgranska och produktion: 31 maj 2023

Du måste ha minst två datumfält associerade med en posttyp för att kunna skapa en tidslinjevy.

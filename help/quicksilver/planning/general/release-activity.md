---
title: Adobe Workfront Planerar aktuell versionsaktivitet
description: Adobe Workfront Planning-funktionerna är för närvarande tillgängliga för vissa Workfront-kunder. Läs den här artikeln ofta och lär dig mer om de funktioner som nyligen släppts för planeringsfunktionerna.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 53911aa3-74fd-4747-9008-f86a521ffba6
source-git-commit: 78e9c4d4ddee8f44d6fafe218c6a9b8c2cb28bf5
workflow-type: tm+mt
source-wordcount: '5786'
ht-degree: 0%

---


# Adobe Workfront Planerar aktuell versionsaktivitet

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
>I vissa fall kan den dokumentation som beskrivs i avsnitten nedan vara tillgänglig efter att de dokumenterade funktionerna släppts till Produktion.

I den här artikeln listas de funktioner som släppts till Workfront Planning under 2024.

Workfront planeringsprogram har startat sedan 22 maj 2023. En lista över alla funktioner som släpptes under 2023 finns i [Aktivitetsarkiv för Adobe Workfront Planning (Planering - lansering) för 2023](/help/quicksilver/planning/general/release-activity-archives-2023.md).

De släppta funktionerna listas i den ordning de släpps, med den senaste först. Kunder som deltar i Workfront Planning Program har tillgång till alla funktioner i produktionsmiljön.

Workfront Planning har tillfälligt tagits bort från förhandsgransknings- och sandlådemiljöerna sedan januari 2024. Alla funktioner som beskrivs i de här artiklarna är för närvarande tillgängliga i Produktion.

## Vecka 29 juli 2024

### Adobe Workfront Planning Public API är nu tillgängligt

Produktion: 30 juli 2024

Förhandsgranska: Ska bestämmas

Adobe Workfront Planning Public API är nu tillgängligt.

Mer information finns i [Grunderna i Adobe Workfront Planning API](/help/quicksilver/planning/general/planning-api-basics.md).

### Infoga och duplicera poster i tabellvyn

Produktion: 1 augusti 2024
Förhandsgranska: Ska bestämmas

Vi har introducerat följande funktioner när vi arbetar med poster i tabellvyn:

* Duplicera poster: du kan snabbt skapa en post genom att duplicera en befintlig.  En identisk post skapas. Den här funktionen är bara tillgänglig i tabellvyn.

* Du kan infoga en ny post ovanför eller under en befintlig post i tabellvyn. Före den här förbättringen lägger du bara till poster längst ned i tabellvyn.

Du kan utföra de nya funktionerna i följande områden:

* Menyn Mer för en post

* Det nya verktygsfältet som har lagts till längst ned på postsidan i tabellvyn

Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md)

### Dela Workfront Planning-vyer offentligt

Produktion: 2 augusti 2024

Förhandsgranska: Ska bestämmas

Om du vill arbeta smidigt med externa intressenter kan du nu dela postvyer med andra utanför organisationen. Du kan dela en offentlig länk till den vy du vill att andra ska ha tillgång till.

Följande funktioner ingår i uppdateringen:

* Dela vyn över en posttypssida med en offentlig länk som skulle ha upphört att gälla ett visst datum.

* Den delade länken är tillgänglig för alla utanför företaget under en begränsad tid, vilket anges med utgångsdatumet. Det krävs ingen inloggning för att visa den delade vyn.

* Personer som kommer åt vyn från den offentliga länken kan inte skapa andra vyer, redigera den delade vyn eller lägga till, ta bort eller redigera postinformation.

Mer information finns i [Dela vyer](/help/quicksilver/planning/access/share-views.md).

## 8 juli 2024

### Öppna uppkopplade objekt direkt i Workfront

Produktion: 9 juli 2024

Förhandsgranska: Ska bestämmas

Vi har tagit bort ett steg när vi använde Workfront-objekt som var kopplade till Workfront Planning-poster.

När du klickar på namnet på ett Workfront-objekt från den Planning-post som är kopplad till det, öppnar du Workfront objektsida. Före den här förbättringen skulle en skrivskyddad Workfront Planning-sida för det anslutna Workfront-objektet öppnas där du kan navigera vidare till Workfront objektsida.

Mer information finns i [Anslut poster](/help/quicksilver/planning/records/connect-records.md).

### Endast användare med Standard eller Plan kan skapa vyer

Produktion: 11 juli 2024

Förhandsgranska: Ska bestämmas

Vi har ändrat vilka typer av användare som kan skapa vyer. Nu kan bara användare med Standard eller Plan skapa vyer. Alla andra användare har skrivskyddad åtkomst till vyer som delas med dem. Före uppdateringen kunde användare med Light- och Worker-licens skapa vyer.

Mer information finns i [Översikt över licenstyper vid användning av Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).

### Sortera och gruppera poster efter sökfält med flera värden

Produktion: 11 juli 2024

Förhandsgranska: Ska bestämmas

Nu kan du sortera och gruppera poster i vilken vy som helst med sökfält med flera värden som inte är summerade. Före den här förbättringen kunde du bara sortera och gruppera efter uppslagsfält som var summerade.

Om sökfältet innehåller flera värden bör du tänka på följande:

* Sorteringen görs med det första värdet

* Posterna grupperas efter varje unik kombination av fältvärden

* Tidslinjen byggs utifrån det första datumvärdet.

Mer information finns i följande artiklar:

* [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md)
* [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md).


## Vecka 24 juni 2024

### Workfront AI Assistant (beta) finns nu för Workfront Planning

AI Assistant (beta) finns nu för Workfront Planning.

AI-assistenten fungerar tillsammans med den valda sidan och med din åtkomst- och behörighetsnivå för att utföra följande åtgärder: generera, uppdatera, ta bort eller återställa poster.

AI-assistenten är för närvarande i en betafas och är tillgänglig för utvalda kunder. Kontakta din kontorepresentant för att få veta om du är berättigad att delta i den här fasen.

Mer information finns i [Översikt över Adobe Workfront Planning AI Assistant](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).

### Ny sökruta när du väljer en arbetsyta eller posttyp

Produktion: 27 juni 2024

Förhandsgranska: Ska bestämmas

Om du vill göra det enklare att navigera mellan arbetsytor eller mellan posttyper kan du nu söka efter en arbetsyta eller en posttyp på den nedrullningsbara menyn till höger om deras namn i sidhuvudet.

Mer information finns i [Redigera posttyper](/help/quicksilver/planning/architecture/edit-record-types.md).

### Infoga ett nytt fält till höger eller vänster om ett befintligt fält i tabellvyn

Produktion: 27 juni 2024

Förhandsgranska: Ska bestämmas

För att förbättra och snabba upp upplevelsen i posttabellvyn har vi lagt till möjligheten att lägga till ett nytt fält mellan två kolumner genom att infoga det till höger eller vänster om en befintlig.

Mer information finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

## Vecka 17 juni 2024

### Uppdaterat utseende och känsla på detaljsidan

Produktion: 17 juni 2024

Förhandsgranska: Ska bestämmas

Vi har uppdaterat utseendet och känslan på detaljsidan med register. Som en del av den här uppdateringen har fältikonerna tagits bort.

Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

### Uppdaterade arbetsytemallar

Produktion: 17 juni 2024

Förhandsgranska: Ska bestämmas

Vi har uppdaterat utseendet och fältet för arbetsytans mallkort i Workfront Planning.

Uppdateringen innehåller följande förbättringar:

* Posttyperna som tillhör varje mall visas som kort.

* Vi har tagit bort mallen för marknadsföringshantering. Vi har lagt till följande mallar för marknadsföring och vi rekommenderar att du använder rätt mallar beroende på hur komplexa dina arbetsflöden är:

   * Grundläggande: Marknadsföringshantering
   * Avancerat: Marknadsföringshantering
   * Enterprise: Marketing Management

Mer information finns i följande artiklar:

* [Lista över arbetsytemallar](/help/quicksilver/planning/architecture/workspace-templates.md)

* [Skapa arbetsytor](/help/quicksilver/planning/architecture/create-workspaces.md)

### Ny upplevelse när du lägger till en miniatyrbild eller en omslagsbild i en post

Produktion: 17 juni 2024

Förhandsgranska: Ska bestämmas

Vi har uppdaterat funktionen att lägga till en miniatyrbild eller omslagsbild till en post från informationssidan. Förbättringarna omfattar följande uppdateringar:

* En miniatyrbild och en omslagsbild tilldelas automatiskt till en post när du skapar den. Du kan redigera dessa bilder senare.

* Du kan lägga till en miniatyrbild från detaljsidan. Före den här förbättringen kunde du bara lägga till en miniatyrbild från tabellvyn.

* Du kan bläddra i ett galleri med bilder för att välja en bild som omslag eller miniatyrbild för en post. Före den här förbättringen kunde du bara överföra din egen bildfil.

Mer information finns i följande artiklar:

* [Lägg till en omslagsbild i en post](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)

* [Lägg till en miniatyrbild i en post](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

### Uppdatera postens titel på informationssidan

Produktion: 17 juni 2024

Förhandsgranska: Ska bestämmas

Titeln på en posts informationssida visar det primära fältet för en post. Före den här uppdateringen visades namnet på posten på en posts informationssida. Du kan redigera den infogade titeln på sidan Detaljer, såvida inte det primära fältet är ett formeltypsfält.

Mer information finns i följande artiklar:

* [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md)

* [Redigera poster](/help/quicksilver/planning/records/edit-records.md)

### Lägga till länken Visa mer/Visa mindre i de anslutna postfälten

Produktion: 17 juni 2024

Förhandsgranska: Ska bestämmas

Vi har lagt till länken Visa mer/Visa mindre i ett anslutet postfält, när det finns poster som annars skulle visas på mer än två rader på detaljsidan för en post.

Mer information finns i [Anslut poster](/help/quicksilver/planning/records/connect-records.md).

### Fyll i namnfältet automatiskt med postnamnet vid anslutning av posttyper

Produktion: 20 juni 2024

Förhandsgranska: Ska bestämmas

När du skapar en anslutning mellan två poster eller mellan en post och ett objekt från ett annat program fylls anslutningsfältets namn automatiskt i med namnet på den anslutna posten. Före den här förbättringen var du tvungen att lägga till ett namn för anslutningsfältet manuellt.

Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).

### Definiera hur kopplade poster visas i anslutna fält

Produktion: 20 juni 2024

Förhandsgranska: Ska bestämmas

Nu kan du bestämma hur kopplade poster ska visas i anslutna fält. När du lägger till en ny anslutning till en posttyp kan du nu välja att visa den anslutna postens titel och dess miniatyrbild eller bara miniatyrbilden.

En posts titel är antingen postens namn eller ett fält som är angivet som primärt fält i posttypens tabellvy.

Den här förbättringen är tillgänglig för poster som är kopplade från Workfront Planning och för resurser som är kopplade från Adobe Experience Manager.

Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).

### Endast användare med Standard eller Plan har behörighet att hantera arbetsytor (titel)

Produktion: 21 juni 2024

Förhandsgranska: Ska bestämmas

Vi har ändrat vilka typer av användare som kan ha fullständig åtkomst till arbetsytor. Nu kan bara användare med Standard- eller Plan-licens ha Hantera-behörighet till arbetsytor. Åtkomsten till posttyper, poster och fält ärvs från en arbetsyta. Alla andra användare har skrivskyddad åtkomst till arbetsytor och deras objekttyper. Innan den här uppdateringen kunde användare med Light- och Worker-licens få Contribute-behörigheter till arbetsytorna.

Mer information finns i [Översikt över licenstyper vid användning av Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).

## Vecka 10 juni 2024

### Upp till 4-nivåreferens för postsökningsfält

Produktion: 12 juni 2024

Förhandsgranska: Ska bestämmas

Nu kan du referera till fält som ligger upp till 4 nivåer från posten när du skapar något av följande:

* Filter

* Sortera

* Gruppering

* Formelfält

Mer information finns i följande artiklar:

* [Skapa fält](/help/quicksilver/planning/fields/create-fields.md)

* [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md)

## Vecka 3 juni 2024

### Ny landningssida för Workfront Planning

Produktion: 7 juni 2024

Förhandsgranska: Ska bestämmas

Vi presenterar en ny landningssida för Workfront Planning när du har klickat på Planning på Main Menu (Planning).

En del av informationen på landningssidan innehåller följande:

* Ett område som visar dina arbetsytor och arbetsytor som delas med dig. Arbetsytans ägare visas på varje arbetsytekort.

* Om du är Workfront-administratör visas följande flikar:

   * Mina arbetsytor: Visar endast arbetsytor som du har skapat.

   * Andra arbetsytor: Visar arbetsytor som du har skapat eller som delas med dig.

* Länkar till dokumentation och publiceringsaktivitet för Workfront Planning

* Kom igång självstudiekurs om Workfront Planning

Mer information finns i [Översikt över Adobe Workfront-planering](/help/quicksilver/planning/general/planning-overview.md).

### Ny startupplevelse för Workfront Planning

Produktion: 7 juni 2024

Förhandsgranska: Ska bestämmas

När nya användare använder Workfront Planning för första gången får de nu ett välkomnande av en självmant självstudiekurs som vägleder dem genom enkla arbetsmoment och definierar de huvudsakliga begreppen för lösningen.

Du kan gå igenom introduktionsprocessen, slutföra uppgifterna eller minimera den och gå tillbaka till den vid ett senare tillfälle.

## Vecka 27 maj 2024

### Introducing the UNIQUE rollup operator for lookup fields

Produktion: 27 maj 2024

Förhandsgranska: Ska bestämmas

Vi har lagt till UNIQUE-operatorn när sökfältvärden sammanställs.

Operatorn UNIQUE tar bort dubbletter från sökfältvärden och bara visar ett unikt värde. Om du till exempel lägger till flera kopplade poster och värdena för ett uppslagsfält är identiska mellan flera poster, visar Workfront bara ett av värdena i uppslagsfältet för den ursprungliga posten.

Operatorn UNIQUE är tillgänglig för alla fälttyper förutom följande:

* Stycke
* Folk
* Kryssrutefält

Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).

### Dela vyer med alla medlemmar på en arbetsyta som standard

Produktion: 30 maj 2024

Förhandsgranska: Ska bestämmas

Vi har nu introducerat ett alternativ där du snabbt kan ge alla medlemmar på en arbetsyta behörigheten Visa. Före den här förbättringen kunde endast användare som du delat en vy med få åtkomst till vyn. Det här alternativet är inte aktiverat som standard.

Mer information finns i [Dela vyer](/help/quicksilver/planning/access/share-views.md).

### Uppdaterat utseende på planeringsikonen på huvudmenyn

Produktion: 30 maj 2024

Förhandsgranska: Ska bestämmas

Vi har uppdaterat utseendet på ikonen för planeringsområdet på huvudmenyn. Mer information finns i [Översikt över Adobe Workfront-planering](/help/quicksilver/planning/general/planning-overview.md).

### Byta namn på Workfront Planning Program

Från och med 30 maj 2024 går Adobe Workfront Planning-programmet över från betaversionen till ett tidigt skede. Du kommer att se den här ändringen i terminologin i vår dokumentation.

Åtkomststeget i förtid är också begränsat till ett fåtal Workfront-kunder.

Din kontorepresentant kommer att informera dig om du är berättigad att delta i ett tidigt skede av processen.

### Ny process för att ta bort en arbetsyta

Produktion: 30 maj 2024

Förhandsgranska: Ska bestämmas

Eftersom effekten av att ta bort en arbetsyta kan vara betydande lägger vi till ett extra steg för att bekräfta borttagningen. Användarna måste nu skriva&quot;delete&quot; innan de kan slutföra den permanenta borttagningen av en arbetsyta.

Borttagna arbetsytor och deras information kan inte återställas.

Mer information finns i [Ta bort arbetsytor](/help/quicksilver/planning/architecture/delete-workspaces.md).

### Uppslagsdatumfält är nu tillgängliga i tidslinjevyn

Produktion: 31 maj 2024

Förhandsgranska: Ska bestämmas

Du kan nu ställa in start- och slutdatum för tidslinjevyn på ett uppslagsfält från en ansluten post eller objekttyp.

Mer information om hur du skapar vyer finns i [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).

## Vecka 20 maj 2024

### Koppla ihop Workfront Planning-poster från Workfront-objekt med Planning-avsnittet

Produktion: 23 maj 2024

Förhandsgranska: Ska bestämmas

Vi har lagt till en ny planeringssektion i den vänstra panelen av Workfront projekt, portfolior och program. I det nya Planning-avsnittet visas de Workfront Planning-poster som är kopplade till Workfront-objektet.

Följande åtgärder är tillgängliga under Planning i Workfront:

* Visa anslutna planeringsposter

* Koppla Workfront Planning-poster till Workfront-objektet

* Koppla från poster

* Öppna förhandsgranskningsrutan eller -sidan med information om du vill visa mer information om de anslutna posterna

Mer information finns i [Hantera poster i planeringsavsnittet för Adobe Workfront-objekt](/help/quicksilver/planning/records/manage-records-in-planning-section.md).

## Vecka 13 maj 2024

### Uppdateringar i realtid i tidslinjevyn efter redigering av poster

Produktion: 14 maj 2024

Förhandsgranska: För bestämning.

När en användare uppdaterar informationen på en post kan andra användare visa den uppdaterade informationen i postens tidslinjevy i realtid. Detta garanterar att alla användare ser den uppdaterade informationen samtidigt, synkroniserat med när ändringarna inträffar.

### Lägg till post från vyhuvudet

Produktion: 14 maj 2024

Förhandsgranska: Ska bestämmas

Vi har lagt till en ny postknapp i huvudet på en posttypssida. Nu kan du skapa poster från vilken vy som helst. Före den här förbättringen kunde du bara skapa poster från tabellvyn.

Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).


### Ny varning om objektsynlighet vid anslutning av poster

Produktion: 15 maj 2024

Förhandsgranska: Ska bestämmas

När du skapar anslutningar till objekttyper utanför Workfront Planning får du nu ett meddelande om att alla som arbetar på den aktuella arbetsytan kommer att ha synlighet för alla länkade objekt och deras sökfält, oavsett deras behörigheter och åtkomstnivåer i det andra programmet.

Om du till exempel länkar projekt från Workfront Planning-kampanjer får alla som har tillgång till Visa kampanjen även tillgång till de länkade projekten och informationen från deras sökfält, även om de inte har någon behörighet till de länkade projekten eller tillgång till projekt i allmänhet. Du får åtkomst till Planning-poster när du får behörighet till arbetsytor.

Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).

### Lägga till avsnitt på postens förhandsgransknings- och informationssidor

Produktion: 15 maj 2024

Förhandsgranska: Ska bestämmas

För att bättre kunna organisera information på postens sida, för effektivare läsbarhet och navigering, har vi skapat avsnitt på postens sida. Avsnittsrubrikerna fungerar som rubriker som organiserar fälten i olika kategorier. Avsnitten är helt anpassningsbara och kan expanderas eller komprimeras om det behövs.

Mer information finns i [Hantera postsidans layout](/help/quicksilver/planning/records/manage-the-record-page.md).

### Realtidsuppdateringar för fältkonfigurationsändringar

Produktion: 16 maj 2024

Förhandsgranska: Ska bestämmas

När en användare ändrar en fältkonfiguration (namn, beskrivning, alternativlista osv) i en posttyp, visar andra användare dessa ändringar i realtid. På så sätt ser du till att alla tittar på rätt fält och deras information samtidigt.

>[!WARNING]
>
>När formeluttryck ändras, eller alternativ läggs till eller tas bort från ett urvalsfält, försvinner data för de poster som redan har information lagrad i de fält vars konfiguration ändras.
>
>Det finns ingen varning eller indikation om att denna dataförlust kan inträffa när du ändrar fältkonfigurationen.
>
>Det finns inget meddelande till andra användare om att fältkonfigurationen har ändrats.

Mer information finns i [Redigera fältinställningar](/help/quicksilver/planning/fields/edit-fields.md).

## Vecka 6 maj 2024

### Uppdaterat utseende på posttypkorten på en arbetsyta

Produktion: 7 maj 2024

Förhandsgranska: Ska bestämmas

Vi har uppdaterat utseendet på posttypkort när vi tittar på dem i en arbetsyta. Uppdateringarna omfattar:

* Borttagning av antalet fält och anslutningar för varje posttyp

* Tillägg av posttypens beskrivning

Mer information finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

### Aktivera Workfront Planning-meddelanden för Adobe Unified Experience-kunder

Produktion: 8 maj 2024

Förhandsgranska: För att bestämma

Om du är kund i Adobe Unified Experience och någon lägger till dig i en kommentar på postsidan får du ett meddelande i appen och ett e-postmeddelande om kommentaren. Du kan hantera dina meddelandeinställningar under Inställningar i din Adobe Experience Cloud-profil. Mer information finns i [Kontoinställningar och meddelanden](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences).

Mer information om Workfront planeringsmeddelanden finns i [Adobe Workfront Planning-meddelanden: Artikelindex](/help/quicksilver/planning/notifications/notifications-information.md).


## Vecka 29 april 2029

### Uppdateringar i realtid i rutan med postinformation och sidan efter redigering av poster i tabellvyn

Produktion: 2 maj 2024

Förhandsgranska: Ska bestämmas

När en användare uppdaterar informationen på en post i tabellvyn kan andra användare visa den uppdaterade informationen i postens informationsruta (inuti en vy) eller sida i realtid. Detta garanterar att alla användare ser den uppdaterade informationen samtidigt, synkroniserat med när ändringarna inträffar.

Mer information om hur du redigerar poster finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

### Uppdateringar i realtid i kalendervyn efter redigering av poster

Produktion: 3 maj 2024

Förhandsgranska: För bestämning.

När en användare uppdaterar informationen på en post kan andra användare visa den uppdaterade informationen i postens kalendervy i realtid. Detta garanterar att alla användare ser den uppdaterade informationen samtidigt, synkroniserat med när ändringarna inträffar.

## Vecka 22 april 2024

### Uppdaterat arbetsflöde vid redigering av en arbetsyta eller posttyp

Produktion: 23 april 2024

Förhandsgranska: Ska bestämmas

Vi har uppdaterat utseendet på arbetsytan Editor och rutan Redigera posttyp.

När du redigerar en arbetsyta eller en posttyp kan du nu definiera ett namn, en beskrivning och tilldela en färg och en ikon till dem.

Mer information finns i följande artiklar:

* [Redigera arbetsytor](/help/quicksilver/planning/architecture/edit-workspaces.md)

* [Redigera posttyper](/help/quicksilver/planning/architecture/edit-record-types.md).

## 8 april 2024

### Kopiera innehållet i en cell och klistra in det i flera markerade celler

Produktion: 10 april 2024

Förhandsgranska: Ska bestämmas

Nu kan du kopiera innehållet i en cell i tabellvyn och klistra in det i flera markerade celler. Du kan också kopiera information från externa källor och klistra in den i tabellvycellerna.

Den här funktionen stöds för alla fälttyper utom för beräknade fält.

Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

## Vecka 1 april 2024

### Ändra ordning på fälten på postsidor

Produktion: 4 april 2024

Förhandsgranska: Ska bestämmas

Som Workspace-chef kan du nu ändra ordning på fälten på postsidan eller förhandsgranskningen. Om du uppdaterar fältordningen ändras fältordningen för alla poster av samma typ, så att alla kan visa postsidan eller postförhandsvisningen.

Mer information finns i [Hantera postsidans layout](/help/quicksilver/planning/records/manage-the-record-page.md).


### Lägg till omslagsbild för att spela in sidor

Produktion: 4 april 2024

Förhandsgranska: Ska bestämmas

När du hanterar postsidor kan du nu lägga till, flytta om och ersätta en omslagsbild på en postsida eller förhandsgranskning för att berika postens presentation och intressenternas engagemang. Omslagsbilder är synliga för alla användare som visar posterna.

Mer information finns i [Hantera postsidans layout](/help/quicksilver/planning/records/manage-the-record-page.md).

## Vecka 25 mars 2024

### Ny flexibel posttypsorganisation för arbetsytor

Produktion: 25 mars 2024

Förhandsgranska: Ska bestämmas

För att du ska bli effektiv när du skapar arbetsytor har vi ändrat sättet att organisera posttyper i en arbetsyta. Några av förbättringarna är:

* Skapa upp till 50 avsnitt med posttyper på varje arbetsyta. Befintliga användningsposttyper och taxonomier-avsnitt finns kvar på de befintliga arbetsytorna.

* Anpassa alla nya arbetsytor och deras nya avsnitt efter era processer och organisationens behov.

* Flytta posttyper dynamiskt inom en arbetsyta genom att dra och släppa dem där de behöver vara, inklusive mellan olika avsnitt.

Mer information finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

### Duplicera vyer

Produktion: 25 mars 2024

Förhandsgranska: Ska bestämmas

För att spara tid och enhetlighet kan du nu duplicera en befintlig vy som du har åtkomstbehörighet till.

När du duplicerar en vy skapas en identisk vy med samma filter, sorteringsvillkor och grupperingar. Behörigheterna för den ursprungliga vyn behålls inte när du duplicerar en vy.

Mer information finns i [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).

### Namnet på Maestro-området på huvudmenyn har ändrats till Planning

Produktion: 27 mars 2024

Förhandsgranska: Ska bestämmas

Vi har bytt namn på Maestro-området på Main Menu till Planning.

En översikt över Adobe Workfront Planning finns i [Översikt över Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

### Ny upplevelse när en posttyp tas bort

Produktion: 27 mars 2024

Förhandsgranska: Ska bestämmas

Vi har gjort om bekräftelserutan när vi tar bort en posttyp. Det är viktigt att du tar bort en posttyp eftersom alla poster, fält, information i fälten samt vyer som är kopplade till posttypen också tas bort. Borttagna posttyper och borttagen information kan inte återställas.

Av den anledningen vill vi se till att användarens avsikt är korrekt när en posttyp tas bort, så vi har tagit ett extra steg för att bekräfta borttagningen. Mer information finns i [Ta bort posttyper](/help/quicksilver/planning/architecture/delete-record-types.md).

## Vecka 18 mars 2024

### Filter som är tillgängliga i kalendervyn

Produktion: 19 mars 2024

Förhandsgranska: Ska bestämmas

Nu kan du filtrera information i kalendervyn. Mer information finns i [Hantera kalendervyn](/help/quicksilver/planning/views/manage-the-calendar-view.md).

### Förhandsgranska med postinformation tillagd i tidslinjen och kalendervyer

Produktion: 19 mars 2024

Förhandsgranska: Ska bestämmas

Du kan nu komma åt förhandsgranskningen med postinformation från tidslinjen och kalendervyer. Du kan redigera poster i postens förhandsvisningsruta i tidslinjen och kalendervyer.

Från postens förhandsgranskning kan du öppna postsidan på en ny webbläsarflik.

Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

### Posttypen Excel-import är tillfälligt inaktiverad

Produktion: 21 mars 2024

Förhandsgranska: Ska bestämmas

Vi inaktiverar temporärt import av posttyper med hjälp av en Excel- eller CSV-fil. Den här funktionen kommer att vara tillgänglig vid ett senare tillfälle.

## Vecka 11 mars 2024

### I korthet visas postdetaljer i tabellvyn

Produktion: 14 mars 2024

Förhandsgranska: Ska bestämmas

För att göra det enklare att visa ytterligare information om poster när du använder tabellvyn har vi introducerat en ny förhandsvisning av detaljer som visar en snabb vy av postens detaljer. Nedan följer en del av informationen som ingår i postförhandsgranskningen:

* Relevanta postdetaljer i korthet

* Möjlighet att ändra postinformation

* En länk för att öppna postens sida

Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

### Ny flikdesign för postvyer

Produktion: 14 mars 2024

Förhandsgranska: Ska bestämmas

För bättre navigering och användarvänlighet har vi omdesignat visningen av postvyer. Vyerna visas nu vågrätt som flikar på posttypssidan, så att du enkelt kan navigera mellan dem. Före den här förbättringen visas vyer i listrutan Visa.

Vyer visas kronologiskt efter tillagda datum från vänster till höger. Delade vyer visas också i kronologisk ordning efter när de delades.

Mer information finns i [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).

### Dynamisk design av en postvy

Produktion: 14 mars 2024
Förhandsgranska: Ska bestämmas

Vi har uppdaterat vyernas utseende och känsla på posttypssidan. De nya vyerna är dynamiskt responsiva och justeras snabbt till skärmstorleken. Alternativetiketterna för verktygsfält är dolda på mindre skärmar för att göra verktygsfältet enklare att använda.

Mer information finns i följande artiklar:

* [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md)
* [Hantera tidslinjevyn](/help/quicksilver/planning/views/manage-the-timeline-view.md).

### Tillåt systemadministratörer att hantera alla delade vyer

Produktion: 14 mars 2024

Förhandsgranska: Ska bestämmas

För att vara konsekvent med alla andra områden i systemet och för att kunna underhålla och styra alla vyer som är tillgängliga för dig som systemadministratör har du nu behörigheten Hantera för alla vyer som delas med dig på posttypssidan. Före den här förbättringen kunde vyskaparna ha gett dig behörighet att visa eller hantera vyn. Om vyn delas med dig och du är systemadministratör får du som standard behörigheten Hantera för vyn.

Mer information finns i [Dela vyer](/help/quicksilver/planning/access/share-views.md).

### Obehörig sida vid delning av vy utan behörighet

Produktion: 14 mars 2024

Förhandsgranska: Ska bestämmas

När en användare tar emot en länk till en posttyp och har åtkomst till arbetsytan men inte till den vy som delas i länken, visas en sida som meddelar användaren om att användaren inte har behörighet att se posttypen.

Mer information finns i [Dela vyer](/help/quicksilver/planning/access/share-views.md).


### Ny etikett för systemadministratörer i delade dialogrutor

Produktion: 14 mars 2024

Förhandsgranska: Ska bestämmas

Nu visas en&quot;Admin&quot;-etikett bredvid systemadministratörens namn i delningsdialogrutan när du delar en vy eller arbetsyta.

Mer information finns i [Översikt över delningsbehörigheter](/help/quicksilver/planning/access/sharing-permissions-overview.md).

### Obehörig sida vid delning av vy utan behörighet

Produktion: 14 mars 2024

Förhandsgranska: Ska bestämmas

När en användare tar emot en länk till en posttyp och har åtkomst till arbetsytan men inte till den vy som delas i länken, visas en sida som meddelar användaren om att användaren inte har behörighet att se posttypen.

Du måste dela vyer förutom att dela arbetsytor så att andra kan komma åt samma posttypssida som du delar med en länk.

Mer information finns i [Dela vyer](/help/quicksilver/planning/access/share-views.md).

## Vecka 4 mars 2024

### Ändra radhöjd i tabellvyn

Produktion: 7 mars 2024

Förhandsgranska: Ska bestämmas

Nu kan du ändra höjden på en rad när du visar poster i tabellvyn.

Du kan uppdatera radhöjden till någon av följande storlekar:

* Kort
* Medium
* Hög.

Mer information finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md).

### Ny kalendervy för poster

Produktion: 7 mars 2024

Förhandsgranska: Ska bestämmas

Nu kan du visa poster i en kalendervy. Du måste ha minst två datumfält på en posttyp för att kunna skapa kalendervyn.

Mer information finns i [Hantera kalendervyn](/help/quicksilver/planning/views/manage-the-calendar-view.md).

## Vecka 26 februari 2024

### Filtrera, sortera och gruppera efter anslutna poster eller sökfält

Produktion: 28 februari 2024

Förhandsgranska: Ska bestämmas

Nu kan du filtrera, sortera och gruppera efter anslutna poster eller deras sökfält. Den här förbättringen hjälper dig att effektivt ordna och visualisera data i både tabell- och tidslinjevyer.

Du kan inte filtrera, sortera eller gruppera efter sökfält som tillåter anslutningar med flera poster.

Mer information finns i [Hantera tabellvyn](/help/quicksilver/planning/views/manage-the-table-view.md) och [Hantera tidslinjevyn](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Vecka 5 februari 2024

### Ändra behörigheter baserat på licenstyper

Produktion: 6 februari 2024

Förhandsgranska: Ska bestämmas

Vi har ändrat behörighetsnivåerna för att ta hänsyn till användarnas licenstyper. Före den här förbättringen fanns det inga skillnader i behörigheter för arbetsytan baserat på användarnas licenstyper.

Följande är de högsta behörighetsnivåerna som användare kan få baserat på användarens licenstyp:

* Användare med en planlicens (eller standardlicens, i den nya licensmodellen) kan skapa och hantera arbetsytor, posttyper och poster.

* Användare med en arbetslicens (eller Light, i den nya licensmodellen) kan visa och bidra till en arbetsyta som delas med dem, samt till den arbetsytans posttyper och poster.  Användare av Work- (eller Light-)-licensen kan också skapa, redigera och ta bort poster i arbetsytor där de har tillgång till Contribute.

* Användare med en licens för Granska eller Begärande (eller Medarbetare, i den nya licensmodellen) kan bara visa de arbetsytor som delas med dem, samt posttyperna och posterna för dessa arbetsytor. De kan inte skapa, redigera eller ta bort posttyper eller poster.

Mer information om den nya licensmodellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Mer information om anslutningen mellan licenstyp och behörigheter i planeringsfunktionerna finns i [Översikt över licenstypen när du använder Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).


### Nytt utseende och ny känsla i RTF-verktygsfältet för postfält

Produktion: 7 februari 2024

Förhandsgranska: Ska bestämmas

Vi har uppdaterat utseendet på verktygsfältet RTF när du redigerar ett stycketextfält.

Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

### Förbättrad upplevelse vid redigering av envalsfält, flervalsfält, personfält och när du lägger till anslutna objekt

Produktion: 8 februari 2024

Förhandsgranska: Ska bestämmas

Vi har gjort om och förbättrat upplevelsen av att lägga till alternativ eller objekt för följande fälttyper:

* Enkelval
* Flera val
* Folk
* Kopplade postfält (vid anslutning av posttyper för planeringsfunktioner eller Workfront-objekt)

Med den nya förbättringen visas en mindre, mer responsiv ruta först.

För anslutna fält kan du lägga till dem på något av följande sätt:

* Lägg till objekt i det anslutna fältet genom att söka efter och markera dem i en lista i tabellvyn, och redigera fältet textbundet
* Klicka för att öppna den större rutan Connect-objekt där du kan visa alla objektnamn förutom mer information om objekten.

Förbättringarna är nu tillgängliga när du uppdaterar fält i tabellvyn för en posttyp.

Mer information finns i [Anslut poster](/help/quicksilver/planning/records/connect-records.md).

## Vecka 29 januari 2024

### Förbättrad delning av vyer och arbetsytor

Produktion: 30 januari 2024

Förhandsgranska: Ska bestämmas

Vi har förbättrat delningen av arbetsytor och vyer med följande förbättringar:

* För att skapa tydlighet kring vad varje behörighetsnivå tillåter en användare att göra, har vi lagt till information för alla behörighetsnivåer när en arbetsyta och en vy delas.

* Nu kan du kopiera en länk till en arbetsyta eller vy och dela den med andra. Användarna måste ha minst behörigheten Visa på arbetsytan eller i vyn för att kunna komma åt dem från den kopierade länken.

Mer information finns i följande artiklar:

* [Dela arbetsytor](/help/quicksilver/planning/access/share-workspaces.md)
* [Visa](/help/quicksilver/planning/access/share-views.md)

### Lägga till miniatyrbilder i poster

Produktion: 1 februari 2024

Förhandsgranska: Ska bestämmas

Nu kan du lägga till enskilda miniatyrbilder till varje post för att skilja dem åt i en vy. I tabellvyn kan du lägga till bildfiler som du tidigare har sparat på datorn som miniatyrbilder. Miniatyrbilderna kan vara unika för varje post och visas i både tabell- och tidslinjevyerna på posttypsidan.

Mer information finns i [Lägga till en miniatyrbild i en post](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

### Ta bort anslutna posttypkort

Produktion: 1 februari 2024

Förhandsgranska: Ska bestämmas

För att undvika förvirring och förenkla hanteringen av arbetsytor har vi tagit bort de automatiskt genererade skrivskyddade posttypkorten för anslutna externa objekt från en arbetsyta.

Mer information finns i [Anslut poster](/help/quicksilver/planning/records/connect-records.md).

## Vecka 22 januari 2024

### Avsnittet Ny historik visar systemaktivitet för poster för planeringsfunktioner

Produktion: 25 januari 2024

Förhandsgranska: Ska bestämmas

För att förbättra granskningsfunktionerna har vi introducerat ett nytt avsnitt på den högra panelen i en post där du kan granska ändringar som gjorts i den post som spelats in av systemet.

Följande information registreras i det nya avsnittet Historik:

* Alla fältändringar

* De gamla och nya värdena i fälten när värdena ändras

* Det fullständiga namnet på användaren som gjorde ändringen

* En datum- och tidsstämpel som anger när ändringen inträffade.

Mer information finns i [Översikt över avsnittet Historik](/help/quicksilver/planning/records/history-section-overview.md).

### Ny etikett för ny postlänk

Produktion: 25 januari 2024

Förhandsgranska: Ska bestämmas

För att skapa konsekvens när du skapar poster har vi ändrat namnet på länken + Ny för att skapa poster till&quot;+ Ny post&quot;.  Före den här uppdateringen innehöll länken posttypens namn. Den nya länken är nu tillgänglig när du skapar operations- och taxonomiposter. Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).

## Vecka 8 januari 2024

### Planeringsfunktioner tas bort från förhandsgransknings- och sandlådemiljöer

Förhandsgranska och sandlåda: 11 januari 2024

Adobe Workfront Planning-funktionerna har tillfälligt tagits bort från förhandsgransknings- och sandlådemiljöerna. De kommer att läggas till i dessa miljöer vid ett senare tillfälle, som vi kommer att informera om i versionsinformationen.

### Planeringsfunktioner behörigheter för arbetsytor och vyer

Produktion: 11 januari 2024

Förhandsgranska: Ska bestämmas

Nu kan du dela en arbetsyta eller en vy med användare och grupper. Du kan ange deras behörigheter till olika nivåer beroende på vilken information de behöver för att visa eller redigera.

När du delar en arbetsyta har användarna behörighet till posttyperna, posterna och fälten på den arbetsytan.

När du delar en arbetsyta får användarna inte delningsbehörigheter till vyerna som är kopplade till posttyperna på arbetsytan. Du måste tilldela olika behörigheter till vyer.

Följande behörighetsnivåer gäller för arbetsytor:

* Visa: Användare kan visa arbetsytor som delas med dem. De kan även visa posttyper och poster från den delade arbetsytan.

* Contribute: Användare kan skapa, redigera eller ta bort poster på arbetsytan som delas med dem.  De kan inte skapa eller redigera posttyper eller arbetsytor som delas med dem.

* Hantera: Användare kan skapa, redigera och ta bort arbetsytor, posttyper, poster och fält på arbetsytor som delas med dem.

Följande behörighetsnivåer gäller för postvyer:

* Visa: Användare kan välja vyn i listrutan Visa på en posttypsida.
* Hantera: Användare kan redigera, dela och ta bort vyn.

Mer information finns i [Åtkomstöversikt](/help/quicksilver/planning/access/access-overview.md) och [Översikt över delningsbehörigheter i Adobe Workfront Planning-funktioner](/help/quicksilver/planning/access/sharing-permissions-overview.md).

### Ny formelfältstyp

Produktion: 11 januari 2024

Förhandsgranska: Ska bestämmas

Nu kan du lägga till ett formeltypsfält till en posttyp.

Formelfält genererar ett nytt värde med hjälp av befintliga värden från andra fält i en posttyp och en funktion som anger hur befintliga värden ska beräknas.

Du kan inte använda uppslagsfält från länkade posttyper i en formelberäkning. Den här funktionen kommer att vara tillgänglig vid ett senare tillfälle.

Mer information finns i [Översikt över formelfält](/help/quicksilver/planning/fields/formula-fields.md).

### Ångra/Gör om åtgärder vid hantering av poster i tabellvyn

Produktion: 11 januari 2024

Förhandsgranska: Ska bestämmas

Du kan nu ångra eller göra om dina ändringar när du utför följande åtgärder i tabellvyn:

* Kopiera/klistra in data
* Redigera post
* Lägg till post
* Ta bort post

Du kan använda följande tangenttryckningar för att ångra eller göra om åtgärder:

* Ångra: CTRL/CMD + Z
* Gör om: CTRL/CMD + Skift+Z

Mer information finns i följande artiklar:

* [Redigera poster](/help/quicksilver/planning/records/edit-records.md)

* [Ta bort poster](/help/quicksilver/planning/records/delete-records.md)

* [Skapa poster](/help/quicksilver/planning/records/create-records.md)



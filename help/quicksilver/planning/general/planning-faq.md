---
title: Vanliga frågor om Adobe Workfront Planning
description: Som marknadsledare kan ni använda Adobe Workfront Planning för att organisera arbetet under hela marknadsföringscykeln för alla era team. Det här är några vanliga frågor om Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 869a1f9e4fd7e3b65591050530b96d6dae9e230c
workflow-type: tm+mt
source-wordcount: '1630'
ht-degree: 0%

---


# Vanliga frågor om Adobe Workfront Planning

<!-- add to TOC and mini TOC-->

Den här artikeln innehåller en lista med de vanligaste frågorna om Adobe Workfront Planning.

Mer information om Workfront Planning finns i [Adobe Workfront Planning - översikt](/help/quicksilver/planning/general/planning-overview.md).

## Vad är Workfront Planning?

Workfront Planning, som tidigare kallades Project Maestro, är en ny funktion som gör det möjligt för team att centralisera sin planering för hela verksamheten, till exempel kampanjer, försäljning, produkthantering, tjänster med mera. Planeringen gör att du kan modellera ditt idealiska arkivsystem med anpassade register, flexibla anslutningsmöjligheter under hela livscykeln och förbättrad synlighet för alla intressenter.

## Hur passar Workfront in i den bredare Workfront-produkten?

Workfront Planning-modulen är en av tre distinkta, men sammankopplade, Workfront-funktioner som tillsammans skapar ett väl fungerande marknadsföringssystem. De tre funktionerna är:

* Planering: De nya avancerade funktionerna i Workfront Planning.

* Arbetsflöde: De samarbetsfunktioner för arbetshantering som du använder idag i Workfront (projekthantering, resurshantering osv.).

* Automatisering och integrering: De omfattande integrerings- och automatiseringsfunktionerna i Workfront Fusion.

## När kommer Workfront Planning att släppas?

Den senaste Workfront Planning-versionen för allmänheten är 28 augusti 2024. Aktuell information om vilka funktioner som är tillgängliga finns i [Adobe Workfront Planning - lanseringsaktivitet](/help/quicksilver/planning/general/release-activity.md).

<!-- To verify this: are we even saying "Beta"? - What happens after the beta program concludes? 

Beta participants that want to leverage Planning in production will be able to purchase it at the GA date. We encourage you to reach out to your sales rep to discuss further details. The environment used for the beta program is not in production and will not be migrated. The data stored in the beta environment will be available until December 2024. -->



KUNDFRÅGOR - SESSION #1 6/13



Processen med att skapa en översikt (AI använder sig av att dra in olika dokument för att dynamiskt skapa en översikt). Är det en del av betan?

Vi förväntar oss att den här funktionen kan testas.

Måste vi migreras till IMS?

Ja, kunder som vill köpa Planning måste migreras till ABP.

Kan du ge exempel på olika arbetsytor?

Du kan ha arbetsytor på olika nivåer, och på grund av systemets flexibilitet, som kan användas för flera syften på teamnivå och personlig nivå. Det primära användningsområdet är större centraliserade arbetsytor för organisationer. Några exempel på arbetsytor är: .......

Kan arbetsytor dela finansieringskonton?

Kan arbetsytor prata med varandra? Eller måste information anges på varje arbetsyta?

I det aktuella läget, finns det några mjuka begränsningar för antalet arbetsytor som kan konfigureras (dvs. försämras prestanda efter denna punkt)? Eventuella begränsningar för antalet arbetsytor som kan konfigureras (dvs. om systemet inte tillåter fler än detta #)?

Upp till 1 000 arbetsytor i din organisations Workfront-instans. Länk till dokument: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/create-workspaces

Kan aktuella objekt i systemet kopplas in eller måste allt detta byggas manuellt?

Du kan skapa anslutningar mellan en Planning-posttyp med WF-portföljer, program, projekt, grupper och företag. När du har upprättat en anslutning, till exempel med WF-projekt, kan du länka för poster i planeringsregistret med WF-projekt. Detta innebär att WF-objekt fortfarande skapas och hanteras i Workfront, men du kan justera dem mot planeringsposterna. Du har lite dokumentation här: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/connect-record-types, och vi planerar också att ha en feedback-session om anslutningar!

Från testning har jag lagt märke till att om du lägger till många poster blir det svårt att skilja mellan dem när de inte finns i tabellvyn. Finns det något sätt att göra poster olika färger? Det vore bra om du kunde göra dem färganpassade, så att de sticker ut från varandra i tidslinjen- och kalendervyerna.

Är människorna som tillhör Workfront eller IMS?

Workfront Instance

Kan dessa listor länkas till flera arbetsytor?

Vi planerar att länka posttyper mellan arbetsytor! Inte färdig än.

Är anpassade fält som du lägger till låsta till posttypen som de skapades under?

Det tillåter inte att jag skapar en anslutning till fälten Start/Slutdatum som är standard. Ska jag lägga till ett nytt om jag vill ansluta till ett fält som redan finns?

Finns det några planer för att hitta formatfält för extern sökning som fälttyp i Planning?

Finns det några planer på att bara ha fälten&quot;Skapad&quot;&quot;Skapad av&quot;&quot;Ändrad&quot; och&quot;Ändrad av&quot; som standard i poster - verkar som en förbrukning för fält som måste läggas till om vi vill spåra poster?

Eftersom modulen länkar till live-objekt i WF, kommer de att påverkas av planeringens betaaktiviteter?

Kommer vi att få uppdateringar för de ändringar som görs i Fusion eller är det något som hanteras separat?

Finns det några planer på att integrera med Canvas Dashboards? Hur rapporterar jag data?

Snart blir Dashboard Canvas snart tillgängligt för att visualisera planeringsdata

Kommer vi att kunna skapa arbetsytemallar?

Är den här taxonomin/poststrukturen ENDAST tillgänglig om du köper Planning?  En taxonomistruktur skulle vara fördelaktig även för vanliga Workfront-användare

Kommer administratörer att kunna skapa egna mallar?

Inte under betaversionen.

Har ni alla en dokumenterad och tillgänglig ERD för att dela för planeringsmodellen och posttyperna? Inte en ERD för tillfället, men vi har detaljerade hjälpartiklar som hjälper dig genom processen att skapa och ansluta posttyper: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/overview-of-record-types https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/connect-record-types

Så det var en gång (årspris) att använda PLANNING, och på den tiden kan vi lägga till så många användare som behövs? eller så debiteras vi per användare -

Planering är ett betalt erbjudande med ett måldatum som är den 28 augusti, den tidpunkt då du måste köpa Planning för att kunna använda det i produktionen. Kontakta din säljare om du vill ha mer information.

Är AI-aktivering endast tillgängligt för WF-systemadministratörer ELLER kan det aktiveras på specifika åtkomstnivåer ELLER kan det aktiveras för ENDAST specifika användare (1 eller 2)?

Först har bara administratörer för primära system åtkomst så att de kan konfigurera via åtkomstnivåer som i sin organisation får åtkomst till dem. Efter den 21 juni aktiverar vi AI för resten av organisationen och de får tillgång till eller inte beroende på konfigurationen som definieras av systemadministratören.

Var bor de FÄLT som skapats här? Kan befintliga FÄLT hämtas in från de som vi har skapat för andra objekt? Är de åtskilda från andra fält som skapas?

För närvarande finns fälten i den posttyp de är skapade i, men vi har ett högprioriterat initiativ för H2 &#39;24 att samla planerings- och Workfront-fälten i ett centraliserat fältbibliotek.

Kommer vi att kunna skapa rapporter baserat på de register/fält vi skapar i planeringen?

Ja! Kommer snart via Dashboard Canvas

Kommer vi att kunna hämta in dessa data även med API:t?

Ja! Vi har redan API:t tillgängligt och Fusion Connector.

Från en marknadsföringsarbetsyta - är det bäst att ha en masterarbetsyta att använda för ett globalt marknadsföringsteam ELLER är det bäst att ha individuella arbetsytor för varje affärsområde, land, varumärke osv. Jag såg att vi kan ha upp till 1 000 arbetsytor och kanske ansluta arbetsytor. är det möjligt att länka poster med arbetsytor? Användningsexempel - tillåt varje produkt en egen arbetsyta, men med delade posttyper. Och sedan vill vi se en delad vy som kombinerar allt.

Kan vi föra in Portfolio och Program till kampanjerna? Är det i sin tur projekt?

Kommer det att vara möjligt att länka projekt till poster i en arbetsyta när projektet skapas, utan att behöva gå till arbetsytan för att länka det?

För närvarande har vi Planering-avsnitt i projekt som visar alla anslutningsposter från Planning-posttyper. Du kan lägga till eller ta bort poster från dessa anslutningar. Vi kommer också snart att lägga till möjligheten att länka till poster i andra typer av Planning-poster, även om anslutningen för närvarande inte har några länkade poster.

Jag är medveten om att vi så småningom kommer att kunna ta emot information/data från någon utanför vår organisation. När kommer den här funktionen att bli tillgänglig i betaversionen?

Kan arbetsytan användas för resurs- och kapacitetsplanering per jobbroll i en kampanj?

Kan vi länka en arbetsytepost för att starta en begäran?

KONTORSTID 6/18

Möjlighet att länka datum till anslutna Workfront-data. Är det aktivt på alla nivåer (projekt, portfolior, program,..)?

Ja, det går att ansluta projekt via uppslagsfält.

Hur vet jag att det finns en allmän vy som är redo att visas?

Delade offentliga vyer visas

Hur delar du en vy internt?

Varje gång du skapar en ny arbetsyta måste du dela vyer igen?

Ja, varje gång du skapar en ny arbetsyta så att den blir en ny posttyp. Vyer är specifika för posttyper och du måste därför dela om dem.

Kan miniatyrer komma från innehållet? d.v.s. Ställ in miniatyrbilden som .pdf eller video. Vi arbetar med kreativa personer och att ha en miniatyrbildsvy som är valbar skulle vara ett bra sätt att hålla teamen engagerade i de möten på högre nivå där de kommer att diskutera vår innehållskarta - en länk till innehållet direkt vore också bra.

Kan du anpassa behörigheterna utöver vad basen är? För närvarande kan du med andra Workfront-objekt anpassa vad Contribute/manage/view-åtkomst kan göra.

För närvarande har vi bara behörighet på arbetsyta- och visningsnivå, men inte behörighet för posttyp eller enskild postnivå.

Kan vi anpassa arbetsyteikoner som liknar hur vi kan anpassa miniatyrbilder?

Kommer det att finnas anpassningsbara API:er för att använda vår egen DAM istället för Adobe DAM?

Vi har skapat ett offentligt API för Planning och vi har också Fusion Connector. API-dokumentationen publiceras och kan användas för att skapa anslutningar.

Jag ser värdet i Planning (anställda som använder Airtable). Fram tills nu har vi varit.. nyfiken backend-anslutning efter x som knyts tillbaka till ~10,47 am
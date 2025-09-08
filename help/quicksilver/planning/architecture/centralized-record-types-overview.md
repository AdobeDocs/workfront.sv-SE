---
title: Översikt över centraliserade posttyper
description: Centraliserade posttyper kan läggas till på flera arbetsytor från en central eller primär arbetsyta i Adobe Workfront Planning.
hidefromtoc: true
hide: true
source-git-commit: 9b95b5a52576327a3df8d6955925b96c2e45848f
workflow-type: tm+mt
source-wordcount: '1019'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Översikt över centraliserade posttyper

Centraliserade posttyper kan läggas till på flera arbetsytor från en central eller primär arbetsyta i Adobe Workfront Planning.

## Översikt över centraliserade posttyper

När du implementerar Workfront Planning för en organisation med flera team och gemensamma arbetsflöden kan du behöva definiera en sammanhängande struktur och metadata för nyckelposttyper (som kampanjer och slutprodukter) som kan läggas till i varje teames arbetsytor för att fånga och hantera deras arbete.

Ni kan också behöva varje teames arbete för att komma upp på en central nivå.

I ett sådant arbetsflöde kan du se till att teamen hämtar sitt arbete på ett enhetligt sätt samtidigt som de låser upp synligheten mellan team, utan att behöva lägga till allt på en arbetsyta, eller så kan alla i organisationen göra det på varje arbetsyta. Du kan använda centraliserade posttyper för att uppnå detta.

Så här använder du centraliserade posttyper:

1. Konfigurera en posttyp som ska centraliseras på en viss arbetsyta.

   En arbetsytehanterare kan välja användare med en standardlicens, team, grupper, roller eller företag att lägga till en vald posttyp i de arbetsytor som de hanterar.

   Den ursprungliga posttypen kommer att finnas på den ursprungliga arbetsytan, men kommer att synas från alla andra arbetsytor.

   Mer information finns i [Konfigurera funktioner för arbetsytan över arbetsytor för posttyper](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Lägg till en befintlig posttyp från en befintlig som har konfigurerats som en centraliserad typ på ett teams arbetsyta.

   Posttypen kommer att finnas på följande arbetsytor:

   * Den ursprungliga arbetsytan där den angavs som en centraliserad posttyp.
   * Teamets arbetsyta.

   Mer information finns i [Lägga till befintliga posttyper](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md).

   I följande avsnitt beskrivs överväganden om centraliserade posttyper antingen på deras ursprungliga arbetsytor eller efter att de har lagts till på en grupps arbetsytor.

## Att tänka på när det gäller de centraliserade posttyperna på deras ursprungliga arbetsyta

Posttypen som konfigurerats för centralisering har följande egenskaper:

* All information kan bara redigeras på den ursprungliga arbetsytan.

* Du kan utföra följande åtgärder på den centraliserade posttypen från den ursprungliga arbetsytan för en centraliserad posttyp:

   * Redigera den

     När du redigerar en centraliserad posttyp kan du redigera utseendet, arbetsytefunktionerna och alla fält som skapats på den ursprungliga arbetsytan.
   * Skapa förfrågningsformulär
   * Hantera förfrågningsformulär

* Du kan bara ta bort en centraliserad posttyp om den inte har lagts till på en Teams-arbetsyta. När den har lagts till på ett teams arbetsyta genereras ett fel om du försöker ta bort den från den ursprungliga arbetsytan.

  Detta görs så att den centraliserade posttypen kan finnas kvar på arbetsytorna där den redan har lagts till.
* Posterna som du lägger till i en centraliserad posttyp visas bara för användare som har behörigheten Visa på den ursprungliga arbetsytan.
* Posterna som du lägger till från teamets arbetsyta läggs upp och visas på den ursprungliga arbetsytan. Alla medlemmar på den ursprungliga arbetsytan får behörigheten Visa.

* De anslutna posttyperna av en centraliserad posttyp blir tillgängliga för anslutning från de arbetsytor där den här posttypen läggs till.

* Fält som skapats för en centraliserad posttyp från den ursprungliga arbetsytan visas från alla arbetsytor där posttypen läggs till.

## Överväganden om centraliserade posttyper efter att de har lagts till på ett teams arbetsyta

* Medverkande på arbetsytan får Contribute-behörighet till den centraliserade posttypen på arbetsytan. De kan lägga till och hantera poster i den.

* Teamarbetsytevisningsprogram får behörigheten Visa för den centraliserade posttypen på arbetsytan för team. De kan inte lägga till och hantera poster i.

* Teamarbetsytehanterare kan utföra följande åtgärder för den posttyp som läggs till från en centraliserad posttyp på en teamarbetsyta:

   * Lägg till nya fält

     Fält som läggs till i en central post från en arbetsyta i team visas bara från teamets arbetsyta.
   * Dela
   * Ta bort den.

     Om du tar bort posttypen från ett teams arbetsyta tas den bara bort från teamets arbetsyta. Posterna som läggs till i den från teamets arbetsyta tas också bort. Detta tar inte bort posttypen från den ursprungliga arbetsytan eller från andra arbetsytor där den har lagts till.

     Detta görs så att det är möjligt att behålla den redan tillagda centraliserade posttypen i arbetsytor som redan använder den.

* Du kan inte utföra följande åtgärder för den posttyp som lagts till från en centraliserad posttyp på en teamarbetsyta:

   * Redigera den

     Du kan inte redigera utseendet, funktionerna för arbetsytan i flera arbetsytor eller fälten som importerats från den ursprungliga arbetsytan.
   * Skapa förfrågningsformulär
   * Hantera förfrågningsformulär

* Poster som läggs till i ett teams arbetsytor visas från följande arbetsytor, om du har behörigheten Visa eller högre för dessa arbetsytor:

   * Teamets arbetsyta där de läggs till.
   * Den centraliserade posttypens ursprungliga arbetsyta.
   * Alla andra arbetsytor där den centraliserade arbetsytan läggs till.

* Följande scenarier finns för poster som skapats i arbetsytor för team:

   * Om du har behörigheten Hantera på den ursprungliga arbetsytan, och saknar behörigheter på arbetsytorna för team, kan du visa poster som lagts till från teamets arbetsytor i den ursprungliga arbetsytan, men du kan inte hantera dem från den ursprungliga arbetsytan.
   * Om du har behörigheten Hantera på teamets arbetsyta kan du hantera posterna på den centraliserade posttypens ursprungliga arbetsyta eller från den arbetsyta där de lades till.

     Du kan bara visa posterna på ytterligare arbetsytor där den centraliserade posttypen läggs till om du har behörigheten Visa på dessa arbetsytor.

## Åtkomst till anslutningar

Posttyper som är kopplade till den centraliserade posttypen på den ursprungliga arbetsytan blir synliga för arbetsytor där den centraliserade posttypen läggs till.

## API-beteende

När du lägger till poster till en centraliserad posttyp från en arbetsyta i team med Workfront Planning API, kontrollerar systemet om användaren har tillgång till att skapa poster på den ursprungliga arbetsytan för den centraliserade posttypen.

Följande fall finns:

* Om användaren har åtkomst skapas posten på den centraliserade posttypens ursprungliga arbetsyta.

* Om användaren inte har åtkomst får användaren ett felmeddelande om att han/hon inte har åtkomst till den centraliserade posttypens ursprungliga arbetsyta och måste ange det arbetsyte-ID där han/hon har åtkomst för att skapa poster.
---
title: Posttyper för flera arbetsytor - översikt
description: Centraliserade posttyper kan läggas till på flera arbetsytor från en central eller primär arbetsyta i Adobe Workfront Planning.
hidefromtoc: true
hide: true
source-git-commit: ff5bc262a5ed2a22099c058ebdb61bc32485b201
workflow-type: tm+mt
source-wordcount: '1320'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Posttyper för flera arbetsytor - översikt

I Adobe Workfront Planning kan du aktivera funktioner för flera arbetsytor för en posttyp som gör att du kan referera till en posttyp på mer än en arbetsyta.

Följande är funktioner för olika arbetsytor för posttyper:

* Du kan ange en posttyp som centraliserad. Användarna kan lägga till centraliserade posttyper i andra arbetsytor som de kan hantera.
* Du kan ange en posttyp som anslutningsbar. Användare kan ansluta till den här posttypen från andra arbetsytor.

I den här artikeln finns en översikt över posttyper för arbetsytor. Mer information om hur du definierar en posttyps funktioner för arbetsytan mellan olika arbetsytor finns i [Konfigurera funktioner för arbetsytor mellan arbetsytor för posttyper](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).


## Översikt över centraliserade posttyper

Centraliserade posttyper kan läggas till på flera arbetsytor från en central eller primär arbetsyta i Adobe Workfront Planning.

När du implementerar Workfront Planning för en organisation med flera team och gemensamma arbetsflöden kan du behöva definiera en sammanhängande struktur och metadata för nyckelposttyper (som kampanjer och slutprodukter) som kan läggas till i varje teames arbetsytor för att fånga och hantera deras arbete.

Ni kan också behöva varje teames arbete för att komma upp på en central nivå.

I ett sådant arbetsflöde kan du se till att teamen hämtar sitt arbete på ett enhetligt sätt samtidigt som de låser upp synligheten mellan team, utan att behöva lägga till allt på en arbetsyta, eller så kan alla i organisationen göra det på varje arbetsyta. Du kan använda centraliserade posttyper för att uppnå detta.

Så här använder du centraliserade posttyper:

1. Konfigurera en posttyp som ska centraliseras på en viss arbetsyta.

   En arbetsytehanterare kan välja användare med en standardlicens, team, grupper, roller eller företag att lägga till en vald posttyp i de arbetsytor som de hanterar.

   Den ursprungliga posttypen kommer att finnas på den ursprungliga arbetsytan, men kommer att synas från alla andra arbetsytor.

   Mer information finns i [Konfigurera funktioner för arbetsytan över arbetsytor för posttyper](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Lägg till en posttyp från en befintlig som har konfigurerats som en centraliserad posttyp på en sekundär arbetsyta.

   Posttypen kommer att finnas på följande arbetsytor:

   * Den ursprungliga arbetsytan där den angavs som en centraliserad posttyp.
   * En sekundär arbetsyta.

   Mer information finns i [Lägga till befintliga posttyper från en annan arbetsyta](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

   I följande avsnitt beskrivs överväganden om centraliserade posttyper och hur de fungerar på antingen den ursprungliga eller den sekundära arbetsytan.

### Att tänka på när det gäller de centraliserade posttyperna på deras ursprungliga arbetsyta

Posttypen som konfigurerats för centralisering har följande egenskaper:

* All information kan bara redigeras på den ursprungliga arbetsytan.

* Du kan utföra följande åtgärder på den centraliserade posttypen från den ursprungliga arbetsytan för en centraliserad posttyp:

   * Redigera den

     När du redigerar en centraliserad posttyp kan du redigera utseendet, arbetsytefunktionerna och alla fält som skapats på den ursprungliga arbetsytan.
   * Skapa förfrågningsformulär
   * Hantera förfrågningsformulär

* Du kan bara ta bort en centraliserad posttyp om den inte har lagts till på en sekundär arbetsyta. När den har lagts till i en annan arbetsyta genereras ett fel om du försöker ta bort den från den ursprungliga arbetsytan.

  Detta görs så att den centraliserade posttypen kan finnas kvar på arbetsytorna där den redan har lagts till.
* Posterna som du lägger till i en centraliserad posttyp visas bara för användare som har behörigheten Visa på arbetsytan där de lades till.
* Posterna som du lägger till från en sekundär arbetsyta läggs upp och visas på den ursprungliga arbetsytan. Alla medlemmar på den ursprungliga arbetsytan får behörigheten Visa.

* De anslutna posttyperna av en centraliserad posttyp blir tillgängliga för anslutning från de arbetsytor där den här posttypen läggs till.

  Om du till exempel har en Campaign-posttyp som har en anslutning till posttypen Region, och du lägger till posttypen Campaign på en sekundär arbetsyta, kommer regioner att bli anslutningsbara mellan arbetsytor för den sekundära arbetsytan. Medlemmar i den sekundära arbetsytan kan nu skapa kampanjer och länka dem till regioner.

* Fält som skapats för en centraliserad posttyp från den ursprungliga arbetsytan visas från alla arbetsytor där posttypen läggs till. Fält från en ursprunglig arbetsyta är skrivskyddade i de sekundära arbetsytorna.

### Att tänka på när centraliserade posttyper läggs till på en sekundär arbetsyta

* Deltagare på den sekundära arbetsytan får Contribute-behörighet till den centraliserade posttypen på deras arbetsyta. De kan lägga till och hantera poster i den.

* De sekundära arbetsytevisningsprogrammen får behörigheten Visa för den centraliserade posttypen på deras arbetsyta. De kan inte lägga till och hantera poster i.

* Sekundära arbetsytehanterare kan utföra följande åtgärder för den posttyp som lagts till från en centraliserad posttyp på en sekundär arbetsyta:

   * Ta bort den.

     Om du tar bort posttypen från en sekundär arbetsyta tas den bara bort från den sekundära arbetsytan. Posterna som läggs till på den sekundära arbetsytan tas också bort. Detta tar inte bort posttypen från den ursprungliga arbetsytan eller från andra sekundära arbetsytor där den har lagts till.

  <!--These two capabilities will come later:
    * Add new fields
        Fields added to a centralized record from a secondary workspace are visible only from the secondary workspace. 
    * Share it-->

* Du kan inte utföra följande åtgärder för den posttyp som lagts till från en centraliserad posttyp på en sekundär arbetsyta:

   * Redigera den

     Du kan inte redigera utseendet, funktionerna för en arbetsyta eller fälten som lagts till från den ursprungliga arbetsytan.
   * Skapa och hantera förfrågningsformulär
   * Skapa och hantera förfrågningsformulär

* Poster som läggs till i en sekundär arbetsyta visas från följande arbetsytor, om du har behörighet att visa eller högre på dessa arbetsytor:

   * Den sekundära arbetsytan där de läggs till.
   * Den centraliserade posttypens ursprungliga arbetsyta.
   * Alla andra arbetsytor där den centraliserade arbetsytan läggs till.

* Följande scenarier finns för poster som skapats i arbetsytor för team:

   * Om du har behörigheten Hantera på den ursprungliga arbetsytan, och inga behörigheter på en sekundär arbetsyta, kan du visa poster som lagts till från den sekundära arbetsytan i den ursprungliga arbetsytan, men du kan inte hantera dem från den ursprungliga arbetsytan.
   * Om du har behörigheten Hantera på den sekundära arbetsytan kan du hantera posterna på den centraliserade posttypens ursprungliga arbetsyta eller från den arbetsyta där de lades till.

     Du kan bara visa posterna på ytterligare sekundära arbetsytor där den centraliserade posttypen läggs till om du har behörigheten Visa på dessa arbetsytor.

### Åtkomst till anslutningar av en centraliserad posttyp

Posttyper som är kopplade till den centraliserade posttypen på den ursprungliga arbetsytan blir synliga från andra arbetsytor där den centraliserade posttypen läggs till.

### API-åtkomst för en centraliserad posttyp

När du lägger till poster till en centraliserad posttyp från en sekundär arbetsyta med hjälp av Workfront Planning API, kontrollerar systemet om användaren har tillgång till att skapa poster på den ursprungliga arbetsytan för den centraliserade posttypen.

Följande fall finns:

* Om användaren har åtkomst skapas posten på den centraliserade posttypens ursprungliga arbetsyta.

* Om användaren inte har åtkomst får användaren ett felmeddelande om att han/hon inte har åtkomst till den centraliserade posttypens ursprungliga arbetsyta och måste ange det arbetsyte-ID där han/hon har åtkomst för att skapa poster.

## Översikt över kopplingsbara posttyper

Du kan ansluta till en posttyp som har definierats som anslutningsbar från en arbetsyta som du hanterar.

Dina team kan behöva länka sina poster till posttyper från andra arbetsytor eller visa information som samlats in på poster som tillhör poster på andra arbetsytor. Du kan uppnå den här konfigurationen genom att ange en posttyp som anslutningsbar.

Så här använder du kopplingsbara posttyper:

1. Konfigurera en posttyp som ska kunna anslutas på en viss arbetsyta.

   En arbetsytehanterare kan välja vilka arbetsytor en angiven posttyp kan ansluta till.

   Den ursprungliga posttypen finns på den ursprungliga arbetsytan och kommer att läggas till som en kopplad posttyp på en annan arbetsyta.

   Mer information finns i [Konfigurera funktioner för arbetsytan över arbetsytor för posttyper](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Anslut till en posttyp som är angiven som anslutningsbar från en annan arbetsyta som du hanterar.

   Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).

   I följande avsnitt beskrivs överväganden om centraliserade posttyper och hur de fungerar på antingen den ursprungliga eller den sekundära arbetsytan.
---
title: 'Bridge: Ansluta strategisk återgivning till projekt'
description: Lär dig hur du skapar en"strategisk koppling" mellan dina högnivåplaner i Adobe Workfront Planning och det dagliga genomförandet av arbetsflöden i Adobe Workfront.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 0%

---


# Bron: koppla ihop strategisk avsikt med projekt


## Mål

Lär dig hur du skapar en&quot;strategisk tråd&quot; mellan dina högnivåplaner i Workfront Planning och din dagliga körning i arbetsflödesmodulen.



## Översikt

Att koppla er strategi till ert dagliga arbete omvandlar visionen till verklighet. När högnivåplaner är synkroniserade med körning skapar du en **strategisk tråd** som ser till att alla projekt och aktiviteter flyttar verksamheten framåt.



För att uppnå den här justeringen krävs en uppsättning tekniska länkar och processskyddsinstruktioner som kopplar aktiviteter i **arbetsflödesmodulen** med strategiska poster i **Workfront Planning (WFP)**. Genom att överbrygga klyftan mellan planering och handling ser du till att teamets energi alltid är inriktad på de mål som har högst prioritet.



## Grunden: Upprätta anslutningen

Innan du kan överbrygga planering och körning måste en arbetsytehanterare definiera vilka posttyper som är berättigade för en anslutning.



### Anslutningsfältet: Den tekniska handskakningen

Bryggan börjar med ett **anslutningsfält**. Den här fälttypen är motorn bakom alla relationer i WFP. Det är ett avsiktsuttryck, i den bemärkelsen att det går att länka en viss posttyp (som en *kanaltaktik*) till andra objekt, oavsett om de finns i arbetsflödesmodulen eller i själva planeringen.



### Avgör anslutning

Att fastställa den här toleransen är ett beslut på konfigurationsnivå som vanligtvis inträffar innan något arbete skapas. Genom att lägga till ett anslutningsfält skapar du en miljö med stöd för en&quot;strategisk tråd&quot;, oavsett hur de enskilda posterna slutligen skapas.



## Strategi och genomförande synkroniserat

För att behålla det strategiska lagret i fokus rekommenderar vi att du fokuserar dina planeringsdokument på hög nivå samtidigt som du använder arbetsflödesmodulen för taktiskt genomförande. Detta tillvägagångssätt använder de unika styrkorna hos båda modulerna:



* **Workfront Planning (det strategiska lagret):** Står på hög nivå. Den spårar *kampanjen*, *kanalaktiviteten* och *budgeten*. Det är bullerfritt och verkställande.

* **Arbetsflödesmodulen (körningslagret):** Hantera de taktiska detaljerna. Enskilda&quot;upplevelser&quot; eller&quot;aktiviteter&quot; hanteras här som **projekt, aktiviteter och problem**.



## Aktivera bryggan: Från avsikt till åtgärd

När anslutningen har konfigurerats måste du bestämma hur länken mellan en viss strategisk post och ett körningsprojekt ska aktiveras.



### Professionell triage: Den tabellledda sökvägen

Strategister och avancerade användare använder ofta **tabellvyn** som &quot;workbench&quot; för att förfina planer över tiden.

* **Frigör överlämning:** Som standard skapas ingen länk till arbetsflödesmodulen när en post skapas i en tabell. Anslutningen till ett körningsprojekt upprättas när en användare bestämmer sig för att aktivera länken. Detta kan du göra genom att manuellt skapa ett underordnat anslutet projekt direkt från anslutningsfältet i WFP eller en valfri **anslutningsvy** i postens detaljvy. Observera att manuellt skapande resulterar i ett tomt projekt utan specifika anpassade formulär. För mer komplexa behov kan du använda en **inbyggd WFP-automatisering**. Dessa automatiseringar är tillgängliga när du markerar en rad i en tabell och visas som knappar i det blå åtgärdsfältet längst ned på skärmen. Detta gör att man kan lägga in tillsyn eller platshållare, vilket säkerställer att projekten bara genereras i arbetsflödesmiljön när de verkligen behövs.



### Automatiserad aktivering

För organisationer med stora volymer eller avancerade automatiseringsbehov kan bryggan aktiveras automatiskt baserat på specifika händelser eller fältvärden.

* **Överföringsutlösare:** Eftersom formulär innehåller en enda, ren &quot;överföringshändelse&quot; kan de användas som utlösare för **Fusion Automations**. Ett scenario kan identifiera en formuläröverföring och omedelbart generera ett länkat projekt i arbetsflödesmodulen.

* **Fältvärdesutlösare:** För större automatisering kan du konfigurera **Fusion** så att specifika fält övervakas. En enkel kryssruta som heter&quot;körklar&quot; kan till exempel fungera som katalysator och automatiskt upprätta bryggan när den är markerad.



## Synlighet för yta: Sök efter fält

När ett projekt har länkats kan du visa realtidsdata från arbetsflödesmodulen direkt i WFP-posten.



En arbetsytehanterare kan ställa in **uppslagsfält** så att inbyggda eller anpassade fält från det länkade projektet (till exempel *faktiskt slutförandedatum* eller *kreativt lead*) hämtas till WFP-posttypen. När dessa data har samlats in kan de samlas in på flera nivåer i er strategiska hierarki - ända hela vägen till kampanjnivån. Detta ger en kraftfull aggregerad rapportering för intressenter under hela marknadsföringscykeln, så att de hålls informerade utan att behöva lämna planeringsmiljön.



## En strategi-till-åtgärd-synlighet

Det slutliga värdet för bryggan är **synlighet i realtid**. Genom att koppla avsikt till åtgärd kan du snabbt besvara viktiga affärsfrågor:



* &quot;Levererar vår kampanj &quot;FY26 Brand Awareness&quot; aktivt resultat just nu?&quot;

* &quot;Var behöver vår strategiska strategi mer kreativ support för att hålla tidsplanen?&quot;

* &quot;Hur anpassar vi våra resurser till våra strategiska pelare med högsta prioritet?&quot;



## God praxis och tips



### Gör:

* **Använd metaforen för strategisk tråd.** Påminn team om att varje projekt ska vara en&quot;pärm&quot; i en strategisk sträng.

* **Automatisera överföringen.** Använd automatisering för att utlösa projektskapande för att spara tid och arbete samtidigt som dataanslutningen och styrningen förbättras.

* **Länk, duplicera inte.** Använd sökfält för att visa körningsdata i realtid (som status eller slutförandedatum) i dina strategiska poster. Detta gör att dina strategiska vyer alltid är korrekta utan att ditt team behöver göra manuella uppdateringar.



### Gör inte:

* **Hantera inte planeringsposter som uppgiftslistor.** Bryggan är utformad för att ansluta strategisk avsikt till körningsprojekt. Håll dina planeringsdokument fokuserade på&quot;vad&quot; och&quot;varför&quot; och låt arbetsflödesmodulen hantera detaljerade&quot;hur&quot;-uppgifter och ärenden.

* **Översynkronisera inte.** Du behöver inte synkronisera alla projektnivådetaljer tillbaka till Planering. Håll det strategiska lagret högt och utan brus.

* **Åsidosätt inte bron.** Om arbetet startar i arbetsflödesmodulen utan någon länk till Planering har du skapat en&quot;Skuggplan&quot; som inte syns för ledningen.





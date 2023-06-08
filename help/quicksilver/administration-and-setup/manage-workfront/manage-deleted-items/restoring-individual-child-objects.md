---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Återställa enskilda underordnade objekt
description: I det här dokumentet beskrivs hur du kan få hjälp med att återställa enskilda underordnade objekt som har tagits bort från Adobe Workfront-produktions- eller förhandsvisningsmiljöer mindre än 30 dagar tidigare.
feature: System Setup and Administration
role: Admin
exl-id: e2e4fbb7-5433-4d88-8e36-d82f4cc8a194
source-git-commit: 8bcc2859b3b6ce7a264c8f234536a93b7761ab6b
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# Återställa enskilda underordnade objekt

I det här dokumentet beskrivs hur du kan få hjälp med att återställa enskilda underordnade objekt som har tagits bort från Adobe Workfront-produktions- eller förhandsvisningsmiljöer mindre än 30 dagar tidigare.

En Workfront-administratör kan återställa projekt, uppgifter, problem och dokument i varje Workfront-instans enligt beskrivningen i [Återställ borttagna objekt](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md). Men det är bara Workfront databasteam som kan återställa objekt som uppgifter, ärenden, dokument, anpassade formulär, timmar och anteckningar oberoende av deras överordnade objekt.

Data från din livemiljö är tillgängliga i sandlådan Preview i upp till 7 dagar. Det innebär att du kan exportera fristående data från sandlådemiljön för förhandsgranskning på följande sätt:

* Spark-Starts
* Bygga en rapport och exportera resultaten

Mer information om att exportera data från Workfront finns i [Exportera data](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

Du kan importera exporterade data på följande sätt:

* Om du använder exporterade rapporter manuellt
* Oftast om du använder Spark-Starts

   Mer information om hur du importerar data till Workfront med Quick-Starts finns i [Importera data till Adobe Workfront med en snabbstartsmall](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

Sandlådemiljön för förhandsgranskning uppdateras under våra underhållsperioder under helgen.

Mer information om underhållsfönstren för förhandsvisningens sandlådemiljö finns i [Adobe statuswebbplats](https://status.adobe.com).

>[!IMPORTANT]
>
>Dokument är ett undantag från dessa återställningsmetoder. Du kan hämta dem manuellt från förhandsvisningsmiljön och överföra dem till produktionsmiljön igen. Om du vill ladda ned och överföra flera dokument samtidigt måste du begära en dataåterställning från Workfront.

## Information som behövs för en dataåterställning

När du har fastställt att ett borttaget objekt behöver återställas av vårt databasteam samlar du in så mycket information du har om det. Följande information krävs för att våra databasadministratörer ska kunna hitta objektet och initiera en återställning:

* Objektnamn
* Objekttyp (Aktivitet, Utgåva, Projekt osv.)
* Beräknat datum och tid för borttagning
* Objekt-GUID (om möjligt)

   Se följande information när du söker efter GUID för ett objekt:

   * GUID kan hittas genom att referera till e-postmeddelanden som utlöses av interaktion med objektet (tilldelningar till, kommentarer till osv.)
   * Exempel på ett GUID som finns i slutet av en URL: `yourdomain.my.workfront.com/issue/view?ID=568bfa96011220154c8ca4c4e691556b`

När du har samlat in den här informationen eller om du behöver hjälp, ring vårt kundsupportteam på 844-306-HELP(4357) eller skicka in en biljett online.

## Dataåterställningsprocess

1. När vårt kundsupportteam har tagit emot din information eskalerar de den till vårt kundsupportteam.
1. Vårt kundsupportteam kommer att kontakta vårt databasteam.
1. När databasteamet har haft möjlighet att granska de data som återställs kan en mer korrekt uppskattning av det elektroniska referensdokumentet tillhandahållas. En återställning tar i allmänhet tre dagar, men kan ta längre tid beroende på vilken typ av data som återställs och vilken volym de innehåller.
1. Databasgruppen återställer informationen till din förhandsgranskningssandlådemiljö där du kan granska återställda data. Vårt kundsupportteam meddelar dig när informationen finns i förhandsgranskningssandlådan.
1. När du är nöjd med återställningen i sandlådan ska du informera vårt kundsupportteam och de kommer att kontakta vårt databasteam för att meddela dem att de kan återställa data till din produktionsmiljö.
1. Du kan granska återställda data innan begäran stängs.

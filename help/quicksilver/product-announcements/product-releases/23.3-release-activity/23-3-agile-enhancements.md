---
title: 23.3 Agile-förbättringar
description: 23.3 Agile-förbättringar
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a47d2592-0f00-4bcd-bc8e-75f8e707a573
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1315'
ht-degree: 0%

---

# 23.3 Agile-förbättringar

Den här sidan beskriver alla brädor och smidiga förbättringar som gjorts i version 23.3. Dessa förbättringar gjordes tillgängliga i produktionsmiljön med version 23.3 den 20 och 21 juli 2023.

En lista över alla ändringar som är tillgängliga vid den här tidpunkten i 23.3-versionscykeln finns på [23.3 Versionsöversikt](/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-release-overview.md).

Mer information om hur du väljer att använda nya funktioner i Boards före kvartalsversionen finns i [Tidig registrering av nya funktioner för Adobe Workfront Boards](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

## Agile View of a project displays a kanban board

Agile View för ett projekt innehåller nu ytterligare funktioner för att filtrera, gruppera och sortera arbetet på en kanban-tavla. Den nya flexibla designen av vyn innehåller en robust sökfunktion och möjlighet att lägga till nya uppgifter direkt från styrelsen.

>[!NOTE]
>
>Agile-vyn finns bara för ett projekt eftersom det är en alternativ vy av projektet och du kan inte komma åt det från andra delar av Workfront, till exempel kontrollpanelen för anslagstavlor.

När du sitter i styrelsen kan du växla till den äldre Agile-vyn.

Mer information finns i [Hantera ett projekt i flexibel vy](/help/quicksilver/manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

[Visa en videodemonstration av den här funktionen.](https://video.tv.adobe.com/v/3421283/){target=_blank}

## Sortera efter kortkolumner

Vi har lagt till möjligheten att sortera korten i kolumnerna på en anslagstavla. När du väljer ett alternativ att sortera efter sorteras alla kolumner. Det går inte att sortera en enstaka kolumn, och eftersläpningen eller inloppskolumnen sorteras inte.

Du kan sortera i stigande eller fallande ordning efter kortnamn, förfallodatum, uppskattning, status eller anslutning (projektnamn). Anslutningen gäller endast anslutna kort, och de andra alternativen sorterar både anslutna kort och ad hoc-kort i kolumnen.

Alternativet &quot;användarordning&quot; returnerar korten i den ordning de ställdes in manuellt, innan några andra sorteringsalternativ tillämpades. Det här är standardsorteringen för kolumnerna.

Mer information finns i [Filtrera och söka på en anslagstavla](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

[Visa en videodemonstration av den här funktionen.](https://video.tv.adobe.com/v/3420932/){target=_blank}

## Mörkt läge finns nu på Adobe Workfront-kort

Nu kan du visa alla dina brädor och arbetsflöden i mörkt läge. Den nya inställningen är tillgänglig via inställningarna på panelpanelen.

>[!NOTE]
>
>Om din organisations instans av Workfront har tagits med i Adobe Unified Experience kan du aktivera mörk temaformatering för alla Adobe Experience Cloud via din inställningsmeny (din profilbild) och du kommer inte att se något separat alternativ för mörkt läge för Workfront Boards.

Mer information finns i [E-postmeddelanden och inställningar för anslagstavlor](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

## Mål som är tillgängliga i arbetsströmsversioner på Adobe Workfront-anslagstavlor

Vi har lagt till möjligheten att lägga till mål i en iteration, utan att behöva lista målen på ett kort. Mål läggs till i ett checklisteformat och kan markeras som fullständiga. Mätområdet högst upp till höger om iterationen visar hur många mål som finns och hur många som har slutförts.

Dessutom är kolumnen Nästa iteration nu tillgänglig på itereringspaneler. När du placerar ett kort i den här kolumnen överförs det automatiskt till nästa iteration och återgår inte till eftersläpningen. På nästa iteration visas kortet i den kolumn som motsvarar dess status.

Mer information finns i [Skapa en iteration i ett arbetsflöde](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

## Lägga till kommentarer till kort på anslagstavlor

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att man väljer den tidiga funktionen för Workfront Boards.

Nu kan du lägga till kommentarer i både ad hoc-kort och anslutna kort på anslagstavlan och tagga andra användare på kommentarerna. Kommentarerna finns i kortinformationen. Kommentarsfunktionen för anslagstavlor använder den nya kommentarsfunktionen från Adobe Workfront.

Mer information finns i [Lägga till ett ad hoc-kort till en anslagstavla](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md) och [Använd anslutna kort på ritytor](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

[Visa en videodemonstration av den här funktionen](https://video.tv.adobe.com/v/3420832/){target=_blank}

## Förbättringar av tagghanteraren Boards

Tagghanteringsgränssnittet har förbättrats så att du snabbt kan skapa nya taggar och använda dem på kort. Du kan också skapa taggar för arbetsflöden.

Mer information finns i [Lägg till taggar](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

## Enkla filter finns på inloppskolumner

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att man väljer den tidiga funktionen för Workfront Boards.

Förenklade filter har lagts till i inställningen för inloppskolumnen så att du kan definiera inloppskolumnen snabbare. De tillgängliga filtren är Workfront-projekt och uppdrag per team eller användare. Du kan växla till de avancerade filtren om du vill.

Mer information finns i [Lägga till en inloppskolumn på en anslagstavla](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

[Visa en videodemonstration av den här funktionen](https://video.tv.adobe.com/v/3419420/){target=_blank}

## Enkla filter har lagts till i mallen för dynamiska kort

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att man väljer den tidiga funktionen för Workfront Boards.

Filtren i den dynamiska kortmallen har förenklats så att du kan skapa en anslagstavla snabbare. De tillgängliga filtren är Workfront-projekt och uppdrag per team eller användare. Du kan växla till de avancerade filtren om du vill. De här filteralternativen finns även på panelen Konfigurera för dynamiska ritytor.

Mer information finns i [Skapa eller redigera en anslagstavla](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## Dynamisk kortmall

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att man väljer den tidiga funktionen för Workfront Boards.

En ny mall, Dynamic Board, är nu tillgänglig för fristående anslagstavlor. Den här mallen är inte tillgänglig för ritytor i en arbetsström.

På den dynamiska panelen kan du automatiskt fylla i en anslagstavla med kort som är baserade på ett Workfront-projekt. Med hjälp av filter läggs kort till i kolumner baserat på deras status.

Mer information finns i [Skapa eller redigera en anslagstavla](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

[Visa en videodemonstration av den här funktionen](https://video.tv.adobe.com/v/3418600/){target=_blank}

## Migrera smidiga team-kanban-kort till styrelser

En ny **Lägg till i anslagstavlor** -knapp på ett smidigt team Kanban boards gör att du kan lägga till alla kort från Kanban-tavlan till en Workfront-styrelse. Du kan välja att skapa ett nytt Workfront-kort eller lägga till korten på en befintlig anslagstavla.

Kortens placering på Workfront board baseras på spaltregler. (En princip kan till exempel flytta alla kort med statusen &quot;Pågår&quot; till en viss kolumn.) Om det inte finns några profiler eller om korten inte matchar profilerna placeras korten i kolumnen längst till vänster. För närvarande läggs inga kort i kolumnen Eftersläpning på det äldre kortet till på Workfront-kortet.

Korten tas inte bort från den flexibla teamets Kanban-tavla, och kortstatusändringarna synkroniseras med båda tavlorna. Du kan låta båda styrelserna vara aktiva tills du är redo att byta till Workfront Boards.

Mer information finns i [Migrera smidiga team-kanban-kort till Workfront-styrelser](/help/quicksilver/agile/use-boards-agile-planning-tools/migrate-kanban-cards-to-boards.md).

[Visa en videodemonstration av den här funktionen](https://video.tv.adobe.com/v/3420425/){target=_blank}

## Vänster navigering har lagts till i kortinformation på korten

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att man väljer den tidiga funktionen för Workfront Boards.

I takt med att fler fältalternativ läggs till på kort på Workfront Boards har kortinformationen blivit längre. Med en ny navigeringspanel till vänster om kortinformationen kan du markera ett avsnitt och automatiskt flytta till den gruppen med fält.

Nu kan du även lägga till URL:er i fältet Beskrivning och de blir klickbara länkar när kortinformationen sparas. Uppdateringarna gäller både ad hoc-kort och anslutna kort.

Mer information finns i [Lägga till ett ad hoc-kort till en anslagstavla](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md) och [Använd anslutna kort på ritytor](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

[Visa en videodemonstration av den här funktionen.](https://video.tv.adobe.com/v/3418598/){target=_blank}

## E-postmeddelanden och inställningar för anslagstavlor

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att man väljer den tidiga funktionen för Workfront Boards. Eftersom e-postmeddelanden i allmänhet inte används i Förhandsgranska, släpptes den här funktionen samtidigt för kunder som vill anmäla sig tidigt (endast för tidiga användare).

E-postmeddelanden är nu tillgängliga för Adobe Workfront Boards. Meddelandena är aktiverade som standard och du kan välja vilka e-postmeddelanden du vill få i inställningarna. Du får ett e-postmeddelande när du läggs till på en anslagstavla och när du tilldelas ett kort.

Mer information finns i [E-postmeddelanden och inställningar för anslagstavlor](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

[Visa en videodemonstration av den här funktionen](https://video.tv.adobe.com/v/3418597/){target=_blank}

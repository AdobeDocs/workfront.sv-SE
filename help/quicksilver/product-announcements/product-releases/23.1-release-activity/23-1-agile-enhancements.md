---
title: 23.1 Agile-förbättringar
description: 23.1 Agile-förbättringar
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4bd041a5-a6e3-4fe3-ae23-45980701e904
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 0%

---

# 23.1 Agile-förbättringar

Den här sidan beskriver alla Agile-förbättringar som gjorts i version 23.1 till förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön den 16 januari 2023.

En lista över alla ändringar som är tillgängliga i version 23.1 finns i [23.1 Versionsöversikt](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

## Scrum planning for Workfront Boards

De nya Scrum-planeringsfunktionerna i Adobe Workfront Boards erbjuder flexibla alternativ för att hantera era Agile-processer. Med dessa verktyg kan du

* Spåra arbeten i iterationer och fjädrar
* Använd snabbhet för att vägleda teamets åtaganden
* Spåra nedbränning och slutförandegrad

Planeringsfunktionerna för Scrum kommer snabbt efter version 23.1.

## Förfallodatum för kort mappas till planerat slutdatum för Workfront-objekt

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att man väljer den tidiga funktionen för Workfront Boards.

Förfallodatum för anslutna kort i Workfront Boards mappas nu till det planerade slutförandedatumet på det associerade Workfront-objektet. Om du uppdaterar förfallodatumet på ett kort uppdateras det planerade slutförandedatumet för uppgiften eller utgåvan. Om du ändrar det planerade slutförandedatumet ändras även kortets förfallodatum. Tidigare var kortets förfallodatum en manuell inmatning och mappades inte till något datum för en uppgift eller utgåva.

Datummappning gäller även anslutna checklisteobjekt som synkroniseras med underaktiviteter.

Förfallodatumet på både anslutna kort och ad hoc-kort innehåller nu även ett tidsfält.

Mer information finns i [Använda anslutna kort på kort](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

[Visa en videodemonstration av den här funktionen](https://video.tv.adobe.com/v/3411952/){target=_blank}

## Poster i checklistan för anslagstavlor och Workfront-underuppgifter är nu länkade

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att man väljer den tidiga funktionen för Workfront Boards.

När du lägger till ett anslutet kort till en anslagstavla för en Workfront-uppgift importeras alla underuppgifter som checklisteobjekt på kortet. När du skapar ett checklisteobjekt på ett anslutet kort läggs en underuppgift till i Workfront-uppgiften. Checklisteobjekt vid problem är inte kopplade till några Workfront-objekt.

Objekt och underaktiviteter i checklistor länkades inte tidigare. Om du vill ta med en underuppgift på anslagstavlan kan du importera den som ett separat anslutet kort eller manuellt lägga till ett checklisteobjekt på ett kort.

Mer information finns i [Använda anslutna kort på kort](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) och [Hantera checklisteobjekt på kort](/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md).

[Visa en videodemonstration av den här funktionen](https://video.tv.adobe.com/v/3411951/){target=_blank}

## Korträknare i kortkolumner

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att man väljer den tidiga funktionen för Workfront Boards.

Det finns en ny konfigurationsinställning för att aktivera korträknare för alla kolumner på en anslagstavla. Om du använder PIA-gränsen för en kolumn läggs ingen separat korträknare till.

Mer information finns i [Hantera kortpanelskolumner](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

## Söka och sortera på panelkontrollpanelen

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att man väljer den tidiga funktionen för Workfront Boards.

Nu kan du sortera panelernas kontrollpanel efter panelnamn eller datum och söka efter en viss panel i listan.

Mer information finns i [Använda panelkontrollpanelen](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md).

## Status visas på kortet

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att man väljer den tidiga funktionen för Workfront Boards.

Om ett kort på en anslagstavla har tilldelats en status, visas nu statusen på kortet så att du inte behöver öppna kortet för att se statusen. Den här förbättringen gäller för både ad hoc-kort och anslutna kort.

Mer information finns i [Använd anslutna kort på kort](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) och [Lägg till ett ad hoc-kort på en anslagstavla](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

![status på kortet](/help/quicksilver/product-announcements/product-releases/assets/boards-connected-card-details-110922.png)

## Länkbara kort finns nu tillgängliga på ritytor

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att man väljer den tidiga funktionen för Workfront Boards.

Nu kan du skicka en länk till ett visst kort till en annan kortanvändare. Personen måste ha tillgång till för att kunna visa styrelsen innan de kan öppna länken.

När du öppnar ett kort på en anslagstavla ser webbläsarens URL ut så här:

```
https://<Workfront-URL>/boards/<board-id>/card/<card-id>. 
```

Du kan kopiera den fullständiga URL:en och skicka den till någon annan. De går direkt till det öppna kortet när de öppnar länken.

Tidigare var länkar tillgängliga för anslagstavlor men inte för specifika kort.

Mer information om kort finns i [Lägga till ett ad hoc-kort på en anslagstavla](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md) och [Använda anslutna kort på anslagstavlor](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Filtrera efter anslutning på anslagstavlor

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att man väljer den tidiga funktionen för Workfront Boards.

Listan med filter på en anslagstavla innehåller nu alternativet att filtrera efter anslutning, som visar alla anslutna kort för ett visst projekt. Du kan även filtrera efter kort som inte är anslutna.

Mer information finns i [Filtrera och söka på en anslagstavla](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

[Visa en videodemonstration av den här funktionen](https://video.tv.adobe.com/v/3412381/){target=_blank}

## Arkivera kort från en styrelse enligt ett schema

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att man väljer den tidiga funktionen för Workfront Boards.

Du kan konfigurera en styrelse så att kort arkiveras, eller&quot;faller bort&quot; från styrelsen, enligt ett schema. Det finns alternativ för att ange att kort i en viss kolumn ska arkiveras på ett visst antal dagar eller veckor. Du kan till exempel definiera utfallet så att kort i en fullständig kolumn arkiveras efter att de finns i kolumnen i två veckor.

Om du vill visa korten igen när de har fallit bort från anslagstavlan kan du ställa in kortfiltret så att det visar arkiverade kort.

Mer information finns i [Konfigurera kortutfall](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).

[Visa en videodemonstration av den här funktionen](https://video.tv.adobe.com/v/3412323/){target=_blank}

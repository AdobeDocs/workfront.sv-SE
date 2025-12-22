---
title: 23.2 Agile-förbättringar
description: 23.2 Agile-förbättringar
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: dc97f4a2-9c51-4ccd-8121-c00fd1ac6988
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '1198'
ht-degree: 0%

---

# 23.2 Agile-förbättringar

Den här sidan beskriver alla Agile-förbättringar som gjorts i version 23.2 till förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön med version 23.2.

En lista över alla ändringar som är tillgängliga vid den här tidpunkten i 23.2-versionscykeln finns i [23.2 Versionsöversikt](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

## Lägga till uppgifter och problem från objektinformation på en Workfront-arbetsyta eller i ett arbetsflöde

Nu kan du lägga till befintliga uppgifter eller problem i en lista med Workfront-kort eller arbetsflödeskort direkt från objektinformationen. Alla objekt som du lägger till på en anslagstavla blir anslutna kort och alla objekt som läggs till i en arbetsström läggs till i kortlistan som oplanerade kort.

Mer information finns i [Lägga till befintliga uppgifter eller ärenden på en anslagstavla](/help/quicksilver/agile/get-started-with-boards/add-card-from-list-to-board.md).

## Iterationsfunktioner som finns i Adobe Workfront Boards

Flera nya funktioner som finns på Workfront Boards gör det möjligt att använda funktionerna i Agile Scrum. Bland dessa funktioner finns:

* Arbetsflöden för att gruppera anslagstavlor som hör till samma team och för samarbete i arbetsgrupper
* En lista med kort, eller en eftersläpning i arbetet, med möjlighet att använda källor för att ansluta kort till Workfront uppgifter och problem
* Processtavlor för iterationsplanering och iteration

Observera att samlingar har bytt namn till arbetsflöden. Med arbetsflöden kan ni visualisera data på olika sätt. Du kan visa objekt på kort i en lista, på en bräda eller på en iteration. Kort i en arbetsström kan också delas mellan flera ritytor. Du kan enkelt underlätta arbetsflöden med kort och kort i en arbetsström.

Mer information finns i [Hantera arbetsflöden](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md), [Skapa en iteration i ett arbetsflöde](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md) och [Använd kortlistan](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

[Visa en videodemonstration av den här funktionen](https://video.tv.adobe.com/v/3417059/){target=_blank}

## Lägga till uppgifter och problem från listor och rapporter till en lista med arbetsflödeskort

Nu kan du lägga till befintliga uppgifter eller problem i ett arbetsflöde i Workfront Boards direkt från en list- eller rapportvy. Alla objekt som du lägger till i arbetsflödet läggs till i kortlistan som oplanerade kort.

Mer information finns i [Lägga till befintliga uppgifter eller ärenden på en anslagstavla](/help/quicksilver/agile/get-started-with-boards/add-card-from-list-to-board.md).

## Lägg till anpassade fält på kort på en anslagstavla

Nu kan du inkludera anpassade fält på Adobe Workfront Boards. Fältet måste redan ha skapats i Workfront. Du kan inte designa och skapa nya anpassade fält på en anslagstavla.

Precis som med standardfälten kan du välja att visa det anpassade fältet i den fullständiga vyn av ett kort och den komprimerade vyn på kortet.

Alla data från det anpassade fältet på kortet är skrivskyddade.

Mer information finns i [Anpassa vilka fält som ska visas på ett kort](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

## Lägga till uppgifter och problem från listor och rapporter till en Workfront-styrelse

Nu kan du lägga till befintliga uppgifter eller problem på en Workfront-styrelse direkt från en list- eller rapportvy. Alla objekt som du lägger till på anslagstavlan blir anslutna kort.

Fältet för anslagstavlor är nu även tillgängligt för att lägga till i listor och rapporter för uppgifter eller problem. I det här fältet visas alla anslagstavlor som en uppgift eller ett problem har lagts till i.

Mer information finns i [Lägga till befintliga uppgifter eller ärenden på en anslagstavla](/help/quicksilver/agile/get-started-with-boards/add-card-from-list-to-board.md).


## Logga timmar på anslutna kort på anslagstavlan

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att man väljer den tidiga funktionen för Workfront Boards.

Nu kan du logga timmar på anslutna kort, på samma sätt som du gör för en uppgift eller ett problem. Du måste ha rätt behörighet för aktiviteten eller problemet för att kunna logga tiden.

Fälten för tidsloggning visas inte på anslutna kort som standard. Du måste aktivera **Timmar** i området Konfigurera under Kort.

Mer information finns i [Använda anslutna kort på kort](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).


## Anpassa visning av fält på ett kort

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att man väljer den tidiga funktionen för Workfront Boards.


Anpassning är nu tillgängligt för att konfigurera vilka fält som ska visas på ett kort, både i den fullständiga vyn när kortet är öppet och i den komprimerade kortvyn på kortet. När du inaktiverar ett fält visas inte i någon av vyerna. Du kan även aktivera ett fält i den fullständiga vyn och dölja det i den komprimerade vyn.

Mer information finns i [Anpassa vilka fält som ska visas på ett kort](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

[Visa en videodemonstration av den här funktionen](https://video.tv.adobe.com/v/3415710/){target=_blank}

## Definiera en standardstatus för kort som flyttas till en kortkolumn

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att man väljer den tidiga funktionen för Workfront Boards.

Du kan nu ange en standardstatus som ska gälla för kort som flyttas till en viss kolumn genom att välja en anpassad status och en systemstatus i kolumnprofilerna. När du flyttar ett kort till kolumnen försöker Workfront först att använda den anpassade statusen (till exempel Väntar på feedback). Om den anpassade statusen inte är tillgänglig för det kortet kommer Workfront att använda systemstatusen i stället (till exempel Väntande). Om statusen för den anslutna aktiviteten eller utgåvan ändras till den anpassade statusen eller systemstatusen som anges i kolumnprincipen, flyttas kortet automatiskt till kolumnen.

Tidigare uppmanades du att välja en status för varje kort som flyttats till kolumnen, om flera statusar var tillgängliga.

Mer information finns i [Hantera kolumner](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

[Visa en videodemonstration av den här funktionen](https://video.tv.adobe.com/v/3415711/){target=_blank}

## Samlingar finns nu i Adobe Workfront Boards

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att man väljer den tidiga funktionen för Workfront Boards.

Nu kan du skapa samlingar på panelkontrollpanelen. En samling är en grupp styrelser för samarbete i arbete. När du har namngett samlingen kan du lägga till ritytor i samlingen med hjälp av en uppsättning mallar med fördefinierade inställningar, till exempel kolumnnamn. Du kan också flytta fristående anslagstavlor till en samling. När en styrelse finns i en samling kan den flyttas till en annan samling, men den kan inte bli en fristående styrelse.

Att lägga till medlemmar i en samling fungerar på samma sätt som att lägga till medlemmar i en styrelse. En person eller ett team måste vara medlem i samlingen innan de kan läggas till som medlemmar i en styrelse i samlingen.

Mer information finns i [Hantera samlingar](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

[Visa en videodemonstration av den här funktionen](https://video.tv.adobe.com/v/3415609/){target=_blank}

## Beräkningsfält på anslutna kort mappar till artikelpunktsfält på Workfront-objekt

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att man väljer den tidiga funktionen för Workfront Boards.

Beräkningsfältet på anslutna kort i Workfront Boards mappar nu till artikelpunktsfältet för det associerade Workfront-objektet.

Det nya fältet Artikelpunkter är ett redigerbart frihandsfält som du kan lägga till i en vy i en lista eller rapport för uppgifter eller problem. Det är inte knutet till planerade timmar eller teamuppdrag.

Tidigare var kortberäkningen en manuell inmatning och mappades inte till något fält i en uppgift eller ett problem.

Uppskattningsfältet på både ad hoc-kort och anslutna kort har inte längre någon teckengräns. Tidigare var det maximala antalet tecken 99.

Mer information finns i [Använda anslutna kort på kort](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Kort för förhandsgranskning i inloppskolumnen

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att man väljer den tidiga funktionen för Workfront Boards.

Nu kan du klicka på ett anslutet kort i intag-kolumnen för att se en version av innehållet som bara är för visning. Du kan inte redigera kortets innehåll förrän kortet flyttas från inmatningskolumnen till en annan kolumn på kortet.

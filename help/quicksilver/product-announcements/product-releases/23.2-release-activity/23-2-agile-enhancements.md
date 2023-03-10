---
title: 23.2 Agile-förbättringar
description: 23.2 Agile-förbättringar
author: Courtney
draft: Probably
feature: Product Announcements
source-git-commit: d9fa1c876f2b789c3c387387964ba749c5453a1e
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 0%

---

# 23.2 Agile-förbättringar

Den här sidan beskriver alla smidiga förbättringar som gjorts i version 23.2 till förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön med version 23.2.

En lista över alla ändringar som är tillgängliga i version 23.2 finns i [23.2 Versionsöversikt](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

## Lägga till uppgifter och problem i Workfront-styrelser från listor och rapporter

Nu kan du lägga till befintliga uppgifter eller problem på en Workfront-styrelse direkt från en list- eller rapportvy. Alla objekt som du lägger till på anslagstavlan blir anslutna kort.

Fältet för anslagstavlor är nu även tillgängligt för att lägga till i listor och rapporter för uppgifter eller problem. I det här fältet visas alla anslagstavlor som en uppgift eller ett problem har lagts till i.

Mer information finns i [Lägga till befintliga uppgifter eller problem i en styrelse](/help/quicksilver/agile/get-started-with-boards/add-card-from-list-to-board.md).

## Logga timmar på anslutna kort på anslagstavlan

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att du har anmält dig till Workfront Boards så snart som möjligt.

Nu kan du logga timmar på anslutna kort, på samma sätt som du gör för en uppgift eller ett problem. Du måste ha rätt behörighet för aktiviteten eller problemet för att kunna logga tiden.

Fälten för tidsloggning visas inte på anslutna kort som standard. Du måste aktivera **Timmar** i området Konfigurera under Kort.

Mer information finns i [Använd anslutna kort på ritytor](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Anpassa visning av fält på ett kort

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att du har anmält dig till Workfront Boards så snart som möjligt.


Anpassning är nu tillgängligt för att konfigurera vilka fält som ska visas på ett kort, både i den fullständiga vyn när kortet är öppet och i den komprimerade kortvyn på kortet. När du inaktiverar ett fält visas inte i någon av vyerna. Du kan även aktivera ett fält i den fullständiga vyn och dölja det i den komprimerade vyn.

Mer information finns i [Anpassa vilka fält som visas på ett kort](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

[Visa en videodemonstration av den här funktionen](https://video.tv.adobe.com/v/3415710/){target=_blank}

## Definiera en standardstatus för kort som flyttas till en kortkolumn

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att du har anmält dig till Workfront Boards så snart som möjligt.

Du kan nu ange en standardstatus som ska gälla för kort som flyttas till en viss kolumn genom att välja en anpassad status och en systemstatus i kolumnprofilerna. När du flyttar ett kort till kolumnen försöker Workfront först att använda den anpassade statusen (till exempel Väntar på feedback). Om den anpassade statusen inte är tillgänglig för det kortet kommer Workfront att använda systemstatusen i stället (till exempel Väntande). Om statusen för den anslutna aktiviteten eller utgåvan ändras till den anpassade statusen eller systemstatusen som anges i kolumnprincipen flyttas kortet automatiskt till kolumnen.

Tidigare uppmanades du att välja en status för varje kort som flyttats till kolumnen, om flera statusar var tillgängliga.

Mer information finns i [Hantera kolumner](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

[Visa en videodemonstration av den här funktionen](https://video.tv.adobe.com/v/3415711/){target=_blank}

## Samlingar finns nu i Adobe Workfront Boards

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att du har anmält dig till Workfront Boards så snart som möjligt.

Nu kan du skapa samlingar på panelkontrollpanelen. En samling är en grupp styrelser för samarbete i arbete. När du har namngett samlingen kan du lägga till ritytor i samlingen med hjälp av en uppsättning mallar med fördefinierade inställningar, till exempel kolumnnamn. Du kan också flytta fristående anslagstavlor till en samling. När en styrelse finns i en samling kan den flyttas till en annan samling, men den kan inte bli en fristående styrelse.

Att lägga till medlemmar i en samling fungerar på samma sätt som att lägga till medlemmar i en styrelse. En person eller ett team måste vara medlem i samlingen innan de kan läggas till som medlemmar i en styrelse i samlingen.

Mer information finns i [Hantera samlingar](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

[Visa en videodemonstration av den här funktionen](https://video.tv.adobe.com/v/3415609/){target=_blank}

## Beräkningsfält på anslutna kort mappar till artikelpunktsfält på Workfront-objekt

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att du har anmält dig till Workfront Boards så snart som möjligt.

Beräkningsfältet på anslutna kort i Workfront Boards mappar nu till artikelpunktsfältet för det associerade Workfront-objektet.

Det nya fältet Artikelpunkter är ett redigerbart frihandsfält som du kan lägga till i en vy i en lista eller rapport för uppgifter eller problem. Det är inte knutet till planerade timmar eller teamuppdrag.

Tidigare var kortberäkningen en manuell inmatning och mappades inte till något fält i en uppgift eller ett problem.

Uppskattningsfältet på både ad hoc-kort och anslutna kort har inte längre någon teckengräns. Tidigare var det maximala antalet tecken 99.

Mer information finns i [Använd anslutna kort på ritytor](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Kort för förhandsgranskning i inloppskolumnen

>[!NOTE]
>
>Den här funktionen är endast tillgänglig genom att du har anmält dig till Workfront Boards så snart som möjligt.

Nu kan du klicka på ett anslutet kort i intag-kolumnen för att se en version av innehållet som bara är för visning. Du kan inte redigera kortets innehåll förrän kortet flyttas från inmatningskolumnen till en annan kolumn på kortet.

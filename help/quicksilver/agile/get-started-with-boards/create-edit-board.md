---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Skapa eller redigera en anslagstavla
description: Från [!UICONTROL boards] kan du skapa en ny panel eller redigera en befintlig panel.
author: Lisa
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 0%

---

# Skapa eller redigera en anslagstavla

<!-- Audited: 12/2023 -->

Från [!UICONTROL boards] kan du skapa en ny panel eller redigera en befintlig panel.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td> <p>Nytt: Medarbetare eller högre </p>
 <p>eller</p> 
<p>Aktuell: [!UICONTROL Request] eller högre </p> 
</td> 
  </tr>
 </tbody> 
</table>

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa en ny anslagstavla

{{step1-to-boards}}

1. Klicka på **[!UICONTROL Add board]**.

1. Välj en mall för styrelsen.

   | Mall | Beskrivning |
   |---------|----------|
   | Grundläggande bräde | Tre standardkolumner finns på ritytan. Du kan lägga till nya kolumner och byta namn på eller ta bort standardkolumnerna. <p>Tre standardkolumner finns på ritytan. Du kan lägga till nya kolumner och byta namn på eller ta bort standardkolumnerna. |
   | Kanban board | Följande kolumner finns på ritytan: Backlog, New, In Progress, Complete och On Hold (Väntande). Du kan lägga till nya kolumner och byta namn på eller ta bort standardkolumnerna.<p>Om du vill använda eftersläpningen måste du ställa in filter för inloppskolumnen. Mer information finns i [Lägga till en inloppskolumn på en anslagstavla](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Om du vill granska standardprofilerna för varje kolumn klickar du på [!UICONTROL **Mer** meny] i en kolumn och markera [!UICONTROL **Redigera**]. Du kan ändra vilken profil som helst av dessa förinställda profiler. Mer information finns i [Hantera kortkolumner](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
   | Retrospektivkort | Följande kolumner finns i styrelsen: Vad gick bra? Vad skulle kunna förbättras? Vem ska vi fira? Vad kan vi göra för att gå fortare? Du kan lägga till nya kolumner och byta namn på eller ta bort standardkolumnerna. <p>Inga kolumnprinciper används. |
   | Dynamiskt kort | Följande kolumner finns på ritytan: Avmarkerad, Ny, Pågår, Väntande och Fullständig. Du kan lägga till nya kolumner och byta namn på eller ta bort standardkolumnerna. (Kolumnen Omarkerad kan byta namn men inte tas bort. Den här kolumnen innehåller alla kort med en status som inte matchar någon av de andra kolumnstatusarna.) <p>Standardkolumnprinciperna tilldelar kort till kolumner baserat på deras status. Mer information finns i [Hantera kortkolumner](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

1. För ett dynamiskt kort följer du stegen i installationsguiden:

   1. Ange ett namn för styrelsen och klicka på [!UICONTROL **Nästa**].
   1. Sök efter och markera [!DNL Workfront] [!UICONTROL **Projekt**] för att lägga in uppgifter och frågor i styrelsen.
   1. Sök efter och markera [!UICONTROL **Uppdrag**] för att lägga in uppgifter och frågor i styrelsen.

      Alla objekt visas på kortet som anslutna kort.

      The [!UICONTROL **Kort som läggs till**] räknaren visar hur många kort som kommer att finnas ombord. Om du till exempel markerar ett projekt med 100 uppgifter och ärenden visas 100 i räknaren. Om du lägger till en användartilldelning och den personen tilldelas 5 uppgifter i projektet visas 5.

      >[!NOTE]
      >
      >Kortgränsen för dynamiska kort är 700 uppgifter och 700 utgåvor, totalt 1 400 kort. Ett stort antal kort på kortet kan påverka kortets prestanda.

   1. (Valfritt) Välj [!UICONTROL **Arkivera inte färdiga kort**] för att lägga till slutförda uppgifter och ärenden till styrelsen som synliga kort i kolumnen Slutfört. När det här alternativet inte är markerat hämtas färdiga kort när styrelsen skapas till styrelsen som arkiverade kort.

      >[!NOTE]
      >
      >Som standard visas inte arkiverade kort på anslagstavlan. Om du vill visa arkiverade kort måste du aktivera en konfigurationsinställning och sedan filtrera ritytan så att arkiverade kort visas. Mer information finns i [Anpassa vilka fält som visas på ett kort](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md) och [Filtrera och söka på en anslagstavla](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

   1. (Valfritt) Klicka på [!UICONTROL **Använd avancerade filter**] om du vill visa ytterligare filteralternativ.

      Detta är samma process som när du skapar ett filter för en inloppskolumn. Mer information finns i [Lägga till en inloppskolumn på en anslagstavla](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

      Om du uppdaterar filtren på ett dynamiskt kort efter att det har skapats, återställs kortinställningar som inte ingår i Workfront-aktiviteten eller -problemet (till exempel taggar).

   1. När du lagt till filtren klickar du på [!UICONTROL **Skapa anslagstavla**].

1. Ange ett namn för styrelsen i **[!UICONTROL Board]** och tryck på Retur.
1. Konfigurera styrelsen efter behov.

   Mer information finns i [Lägga till eller ta bort medlemmar från en anslagstavla](../../agile/get-started-with-boards/add-members-to-board.md), [Hantera kortkolumner](../../agile/get-started-with-boards/manage-board-columns.md), [Lägga till ett ad hoc-kort till en anslagstavla](../../agile/get-started-with-boards/add-card-to-board.md)och [Använd anslutna kort på ritytor](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

1. Klicka **[!UICONTROL All Boards]** för att gå tillbaka till panelernas kontrollpanel.

   Du kan också hitta den nedrullningsbara menyn som är märkt med namnet på aktuell anslagstavla och klicka på den för att växla till en annan anslagstavla.

   ![Förteckning över styrelser](assets/boards-button-list-of-boards-350x188.png)

## Redigera en befintlig styrelse

{{step1-to-boards}}

1. På kontrollpanelen väljer du den panel som ska öppnas.
1. Redigera styrelsen efter behov. Du kan klicka på styrelsens namn för att byta namn på det.

   Mer information finns i [Lägga till eller ta bort medlemmar från en anslagstavla](../../agile/get-started-with-boards/add-members-to-board.md), [Hantera kortkolumner](../../agile/get-started-with-boards/manage-board-columns.md)och [Lägg till ett kort till en anslagstavla](../../agile/get-started-with-boards/add-card-to-board.md).

1. Klicka **[!UICONTROL All Boards]** för att gå tillbaka till panelernas kontrollpanel.

   Du kan också hitta den nedrullningsbara menyn som är märkt med namnet på aktuell anslagstavla och klicka på den för att växla till en annan anslagstavla.


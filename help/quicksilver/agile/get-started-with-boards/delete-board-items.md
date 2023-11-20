---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Ta bort eller arkivera ett kort från en anslagstavla
description: När du tar bort ett kort från en anslagstavla tas det bort permanent och kan inte återställas. När du arkiverar ett kort skickas det till arkivet och du kan återställa det till styrelsen senare.
author: Lisa
feature: Agile
exl-id: 68b7d2e5-92f0-462d-8122-eaecb1e6b87c
source-git-commit: b6a824ac6248c86043f7f21866c8a14a6c97602f
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# Ta bort eller arkivera ett kort från en anslagstavla

När du tar bort ett kort från en anslagstavla tas det bort permanent och kan inte återställas. När du arkiverar ett kort skickas det till arkivet och du kan återställa det till styrelsen senare.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>[!UICONTROL Request] eller högre</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta din [!DNL Workfront] administratör.

## Ta bort ett kort från en anslagstavla

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Boards]**.
1. Gå till en styrelse. Mer information finns i [Skapa eller redigera en anslagstavla](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicka på **[!UICONTROL More]** meny ![Menyn Mer](assets/more-icon-spectrum.png) på kortet och välj **[!UICONTROL Delete]**.
1. Klicka **[!UICONTROL Delete]** på bekräftelsemeddelandet.

## Arkivera ett kort från en styrelse

1. Gå till styrelsen.
1. Klicka på **[!UICONTROL More]** meny ![Menyn Mer](assets/more-icon-spectrum.png) på kortet och välj **[!UICONTROL Archive]**.

   Arkiverade kort är dolda från anslagstavlan om du inte använder ett filter för att visa dem. Mer information finns i [Filtrera en anslagstavla för att visa arkiverade kort](#filter-a-board-to-show-archived-cards) i den här artikeln.

   An [!UICONTROL Archive] icon ![Arkiv](assets/archive-icon-spectrum-25x20.png) visas på arkiverade kort. Du kan inte redigera ett arkiverat kort, men du kan ta bort det eller flytta det till en annan kolumn.

1. Klicka på knappen **[!UICONTROL More]** meny ![Menyn Mer](assets/more-icon-spectrum.png) på kortet och välj **[!UICONTROL Restore]**.

## Filtrera en anslagstavla för att visa arkiverade kort {#filter-a-board-to-show-archived-cards}

Som standard visas bara aktiva kort på en anslagstavla. Du kan filtrera anslagstavlan så att även arkiverade kort visas.

1. Gå till styrelsen.
1. Klicka [!UICONTROL **Konfigurera**] till höger om ritytan för att öppna panelen Konfigurera.
1. Expandera [!UICONTROL **Kort**].
1. Aktivera [!UICONTROL **Visa arkiverade kort direkt**].
1. Klicka [!UICONTROL **Filter**], expandera [!UICONTROL Archived Cards] och markera **[!UICONTROL Archived cards]** för att visa eventuella arkiverade kort.

   Filtret visar antalet arkiverade kort.

   ![Filtrera arkiverade kort](assets/filter-by-archived-cards.png)

   >[!NOTE]
   >
   >The [!UICONTROL Archived Cards] -avsnittet är inte tillgängligt i filtret om du inte har aktiverat konfigurationsinställningen för att visa arkiverade kort. Mer information finns i [Anpassa vilka fält som visas på ett kort](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Välj **[!UICONTROL Archived cards]** igen för att ta bort alternativet och endast visa aktiva kort.

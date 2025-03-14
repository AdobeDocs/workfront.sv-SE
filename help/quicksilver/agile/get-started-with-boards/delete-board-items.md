---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Ta bort eller arkivera ett kort från en styrelse
description: När du tar bort ett kort från en anslagstavla tas det bort permanent och kan inte återställas. När du arkiverar ett kort skickas det till arkivet och du kan återställa det till styrelsen senare.
author: Lisa
feature: Agile
exl-id: 68b7d2e5-92f0-462d-8122-eaecb1e6b87c
source-git-commit: 81e87793905fd925db00c7a0ac107150263a1365
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# Ta bort eller arkivera ett kort från en anslagstavla

När du tar bort ett ad hoc-kort från en anslagstavla tas det bort permanent och kan inte återställas. Anslutna kort kan läggas till manuellt på en bräda när de har tagits bort.

Om du tar bort ett anslutet kort från en dynamisk anslagstavla visas det igen när du uppdaterar anslagstavlan eftersom den här typen av kort hämtar alla uppgifter och problem från ett visst projekt. Om du vill ta bort kortet måste du ta bort den anslutna aktiviteten eller utgåvan från Workfront-projektet.

När du tar bort ett anslutet kort från en annan korttyp som har en inloppskolonn, visas kortet igen i inloppskolonnen när du uppdaterar kortet om den anslutna aktiviteten eller utdraget inte har markerats som slutfört än. Mer information om inloppskolumner finns i [Lägga till en inloppskolumn på en anslagstavla](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

När du arkiverar ett kort skickas det till arkivet och du kan återställa det till styrelsen senare.

Arkiverade kort synkroniseras inte med Workfront-uppgifter och -problem. Om du återställer ett kort synkroniseras det igen.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td> 
   <p>Nytt: [!UICONTROL Contributor] eller senare</p> 
   <p>eller</p>
   <p>Aktuell: [!UICONTROL Request] eller högre</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ta bort ett kort från en anslagstavla

{{step1-to-boards}}

1. Gå till en styrelse. Mer information finns i [Skapa eller redigera en anslagstavla](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicka på **[!UICONTROL More]**-menyn ![Mer meny](assets/more-icon-spectrum.png) på kortet och välj **[!UICONTROL Delete]**.
1. Klicka på **[!UICONTROL Delete]** i bekräftelsemeddelandet.

## Arkivera ett kort från en styrelse

1. Gå till styrelsen.
1. Klicka på **[!UICONTROL More]**-menyn ![Mer meny](assets/more-icon-spectrum.png) på kortet och välj **[!UICONTROL Archive]**.

   Arkiverade kort är dolda från anslagstavlan om du inte använder ett filter för att visa dem. Mer information finns i [Filtrera en anslagstavla för att visa arkiverade kort](#filter-a-board-to-show-archived-cards) i den här artikeln.

   En [!UICONTROL Archive]-ikon ![Arkiv](assets/archive-icon-spectrum-25x20.png) visas på arkiverade kort. Du kan inte redigera ett arkiverat kort, men du kan ta bort det eller flytta det till en annan kolumn.

1. Om du vill återställa ett arkiverat kort klickar du på **[!UICONTROL More]**-menyn ![Mer-menyn](assets/more-icon-spectrum.png) på kortet och väljer **[!UICONTROL Restore]**.

## Filtrera en anslagstavla för att visa arkiverade kort

Som standard visas bara aktiva kort på en anslagstavla. Du kan filtrera anslagstavlan så att även arkiverade kort visas.

1. Gå till styrelsen.
1. Klicka på [!UICONTROL **Konfigurera**] till höger på kortet för att öppna konfigurationspanelen.
1. Expandera [!UICONTROL **kort**].
1. Aktivera [!UICONTROL **Visa arkiverade kort på anslagstavlan**].
1. Klicka på [!UICONTROL **Filter**], expandera avsnittet [!UICONTROL Archived Cards] och välj **[!UICONTROL Archived cards]** om du vill visa arkiverade kort.

   Filtret visar antalet arkiverade kort.

   ![Filtrera arkiverade kort](assets/filter-by-archived-cards.png)

   >[!NOTE]
   >
   >Avsnittet [!UICONTROL Archived Cards] är inte tillgängligt i filtret om du inte har aktiverat konfigurationsinställningen för att visa arkiverade kort. Mer information finns i [Anpassa vilka fält som ska visas på ett kort](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Välj **[!UICONTROL Archived cards]** igen om du vill ta bort alternativet och bara visa aktiva kort.

---
filename: configure-card-falloff.md
content-type: reference
navigation-topic: boards
title: Konfigurera kortutfall
description: Du kan konfigurera en styrelse så att kort arkiveras eller faller bort från styrelsen enligt ett schema.
author: Lisa
exl-id: 0e4f6b3c-75aa-4314-9cb0-737e5a9d3bda
source-git-commit: 5114a135c510d5a7020fd0a0862f9dcc61d9ad93
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---

# Konfigurera kortutfall

Du kan konfigurera en styrelse så att kort arkiveras, eller&quot;faller bort&quot; från styrelsen, enligt ett schema. Du kan ange att kort i en viss kolumn ska dras av från anslaget på ett visst antal dagar eller veckor.

När ett kort faller utanför styrelsen arkiveras det. Du kan visa arkiverade kort med ett filter. Mer information finns i [Filtrera och söka på en anslagstavla](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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

&#42;Kontakta [!DNL Workfront] administratör.

## Konfigurera kortutfall

1. Klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Boards]**.
1. Gå till en anslagstavla. Mer information finns i [Skapa eller redigera en anslagstavla](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicka **[!UICONTROL Configure]** till höger om anslagstavlan för att öppna konfigurationspanelen.
1. Expandera **[!UICONTROL Cards]**.
1. Aktivera **[!UICONTROL Automatically archive cards from the board]**.

   ![Inställningar för kortavstängning](assets/card-falloff-switch.png)

1. Välj när kort ska arkiveras från styrelsen. Du kan välja upp till 8 veckor eller upp till 60 dagar.

   Datumet avgörs från när kortet senast ändrades.

1. Välj vilken kolumn du vill ta bort kort från.
1. Klicka **[!UICONTROL Save]** på bekräftelsemeddelandet.
1. Klicka **[!UICONTROL Hide configure]** för att stänga [!UICONTROL Configure] -panelen. Konfigurationsinställningarna används automatiskt när du uppdaterar ritytan.

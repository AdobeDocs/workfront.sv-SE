---
filename: configure-card-falloff.md
content-type: reference
navigation-topic: boards
title: Konfigurera kortutfall
description: Du kan konfigurera en styrelse så att kort arkiveras eller faller bort från styrelsen enligt ett schema.
author: Jenny
feature: Agile
exl-id: 0e4f6b3c-75aa-4314-9cb0-737e5a9d3bda
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# Konfigurera kortutfall

Du kan konfigurera en styrelse så att kort arkiveras, eller&quot;faller bort&quot; från styrelsen, enligt ett schema. Du kan ange att kort i en viss kolumn ska dras av från anslaget på ett visst antal dagar eller veckor.

När ett kort faller utanför styrelsen arkiveras det. Du kan visa arkiverade kort med ett filter. Mer information finns i [Filtrera och söka på en anslagstavla](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> 
   <p>Medarbetare eller högre</p> 
   <p>Begäran eller senare</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurera kortutfall

{{step1-to-boards}}

1. Gå till en styrelse. Mer information finns i [Skapa eller redigera en anslagstavla](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicka på **[!UICONTROL Configure]** till höger om kortet för att öppna konfigurationspanelen.
1. Expandera **[!UICONTROL Cards]**.
1. Aktivera **[!UICONTROL Automatically archive cards from the board]**.

   ![Inställningar för kortavstängning](assets/card-falloff-switch.png)

1. Välj när kort ska arkiveras från styrelsen. Du kan välja upp till 8 veckor eller upp till 60 dagar.

   Datumet avgörs från när kortet senast ändrades.

1. Välj vilken kolumn du vill ta bort kort från.
1. Klicka på **[!UICONTROL Save]** i bekräftelsemeddelandet.
1. Klicka på **[!UICONTROL Hide configure]** för att stänga panelen [!UICONTROL Configure]. Konfigurationsinställningarna används automatiskt när du uppdaterar ritytan.

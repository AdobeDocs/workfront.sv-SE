---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: Hantera PIA-gränsen (Work in Progress) på en moderlista
description: Du kan konfigurera en PIA-gräns (Work In Progress) för varje kolumn på en anslagstavla.
author: Lisa
feature: Agile
exl-id: 7901c6e7-75a4-41e4-b288-d527c4a6d031
source-git-commit: 09ab9912df9ad2ac30a461f22b585d633fc73b23
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# Hantera [!UICONTROL Work in Progress] (PIA) begränsning av antalet anställda

Du kan konfigurera en [!UICONTROL Work In Progress] (PIA) för varje kolumn på en anslagstavla.

Pågående arbete-begränsningen är bara en visuell varning och förhindrar inte att du har fler objekt i varje kolumn än den gräns du anger.

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

## Ange PIA-gräns för en kolumn

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Boards]**.
1. Gå till en anslagstavla. Mer information finns i [Skapa eller redigera en anslagstavla](../../agile/get-started-with-boards/create-edit-board.md).
1. Leta reda på den kolumn som du vill lägga till PIA-gränsen i.

   Information om hur du lägger till en ny kolumn finns i [Hantera kortkolumner](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

1. Klicka på **[!UICONTROL More]** -menyn i kolumnen och väljer **[!UICONTROL Edit]** för att öppna området Inställningar.
1. Under [!UICONTROL Column Policies], aktivera **[!UICONTROL Work in progress]limit** princip för att begränsa antalet kort som kan läggas till i kolumnen.
1. Ange begränsningsnumret i dialogrutan **[!UICONTROL Set limit]** fält.

   ![PIA-gräns för kolumn](assets/boards-wip-limit-in-column.png)

   Antalet kort och gränsen visas överst i kolumnen. Om kolumnen innehåller fler kort än gränsen blir räknaren röd.

   ![Räknare för PIA-begränsning](assets/boards-wip-limit-counter.png)

1. Klicka **[!UICONTROL Close]** för att avsluta [!UICONTROL Settings] och visa kolumnen och dess kort.

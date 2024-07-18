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

# Hantera gränsen för [!UICONTROL Work in Progress] (PIA) på ett moderkort

Du kan konfigurera en [!UICONTROL Work In Progress] (WIP)-gräns för varje kolumn på en anslagstavla.

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

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Ange PIA-gräns för en kolumn

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront] och klicka sedan på **[!UICONTROL Boards]**.
1. Gå till en styrelse. Mer information finns i [Skapa eller redigera en anslagstavla](../../agile/get-started-with-boards/create-edit-board.md).
1. Leta reda på den kolumn som du vill lägga till PIA-gränsen i.

   Mer information om hur du lägger till en ny kolumn finns i [Hantera kortpanelskolumner](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

1. Klicka på menyn **[!UICONTROL More]** i kolumnen och välj **[!UICONTROL Edit]** för att öppna inställningsområdet.
1. Under [!UICONTROL Column Policies] aktiverar du principen **[!UICONTROL Work in progress]limit** för att begränsa antalet kort som kan läggas till i kolumnen.
1. Skriv gränsnumret i fältet **[!UICONTROL Set limit]**.

   ![Pågående arbete-begränsning för kolumn](assets/boards-wip-limit-in-column.png)

   Antalet kort och gränsen visas överst i kolumnen. Om kolumnen innehåller fler kort än gränsen blir räknaren röd.

   ![Räknare för PIA-begränsning](assets/boards-wip-limit-counter.png)

1. Klicka på **[!UICONTROL Close]** för att avsluta området [!UICONTROL Settings] och visa kolumnen och dess kort.

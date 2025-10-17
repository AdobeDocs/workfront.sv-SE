---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: Hantera PIA-gränsen (Work in Progress) för en styrelse
description: Du kan konfigurera en PIA-gräns (Work In Progress) för varje kolumn på en anslagstavla.
author: Jenny
feature: Agile
exl-id: 7901c6e7-75a4-41e4-b288-d527c4a6d031
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 0%

---

# Hantera gränsen för [!UICONTROL Work in Progress] (PIA) på ett moderkort

Du kan konfigurera en [!UICONTROL Work In Progress] (WIP)-gräns för varje kolumn på en anslagstavla.

Pågående arbete-begränsningen är bara en visuell varning och förhindrar inte att du har fler objekt i varje kolumn än den gräns du anger.

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

## Ange PIA-gräns för en kolumn

{{step1-to-boards}}

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

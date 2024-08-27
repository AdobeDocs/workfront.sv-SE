---
content-type: reference
navigation-topic: boards
title: Migrera Agile Team Kanban-kort till Workfront Boards
description: Du kan migrera dina arbetsuppgifter från en smidig team-kanban-styrelse till en ny eller befintlig Workfront-styrelse.
author: Lisa
feature: Agile
exl-id: 72e3902b-af9a-497c-817f-63630c4fb73b
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# Migrera smidiga team-kanban-kort till Workfront-styrelser

Du kan migrera dina arbetsuppgifter från en smidig team-kanban-styrelse till en ny eller befintlig Workfront-styrelse. När du kör migreringen kopieras alla kort på Kanban-tavlan till Workfront styrelse. Du får inte välja specifika kort.

Kortens placering på Workfront board baseras på spaltregler. (En princip kan till exempel flytta alla kort med statusen &quot;Pågår&quot; till en viss kolumn. Mer information om kolumnprinciper finns i [Hantera board-kolumner](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).) Om det inte finns några profiler eller om korten inte matchar profilerna placeras korten i kolumnen längst till vänster på ritytan. För närvarande läggs inga kort i kolumnen Eftersläpning på det äldre kortet till på Workfront-kortet.

Korten tas inte bort från den flexibla teamets Kanban-tavla, och kortstatusändringarna synkroniseras med båda tavlorna. Du kan låta båda styrelserna vara aktiva tills du är redo att byta till Workfront Boards.

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

## Migrera Kanban-kort till en ny anslagstavla

{{step1-to-team}}

1. Gå till en kanban-tavla.
1. Klicka på [!UICONTROL **Lägg till i anslagstavlor**] och välj [!UICONTROL **Ny anslagstavla**].
1. I dialogrutan [!UICONTROL Add to new board] anger du ett namn för den nya ritytan (namnet på den aktuella [!UICONTROL Kanban]-ritytan visas automatiskt) och klickar på [!UICONTROL **Lägg till**].

   ![Lägg till kanban-kort till ny anslagstavla](assets/add-kanban-cards-to-new-board-dialog.png)

1. (Valfritt) Klicka på länken för att öppna den nya anslagstavlan i det meddelande som visas.

## Migrera kanban-kort till en befintlig anslagstavla

{{step1-to-team}}

1. Gå till en kanban-tavla.
1. Klicka på [!UICONTROL **Lägg till i anslagstavlor**] och välj [!UICONTROL **Befintlig anslagstavla**].
1. I dialogrutan [!UICONTROL Add to existing board] söker du efter och väljer den anslagstavla som korten ska migreras till. Klicka sedan på [!UICONTROL **Lägg till**].

   ![Lägg till kanban-kort till befintlig anslagstavla](assets/add-kanban-cards-to-existing-board-dialog.png)

1. (Valfritt) Klicka på länken för att öppna anslagstavlan i det meddelande som visas.

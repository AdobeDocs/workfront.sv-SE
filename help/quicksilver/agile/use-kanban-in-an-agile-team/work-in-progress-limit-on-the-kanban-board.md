---
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: Hantera gränsen för pågående arbete på Kanban-tavlan
description: Du kan konfigurera en PIA-gräns (Work In Progress) för varje kolumn på Kanban-tavlan. Gränsen för pågående arbete är bara en visuell varning och förhindrar inte ditt team från att ha fler objekt i varje statuskolumn än den gräns som du anger.
author: Lisa
feature: Agile
exl-id: 540880ad-46af-416b-8e0b-5df869555424
source-git-commit: 33daf0633701a1c271552e796ffe22a58645c561
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---

# Hantera [!UICONTROL work in progress] (PIA) gräns för Kanban-tavlan

Du kan konfigurera en [!UICONTROL Work In Progress] (PIA) för varje kolumn på [!UICONTROL Kanban] board, enligt beskrivningen i artikeln [Konfigurera Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

Gränsen för pågående arbete är bara en visuell varning och förhindrar inte ditt team från att ha fler objekt i varje statuskolumn än den gräns som du anger.

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
   <td> <p>[!UICONTROL Work] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>[!UICONTROL Worker] eller högre</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] administratören kan ändra din åtkomstnivå, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Visa [!UICONTROL Work In Progress] (PIA) på [!UICONTROL Kanban] board

När en PIA-gräns har konfigurerats för ditt mobila team visas den i det övre högra hörnet i varje kolumn på Kanban-tavlan (med undantag för [!UICONTROL Complete] kolumn).

Varje gång som gränsen överskrids för en kolumn på [!UICONTROL Kanban] boardtavlan markeras gränsen i rött och ett meddelande visas.\
![PIA-gräns](assets/kanban-wip.png)

## Uppdatera [!UICONTROL Work In Progress] (PIA) från [!UICONTROL Kanban] board

Gruppmedlemmar med [!UICONTROL Edit] rättigheter kan uppdatera PIA-gränsen för varje statuskolumn direkt från [!UICONTROL Kanban] bräda. Du kan även uppdatera PIA-gränsen enligt beskrivningen i artikeln [Konfigurera Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Teams]**.

1. (Valfritt) Klicka på **[!UICONTROL Switch team]** icon ![Byt ikon för team](assets/switch-team-icon.png)och sedan antingen välja en ny [!UICONTROL Kanban] i listrutan eller sök efter ett team i sökfältet.

1. På [!UICONTROL Kanban] går du till WIP-gränsen i det övre högra hörnet av varje kolumn på Kanban-tavlan.
1. Klicka på den PIA-gräns som du vill ändra och ange sedan en ny gräns.
1. Tryck **[!UICONTROL Enter]**.

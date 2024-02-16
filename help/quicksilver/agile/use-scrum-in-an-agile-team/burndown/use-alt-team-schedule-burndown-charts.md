---
product-area: agile-and-teams
navigation-topic: burndown
title: Använd ett alternativt teamschema för nedladdningsscheman
description: Scheman som definieras i [!DNL Adobe Workfront] påverka nedladdningsschemat genom att utesluta dagar lediga (helger och helgdagar) från nedladdningen.
author: Lisa
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
source-git-commit: ddff70b61a2c3b3479e278bb3bb8628ac83f5c97
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Använd ett alternativt teamschema för nedladdningsscheman

Scheman som definieras i [!DNL Adobe Workfront] påverka nedladdningsschemat genom att utesluta dagar lediga (helger och helgdagar) från nedladdningen.

Som standard används standardschemat för nedladdningsschemat. Förutom standardschemat kan team även välja att använda ett alternativt schema för att inkludera teamspecifika, icke-arbetsrelaterade dagar. Det alternativa schemat visas sedan i nedladdningsschemat för alla upprepningar som har tilldelats teamet. Det alternativa schemat påverkar bara nedladdningsschemat. (Mer information om standardschemat och hur [!DNL Workfront] administratörer kan skapa ett teamspecifikt schema, se [Skapa ett schema](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).)

Nedladdningsschemat tar inte hänsyn till vissa dagar. Om ditt team till exempel arbetar fyra timmar varje fredag visas det som en heldag i nedladdningsschemat.

Mer information om hur du använder nedladdningsschemat finns i [Översikt över Agile-nedladdningsdiagram](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

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
   <td> <p>[!UICONTROL Work] eller högre</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Om du vill veta vilken plan eller licenstyp du har kontaktar du [!DNL Workfront] administratör.

## Använd ett alternativt teamschema för nedladdningsscheman

1. Se till att [!DNL Workfront] administratören har redan skapat det alternativa schemat, vilket beskrivs i [Skapa ett schema](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Teams]**.

1. (Valfritt) Klicka på **[!UICONTROL Switch team]** icon ![Byt ikon för team](assets/switch-team-icon.png)väljer du sedan ett nytt Scrum-team i listrutan eller söker efter ett team i sökfältet.

1. Välj det flexibla team som du vill hantera.
1. Klicka på **[!UICONTROL More]** väljer du **[!UICONTROL Edit]**.

1. I **[!UICONTROL Agile]** i **[!UICONTROL Schedule]** väljer du det nya schemat i listrutan.

1. Klicka på **[!UICONTROL Save Changes]**.

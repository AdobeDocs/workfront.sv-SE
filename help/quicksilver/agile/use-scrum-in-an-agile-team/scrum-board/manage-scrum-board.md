---
product-area: agile-and-teams;projects;user-management
navigation-topic: scrum-board
title: Hantera artiklar och ärenden på Scrum Board
description: Du kan flytta en artikel eller ett problem från Urklipp till en annan upprepning eller till eftersläpningen, eller ta bort det från Urklipp. När du tar bort en artikel eller ett problem flyttas den till papperskorgen i 30 dagar och kan endast återställas av systemadministratören.
author: Jenny
feature: Agile
exl-id: 72990251-0264-4e68-83ef-1a9cde5b685c
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Hantera artiklar och problem på [!UICONTROL Scrum]-panelen

Du kan flytta en artikel eller ett problem från [!UICONTROL Scrum]-panelen till en annan iteration eller till eftersläpningen, eller ta bort den från [!UICONTROL Scrum]-panelen. När du tar bort en artikel eller ett problem flyttas den till papperskorgen i 30 dagar och kan endast återställas av systemadministratören.

Om du vill ta bort en uppgift eller ett problem från upprepningen utan att ta bort den eller skicka den till eftersläpningen går du till projektet och tar bort teamet från uppdragskolumnen. Detta tar bort uppgiften eller problemet från kontrollpanelen, men det finns kvar i projektet.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td> <p>Nytt: [!UICONTROL Standard]</p> 
   eller
   <p>Aktuell: [!UICONTROL Work] eller högre</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>[!UICONTROL Manage] behörighet till uppgiften eller problemet </td> 
  </tr>
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Flytta en artikel eller ett problem från [!UICONTROL Scrum]-panelen

{{step1-to-team}}

1. Klicka på ikonen **[!UICONTROL Switch team]** ![Byt ikon för team](assets/switch-team-icon.png) och välj sedan ett Scrum-team i listrutan eller sök efter ett team i sökfältet.
1. I den vänstra panelen väljer du **[!UICONTROL Iterations]** om du vill välja en viss iteration eller **[!UICONTROL Current Iteration]**.
1. Klicka på ikonen **[!UICONTROL More]** för artikeln eller utgåvan och välj **[!UICONTROL Move to]**.

   ![Ta bort eller flytta en artikel från Urklipp](assets/scrum-delete-move-story.png)

1. Välj något av följande i bekräftelsemeddelandet:

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Another iteration]</strong></td>
        <td>Välj att flytta objektet till en annan iteration och välj sedan vilken iteration artikeln eller utgåvan ska flyttas till. Om inga framtida iterationer definieras kan du inte flytta objektet.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Backlog]</strong></td>
        <td>Välj om du vill flytta artikeln eller utgåvan till teamets eftersläpning.</td>
    </tr>
   </table>

   >[!NOTE]
   >
   >Arbetsobjektet [!UICONTROL Planned Start Date] och [!UICONTROL Planned Completion Date] påverkas av en inställning på sidan [!UICONTROL Edit Team]. Mer information finns i avsnittet [[!UICONTROL Configure] om hur datum tillämpas när arbetsobjekt läggs till i en iteration](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) i artikeln [Konfigurera repet](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Klicka på **[!UICONTROL Move]**.

## Ta bort en artikel eller ett problem från [!UICONTROL Scrum]-panelen

{{step1-to-team}}

1. Klicka på ikonen **[!UICONTROL Switch team]** ![Byt ikon för team](assets/switch-team-icon.png) och välj sedan ett Scrum-team i listrutan eller sök efter ett team i sökfältet.
1. I den vänstra panelen väljer du **[!UICONTROL Iterations]** om du vill välja en viss iteration eller **[!UICONTROL Current Iteration]**.
1. Klicka på ikonen **[!UICONTROL More]** för artikeln eller utgåvan och välj **[!UICONTROL Delete Story]** eller **[!UICONTROL Delete Issue]**.

   ![Ta bort eller flytta en artikel från Urklipp](assets/scrum-delete-move-story.png)

1. Klicka på **[!UICONTROL Yes, delete it]** i bekräftelsemeddelandet.

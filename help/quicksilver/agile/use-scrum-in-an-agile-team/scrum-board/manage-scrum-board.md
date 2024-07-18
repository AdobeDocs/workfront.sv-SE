---
product-area: agile-and-teams;projects;user-management
navigation-topic: scrum-board
title: Hantera artiklar och problem på Scrum board
description: Du kan flytta en artikel eller ett problem från Urklipp till en annan upprepning eller till eftersläpningen, eller ta bort det från Urklipp. När du tar bort en artikel eller ett problem flyttas den till papperskorgen i 30 dagar och kan endast återställas av systemadministratören.
author: Lisa
feature: Agile
exl-id: 72990251-0264-4e68-83ef-1a9cde5b685c
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---

# Hantera artiklar och problem på [!UICONTROL Scrum]-panelen

Du kan flytta en artikel eller ett problem från [!UICONTROL Scrum]-panelen till en annan iteration eller till eftersläpningen, eller ta bort den från [!UICONTROL Scrum]-panelen. När du tar bort en artikel eller ett problem flyttas den till papperskorgen i 30 dagar och kan endast återställas av systemadministratören.

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
   <td> <p>[!UICONTROL Worker] eller högre</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>[!UICONTROL Manage] behörighet till uppgiften eller problemet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Flytta en artikel eller ett problem från [!UICONTROL Scrum]-panelen

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront] och klicka sedan på **[!UICONTROL Teams]**.
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

## Ta bort artikeln eller utgåvan från [!UICONTROL Scrum]-tavlan

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront] och klicka sedan på **[!UICONTROL Teams]**.
1. Klicka på ikonen **[!UICONTROL Switch team]** ![Byt ikon för team](assets/switch-team-icon.png) och välj sedan ett Scrum-team i listrutan eller sök efter ett team i sökfältet.
1. I den vänstra panelen väljer du **[!UICONTROL Iterations]** om du vill välja en viss iteration eller **[!UICONTROL Current Iteration]**.
1. Klicka på ikonen **[!UICONTROL More]** för artikeln eller utgåvan och välj **[!UICONTROL Delete Story]** eller **[!UICONTROL Delete Issue]**.

   ![Ta bort eller flytta en artikel från Urklipp](assets/scrum-delete-move-story.png)

1. Klicka på **[!UICONTROL Yes, delete it]** i bekräftelsemeddelandet.

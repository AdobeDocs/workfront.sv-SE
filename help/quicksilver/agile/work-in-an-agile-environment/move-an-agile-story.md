---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Flytta en flexibel artikel
description: Du kan flytta en flexibel artikel till en annan upprepning (för Scrum-team) eller till eftersläpningen (för Kanban- och Scrum-team).
author: Lisa
feature: Agile
exl-id: 0058792e-66b8-4e54-8ce3-50171adff875
source-git-commit: 11009f24cd482e83319ed9f1ecf3f7a2f4e79d52
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 1%

---

# Flytta en flexibel artikel

Du kan flytta en flexibel artikel till en annan upprepning (för Scrum-team) eller till eftersläpningen (för Kanban- och Scrum-team).

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
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>[!UICONTROL Worker] eller högre</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>[!UICONTROL Manage] åtkomst till artikeln</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Flytta en artikel från en iteration eller en kanban-tavla till eftersläpningen

1. Gå till den iteration eller den kanban-panel som innehåller artikeln som du vill flytta till eftersläpningen.
1. Klicka på upprepningsrubriken överst på sidan.
1. På **[!UICONTROL Stories]** markerar du de artiklar som du vill flytta.
1. Klicka på **[!UICONTROL More]** > **[!UICONTROL Move to]**.

   The **[!UICONTROL Move Story]** visas.

   ![Dialogrutan Flytta artikel](assets/iteration-story-move.png)

1. Välj *team_name*&#39;s Backlog.\
   I ovanstående exempel är teamnamnet &#x200B; **Marknadsföring.**

1. Klicka på **[!UICONTROL Move Story]**.

## Flytta en artikel till en annan upprepning

Du kan flytta en berättelse till en annan upprepning för ditt Scrum-team.

>[!NOTE]
>
>The **[!UICONTROL Move to]** är inte tillgängligt för överordnade artiklar på en iteration. Du kan bara flytta underaktiviteter till en annan iteration.

1. Gå till den iteration som innehåller artikeln som du vill flytta.
1. Klicka på upprepningsrubriken överst på sidan.
1. På **[!UICONTROL Stories]** markerar du de artiklar som du vill flytta.
1. Klicka på **[!UICONTROL More]** > **[!UICONTROL Move to]**.

   The **[!UICONTROL Move Story]** visas.

   ![Dialogrutan Flytta artikel](assets/iteration-story-move.png)

1. Välj **[!UICONTROL Another Iteration]** väljer du den iteration där du vill flytta artikeln i listrutan.

   >[!NOTE]
   >
   >Arbetsuppgiften [!UICONTROL Planned Start Date] och [!UICONTROL Planned Completion Date] påverkas av en inställning på [!UICONTROL Edit Team] sida. Mer information finns i avsnittet [[!UICONTROL Configure] hur datum används när arbetsobjekt läggs till i en iteration](../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) i artikeln [Konfigurera Scrum](../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Klicka på **[!UICONTROL Move Story]**.

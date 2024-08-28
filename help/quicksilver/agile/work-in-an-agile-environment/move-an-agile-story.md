---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Flytta en Agile Story
description: Du kan flytta en flexibel artikel till en annan upprepning (för Scrum-team) eller till eftersläpningen (för Kanban- och Scrum-team).
author: Lisa
feature: Agile
exl-id: 0058792e-66b8-4e54-8ce3-50171adff875
source-git-commit: 452f8ddc5268a0d67e32090d166199f2fad7dbc7
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# Flytta en flexibel artikel

Du kan flytta en flexibel artikel till en annan upprepning (för Scrum-team) eller till eftersläpningen (för Kanban- och Scrum-team).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td>[!UICONTROL Manage] åtkomst till artikeln</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Flytta en artikel från en iteration eller en kanban-tavla till eftersläpningen

1. Gå till den iteration eller den kanban-panel som innehåller artikeln som du vill flytta till eftersläpningen.
1. Klicka på iterationshuvudet högst upp på sidan.
1. Markera de artiklar som du vill flytta på fliken **[!UICONTROL Stories]**.
1. Klicka på **[!UICONTROL More]** > **[!UICONTROL Move to]**.

   Dialogrutan **[!UICONTROL Move Story]** visas.

   ![Dialogrutan Flytta artikel](assets/iteration-story-move.png)

1. Välj **team_name&#39;s Backlog**.
I ovanstående exempel är teamnamnet **Marknadsföring**.

1. Klicka på **[!UICONTROL Move Story]**.

## Flytta en artikel till en annan upprepning

Du kan flytta en berättelse till en annan upprepning för ditt Scrum-team.

>[!NOTE]
>
>Alternativet **[!UICONTROL Move to]** är inte tillgängligt för överordnade artiklar i en iteration. Du kan bara flytta underaktiviteter till en annan iteration.

1. Gå till den iteration som innehåller artikeln som du vill flytta.
1. Klicka på iterationshuvudet högst upp på sidan.
1. Markera de artiklar som du vill flytta på fliken **[!UICONTROL Stories]**.
1. Klicka på **[!UICONTROL More]** > **[!UICONTROL Move to]**.

   Dialogrutan **[!UICONTROL Move Story]** visas.

   ![Dialogrutan Flytta artikel](assets/iteration-story-move.png)

1. Välj **[!UICONTROL Another Iteration]** och välj sedan den iteration där du vill flytta artikeln i den nedrullningsbara menyn.

   >[!NOTE]
   >
   >Arbetsobjektet [!UICONTROL Planned Start Date] och [!UICONTROL Planned Completion Date] påverkas av en inställning på sidan [!UICONTROL Edit Team]. Mer information finns i avsnittet [[!UICONTROL Configure] om hur datum tillämpas när arbetsobjekt läggs till i en iteration](../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) i artikeln [Konfigurera repet](../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Klicka på **[!UICONTROL Move Story]**.

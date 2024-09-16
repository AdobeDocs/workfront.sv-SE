---
product-area: enterprise-scenario-planner-product-area
keywords: plan,behörigheter,resurs,initiativ,,scenarier,scenario
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Begär åtkomst till en plan i scenarioplanen
description: Du kan begära åtkomst till en plan i Adobe Workfront Scenarioplan när länken till planen delas med dig.
author: Alina
feature: Workfront Scenario Planner
exl-id: fa47cb8c-a3ca-4748-b67d-2d8ed34b9b4a
source-git-commit: bbc3ac852dae3d9a503b4585dfc229d43c9aed28
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---

# Begär åtkomst till en plan i [!DNL Scenario Planner]

Du kan begära åtkomst till en plan i [!DNL Adobe Workfront Scenario Planner] när länken till planen delas med dig.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>Nytt: Ultimate </p></li>
   <p>Scenarioplanen är inte tillgänglig för de nya Workfront Select- eller Workfront Prime-planerna. </p>
   <li><p>Aktuell: [!UICONTROL Business] eller högre</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licens*</p> </td> 
   <td> <p>Nytt: Ljus eller högre</p> 
   <p>Aktuell: [!UICONTROL Review] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td>Produkt* </td> 
   <td> <ul><li><p>För nya Workfront-planer:</p><p> Adobe Workfront</li></p>
   <li><p>För nuvarande Workfront-planer: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>

<p>Mer information finns i <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Åtkomst krävs för att använda [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Åtkomstnivå </td> 
   <td>  <p>[!UICONTROL View] eller högre åtkomst till [!DNL Scenario Planner]</p>  </td> 
  </tr>
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav för Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Innan du kan begära åtkomst till en plan i [!DNL Scenario Planner] måste du ha följande:

* En länk till planen.

>[!NOTE]
>
>Om du inte har åtkomstnivåbehörighet till [!DNL Scenario Planner] och du försöker komma åt en plan från en länk, kan du inte begära åtkomst till planen. I stället visas en skärm som informerar dig om att kontakta administratören för [!DNL Workfront].

## Begär åtkomst för planer i [!DNL Workfront Scenario Planner]

Om du inte redan har behörighet för en plan och navigerar till den från en länk som delas med dig, visas en skärm som informerar dig om att du inte har behörighet att visa planen. Du uppmanas att begära behörigheter från den som skapat planen.

>[!TIP]
>
>Du kan bara begära behörigheter från ägaren eller den som har skapat en plan. Du kan inte begära behörigheter från andra användare som också har tillgång till planen.

Så här begär du behörigheter:

1. Klicka på en länk till en plan.

   ![](assets/request-access-to-plan-350x277.png)

1. Ange vilken behörighetsnivå du vill bevilja i listrutan **[!UICONTROL Request access to]**. Välj bland följande:

   * [!UICONTROL View]
   * [!UICONTROL Manage]

   Du kan inte begära en behörighet som är högre än din åtkomstnivå till [!DNL Scenario Planner]. Du kan till exempel inte begära [!UICONTROL Manage] behörigheter om du har åtkomst till [!DNL Scenario Planner].

   Mer information om olika behörighetsnivåer finns i [Dela en plan i  [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

   Mer information om hur en Workfront-administratör kan hantera åtkomst till [!DNL Scenario Planner] finns i [Bevilja åtkomst till  [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

1. (Valfritt) Ange en kommentar eller förfrågan i **[!UICONTROL Leave comment box]** och klicka sedan på **[!UICONTROL Request access]**.

   Följande händer:

   * [!DNL Workfront] skickar ett e-postmeddelande till planägaren, där de kan bevilja de begärda behörigheterna.\
     ![](assets/request-access-to-plan-email-350x156.png)

   * När planägaren har beviljat de begärda behörigheterna får du ett e-postmeddelande om att behörigheterna har beviljats om administratören för [!DNL Workfront] har objektresursen till användarmeddelandet aktiverat i ditt system och du aktiverar e-postmeddelandet för [!UICONTROL Someone shares an object with me] i din profil.

     ![](assets/access-granted-to-plan-email-350x172.png)

   * Du kan också bevilja behörigheter till planer från området [!UICONTROL Home] och från mobilappen [!DNL Workfront].

   Mer information om hur du aktiverar systemmeddelanden finns i [Konfigurera händelsemeddelanden för alla i systemet](../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

   Mer information om hur du aktiverar meddelanden i din profil finns i [Meddelanden: Övrig information](../workfront-basics/using-notifications/notifications-misc-information.md).

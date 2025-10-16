---
product-area: enterprise-scenario-planner-product-area
keywords: plan,behörigheter,resurs,initiativ,,scenarier,scenario
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Begär åtkomst till en plan i scenarioplaneraren
description: Du kan begära åtkomst till en plan i Adobe Workfront Scenarioplan när länken till planen delas med dig.
author: Alina
feature: Workfront Scenario Planner
exl-id: fa47cb8c-a3ca-4748-b67d-2d8ed34b9b4a
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '471'
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
   <td> <p>[!DNL Adobe Workfront] package</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>ANMÄRKNING</b></p>
<p>Kontakta Workfront om du har ett annat Workfront-paket.</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licens</p> </td> 
   <td> <p>[!UICONTROL Light] eller högre</p> 
   <p>[!UICONTROL Review] eller högre</p> </td> 
  </tr> 
    <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>[!UICONTROL View] eller högre åtkomst till [!DNL Scenario Planner]</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om åtkomst till scenarioplanen finns i [Åtkomst krävs för att använda  [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav för Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td>  <p>[!UICONTROL View] or higher access to the [!DNL Scenario Planner]</p>  </td> 
  </tr>
 </tbody> 
</table>-->

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

   ![Begär åtkomst till planen](assets/request-access-to-plan-350x277.png)

1. Ange vilken behörighetsnivå du vill bevilja i listrutan **[!UICONTROL Request access to]**. Välj bland följande:

   * [!UICONTROL View]
   * [!UICONTROL Manage]

   Du kan inte begära en behörighet som är högre än din åtkomstnivå till [!DNL Scenario Planner]. Du kan till exempel inte begära [!UICONTROL Manage] behörigheter om du har åtkomst till [!DNL Scenario Planner].

   Mer information om olika behörighetsnivåer finns i [Dela en plan i  [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

   Mer information om hur en Workfront-administratör kan hantera åtkomst till [!DNL Scenario Planner] finns i [Bevilja åtkomst till  [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

1. (Valfritt) Ange en kommentar eller förfrågan i **[!UICONTROL Leave comment box]** och klicka sedan på **[!UICONTROL Request access]**.

   Följande händer:

   * [!DNL Workfront] skickar ett e-postmeddelande till planägaren, där de kan bevilja de begärda behörigheterna.\
     ![Begär e-postmeddelande om åtkomst](assets/request-access-to-plan-email-350x156.png)

   * När planägaren har beviljat de begärda behörigheterna får du ett e-postmeddelande om att behörigheterna har beviljats om administratören för [!DNL Workfront] har objektresursen till användarmeddelandet aktiverat i ditt system och du aktiverar e-postmeddelandet för [!UICONTROL Someone shares an object with me] i din profil.

     ![Åtkomst beviljad e-post](assets/access-granted-to-plan-email-350x172.png)

   * Du kan också bevilja behörigheter till planer från området [!UICONTROL Home] och från mobilappen [!DNL Workfront].

   Mer information om hur du aktiverar systemmeddelanden finns i [Konfigurera händelsemeddelanden för alla i systemet](../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

   Mer information om hur du aktiverar meddelanden i din profil finns i [Meddelanden: Övrig information](../workfront-basics/using-notifications/notifications-misc-information.md).

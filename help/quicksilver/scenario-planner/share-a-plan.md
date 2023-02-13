---
product-area: enterprise-scenario-planner-product-area
keywords: plan,behörigheter,dela,initiativ,scenarier,scenario
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Dela en plan i scenarioplanen
description: Du kan dela en plan som du har skapat i Adobe Workfront Scenarioplan med andra användare.
author: Alina
feature: Workfront Scenario Planner
exl-id: b8bbb533-4384-414c-8574-4e137962b8ca
source-git-commit: 82a5102d28700368a094502dcd6026462c149eb1
workflow-type: tm+mt
source-wordcount: '880'
ht-degree: 0%

---

# Dela en plan i [!DNL Scenario Planner]

Du kan dela en plan i [!DNL Adobe Workfront Scenario Planner] med andra användare, så att de kan samarbeta i samma arbete som du.

>[!TIP]
>
>Om du skickar en länk till en plan till andra måste du också dela planen med dem för att de ska kunna se den.

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plan*</b> </p> </td> 
   <td>[!UICONTROL Business] eller högre</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licens*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td><b>Produkt</b> </td> 
   <td> <p>Du måste köpa ytterligare en licens för [!DNL Adobe Workfront Scenario Planner] för att få tillgång till funktioner som beskrivs i den här artikeln.</p> <p>Mer information om hur du får [!DNL Workfront Scenario Planner], se <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Åtkomst krävs för att använda [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Konfigurationer på åtkomstnivå*</strong> </td> 
   <td> <p>[!UICONTROL Edit] åtkomst till [!DNL Scenario Planner]</p> <p>Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] administratören kan ändra din åtkomstnivå, se <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objektbehörigheter</strong> </p> </td> 
   <td> <p> [!UICONTROL Manage] behörigheter till planen
     <p>Mer information om hur du begär ytterligare åtkomst till en plan finns i <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">[!UICONTROL Request] tillgång till en plan i [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

* De användare som ges behörigheter till planen måste ha tillgång till [!DNL Scenario Planner] området i deras åtkomstnivåer, enligt din [!DNL Workfront] administratör för att få behörighet till en plan.

   Till exempel: [!UICONTROL Requestors] kan inte visa, skapa eller redigera planer. Du bör tänka på detta när du delar en plan med en användare som har en begärande licens.

<!--
  NOTE: ensure this stays this way and they don't restrict Workers from SP as well?? OR ensure you can even SEE Requestors as an option or they are not grayed out??)
  -->

Mer information om åtkomst till [!DNL Scenario Planner] för olika licenstyper, se [Bevilja åtkomst till [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

## Att tänka på när det gäller delning av plan

* Du kan dela en plan, eller dela flera planer, i grupp.
* Du kan inte visa planer som du inte har skapat eller som inte delas med dig.
* Du kan bara dela en plan med andra användare. Du kan inte dela planer med grupper, team eller företag.
* Du måste spara en plan innan du kan dela den.
* Du kan dela en URL till en plan med en annan användare. Om användaren inte har behörighet att åtminstone visa planen kan han/hon begära åtkomst till planen från en annan användare när han/hon får URL:en. Mer information om hur du begär åtkomst till en plan finns i [Begär åtkomst till en plan i [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).
* När du delar flera planer som redan har delats med andra, ersätts inte de användare du delar med utan läggs till de befintliga användarna i varje plan som du har valt.

## Dela planer

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **[!UICONTROL Scenarios]**.
1. Klicka på namnet på en plan för att öppna den

   eller

   Välj flera planer att dela dem i grupp.

   >[!TIP]
   >
   >Du kan dela en plan genom att klicka på de avatarer för användare som planen delas med i det övre högra hörnet av planhuvudet.

1. (Villkorligt) Om du har öppnat en plan klickar du på **[!UICONTROL More]** icon ![](assets/more-icon.png) till höger om [!UICONTROL Plan] namn och klicka sedan på **[!UICONTROL Share]**

   eller

   Om du har valt flera planer för att dela dem samtidigt klickar du på **[!UICONTROL Share]** icon ![](assets/share-icon-26x26.png) högst upp i listan över planer att öppna [!UICONTROL Plan] åtkomstruta.

   >[!TIP]
   >
   >* Användare som har behörighet till alla planer du väljer visas i [!UICONTROL Plan] åtkomstruta.
   >* Eventuella ytterligare användare läggs till i och ersätter inte befintliga användare för alla valda planer.


1. I **[!UICONTROL Give plan access to]** börjar du skriva namnet på de användare som du vill dela planen med och väljer dem sedan när de visas i listan.
1. I listrutan Behörigheter till höger om användarnamnet väljer du den behörighetsnivå som du vill ge dem till planen.
1. Välj bland följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL View]</td> 
      <td>Användare som du delar planen med får behörighet att visa planen. De kan inte redigera information om planen, lägga till initiativ, scenarier eller publicera scenarier. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Manage]</td> 
      <td> <p>Användare som du delar planen med har behörighet att hantera planen, vilket inkluderar redigeringsinformation, tillägg av initiativ, scenarier och publicering av planen. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Du kan bara ta bort en plan när du har skapat den. Du kan inte ta bort planer som delas med dig.

1. Klicka på **[!UICONTROL Save]**.

   Planen delas nu med de användare som du har angett.

   Du kan visa användare som har behörighet till planen i kolumnen Delad med mig i en lista över planer eller i det övre högra hörnet av planhuvudet.

   >[!TIP]
   >
   >Du kan visa planer som delas med dig genom att använda [!UICONTROL Shared with me] i en lista med planer.

## Alternativ för planbehörigheter

I följande tabell visas de behörigheter som du kan ge när du delar en plan. Mer information om vilka användare som får åtkomst baserat på deras licens finns i [Bevilja åtkomst till [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Åtgärder</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Manage]</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL View]</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Visa plan </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Visa initiativ </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Visa scenarier</td> 
   <td>✓</td> 
   <td><span style="font-weight: normal;">✓</span> </td> 
  </tr> 
  <tr> 
   <td>Visa jobbroller</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Visa kostnads- och budgetinformation*</td> 
   <td>✓</td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td>Hantera kostnads- och budgetinformation*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Skapa initiativ</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Skapa scenarier</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ta bort initiativ eller scenarier</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Kopiera scenarier</td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Publicera scenarier**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*Du måste ha tillgång till finansiella data för att kunna visa eller hantera finansiell information om planer, även om du har behörighet att hantera planer. Mer information om åtkomst till finansiella data finns i [Bevilja åtkomst till finansiella uppgifter](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

**Du måste ha behörighet att skapa och hantera projekt för att kunna publicera scenarier.

Mer information om åtkomstnivå för projekt finns i [Bevilja åtkomst till projekt](../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Mer information om projektbehörigheter finns i [Dela ett projekt i [!DNL Adobe Workfront]](../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

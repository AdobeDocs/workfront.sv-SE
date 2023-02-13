---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Uppdatera initiala prioriteringar i scenarioplanen
description: Det är viktigt att prioritera initiativ eftersom initiativen får jobbroller och budgetresurser från planen i den ordning de anges i planen.
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---

# Uppdatera initiala prioriteringar i [!DNL Scenario Planner]

Det är viktigt att prioritera initiativ eftersom initiativen får jobbroller och budgetresurser från planen i den ordning de anges i planen.

Du kan prioritera initiativ för en plan som du har skapat eller för en plan som någon har delat med dig.

Mer information om att skapa planer finns i [Skapa och redigera planer i [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Mer information om hur du skapar initiativ finns i [Skapa och redigera i [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## Åtkomstkrav

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
   <td> <p>[!UICONTROL Edit] åtkomst eller högre till [!DNL Scenario Planner]</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] administratören kan ändra din åtkomstnivå, se <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objektbehörigheter</strong> </p> </td> 
   <td> <p>[!UICONTROL Manage] behörigheter till en plan</p> <p>Mer information om hur du begär ytterligare åtkomst till en plan finns i <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Begär åtkomst till en plan i [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Uppdatera initiala prioriteringar

När du ändrar prioritet för initiativ ändrar du deras listordning i planen.

Vi rekommenderar att ni sätter mer brådskande initiativ överst i en plan och de smidigare - som kan göras när som helst och bara om det finns resurser - längst ned i planen.

>[!NOTE]
>
>[!DNL Workfront] tilldelar planresurser till initiativ i den ordning de anges i planen.
>
>Om planen t.ex. har tre tillgängliga ingenjörer och Initiative 1 och Initiative 2 båda kräver två ingenjörer att slutföra, och båda är schemalagda för samma tidsram, så associerar Workfront två ingenjörer med Initiative 1 och en fortfarande tillgänglig ingenjör med Initiative 2. I det här fallet visar Initiativ 2 att det finns en konflikt, eftersom det saknar en ingenjör. Ibland är det enda sättet att undvika konflikter i en plan att ändra prioriteten för era initiativ.

Så här uppdaterar du prioritet:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png)och sedan klicka [!UICONTROL Scenarios].

   En lista över planer visas.

1. Klicka på namnet på en plan för att öppna den och leta sedan reda på initiativen som du vill prioritera.
1. Klicka i rutan till vänster om namnet på en eller flera initiativ och gör något av följande:

   * Klicka på handtaget till vänster om namnet på en av de valda initiativen och dra den sedan uppåt eller nedåt i listan för att ändra prioriteten för initiativet.

      Workfront visar antalet valda initiativ.

      ![](assets/multi-select-initiative-number.png)

   * Klicka på **[!UICONTROL Prioritize]** längst ned i planen och välj sedan bland följande alternativ:

      * **[!UICONTROL Top]**: Flyttar de valda initiativen högst upp i initieringslistan. De valda initiativen listas först i planen.
      * **[!UICONTROL Bottom]**: Flyttar de valda initiativen längst ned i initieringslistan. De valda initiativen listas sist i planen.
      * **[!UICONTROL Select a number]**: Flyttar de valda initiativen efter det initiativ du anger här.

         ![](assets/prioritize-initiatives-expanded-highlighted-350x171.png)
      [!DNL Workfront] placerar omedelbart de valda initiativen där du anger detta och antalet alla initiativ uppdateras därefter.


1. Klicka **[!UICONTROL Save Plan]** för att spara ändringarna.

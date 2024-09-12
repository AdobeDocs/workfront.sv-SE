---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Uppdatera initiala prioriteringar i scenarioplanen
description: Det är viktigt att prioritera initiativ eftersom initiativen får jobbroller och budgetresurser från planen i den ordning de anges i planen.
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# Uppdatera initiala prioriteringar i [!DNL Scenario Planner]

Det är viktigt att prioritera initiativ eftersom initiativen får jobbroller och budgetresurser från planen i den ordning de anges i planen.

Du kan prioritera initiativ för en plan som du har skapat eller för en plan som någon har delat med dig.

Mer information om hur du skapar planer finns i [Skapa och redigera planer i  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Mer information om hur du skapar initiativ finns i [Skapa och redigera initiativ i  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

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
   <p>Scenarioplanen är inte tillgänglig för nya Workfront Select eller Workfront Plan. </p>
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
   <td> <p>[!UICONTROL Edit] åtkomst till [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objektbehörigheter </p> </td> 
   <td> <p>[!UICONTROL Manage] behörigheter till en plan</p> <p>Mer information om hur du begär ytterligare åtkomst till en plan finns i <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Begär åtkomst till en plan i [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav för Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Uppdatera initiala prioriteringar

När du ändrar prioritet för initiativ ändrar du deras listordning i planen.

Vi rekommenderar att ni sätter mer brådskande initiativ överst i en plan och de smidigare - som kan göras när som helst och bara om det finns resurser - längst ned i planen.

>[!NOTE]
>
>[!DNL Workfront] allokerar planresurser till initiativ i den ordning som de anges i planen.
>
>Om planen t.ex. har tre tillgängliga ingenjörer och Initiative 1 och Initiative 2 båda kräver två ingenjörer att slutföra, och båda är schemalagda för samma tidsram, så associerar Workfront två ingenjörer med Initiative 1 och en fortfarande tillgänglig ingenjör med Initiative 2. I det här fallet visar Initiativ 2 att det finns en konflikt, eftersom det saknar en ingenjör. Ibland är det enda sättet att undvika konflikter i en plan att ändra prioriteten för era initiativ.

Så här uppdaterar du prioritet:

{{step1-to-scenario-planner}}

En lista över planer visas.

1. Klicka på namnet på en plan för att öppna den och leta sedan reda på initiativen som du vill prioritera.
1. Klicka i rutan till vänster om namnet på en eller flera initiativ och gör något av följande:

   * Klicka på handtaget till vänster om namnet på en av de valda initiativen och dra den sedan uppåt eller nedåt i listan för att ändra prioriteten för initiativet.

     Workfront visar antalet valda initiativ.

     ![](assets/multi-select-initiative-number.png)

   * Klicka på rutan **[!UICONTROL Prioritize]** längst ned i planen och välj sedan bland följande alternativ:

      * **[!UICONTROL Top]**: Flyttar de valda initiativen högst upp i initieringslistan. De valda initiativen listas först i planen.
      * **[!UICONTROL Bottom]**: Flyttar de valda initiativen längst ned i initieringslistan. De valda initiativen listas sist i planen.
      * **[!UICONTROL Select a number]**: Flyttar de valda initiativen efter det initiativ du anger här.

        ![](assets/prioritize-initiatives-expanded-highlighted-350x171.png)

     [!DNL Workfront] placerar omedelbart de valda initiativen där du anger detta och antalet alla initiativ uppdateras därefter.

1. Klicka på **[!UICONTROL Save Plan]** om du vill spara ändringarna.

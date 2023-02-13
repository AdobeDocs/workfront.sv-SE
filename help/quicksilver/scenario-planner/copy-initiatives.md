---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Kopiera initiativ i scenarioplaneraren
description: Du kan skapa initiativ genom att kopiera befintliga initiativ. Du kan kopiera initiativ för en plan som du skapar eller för en plan som någon delar med dig.
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---

# Kopiera initiativ i [!DNL Scenario Planner]

Du kan skapa initiativ genom att kopiera befintliga initiativ. Du kan kopiera initiativ för en plan som du skapar eller för en plan som någon delar med dig.

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
   <td> <p>[!DNL Adobe Workfront]<b> licens</b>*</p> </td> 
   <td> <p>[!UICONTROL Review] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td><b>Produkt</b> </td> 
   <td> <p>Du måste köpa ytterligare en licens för [!DNL Adobe Workfront Scenario Planner] för att få tillgång till funktioner som beskrivs i den här artikeln.</p> <p>Mer information om hur du får [!DNL Workfront Scenario Planner], se <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Åtkomst krävs för att använda [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Konfigurationer på åtkomstnivå*</strong> </td> 
   <td> <p>[!UICONTROL Edit] åtkomst eller högre till [!DNL Scenario Planner]</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] administratören kan ändra din åtkomstnivå, se <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objektbehörigheter</strong> </p> </td> 
   <td> <p>[!UICONTROL Manage] behörigheter till en plan</p> <p>Mer information om hur du begär ytterligare åtkomst till en plan finns i <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Begär åtkomst till en plan i [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Kopiera initiativ

Tänk på följande när du kopierar:

* Om du kopierar ett initiativ läggs kopian in i samma plan som det ursprungliga initiativet.
* Om du kopierar ett initiativ kopieras följande information från det ursprungliga initiativet till det nya initiativet:

   * [!UICONTROL Duration]
   * [!UICONTROL Job roles]
   * [!UICONTROL People] och [!UICONTROL Fixed Costs]
   * [!UICONTROL Planned Benefit]

* Om du kopierar ett initiativ kan du ändra följande information för planen, om informationen finns i det ursprungliga initiativet:

   * Nödvändigt antal jobbroller
   * [!UICONTROL Costs]
   * [!UICONTROL Plan Utilization]
   * Utnyttjande av jobbroll
   * [!UICONTROL Net Value]

* Om du kopierar ett projekt som har skapats genom import av ett projekt eller publicerats till ett projekt minst en gång får det följande konsekvenser:

   * Det duplicerar inte det projekt som är associerat med initiativet.
   * Den kopplar inte det kopierade initiativet till projektet.
   * Det ändrar inte [!DNL Scenario Planner] -avsnittet i projektet, för projekt som har publicerats minst en gång.

   Mer information om publicering av projekt finns i [Uppdatera eller skapa projekt genom att publicera i [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

   Mer information om hur du skapar initiativ genom att importera projekt finns i [Importera projekt till planer i [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

## Kopiera initiativ

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png)och sedan klicka [!UICONTROL Scenarios].

   En lista över planer visas.

1. Klicka på namnet på en plan för att öppna den och leta sedan reda på initiativen som du vill kopiera.
1. Markera rutan till vänster om det eller de initiativ du vill kopiera och klicka sedan på **[!UICONTROL Copy]** på menyn som visas längst ned i planen.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   [!DNL Workfront] kopierar initiativen omedelbart och placerar dem under det senast valda initiativet.

   Namnet på det kopierade initiativet är *[!UICONTROL Copy of]`<Name of original initiative>`*.

   >[!NOTE]
   >
   >Beroende på var du infogar de nya initiativen kan antalet befintliga initiativ ändras.

1. Uppdatera namnet på det kopierade initiativet.

   >[!TIP]
   >
   >Vi rekommenderar att du alltid uppdaterar namnet på initiativet för att undvika förvirring om du vill kopiera dem igen.

1. (Valfritt) Uppdatera prioriteten för dina nya initiativ.

   Mer information om att prioritera initiativ finns i [Uppdatera initiala prioriteringar i [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Klicka **[!UICONTROL Save Plan]** för att spara ändringarna.

---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Kopiera initiativ i scenarioplanen
description: Du kan skapa initiativ genom att kopiera befintliga initiativ. Du kan kopiera initiativ för en plan som du skapar eller för en plan som någon delar med dig.
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 0%

---

# Kopiera initiativ i [!DNL Scenario Planner]

<!--Audited: 07/2024-->

Du kan skapa initiativ genom att kopiera befintliga initiativ. Du kan kopiera initiativ för en plan som du skapar eller för en plan som någon delar med dig.

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
   <td> <p>[!UICONTROL Edit] åtkomst till [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Objektbehörigheter </p> </td> 
   <td> <p>[!UICONTROL Manage] behörigheter till en plan</p> </td> 
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
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Kopiera initiativ

Tänk på följande när du kopierar:

* Om du kopierar ett initiativ läggs kopian in i samma plan som det ursprungliga initiativet.
* Om du kopierar ett initiativ kopieras följande information från det ursprungliga initiativet till det nya initiativet:

   * [!UICONTROL Duration]
   * [!UICONTROL Job roles]
   * [!UICONTROL People] och [!UICONTROL Fixed Costs]
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
   * Det ändrar inte avsnittet [!DNL Scenario Planner] i projektet, för projekt som har publicerats minst en gång.

  Mer information om publicering av projekt finns i [Uppdatera eller skapa projekt genom publicering i  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

  Mer information om hur du skapar initiativ genom att importera projekt finns i [Importera projekt till planer i  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

## Kopiera initiativ

{{step1-to-scenario-planner}}

En lista över planer visas.

1. Klicka på namnet på en plan för att öppna den och leta sedan reda på initiativen som du vill kopiera.
1. Markera rutan till vänster om det eller de initiativ du vill kopiera och klicka sedan på **[!UICONTROL Copy]** på menyn som visas längst ned i planen.

   ![Kopiera initiativ](assets/bottom-manage-initiative-menu-350x45.png)

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

   Mer information om att prioritera initiativ finns i [Uppdatera prioriteter för initiativ i  [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Klicka på **[!UICONTROL Save Plan]** om du vill spara ändringarna.

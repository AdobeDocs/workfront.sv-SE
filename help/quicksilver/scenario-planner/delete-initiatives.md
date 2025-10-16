---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Ta bort initiativ i scenarioplanen
description: Du kan ta bort initiativ för en plan som du har skapat eller för en plan som någon har delat med dig. Du kan inte återställa initiativ som du har tagit bort.
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---

# Ta bort initiativ i [!DNL Scenario Planner]

Du kan ta bort initiativ för en plan som du har skapat eller för en plan som någon har delat med dig. Du kan inte återställa initiativ som du har tagit bort.

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
</table>

*For information, see [Access requirements to Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Ta bort initiativ

Tänk på följande när du tar bort initiativ:

* När du tar bort ett initiativ tas mängden jobbroller och den kostnadsinformation som är kopplad till initiativet bort från planen.
* Om du tar bort ett initiativ som skapats genom att ett projekt importeras, tas inte det projekt som är kopplat till initiativet bort.
* Borttagning av ett projekt som har publicerats till ett projekt minst en gång ger följande resultat:

   * Initiativet tas bort från scenariot, men området [!DNL Scenario Planner] finns kvar i avsnittet [!UICONTROL Project Details].
   * Om det initiativ du tar bort är det enda publicerade initiativet i scenariot, tas även indikatorn för att planen har publicerats bort.

     Mer information om publicering av projekt finns i [Uppdatera eller skapa projekt genom publicering i  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

     Mer information om hur du skapar initiativ genom att importera projekt finns i [Importera projekt till planer i  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

Du kan ta bort ett initiativ åt gången eller ta bort flera initiativ samtidigt.

* [Ta bort ett initiativ](#delete-one-initiative)
* [Ta bort satsningar](#delete-initiatives-in-bulk)

### Ta bort ett initiativ {#delete-one-initiative}

{{step1-to-scenario-planner}}

En lista över planer visas.

1. Klicka på namnet på en plan för att öppna den och leta sedan reda på det initiativ du vill ta bort.
1. Gör något av följande:

   * Klicka på **[!UICONTROL More menu]** ![Mer-menyn](assets/more-menu.png) till höger om företagsnamnet och klicka sedan på **[!UICONTROL Delete]** > **[!UICONTROL Yes, delete it]**.

   * Markera rutan till vänster om initiativet, klicka sedan på **[!UICONTROL Delete]** på den flytande menyn som visas längst ned i planen och klicka sedan på **[!UICONTROL Yes, delete it]**.

   Initiativet, dess befattning och kostnadsinformation tas bort från planen.

1. Klicka på **[!UICONTROL Save Plan]** om du vill spara ändringarna.

### Ta bort satsningar {#delete-initiatives-in-bulk}

{{step1-to-scenario-planner}}

En lista över planer visas.

1. Klicka på namnet på en plan för att öppna den och leta sedan reda på det initiativ du vill ta bort.
1. Markera rutorna till vänster om de initiativ som du vill ta bort, klicka sedan på **[!UICONTROL Delete]** på menyn som visas längst ned i planen och klicka sedan på **[!UICONTROL Yes, delete them]**.

   ![Hantera initieringsmeny](assets/bottom-manage-initiative-menu-350x45.png)

   Initiativen och deras jobbroll och kostnadsinformation tas bort från planen.

1. Klicka på **[!UICONTROL Save Plan]** om du vill spara ändringarna.

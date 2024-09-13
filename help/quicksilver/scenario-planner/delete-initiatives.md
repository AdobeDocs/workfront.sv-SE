---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Ta bort initiativ i scenarioplanen
description: Du kan ta bort initiativ för en plan som du har skapat eller för en plan som någon har delat med dig. Du kan inte återställa initiativ som du har tagit bort.
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: bbc3ac852dae3d9a503b4585dfc229d43c9aed28
workflow-type: tm+mt
source-wordcount: '485'
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

   * Klicka på **[!UICONTROL More menu]** ![](assets/more-menu.png) till höger om företagsnamnet och klicka sedan på **[!UICONTROL Delete]** > **[!UICONTROL Yes, delete it]**.

   * Markera rutan till vänster om initiativet, klicka sedan på **[!UICONTROL Delete]** på den flytande menyn som visas längst ned i planen och klicka sedan på **[!UICONTROL Yes, delete it]**.

   Initiativet, dess befattning och kostnadsinformation tas bort från planen.

1. Klicka på **[!UICONTROL Save Plan]** om du vill spara ändringarna.

### Ta bort satsningar {#delete-initiatives-in-bulk}

{{step1-to-scenario-planner}}

En lista över planer visas.

1. Klicka på namnet på en plan för att öppna den och leta sedan reda på det initiativ du vill ta bort.
1. Markera rutorna till vänster om de initiativ som du vill ta bort, klicka sedan på **[!UICONTROL Delete]** på menyn som visas längst ned i planen och klicka sedan på **[!UICONTROL Yes, delete them]**.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   Initiativen och deras jobbroll och kostnadsinformation tas bort från planen.

1. Klicka på **[!UICONTROL Save Plan]** om du vill spara ändringarna.
